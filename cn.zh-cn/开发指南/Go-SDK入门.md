# Go SDK入门<a name="sdk_03_0002"></a>

欢迎使用华为云开发者工具套件（Go SDK）。Go SDK让您轻松编程即可访问云服务。

本教程介绍如何安装和使用Go SDK，并提供示例，方便您快速入门。

我们支持的Go SDK基于Gophercloud开发。

## 支持的云服务列表<a name="section17155134542410"></a>

Go SDK支持的云服务产品如下：

-   [弹性云服务器 ECS](ECS-Go-SDK用户指导.md)
-   [云硬盘 EVS](EVS-Go-SDK用户指导.md)
-   [虚拟私有云 VPC](VPC-Go-SDK用户指导.md)
-   [统一身份认证 IAM](IAM-Go-SDK用户指导.md)
-   [镜像服务 IMS](IMS-Go-SDK用户指导.md)
-   [弹性负载均衡 ELB](ELB-Go-SDK用户指导.md)
-   [弹性伸缩 AS](AS-Go-SDK用户指导.md)
-   [运营能力 BSS](BSS-Python-SDK示例.md)

## 前提条件<a name="section6648223"></a>

1.  已经申请到云平台账号，并开通所需的服务。
2.  使用Go SDK时，推荐使用Go 1.9.1版本。

## SDK获取和安装<a name="section55709224162346"></a>

请从GitHub上获取Go SDK源代码：

[https://github.com/huaweicloud/huaweicloud-sdk-release/tree/master/go-sdk](https://github.com/huaweicloud/huaweicloud-sdk-release/tree/master/go-sdk)

在Linux系统上进行安装：

安装前，必须确保GOPATH环境变量指向待安装Gophercloud的目标目录：

```
mkdir $HOME/go
mkdir -p $HOME/go/src
export GOPATH=$HOME/go
```

下载源代码，解压安装到go的src目录下，然后执行go build 命令：

```
# unzip source code
unzip -d $GOPATH/src xxxxxx.zip
#run go build 
cd $GOPATH/src/github.com/gophercloud/gophercloud
go build 
```

## 开始使用<a name="section173333918515"></a>

配置相关的参数，完成认证，然后就可以调用SDK来访问服务的API。参数详情请参考[表1](#table4561115173218)。

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

<a name="table4561115173218"></a>
<table><thead align="left"><tr id="row12561105113219"><th class="cellrowborder" valign="top" width="17.64176417641764%" id="mcps1.2.4.1.1"><p id="p195611252321"><a name="p195611252321"></a><a name="p195611252321"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="37.643764376437645%" id="mcps1.2.4.1.2"><p id="p456145133212"><a name="p456145133212"></a><a name="p456145133212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="44.71447144714472%" id="mcps1.2.4.1.3"><p id="p175619553214"><a name="p175619553214"></a><a name="p175619553214"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row175617593220"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="p155611355329"><a name="p155611355329"></a><a name="p155611355329"></a>IdentityEndpoint</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="p082312211563"><a name="p082312211563"></a><a name="p082312211563"></a>认证服务（IAM）的Endpoint。</p>
<p id="zh-cn_topic_0121671869_li10140171754817p0"><a name="zh-cn_topic_0121671869_li10140171754817p0"></a><a name="zh-cn_topic_0121671869_li10140171754817p0"></a>“https://iam.<em id="i86181317204018"><a name="i86181317204018"></a><a name="i86181317204018"></a>example</em>.com/v3”中的“example”为“区域.云平台域名”，参数详情可以访问<a href="https://developer.huaweicloud.com/endpoint" target="_blank" rel="noopener noreferrer">这里</a>了解。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p105621519321"><a name="p105621519321"></a><a name="p105621519321"></a>https://iam.cn-north-1.myhuaweicloud.com/v3</p>
</td>
</tr>
<tr id="row12948127133512"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="p9949147153520"><a name="p9949147153520"></a><a name="p9949147153520"></a>Username</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="p1094911703517"><a name="p1094911703517"></a><a name="p1094911703517"></a>IAM用户名。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p59491872353"><a name="p59491872353"></a><a name="p59491872353"></a>-</p>
</td>
</tr>
<tr id="row0606191011354"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="p4607010193512"><a name="p4607010193512"></a><a name="p4607010193512"></a>Password</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="p126071410143517"><a name="p126071410143517"></a><a name="p126071410143517"></a>IAM用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p12607610133518"><a name="p12607610133518"></a><a name="p12607610133518"></a>-</p>
</td>
</tr>
<tr id="row1656275163214"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="p993913484"><a name="p993913484"></a><a name="p993913484"></a>ProjectID</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="p664771152820"><a name="p664771152820"></a><a name="p664771152820"></a>项目ID。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p2056295203213"><a name="p2056295203213"></a><a name="p2056295203213"></a>-</p>
</td>
</tr>
<tr id="row856217512326"><td class="cellrowborder" valign="top" width="17.64176417641764%" headers="mcps1.2.4.1.1 "><p id="p656217518325"><a name="p656217518325"></a><a name="p656217518325"></a>DomainID</p>
</td>
<td class="cellrowborder" valign="top" width="37.643764376437645%" headers="mcps1.2.4.1.2 "><p id="p856285113212"><a name="p856285113212"></a><a name="p856285113212"></a>账号ID。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p25628523215"><a name="p25628523215"></a><a name="p25628523215"></a>-</p>
</td>
</tr>
</tbody>
</table>

