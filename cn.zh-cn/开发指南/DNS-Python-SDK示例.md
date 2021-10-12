# DNS Python SDK示例<a name="sdk_02_0021"></a>

## DNS Python OpenStack SDK示例<a name="section51200923195823"></a>

云解析（Domain Name Service）提供高可用，高扩展的权威DNS服务和DNS管理服务，把人们常用的域名或应用资源转换成计算机用于连接的IP地址，从而将最终用户路由到相应的应用资源上。

## 创建内网域名<a name="section9090701191853"></a>

用户在VPC内使用云解析服务进行内网域名托管，需使用增加内网域名功能，用户可使用Python OpenStack SDK创建一个内网域名，详细操作如下：

1.  指定需要关联的VPC。
2.  创建内网域名。

下面代码为内网域名创建的过程，用户可以根据需求进行相应的参数配置，创建完成后，新增的域名会在DNS服务的内网域名页面上显示。

```
def setUpClass(cls):      
    super(TestZone, cls).setUpClass()      
    # get a router      
    routers = cls.conn.network.routers(limit=2)      
    idx = 0      
    for _router in routers:          
        idx += 1          
        print _router          
        if idx == 1:              
            cls.router = _router          
        if idx == 2:              
            cls.router2 = _router              
            break        
    # create zone       
    cls.zone = auto_create_private_zone(cls.conn, cls.NAME, cls.router.id,region)
```

## 关联VPC<a name="section7785359192434"></a>

当用户创建的内网域名需要新关联VPC时，可以利用Python OpenStack SDK在云平台上进行关联操作。 详细操作如下：

1.  指定需要关联的VPC。
2.  选择待关联VPC的内网域名并进行关联。

以下代码显示了内网域名与VPC相关联的过程，用户可以根据需要修改这些配置。

```
def add_router_to_zone(self):
    # Designate a router  
    resource2.wait_for_status(self.conn.dns._session, self.zone, "ACTIVE", interval=5, failures=["ERROR"])
    # Associate the private zone to the router  
    result = self.conn.dns.add_router_to_zone(self.zone, **{"router_id": self.router2.id,"router_region": region})  
    self.assertEqual(result.router_id, self.router2.id)  
    self.assertEqual(result.router_region, region)  
    zone = self.conn.dns.get_zone(self.zone)  
    self.assertEqual(2, len(zone.routers))  
    router_ids = [_router["router_id"] for _router in zone.routers]      self.assertIn(self.router.id, router_ids)
```

## 解关联VPC<a name="section40028305192855"></a>

当用户创建的内网域名不需要关联某个VPC时，可以利用Python OpenStack SDK在云平台上进行进行解关联操作。代码如下： .

```
def remove_router_of_zone(self):      
    resource2.wait_for_status(self.conn.dns._session, self.zone, "ACTIVE", interval=5, failures=["ERROR"])      
    result = self.conn.dns.remove_router_from_zone(self.zone, **{          "router_id": self.router.id,          
      "router_region": region     
    })      
    self.assertEqual(result.router_id, self.router.id)            
    self.assertEqual(result.router_region, region)
```

## 删除内网域名<a name="section15079333193224"></a>

当用户无需使用云解析服务托管该内网域名时，可以使用删除内网域名功能。删除内网域名后，该内网域名包含的域名将无法再被解析。

执行删除内网域名操作前，请确认已备份该内网域名下所有用户创建的记录集。代码如下：

```
def tearDownClass(cls):      
    # delete zone      
    cls.conn.dns.delete_zone(cls.zone)
```

