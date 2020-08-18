# Python SDK认证方式<a name="sdk_02_0005"></a>

Python SDK支持两种认证方式：token认证和AK/SK认证。

## token认证<a name="section1468872013368"></a>

token认证方式示例代码，参数详情请参考[表1](#table132650108153)。

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

<a name="table132650108153"></a>
<table><thead align="left"><tr id="sdk_02_0002_row12561105113219"><th class="cellrowborder" valign="top" width="15.901590159015901%" id="mcps1.2.4.1.1"><p id="sdk_02_0002_p195611252321"><a name="sdk_02_0002_p195611252321"></a><a name="sdk_02_0002_p195611252321"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="39.38393839383938%" id="mcps1.2.4.1.2"><p id="sdk_02_0002_p456145133212"><a name="sdk_02_0002_p456145133212"></a><a name="sdk_02_0002_p456145133212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="44.71447144714472%" id="mcps1.2.4.1.3"><p id="sdk_02_0002_p175619553214"><a name="sdk_02_0002_p175619553214"></a><a name="sdk_02_0002_p175619553214"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="sdk_02_0002_row175617593220"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="sdk_02_0002_p791817161131"><a name="sdk_02_0002_p791817161131"></a><a name="sdk_02_0002_p791817161131"></a>auth_url</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="sdk_02_0002_p082312211563"><a name="sdk_02_0002_p082312211563"></a><a name="sdk_02_0002_p082312211563"></a>认证服务（IAM）的Endpoint。</p>
<p id="sdk_02_0002_zh-cn_topic_0121671869_li10140171754817p0"><a name="sdk_02_0002_zh-cn_topic_0121671869_li10140171754817p0"></a><a name="sdk_02_0002_zh-cn_topic_0121671869_li10140171754817p0"></a>“https://iam.<em id="sdk_02_0002_i86181317204018"><a name="sdk_02_0002_i86181317204018"></a><a name="sdk_02_0002_i86181317204018"></a>example</em>.com/v3”中的“example”为“区域.云平台域名”，参数详情可以访问<a href="https://developer.huaweicloud.com/endpoint" target="_blank" rel="noopener noreferrer">这里</a>了解。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_02_0002_p105621519321"><a name="sdk_02_0002_p105621519321"></a><a name="sdk_02_0002_p105621519321"></a>https://iam.cn-north-1.myhuaweicloud.com/v3</p>
</td>
</tr>
<tr id="sdk_02_0002_row15341439173619"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="sdk_02_0002_p1335739143615"><a name="sdk_02_0002_p1335739143615"></a><a name="sdk_02_0002_p1335739143615"></a>username</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="sdk_02_0002_p035113933616"><a name="sdk_02_0002_p035113933616"></a><a name="sdk_02_0002_p035113933616"></a>IAM用户名。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_02_0002_p193510394368"><a name="sdk_02_0002_p193510394368"></a><a name="sdk_02_0002_p193510394368"></a>-</p>
</td>
</tr>
<tr id="sdk_02_0002_row1412173620369"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="sdk_02_0002_p5413183633617"><a name="sdk_02_0002_p5413183633617"></a><a name="sdk_02_0002_p5413183633617"></a>password</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="sdk_02_0002_p241353603618"><a name="sdk_02_0002_p241353603618"></a><a name="sdk_02_0002_p241353603618"></a>IAM用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_02_0002_p541383613368"><a name="sdk_02_0002_p541383613368"></a><a name="sdk_02_0002_p541383613368"></a>-</p>
</td>
</tr>
<tr id="sdk_02_0002_row1656275163214"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="sdk_02_0002_p993913484"><a name="sdk_02_0002_p993913484"></a><a name="sdk_02_0002_p993913484"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="sdk_02_0002_p664771152820"><a name="sdk_02_0002_p664771152820"></a><a name="sdk_02_0002_p664771152820"></a>项目ID。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_02_0002_p2056295203213"><a name="sdk_02_0002_p2056295203213"></a><a name="sdk_02_0002_p2056295203213"></a>-</p>
</td>
</tr>
<tr id="sdk_02_0002_row856217512326"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="sdk_02_0002_p656217518325"><a name="sdk_02_0002_p656217518325"></a><a name="sdk_02_0002_p656217518325"></a>userDomainId</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="sdk_02_0002_p856285113212"><a name="sdk_02_0002_p856285113212"></a><a name="sdk_02_0002_p856285113212"></a>账号ID。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="sdk_02_0002_p25628523215"><a name="sdk_02_0002_p25628523215"></a><a name="sdk_02_0002_p25628523215"></a>-</p>
</td>
</tr>
</tbody>
</table>

## AK/SK认证<a name="section43591440365"></a>

AK/SK认证方式示例代码，参数详情请参考[表2](#table4561115173218)。

```
#encoding=utf-8

from openstack import connection

projectId = "***"
cloud = "myhuaweicloud.com"
region= "***"    # example: region = "cn-north-1"
AK = "***"
SK = "***"

conn = connection.Connection(
              project_id=projectId,
              cloud=cloud,
              region=region,
              ak = AK,
              sk = SK)

def test_compute():
    servers = conn.compute.servers(limit = 3)
    for server in servers:
        print server

if __name__ == "__main__":
    test_compute()
```

**表 2**  参数说明

<a name="table4561115173218"></a>
<table><thead align="left"><tr id="row12561105113219"><th class="cellrowborder" valign="top" width="15.901590159015901%" id="mcps1.2.4.1.1"><p id="p195611252321"><a name="p195611252321"></a><a name="p195611252321"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="39.38393839383938%" id="mcps1.2.4.1.2"><p id="p456145133212"><a name="p456145133212"></a><a name="p456145133212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="44.71447144714472%" id="mcps1.2.4.1.3"><p id="p175619553214"><a name="p175619553214"></a><a name="p175619553214"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row175617593220"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p88021832125310"><a name="p88021832125310"></a><a name="p88021832125310"></a>ak/sk</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p20367134212540"><a name="p20367134212540"></a><a name="p20367134212540"></a>AK/SK访问密钥。</p>
<div class="note" id="note1564918718544"><a name="note1564918718544"></a><a name="note1564918718544"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul161113510548"></a><a name="ul161113510548"></a><ul id="ul161113510548"><li>AK/SK生成说明：登录控制台，进入“我的凭证”，点击“管理访问密钥”创建AK/SK。</li><li>AK/SK签名时间与UTC时间误差不可以超过15分钟，否则会鉴权失败。</li><li>AK/SK签名连续失败超过5次，将锁定对应访问的源IP的AK/SK请求，持续5分钟。</li></ul>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p87781732115313"><a name="p87781732115313"></a><a name="p87781732115313"></a>-</p>
</td>
</tr>
<tr id="row1656275163214"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p993913484"><a name="p993913484"></a><a name="p993913484"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p664771152820"><a name="p664771152820"></a><a name="p664771152820"></a>项目ID。如何获取项目ID请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p2056295203213"><a name="p2056295203213"></a><a name="p2056295203213"></a>-</p>
</td>
</tr>
<tr id="row856217512326"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p3254718185715"><a name="p3254718185715"></a><a name="p3254718185715"></a>region</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p18251173415715"><a name="p18251173415715"></a><a name="p18251173415715"></a>区域名称。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p1563110552585"><a name="p1563110552585"></a><a name="p1563110552585"></a>cn-north-1</p>
</td>
</tr>
<tr id="row14629182212575"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p16785101918461"><a name="p16785101918461"></a><a name="p16785101918461"></a>cloud</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p8630172215574"><a name="p8630172215574"></a><a name="p8630172215574"></a>云平台域名。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p1163015226572"><a name="p1163015226572"></a><a name="p1163015226572"></a>myhuaweicloud.com</p>
</td>
</tr>
</tbody>
</table>

