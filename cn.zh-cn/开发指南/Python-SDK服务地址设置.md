# Python SDK服务地址设置<a name="sdk_02_0008"></a>

使用SDK调用云服务API时，需要获取每个云服务的地址（Endpoint）。

Python SDK支持两种方式：SDK自动获取、手工编码设置。

编码设置云服务Endpoint的示例如下：

```
os.environ.setdefault(
    'OS_CLOUD_EYE_ENDPOINT_OVERRIDE',
    'https://ces.example.com/V1.0/%(project_id)s'
)
os.environ.setdefault(
    'OS_AUTO_SCALING_ENDPOINT_OVERRIDE',
    ('https://as.example.com'
     '/autoscaling-api/v1/%(project_id)s')
)
os.environ.setdefault(
    'OS_DNS_ENDPOINT_OVERRIDE',
    'https://dns.example.com/v2'
)
os.environ.setdefault(
    'OS_VOLUME_BACKUP_ENDPOINT_OVERRIDE',
    'https://vbs.example.com/v2/%(project_id)s'
)
os.environ.setdefault(
    'OS_ELBV1_ENDPOINT_OVERRIDE',
    'https://elb.example.com/v1.0/%(project_id)s'
)
os.environ.setdefault(
    'OS_MAP_REDUCE_ENDPOINT_OVERRIDE',
    'https://mrs.example.com/v1.1/%(project_id)s'
)
os.environ.setdefault(
    'OS_CTS_ENDPOINT_OVERRIDE',
    'https://cts.example.com/v1.0/%(project_id)s'
)
os.environ.setdefault(
    'OS_SMN_ENDPOINT_OVERRIDE',
    'https://smn.example.com/v2/%(project_id)s'
)
os.environ.setdefault(
    'OS_MAAS_ENDPOINT_OVERRIDE',
    'https://maas.example.com/v1/%(project_id)s'
)
os.environ.setdefault(
    'OS_KMS_ENDPOINT_OVERRIDE',
    'https://kms.example.com/v1.0/%(project_id)s'
)
os.environ.setdefault(
    'OS_ANTI_DDOS_ENDPOINT_OVERRIDE',
    'https://antiddos.example.com/v1/%(project_id)s'
)
os.environ.setdefault(
    'OS_DMS_ENDPOINT_OVERRIDE',
    'https://dms.example.com/v1.0/%(project_id)s'
)
os.environ.setdefault(
    'OS_RDSV1_ENDPOINT_OVERRIDE',
    'https://rds.example.com/v3/%(project_id)s'
)
os.environ.setdefault(
    'OS_CDN_ENDPOINT_OVERRIDE', 
    'https://cdn.example.com/v1.0'
)
```

-   上述代码中example的格式为：“区域.云平台域名”，参数详情可以访问[这里](https://developer.huaweicloud.com/endpoint)了解。
-   上述代码中project\_id不需要替换为实际值。
-   单击[此处](https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/override.py)获取使用Python SDK的一个完整代码示例，供参考。

