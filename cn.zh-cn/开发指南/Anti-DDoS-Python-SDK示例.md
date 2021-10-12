# Anti-DDoS Python SDK示例<a name="sdk_02_0028"></a>

## 查询Anti-DDoS配置可选范围<a name="section3944661591450"></a>

查询系统支持的Anti-DDoS防护策略配置的可选范围，用户根据范围列表选择适合自已业务的防护策略进行Anti-DDoS流量清洗。

代码示例如下：

```
def list_config(conn):
    print("list anti-ddos confit")
print(conn.anti_ddos.query_config_list())
```

## 开通Anti-DDoS服务<a name="section26684654172532"></a>

用户开通Anti-DDoS流量清洗防护。作为异步接口，调用成功，只是说明服务节点收到了开通请求，开通是否成功需要通过任务查询接口查询该任务的执行状态。

代码示例如下：

```
def create_eip(conn):
    fip_dict = {'enable_L7': True,
                'traffic_pos_id': 1,
                'http_request_pos_id': 1,
                'cleaning_access_pos_id': 1,
                'app_type_id': 0}

    fip = conn.anti_ddos.create_floating_ip(FLOATING_IP_ID, **fip_dict)
print(fip)
```

## 关闭Anti-DDoS服务<a name="section27490877172539"></a>

用户关闭Anti-DDoS流量清洗防护。作为异步接口，调用成功，只是说明服务节点收到了关闭防护请求，操作是否成功需要通过任务查询接口查询该任务的执行状态。

代码示例如下：

```
def delete_eip(conn):
    fip = conn.anti_ddos.get_floating_ip(FLOATING_IP_ID)
    conn.anti_ddos.delete_floating_ip(fip)
```

## 查询Anti-DDoS服务<a name="section13330669172546"></a>

查询配置的Anti-DDoS防护策略，用户可以查询指定EIP的Anti-DDoS防护策略。

代码示例如下：

```
def get_eip(conn):
    fip = conn.anti_ddos.get_floating_ip(FLOATING_IP_ID)
    print(fip)
```

## 更新Anti-DDoS服务<a name="section11656122172548"></a>

更新指定EIP的Anti-DDoS防护策略配置。调用成功，只是说明服务节点收到了更新配置请求，操作是否成功需要通过任务查询接口查询该任务的执行状态。

代码示例如下：

```
def update_eip(conn):
    fip = conn.anti_ddos.get_floating_ip(FLOATING_IP_ID)

    fip_update_dict = {'enable_L7': False,
                       'traffic_pos_id': 1,
                       'http_request_pos_id': 1,
                       'cleaning_access_pos_id': 1,
                       'app_type_id': 0}
    ufip = conn.anti_ddos.update_floating_ip(fip, **fip_update_dict)
    print(ufip)
```

## 查询Anti-DDoS任务<a name="section24002378172550"></a>

用户查询指定的Anti-DDoS防护配置任务，得到任务当前执行的状态。

代码示例如下：

```
def query_task_status(conn):
    print(conn.anti_ddos.query_task_status(
        '228186d4-4aec-4c37-bae8-cb025aaf5770'))
```

## 查询EIP防护状态列表<a name="section4361571172552"></a>

查询用户所有EIP的Anti-DDoS防护状态信息，用户的EIP无论是否绑定到云服务器，都可以进行查询。

代码示例如下：

```
def list_eips(conn):
    print("list eips by status")
    for l in conn.anti_ddos.floating_ips():
    print(l)

```

## 查询指定EIP防护状态<a name="section54758667172554"></a>

查询指定EIP的Anti-DDoS防护状态。

代码示例如下：

```
def get_eip_status(conn):
    print(conn.anti_ddos.get_eip_status(FLOATING_IP_ID))
```

## 查询指定EIP防护流量<a name="section45228460172556"></a>

查询指定EIP在过去24小时之内的防护流量信息，流量的间隔时间单位为5分钟。

代码示例如下：

```
def get_eip_daily(conn):
    for d in conn.anti_ddos.list_eip_daily(FLOATING_IP_ID):
        print(d)
```

## 查询指定EIP异常事件<a name="section9504791172557"></a>

查询指定EIP在过去24小时之内的异常事件信息，异常事件包括清洗事件和黑洞事件，查询延迟在5分钟之内。

代码示例如下：

```
def get_eip_log(conn):
    for l in conn.anti_ddos.list_eip_log(FLOATING_IP_ID):
        print(l)

```

## 查询周防护统计情况<a name="section61032237172559"></a>

查询用户所有Anti-DDoS防护周统计情况，包括一周内DDoS拦截次数和攻击次数、以及按照被攻击次数进行的排名信息等统计数据。

认证代码示例如下：

```
def get_eip_weekly(conn):
    print(conn.anti_ddos.get_eip_weekly('1006510306'))
```

## 查询告警配置信息<a name="section5968868717261"></a>

查询用户配置信息，用户可以通过此接口查询是否接收某类告警，同时可以配置是手机短信还是电子邮件接收告警信息。

代码示例如下：

```
def get_alert_config(conn):
    print(conn.anti_ddos.get_alert_config())
```

