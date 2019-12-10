# Java 服务地址设置<a name="ZH-CN_TOPIC_0111232099"></a>

使用SDK调用云服务API时，需要获取每个云服务的地址（Endpoint）。

Java SDK支持两种方式：SDK自动获取、手工编码设置。

编码设置云服务Endpoint的示例如下：

```
endpointResolver.addOverrideEndpoint(ServiceType.DNS, 
 "https://dns.example.com");
endpointResolver.addOverrideEndpoint(ServiceType.VOLUME_BACKUP,
 "https://vbs.example.com/v2/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.AUTO_SCALING,
 "https://as.example.com/autoscaling-api/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.CLOUD_EYE,
 "https://ces.example.com/V1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.LOAD_BALANCER,
 "https://elb.example.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.MAP_REDUCE,
 "https://mrs.example.com/v1.1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.KEY_MANAGEMENT,
 "https://kms.example.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.CLOUD_TRACE,
 "https://cts.example.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.ANTI_DDOS,
 "https://antiddos.example.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.Notification,
 "https://smn.example.com/v2/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.MessageQueue,
 "https://dms.example.com/v1.0/%(project_id)s");
```

-   上述代码中example的格式为：“区域.云平台域名”，参数详情可以访问[这里](https://developer.huaweicloud.com/endpoint)了解。
-   上述代码中project\_id不需要替换为实际值。
-   单击[此处](https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/core-sample/src/main/java/com/huawei/openstack/sample/Openstack4jSample.java)获取使用Java SDK的一个完整代码示例，供参考。

