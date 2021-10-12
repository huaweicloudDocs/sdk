# Go SDK认证方式<a name="sdk_03_0005"></a>

Go SDK支持token认证和AK/SK认证两种方式。

## token认证<a name="section14908101113915"></a>

token认证方式示例代码，参数详情请参考[表1](#table18386163519910)。

```
package main

import (
	"github.com/gophercloud/gophercloud/auth/token"
	"github.com/gophercloud/gophercloud"
	"github.com/gophercloud/gophercloud/openstack/compute/v2/servers"
	"github.com/gophercloud/gophercloud/openstack"
	"fmt"
)

func main() {
	//设置认证参数
	tokenOpts := token.TokenOptions{
		IdentityEndpoint: "https://iam.example.com/v3",
		Username:         "{username}",
		Password:         "{password}",
		DomainID:         "{domainid}",
		ProjectID:        "{projectid}",
	}
	//初始化provider client
	provider, providerErr := openstack.AuthenticatedClient(tokenOpts)
	if providerErr != nil {
		fmt.Println("init provider client error:", providerErr)
		panic(providerErr)
	}

	//初始化service client
	sc, serviceErr := openstack.NewComputeV2(provider, gophercloud.EndpointOpts{})
	if serviceErr != nil {
		fmt.Println("init compute service client error:", serviceErr)
		panic(serviceErr)
	}

	//列出所有服务器
	allPages, err := servers.List(sc, servers.ListOpts{}).AllPages()

	if err != nil {
		fmt.Println("request server list error:", err)
		panic(err)
	}
	//解析返回值
	allServers, err := servers.ExtractServers(allPages)
	if err != nil {
		fmt.Println("extract response data error:", err)
		if ue, ok := err.(*gophercloud.UnifiedError); ok {
			fmt.Println("ErrCode:", ue.ErrorCode())
			fmt.Println("Message:", ue.Message())
		}
		return
	}
	//打印信息
	fmt.Println("List Servers:")
	for _, s := range allServers {
		fmt.Println("server ID is :", s.ID)
		fmt.Println("server name is :", s.Name)
		fmt.Println("server Status is :", s.Status)
		fmt.Println("server AvailbiltyZone is :", s.AvailbiltyZone)
	}
}
```

-   ProviderClient 是所有 OpenStack 服务需要的顶级客户端。该客户端包含所有认证详情，如URL及token ID，通过认证后，编写的Go代码就可访问API。
-   访问某个服务时，还需要该服务的Service Client，详见各服务对应的章节。

**表 1**  参数说明

<a name="table18386163519910"></a>
<table><thead align="left"><tr id="sdk_03_0002_row12561105113219"><th class="cellrowborder" valign="top" width="17.64176417641764%" id="mcps1.2.4.1.1"><p id="sdk_03_0002_p195611252321"><a name="sdk_03_0002_p195611252321"></a><a name="sdk_03_0002_p195611252321"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="37.643764376437645%" id="mcps1.2.4.1.2"><p id="sdk_03_0002_p456145133212"><a name="sdk_03_0002_p456145133212"></a><a name="sdk_03_0002_p456145133212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="44.71447144714472%" id="mcps1.2.4.1.3"><p id="sdk_03_0002_p175619553214"><a name="sdk_03_0002_p175619553214"></a><a name="sdk_03_0002_p175619553214"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="sdk_03_0002_row175617593220"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="sdk_03_0002_p155611355329"><a name="sdk_03_0002_p155611355329"></a><a name="sdk_03_0002_p155611355329"></a>IdentityEndpoint</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="sdk_03_0002_p082312211563"><a name="sdk_03_0002_p082312211563"></a><a name="sdk_03_0002_p082312211563"></a>认证服务（IAM）的Endpoint。</p>
<p id="sdk_03_0002_zh-cn_topic_0121671869_li10140171754817p0"><a name="sdk_03_0002_zh-cn_topic_0121671869_li10140171754817p0"></a><a name="sdk_03_0002_zh-cn_topic_0121671869_li10140171754817p0"></a>“https://iam.<em id="sdk_03_0002_i86181317204018"><a name="sdk_03_0002_i86181317204018"></a><a name="sdk_03_0002_i86181317204018"></a>example</em>.com/v3”中的“example”为“区域.云平台域名”，参数详情可以访问<a href="https://developer.huaweicloud.com/endpoint?iam" target="_blank" rel="noopener noreferrer">这里</a>了解。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_03_0002_p105621519321"><a name="sdk_03_0002_p105621519321"></a><a name="sdk_03_0002_p105621519321"></a>https://iam.cn-north-1.myhuaweicloud.com/v3</p>
</td>
</tr>
<tr id="sdk_03_0002_row12948127133512"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="sdk_03_0002_p9949147153520"><a name="sdk_03_0002_p9949147153520"></a><a name="sdk_03_0002_p9949147153520"></a>Username</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="sdk_03_0002_p1094911703517"><a name="sdk_03_0002_p1094911703517"></a><a name="sdk_03_0002_p1094911703517"></a>IAM用户名。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_03_0002_p59491872353"><a name="sdk_03_0002_p59491872353"></a><a name="sdk_03_0002_p59491872353"></a>-</p>
</td>
</tr>
<tr id="sdk_03_0002_row0606191011354"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="sdk_03_0002_p4607010193512"><a name="sdk_03_0002_p4607010193512"></a><a name="sdk_03_0002_p4607010193512"></a>Password</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="sdk_03_0002_p126071410143517"><a name="sdk_03_0002_p126071410143517"></a><a name="sdk_03_0002_p126071410143517"></a>IAM用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_03_0002_p12607610133518"><a name="sdk_03_0002_p12607610133518"></a><a name="sdk_03_0002_p12607610133518"></a>-</p>
</td>
</tr>
<tr id="sdk_03_0002_row1656275163214"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="sdk_03_0002_p993913484"><a name="sdk_03_0002_p993913484"></a><a name="sdk_03_0002_p993913484"></a>ProjectID</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="sdk_03_0002_p664771152820"><a name="sdk_03_0002_p664771152820"></a><a name="sdk_03_0002_p664771152820"></a>项目ID。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_03_0002_p2056295203213"><a name="sdk_03_0002_p2056295203213"></a><a name="sdk_03_0002_p2056295203213"></a>-</p>
</td>
</tr>
<tr id="sdk_03_0002_row856217512326"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="sdk_03_0002_p656217518325"><a name="sdk_03_0002_p656217518325"></a><a name="sdk_03_0002_p656217518325"></a>DomainID</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="sdk_03_0002_p856285113212"><a name="sdk_03_0002_p856285113212"></a><a name="sdk_03_0002_p856285113212"></a><span>账号ID。</span>如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_03_0002_p25628523215"><a name="sdk_03_0002_p25628523215"></a><a name="sdk_03_0002_p25628523215"></a>-</p>
</td>
</tr>
</tbody>
</table>

## AKSK认证<a name="section397714187393"></a>

AK/SK认证方式示例代码，参数详情请参考[表2](#table4561115173218)。

```
package main

import (
	"github.com/gophercloud/gophercloud/auth/aksk"
	"github.com/gophercloud/gophercloud"
	"github.com/gophercloud/gophercloud/openstack/compute/v2/servers"
	"github.com/gophercloud/gophercloud/openstack"
	"fmt"
)

func main() {
	//设置认证参数
	akskOpts := aksk.AKSKOptions{
		IdentityEndpoint: "https://iam.example.com/v3",
		DomainID:         "{domainid}",
		ProjectID:        "{projectid}",
		Cloud:            "myhuaweicloud.com",
		Region:           "cn-north-1",
		AccessKey:        "{your AK string}",
		SecretKey:        "{your SK string}",
	}
	//初始化provider client
	provider, providerErr := openstack.AuthenticatedClient(akskOpts)
	if providerErr != nil {
		fmt.Println("init provider client error:", providerErr)
		panic(providerErr)
	}

	//初始化service client
	sc, serviceErr := openstack.NewComputeV2(provider, gophercloud.EndpointOpts{})
	if serviceErr != nil {
		fmt.Println("init compute service client error:", serviceErr)
		panic(serviceErr)
	}

	//列出所有服务器
	allPages, err := servers.List(sc, servers.ListOpts{}).AllPages()

	if err != nil {
		fmt.Println("request server list error:", err)
		panic(err)
	}
	//解析返回值
	allServers, err := servers.ExtractServers(allPages)
	if err != nil {
		fmt.Println("extract response data error:", err)
		if ue, ok := err.(*gophercloud.UnifiedError); ok {
			fmt.Println("ErrCode:", ue.ErrorCode())
			fmt.Println("Message:", ue.Message())
		}
		return
	}
	//打印信息
	fmt.Println("List Servers:")
	for _, s := range allServers {
		fmt.Println("server ID is :", s.ID)
		fmt.Println("server name is :", s.Name)
		fmt.Println("server Status is :", s.Status)
		fmt.Println("server AvailbiltyZone is :", s.AvailbiltyZone)
	}
}
```

AK/SK生成说明：登录控制台，进入“我的凭证”，点击“管理访问密钥”创建AK/SK。

AKSK签名时间与UTC时间误差不可以超过15分钟，否则会鉴权失败。

AKSK签名连续失败超过5次，将锁定对应访问的源IP的AKSK请求，持续5分钟。

**表 2**  参数说明

<a name="table4561115173218"></a>
<table><thead align="left"><tr id="row12561105113219"><th class="cellrowborder" valign="top" width="18.51185118511851%" id="mcps1.2.4.1.1"><p id="p195611252321"><a name="p195611252321"></a><a name="p195611252321"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="36.773677367736774%" id="mcps1.2.4.1.2"><p id="p456145133212"><a name="p456145133212"></a><a name="p456145133212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="44.71447144714472%" id="mcps1.2.4.1.3"><p id="p175619553214"><a name="p175619553214"></a><a name="p175619553214"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row71371932171914"><td class="cellrowborder" valign="top" width="18.51185118511851%" headers="mcps1.2.4.1.1 "><p id="p7137143201919"><a name="p7137143201919"></a><a name="p7137143201919"></a>IdentityEndpoint</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.2.4.1.2 "><p id="p082312211563"><a name="p082312211563"></a><a name="p082312211563"></a>认证服务（IAM）的Endpoint。</p>
<p id="zh-cn_topic_0121671869_li10140171754817p0"><a name="zh-cn_topic_0121671869_li10140171754817p0"></a><a name="zh-cn_topic_0121671869_li10140171754817p0"></a>“https://iam.<em id="i86181317204018"><a name="i86181317204018"></a><a name="i86181317204018"></a>example</em>.com/v3”中的“example”为“区域.云平台域名”，参数详情可以访问<a href="https://developer.huaweicloud.com/endpoint?iam" target="_blank" rel="noopener noreferrer">这里</a>了解。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p105621519321"><a name="p105621519321"></a><a name="p105621519321"></a>https://iam.cn-north-1.myhuaweicloud.com/v3</p>
</td>
</tr>
<tr id="row18519162992310"><td class="cellrowborder" valign="top" width="18.51185118511851%" headers="mcps1.2.4.1.1 "><p id="p125191529122311"><a name="p125191529122311"></a><a name="p125191529122311"></a>DomainID</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.2.4.1.2 "><p id="p856285113212"><a name="p856285113212"></a><a name="p856285113212"></a><span>账号ID。</span>如何获取账号ID请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p25628523215"><a name="p25628523215"></a><a name="p25628523215"></a>-</p>
</td>
</tr>
<tr id="row5586185120233"><td class="cellrowborder" valign="top" width="18.51185118511851%" headers="mcps1.2.4.1.1 "><p id="p18586175120237"><a name="p18586175120237"></a><a name="p18586175120237"></a>ProjectID</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.2.4.1.2 "><p id="p1460119015257"><a name="p1460119015257"></a><a name="p1460119015257"></a>项目ID。如何获取项目ID请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p460316092514"><a name="p460316092514"></a><a name="p460316092514"></a>-</p>
</td>
</tr>
<tr id="row175617593220"><td class="cellrowborder" valign="top" width="18.51185118511851%" headers="mcps1.2.4.1.1 "><p id="p88021832125310"><a name="p88021832125310"></a><a name="p88021832125310"></a>ak/sk</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.2.4.1.2 "><p id="p20367134212540"><a name="p20367134212540"></a><a name="p20367134212540"></a>AK/SK访问密钥。</p>
<div class="note" id="note1564918718544"><a name="note1564918718544"></a><a name="note1564918718544"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul161113510548"></a><a name="ul161113510548"></a><ul id="ul161113510548"><li>AK/SK生成说明：登录控制台，进入“我的凭证”，点击“管理访问密钥”创建AK/SK。</li><li>AK/SK签名时间与UTC时间误差不可以超过15分钟，否则会鉴权失败。</li><li>AK/SK签名连续失败超过5次，将锁定对应访问的源IP的AKSK请求，持续5分钟。</li></ul>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p87781732115313"><a name="p87781732115313"></a><a name="p87781732115313"></a>-</p>
</td>
</tr>
<tr id="row856217512326"><td class="cellrowborder" valign="top" width="18.51185118511851%" headers="mcps1.2.4.1.1 "><p id="p3254718185715"><a name="p3254718185715"></a><a name="p3254718185715"></a>Region</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.2.4.1.2 "><p id="p18251173415715"><a name="p18251173415715"></a><a name="p18251173415715"></a>区域名称。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p1563110552585"><a name="p1563110552585"></a><a name="p1563110552585"></a>cn-north-1</p>
</td>
</tr>
<tr id="row14629182212575"><td class="cellrowborder" valign="top" width="18.51185118511851%" headers="mcps1.2.4.1.1 "><p id="p19630122135714"><a name="p19630122135714"></a><a name="p19630122135714"></a>Cloud</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.2.4.1.2 "><p id="p8630172215574"><a name="p8630172215574"></a><a name="p8630172215574"></a>云平台域名。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p1163015226572"><a name="p1163015226572"></a><a name="p1163015226572"></a>myhuaweicloud.com</p>
</td>
</tr>
</tbody>
</table>

