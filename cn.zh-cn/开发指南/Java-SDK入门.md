# Java SDK入门<a name="sdk_01_0002"></a>

欢迎使用华为云开发者工具套件（Java SDK）。Java SDK让您轻松编程即可访问云服务。

本教程介绍如何安装和使用Java SDK，并提供示例，方便您快速入门。

我们支持的Java SDK基于OpenStack4j开发。

## 支持的云服务列表<a name="section17155134542410"></a>

Java SDK支持的云服务产品如下：

-   [统一身份认证 IAM](IAM-Java-SDK示例.md)
-   [镜像服务 IMS](IMS-Java-SDK示例.md)
-   [虚拟私有云 VPC](VPC-Java-SDK示例.md)
-   [弹性云服务器 ECS](ECS-Java-SDK示例.md)
-   [云硬盘 EVS](EVS-Java-SDK示例.md)
-   [弹性伸缩 AS](AS-Java-SDK示例.md)
-   [云监控服务 CES](CES-Java-SDK示例.md)
-   [云解析服务 DNS](DNS-Java-SDK示例.md)
-   [弹性负载均衡 ELB](ELB-Java-SDK示例.md)
-   [云硬盘备份 VBS](VBS-Java-SDK示例.md)
-   [云审计服务 CTS](CTS-Java-SDK示例.md)
-   [数据加密服务 KMS](KMS-Java-SDK示例.md)
-   [流量清洗Anti-DDoS](Anti-DDoS-Java-SDK示例.md)
-   [分布式消息服务 DMS](DMS-Java-SDK示例.md)
-   [MapReduce服务 MRS](MRS-Java-SDK示例.md)
-   [内容分发网络 CDN](CDN-Java-SDK示例.md)
-   [运营能力 BSS](BSS-Java-SDK示例.md)
-   [标签管理服务 TMS](TMS-Java-SDK示例.md)
-   [企业管理 EPS](EPS-Java-SDK示例.md)
-   [云数据库 RDS](RDS-Java-SDK示例.md)

## 前提条件<a name="section8152279"></a>

1.  已经申请到云平台账号，并开通所需的云服务。
2.  已经安装好JDK，Java SDK适用于 JDK1.8和以上版本，我们建议您使用 JDK1.8。

## SDK获取和安装<a name="section44512540161625"></a>

通过在pom.xml文件中添加以下Maven依赖安装Java SDK。

```
<dependency>
<groupId>com.huawei</groupId>
<artifactId>openstack4j</artifactId>
<version>1.0.12</version>
</dependency>
```

Java SDK支持的最新版本，请在[这儿](https://mvnrepository.com/artifact/com.huawei/openstack4j)查询。

本文档中涉及的服务使用同一个JAR文件。

## 开始使用<a name="section15818615161648"></a>

设置参数，初始化SDK客户端，然后调用SDK访问服务的API。参数详情请参考[表1](#table4561115173218)。

```
package demo;

import java.util.HashMap;
import java.util.List;
import java.util.Map;

import com.huawei.openstack4j.openstack.OSFactory;
import com.huawei.openstack4j.api.OSClient.OSClientV3;
import com.huawei.openstack4j.core.transport.Config;
import com.huawei.openstack4j.model.common.Identifier;
import com.huawei.openstack4j.model.compute.Server;

public class Demo {
    public static void main(String[] args) {
        //设置认证参数
        String authUrl = "https://iam.example.com/v3";//endpointUrl
        String user = "replace-with-your-username";//用户名
        String password = "replace-with-your-password";//用户密码
        String projectId = "replace-with-your-projectId";//项目ID
        String userDomainId = "replace-with-your-domainId";//账号ID

        //初始化client
        OSClientV3 os = OSFactory.builderV3()
                .endpoint(authUrl)
                .credentials(user, password, Identifier.byId(userDomainId))
                .scopeToProject(Identifier.byId(projectId)).authenticate();

        //设置查询参数
        Map<String, String> filter = new HashMap<String, String>();

        //将需要输入的参数都放入filter里面
        filter.put("limit", "3");

        //调用查询虚拟机列表的接口
        List<? extends Server> serverList = os.compute().servers().list(filter);
        if (serverList.size() > 0) {
            System.out.println("get serverList success, size = " + serverList.size());
            for (Server server : serverList) {
                System.out.println(server);
            }
        } else {
            System.out.println("no server exists.");
        }
    }
}
```

**表 1**  参数说明

<a name="table4561115173218"></a>
<table><thead align="left"><tr id="row12561105113219"><th class="cellrowborder" valign="top" width="15.91159115911591%" id="mcps1.2.4.1.1"><p id="p195611252321"><a name="p195611252321"></a><a name="p195611252321"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="39.373937393739375%" id="mcps1.2.4.1.2"><p id="p456145133212"><a name="p456145133212"></a><a name="p456145133212"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="44.71447144714472%" id="mcps1.2.4.1.3"><p id="p175619553214"><a name="p175619553214"></a><a name="p175619553214"></a>取值样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row175617593220"><td class="cellrowborder" valign="top" width="15.91159115911591%" headers="mcps1.2.4.1.1 "><p id="p155611355329"><a name="p155611355329"></a><a name="p155611355329"></a>authUrl</p>
</td>
<td class="cellrowborder" valign="top" width="39.373937393739375%" headers="mcps1.2.4.1.2 "><p id="p082312211563"><a name="p082312211563"></a><a name="p082312211563"></a>认证服务（IAM）的Endpoint。</p>
<p id="zh-cn_topic_0121671869_li10140171754817p0"><a name="zh-cn_topic_0121671869_li10140171754817p0"></a><a name="zh-cn_topic_0121671869_li10140171754817p0"></a>“https://iam.<em id="i86181317204018"><a name="i86181317204018"></a><a name="i86181317204018"></a>example</em>.com/v3”中的“example”为“区域.云平台域名”，参数详情可以访问<a href="https://developer.huaweicloud.com/endpoint?iam" target="_blank" rel="noopener noreferrer">这里</a>了解。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p105621519321"><a name="p105621519321"></a><a name="p105621519321"></a>https://iam.cn-north-1.myhuaweicloud.com/v3</p>
</td>
</tr>
<tr id="row4367755920"><td class="cellrowborder" valign="top" width="15.91159115911591%" headers="mcps1.2.4.1.1 "><p id="p193691159910"><a name="p193691159910"></a><a name="p193691159910"></a>user</p>
</td>
<td class="cellrowborder" valign="top" width="39.373937393739375%" headers="mcps1.2.4.1.2 "><p id="p636905892"><a name="p636905892"></a><a name="p636905892"></a>IAM用户名。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p8369255915"><a name="p8369255915"></a><a name="p8369255915"></a>-</p>
</td>
</tr>
<tr id="row167262017593"><td class="cellrowborder" valign="top" width="15.91159115911591%" headers="mcps1.2.4.1.1 "><p id="p20726517093"><a name="p20726517093"></a><a name="p20726517093"></a>password</p>
</td>
<td class="cellrowborder" valign="top" width="39.373937393739375%" headers="mcps1.2.4.1.2 "><p id="p15726201718910"><a name="p15726201718910"></a><a name="p15726201718910"></a>IAM用户密码。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p18726111717917"><a name="p18726111717917"></a><a name="p18726111717917"></a>-</p>
</td>
</tr>
<tr id="row1656275163214"><td class="cellrowborder" valign="top" width="15.91159115911591%" headers="mcps1.2.4.1.1 "><p id="p993913484"><a name="p993913484"></a><a name="p993913484"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="39.373937393739375%" headers="mcps1.2.4.1.2 "><p id="p664771152820"><a name="p664771152820"></a><a name="p664771152820"></a>项目ID。如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p2056295203213"><a name="p2056295203213"></a><a name="p2056295203213"></a>-</p>
</td>
</tr>
<tr id="row856217512326"><td class="cellrowborder" valign="top" width="15.91159115911591%" headers="mcps1.2.4.1.1 "><p id="p656217518325"><a name="p656217518325"></a><a name="p656217518325"></a>userDomainId</p>
</td>
<td class="cellrowborder" valign="top" width="39.373937393739375%" headers="mcps1.2.4.1.2 "><p id="p856285113212"><a name="p856285113212"></a><a name="p856285113212"></a><span>账号ID。</span>如何获取，请参考<a href="如何获取IAM-用户名-账号ID以及项目ID.md">如何获取IAM 用户名、账号ID以及项目ID？</a>。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p25628523215"><a name="p25628523215"></a><a name="p25628523215"></a>-</p>
</td>
</tr>
</tbody>
</table>

