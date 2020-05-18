# Python SDK故障排查<a name="sdk_02_0010"></a>

Python SDK打开debug的方法：

```
from openstack import utils
utils.enable_logging(debug=True,stream=sys.stdout)
```

