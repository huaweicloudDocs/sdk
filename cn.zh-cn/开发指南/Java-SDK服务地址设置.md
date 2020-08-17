# Java SDK服务地址设置<a name="sdk_01_0008"></a>

使用SDK调用云服务API时，需要获取每个云服务的地址（Endpoint）。

Java SDK支持两种方式：SDK自动获取、手工编码设置。

编码设置云服务Endpoint的示例如下：

```
endpointResolver.addOverrideEndpoint(ServiceType.CLOUD_EYE, "https://ces.xxx.yyy.com/V1.0/%(project_id)s"); 
endpointResolver.addOverrideEndpoint(ServiceType.DNS, "https://dns.yyy.com");
endpointResolver.addOverrideEndpoint(ServiceType.CDN, "https://cdn.yyy.com/v1.0");
endpointResolver.addOverrideEndpoint(ServiceType.COMPUTE, "https://ecs.xxx.yyy.com/v2/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.NETWORK, "https://vpc.xxx.yyy.com");
endpointResolver.addOverrideEndpoint(ServiceType.IMAGE, "https://ims.xxx.yyy.com");
endpointResolver.addOverrideEndpoint(ServiceType.BLOCK_STORAGE, "https://evs.xxx.yyy.com/v2/%(project_id)s"");
endpointResolver.addOverrideEndpoint(ServiceType.VOLUME_BACKUP, "https://vbs.xxx.yyy.com/v2/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.AUTO_SCALING, "https://as.xxx.yyy.com/autoscaling-api/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.LOAD_BALANCER, "https://elb.xxx.yyy.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.MAP_REDUCE, "https://mrs.xxx.yyy.com/v1.1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.KEY_MANAGEMENT, "https://kms.xxx.yyy.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.CLOUD_TRACE, "https://cts.xxx.yyy.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.ANTI_DDOS, "https://antiddos.xxx.yyy.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.Notification, "https://smn.xxx.yyy.com/v2/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.MessageQueue, "https://dms.xxx.yyy.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.MAAS, "https://maas.xxx.yyy.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.ECS, "https://ecs.xxx.yyy.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.ECS1_1, "https://ecs.xxx.yyy.com/v1.1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.EVS, "https://evs.xxx.yyy.com/v2/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.EVS2_1, "https://evs.xxx.yyy.com/v2.1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.VPC, "https://vpc.xxx.yyy.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.VPC2, "https://vpc.xxx.yyy.com/v2.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.IDENTITY, "https://iam.xxx.yyy.com/v3");
endpointResolver.addOverrideEndpoint(ServiceType.ORCHESTRATION, "https://rts.xxx.yyy.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.NAT, "https://nat.xxx.yyy.com/v2.0");
endpointResolver.addOverrideEndpoint(ServiceType.BMS, "https://bms.xxx.yyy.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.DEH, "https://deh.xxx.yyy.com/v1.0/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.CSBS, "https://csbs.xxx.yyy.com/v1/%(project_id)s");
endpointResolver.addOverrideEndpoint(ServiceType.IAM, "https://iam.xxx.yyy.com/v3");
```

-   上述代码中xxx.yyy的格式为：“区域.云平台域名”，参数详情可以访问[这里](https://developer.huaweicloud.com/endpoint)了解。
-   上述代码中project\_id不需要替换为实际值。
-   单击[此处](https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/core-sample/src/main/java/com/huawei/openstack/sample/Openstack4jSample.java)获取使用Java SDK的一个完整代码示例，供参考。

