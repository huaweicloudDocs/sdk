# IAM Go SDK用户指导<a name="sdk_03_0016"></a>

## Service Client<a name="section21547825201458"></a>

为了能够与OpenStack API进行交互，首先必须将身份验证凭据传递给Provider，此后，如果要检索Identity服务的任何信息，则需要调用NewIdentityV3方法来创建一个Identity服务客户端，然后即可使用相关的SDK。

```
client, err := openstack.NewIdentityV3(provider, gophercloud.EndpointOpts{
 Region: "RegionName",
})
```

## Tokens<a name="section31784618171442"></a>

Token是鉴权时返回的一段任意文本，用于后续访问及控制API资源。每个Token有特定范围，规定了使用该Token可访问的资源。

**Create a token 创建Token**

```
import (    "github.com/gophercloud/gophercloud/openstack/identity/v3/tokens"   )   

func TestCreateTokenByPasswd(t *testing.T){
    scope := tokens.Scope{
        ProjectName:  TenantName,
        DomainID:     DomainID,
    }

    authOptions := tokens.AuthOptions{
        Username:   Username,
        Password:   Password,
        DomainName: DomainName,
        Scope:      scope,
    }


    token, err := tokens.Create(client, &authOptions).Extract()
}
```

**Validate token Token检查**

检查token是否仍然有效。

```
func TestValidateToken(t *testing.T) {
    
    token, err := tokens.Validate(client, "token_id")
}
```

## Service catalog 服务目录<a name="section36519523171442"></a>

服务是指控制某一OpenStack服务功能的RESTful API，被控制的OpenStack服务包括Compute和Object Storage等。服务提供一个或多个终端节点，通过这些终端节点，用户可进行资源的访问并进行一些操作。

**List Services 获取服务列表**

```
import (    "github.com/gophercloud/gophercloud/openstack/identity/v3/services"   )     

func TestServicesList(t *testing.T) {
// List enumerates the services available to a specific user.
listOpts := services.ListOpts{
           ServiceType: "identity",
    }
}
// Retrieve a pager (i.e. a paginated collection)
allPages, err := services.List(client, listOpts).AllPages()

// Define an anonymous function to be executed on each page's iteration
allServices, err := services.ExtractServices(allPages)

for _, service := range allServices {
    // " service " will be a services.Service
}
```

**Get details for a specific service 获取特定服务详情**

```
func TestServicesGet(t *testing.T) {
    service, err := services.Get(client,"service_id").Extract()
}
```

## Endpoints 终端节点<a name="section58639039171442"></a>

终端节点是一个网络可访问的地址，一般为URL地址，通过它可访问某个服务。

**List endpoints 获取终端节点列表**

```
import (    "github.com/gophercloud/gophercloud/openstack/identity/v3/endpoints"   ) 

func TestEndpointsList(t *testing.T) {
    endpointListOpts := endpoints.ListOpts{
           Availability: gophercloud.AvailabilityPublic,
    }
// Retrieve a pager (i.e. a paginated collection)
    allPages, err := endpoints.List(client, endpointListOpts).AllPages()

    // Define an anonymous function to be executed on each page's iteration
allEndpoints, err := endpoints.ExtractEndpoints(allPages)

    for _, endpoint := range allEndpoints {
        // "endpoint " will be a endpoints.Endpoint
    }
}
```

