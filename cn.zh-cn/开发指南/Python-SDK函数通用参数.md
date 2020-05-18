# Python SDK函数通用参数<a name="sdk_02_0011"></a>

Python SDK支持一些通用参数，使用方法如下：

## ignore\_missing<a name="section490672161618"></a>

该参数一般出现在服务的delete接口中，默认参数为True，例如：

delete\_flavor\(self, flavor, ignore\_missing=True\)

delete\_image\(self, image, ignore\_missing=True\)

当设置为True时，如果删除的资源不存在时，不打印异常信息，不抛出异常；

当设置为False时，如果所删除的资源不存在，会抛出openstack.exceptions.ResourceNotFound异常。如果没有处理该异常，会导致程序异常终止执行。

## details<a name="section1668923751612"></a>

该参数一般出现在服务的获取资源详细列表接口中，例如：

flavors\(self, details=True, \*\*query\)

images\(self, details=True, \*\*query\)

只有支持/detail接口的资源才支持传入。

当设置为True，请求资源的URI为\{RES\}/details，返回资源的详细信息；

当设置为False，请求的资源的URI为\{RES\}，返回资源的最基本的信息。

## limit<a name="section267655518169"></a>

该参数一般出现在服务的获取资源详细列表接口中，例如：

flavors\(self, details=True, limit = 5\)

images\(self, details=True, limit = 10\)

当传入limit参数时，查询结果会分页返回，每次返回的个数为limit的数值；

当不传入limit参数时，查询结果会一次返回。

