# Python 故障排查<a name="ZH-CN_TOPIC_0111241272"></a>

Python SDK打开debug的方法：

```
from openstack import utils
utils.enable_logging(debug=True,stream=sys.stdout)
```

