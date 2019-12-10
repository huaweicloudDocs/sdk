# Python 入门<a name="ZH-CN_TOPIC_0070637133"></a>

欢迎使用华为云开发者工具套件（Python SDK）。Python SDK让您轻松编程即可访问云服务。

本教程介绍如何安装和使用Python SDK，并提供示例，方便您快速入门。

我们支持的Python SDK基于Python OpenStack SDK开发。

## 支持的云服务列表<a name="section17155134542410"></a>

Python SDK支持的云服务产品如下：

<a name="table1848320466268"></a>
<table><tbody><tr id="row048394632610"><td class="cellrowborder" valign="top" width="33.463346334633464%"><p id="p548314642615"><a name="p548314642615"></a><a name="p548314642615"></a><a href="IAM-Python-SDK示例.md">统一身份认证 IAM</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.2033203320332%"><p id="p15483746112620"><a name="p15483746112620"></a><a name="p15483746112620"></a><a href="IMS-Python-SDK示例.md">镜像服务 IMS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%"><p id="p184834466266"><a name="p184834466266"></a><a name="p184834466266"></a><a href="VPC-Python-SDK示例.md">虚拟私有云 VPC</a></p>
</td>
</tr>
<tr id="row848314616261"><td class="cellrowborder" valign="top" width="33.463346334633464%"><p id="p8483154672611"><a name="p8483154672611"></a><a name="p8483154672611"></a><a href="ECS-Python-SDK示例.md">弹性云服务器 ECS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.2033203320332%"><p id="p7483546112619"><a name="p7483546112619"></a><a name="p7483546112619"></a><a href="EVS-Python-SDK示例.md">云硬盘 EVS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%"><p id="p348313467267"><a name="p348313467267"></a><a name="p348313467267"></a><a href="RTS-Python-SDK示例.md">资源模板服务 RTS</a></p>
</td>
</tr>
<tr id="row0483114672619"><td class="cellrowborder" valign="top" width="33.463346334633464%"><p id="p6483646192611"><a name="p6483646192611"></a><a name="p6483646192611"></a><a href="AS-Python-SDK示例.md">弹性伸缩 AS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.2033203320332%"><p id="p134831346172620"><a name="p134831346172620"></a><a name="p134831346172620"></a><a href="CES-Python-SDK示例.md">云监控服务 CES</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%"><p id="p1848384618269"><a name="p1848384618269"></a><a name="p1848384618269"></a><a href="DNS-Python-SDK示例.md">云解析服务 DNS</a></p>
</td>
</tr>
<tr id="row12483246172614"><td class="cellrowborder" valign="top" width="33.463346334633464%"><p id="p1348344616268"><a name="p1348344616268"></a><a name="p1348344616268"></a><a href="ELB-Python-SDK示例.md">弹性负载均衡 ELB</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.2033203320332%"><p id="p648416460264"><a name="p648416460264"></a><a name="p648416460264"></a><a href="VBS-Python-SDK示例.md">云硬盘备份 VBS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%"><p id="p116943934313"><a name="p116943934313"></a><a name="p116943934313"></a><a href="KMS-Python-SDK示例.md">数据加密服务 KMS</a></p>
</td>
</tr>
<tr id="row1448484632611"><td class="cellrowborder" valign="top" width="33.463346334633464%"><p id="p104845462264"><a name="p104845462264"></a><a name="p104845462264"></a><a href="Anti-DDoS-Python-SDK示例.md">流量清洗Anti-DDoS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.2033203320332%"><p id="p94841746142617"><a name="p94841746142617"></a><a name="p94841746142617"></a><a href="DMS-Python-SDK示例.md">分布式消息服务 DMS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%"><p id="p3484346192613"><a name="p3484346192613"></a><a name="p3484346192613"></a><a href="MRS-Python-SDK示例.md">MapReduce服务 MRS</a></p>
</td>
</tr>
<tr id="row11484946192618"><td class="cellrowborder" valign="top" width="33.463346334633464%"><p id="p76902021442"><a name="p76902021442"></a><a name="p76902021442"></a><a href="RDS-Python-SDK示例.md">关系型数据库 RDS</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.2033203320332%"><p id="p174841446102618"><a name="p174841446102618"></a><a name="p174841446102618"></a><a href="CDN-Python-SDK示例.md">内容分发网络 CDN</a></p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%"><p id="p691116832412"><a name="p691116832412"></a><a name="p691116832412"></a>-</p>
</td>
</tr>
</tbody>
</table>

## 前提条件<a name="section6648223"></a>

1.  已经申请到云平台账号，并开通所需的云服务。
2.  已经安装好Python、pip和git，Python SDK适用于 Python 2.7.10-2.7.15 和 3.4-3.7 系列版本。

## SDK获取和安装<a name="section55709224162346"></a>

使用pip安装，请执行以下命令：

**pip install huaweicloud-sdk**-python****

## 开始使用<a name="section65075345162437"></a>

设置参数，创建连接\(Connection\)，然后调用SDK来访问服务的API。参数详情请参考[表1](#table4561115173218)。

```
# -*- coding:utf-8 -*-
from openstack import connection

# create connection
username = "replace-with-your-username"    #用户名称
password = "replace-with-your-password"    #用户密码
projectId = "replace-with-your-projectId"    #项目ID
userDomainId = "replace-with-your-domainId"  #账户ID
auth_url = "https://iam.example.com/v3"    # endpoint url
conn = connection.Connection(auth_url=auth_url,
                             user_domain_id=userDomainId,
                             project_id=projectId,
                             username=username,
                             password=password)

# set parameters
limit = 5

# define function for listing servers
def list_servers():
    # get server list with params
    servers = conn.compute.servers(limit=limit)
    # iterate servers list
    for server in servers:
        print(server)

# visit API
list_servers()
```

**表 1**  参数说明

<a name="table4561115173218"></a>
<table><thead align="left"><tr id="row12561105113219"><th class="cellrowborder" valign="top" width="15.901590159015901%" id="mcps1.2.4.1.1"><p id="p195611252321"><a name="p195611252321"></a><a name="p195611252321"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="39.38393839383938%" id="mcps1.2.4.1.2"><p id="p456145133212"><a name="p456145133212"></a><a name="p456145133212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="44.71447144714472%" id="mcps1.2.4.1.3"><p id="p175619553214"><a name="p175619553214"></a><a name="p175619553214"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row175617593220"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p791817161131"><a name="p791817161131"></a><a name="p791817161131"></a>auth_url</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p082312211563"><a name="p082312211563"></a><a name="p082312211563"></a>认证服务（IAM）的Endpoint。</p>
<p id="zh-cn_topic_0121671869_li10140171754817p0"><a name="zh-cn_topic_0121671869_li10140171754817p0"></a><a name="zh-cn_topic_0121671869_li10140171754817p0"></a>“https://iam.<em id="i86181317204018"><a name="i86181317204018"></a><a name="i86181317204018"></a>example</em>.com/v3”中的“example”为“区域.云平台域名”，参数详情可以访问<a href="https://developer.huaweicloud.com/endpoint" target="_blank" rel="noopener noreferrer">这里</a>了解。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p105621519321"><a name="p105621519321"></a><a name="p105621519321"></a>https://iam.cn-north-1.myhuaweicloud.com/v3</p>
</td>
</tr>
<tr id="row1656275163214"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p993913484"><a name="p993913484"></a><a name="p993913484"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p664771152820"><a name="p664771152820"></a><a name="p664771152820"></a>项目ID。如何获取项目ID请参考<a href="如何获取domain_name-project_name和project_id.md">如何获取domain_name、project_name和project_id ?</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p2056295203213"><a name="p2056295203213"></a><a name="p2056295203213"></a>-</p>
</td>
</tr>
<tr id="row856217512326"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p656217518325"><a name="p656217518325"></a><a name="p656217518325"></a>userDomainId</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p856285113212"><a name="p856285113212"></a><a name="p856285113212"></a>账号ID。如何获取账号ID请参考<a href="如何获取domain_name-project_name和project_id.md">如何获取domain_name、project_name和project_id ?</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p25628523215"><a name="p25628523215"></a><a name="p25628523215"></a>-</p>
</td>
</tr>
</tbody>
</table>

