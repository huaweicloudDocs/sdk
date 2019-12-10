# IMS Go SDK用户指导<a name="ZH-CN_TOPIC_0090172878"></a>

## Service Client<a name="section24449721201412"></a>

为了能够与OpenStack API进行交互，首先必须将身份验证凭据传递给Provider，此后，如果要检索Image服务的任何信息，则需要调用NewImageServiceV2方法来创建一个Image服务客户端，然后即可使用相关的SDK。

```
client, err := openstack.NewImageServiceV2(provider, gophercloud.EndpointOpts{
 Region: "RegionName",
})
```

## Images 镜像<a name="section16605153171815"></a>

镜像是虚拟机的操作系统，是一系列用于创建或重建服务器的文件。运营商默认提供预置操作系统镜像，但用户也可以从云服务器中创建自定义镜像。

**Create an image 创建镜像**

Create执行创建镜像的请求。

```
import (    "github.com/gophercloud/gophercloud/openstack/imageservice/v2/images"   ) 

func TestImagesCreateDestroyEmptyImage(t *testing.T) {
    protected := false
    visibility := images.ImageVisibilityPrivate
    createOpts := &images.CreateOpts{
           Name:            name,
           ContainerFormat:   "bare",
           DiskFormat:      "vhd",
           MinDisk:         40,
           MinRAM:          1024,
           Protected:       &protected,
           Visibility:      &visibility,
           Tags:            []string{"test","adsfi"},
           Properties: map[string]string{
                  "architecture": "x86_64",
           },
    }
    image, err := images.Create(client, createOpts).Extract()
}
```

**Update an image 更新镜像**

```
func TestImagesUpdate(t *testing.T) {
    updateOpts := images.UpdateOpts{
           images.ReplaceImageName{
               NewName: "alternateName",
           },
    }
    image, err := images.Update(client, "imageupdate_id", updateOpts).Extract()
}
```

**List images 获取镜像列表**

```
func TestImagesListALL(t *testing.T) {
    listOpts := images.ListOpts{
         Visibility: images.ImageVisibilityPublic,
         Owner:      "owner_id",
         Status:     "active",
         Marker:    "marker_id",
         SortKey:    "name",
         SortDir:    "asc",
    }

    // Retrieve a pager (i.e. a paginated collection)
    allPages, err := images.List(client, listOpts).AllPages()

    // Define an anonymous function to be executed on each page's iteration
    allImages, err := images.ExtractImages(allPages)

    for _, image := range allImages {
    // " image " will be a images.Image
    }
}
```

**Get details for a specific image 获取特定镜像详情**

```
func TestImagesGet(t *testing.T) {
    image, err := images.Get(client, "image_id").Extract()
}
```

**Delete an image 删除镜像**

```
func DeleteImage(t *testing.T, client *gophercloud.ServiceClient, image *images.Image) {
    err := images.Delete(client, "image_id").ExtractErr()
}
```

