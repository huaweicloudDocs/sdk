# Java 认证方式<a name="ZH-CN_TOPIC_0111232097"></a>

Java SDK支持两种认证方式：token认证和AK/SK认证。

## token认证<a name="section0702046201112"></a>

token认证方式示例代码，请参考“[入门](Java-入门.md)”。

token具有24小时有效期，如果您的程序运行时间超过24小时，在使用SDK调用API之前，建议您在程序中重新申请一次token，方法如下：

```
import com.huawei.openstack4j.openstack.OSFactory;
OSFactory.refreshToken();
```

## AK/SK认证<a name="section199482591210"></a>

AK/SK认证方式示例代码，参数详情请参考[表1](#table4561115173218)。

```
package demo;

import java.util.HashMap;
import java.util.List;
import java.util.Map;

import com.huawei.openstack4j.api.OSClient.OSClientAKSK;
import com.huawei.openstack4j.core.transport.Config;
import com.huawei.openstack4j.model.compute.Server;
import com.huawei.openstack4j.openstack.OSFactory;

public class Demo {
 
 public static void main(String[] args) {
 
  // 设置认证参数
  String ak = "replace-your-ak";
  String sk = "replace-your-sk";
  String projectId = "replace-your-projectId";
  String region = "replace-your-region"; //example: region = "cn-north-1"
  String cloud = "myhuaweicloud.com";
 
  OSClientAKSK osclient = OSFactory.builderAKSK().credentials(ak, sk, region, projectId, cloud) .authenticate();
 
  // 设置查询参数
  Map<String , String> filter = new HashMap<String, String>();
  // 将需要输入的参数都放入filter里面
  filter.put("limit", "3");
  
  // 调用查询虚拟机列表的接口
  List<? extends Server> serverList = osclient.compute().servers().list(filter);
  if(serverList.size() > 0) 
  {
   System.out.println("get serverList success, size = " + serverList.size());
   for (Server server : serverList) {
    System.out.println(server);
   }
  } 
  else {
   System.out.println("no server exists.");
  }
 }
}
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
<tbody><tr id="row175617593220"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p88021832125310"><a name="p88021832125310"></a><a name="p88021832125310"></a>ak/sk</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p20367134212540"><a name="p20367134212540"></a><a name="p20367134212540"></a>AK/SK访问密钥。</p>
<div class="note" id="note1564918718544"><a name="note1564918718544"></a><a name="note1564918718544"></a><span class="notetitle"> 说明： </span><div class="notebody"><a name="ul161113510548"></a><a name="ul161113510548"></a><ul id="ul161113510548"><li>AK/SK生成说明：登录控制台，进入“我的凭证”，点击“管理访问密钥”创建AK/SK。</li><li>AK/SK签名时间与UTC时间误差不可以超过15分钟，否则会鉴权失败。</li><li>AK/SK签名连续失败超过5次，将锁定对应访问的源IP的AK/SK请求，持续5分钟。</li></ul>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p87781732115313"><a name="p87781732115313"></a><a name="p87781732115313"></a>-</p>
</td>
</tr>
<tr id="row1656275163214"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p993913484"><a name="p993913484"></a><a name="p993913484"></a>projectId</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p664771152820"><a name="p664771152820"></a><a name="p664771152820"></a>项目ID。如何获取项目ID请参考<a href="如何获取domain_name-project_name和project_id.md">如何获取domain_name、project_name和project_id ?</a>。</p>
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
<tr id="row14629182212575"><td class="cellrowborder" valign="top" width="15.901590159015901%" headers="mcps1.2.4.1.1 "><p id="p02557409242"><a name="p02557409242"></a><a name="p02557409242"></a>cloud</p>
</td>
<td class="cellrowborder" valign="top" width="39.38393839383938%" headers="mcps1.2.4.1.2 "><p id="p8630172215574"><a name="p8630172215574"></a><a name="p8630172215574"></a>云平台域名。</p>
</td>
<td class="cellrowborder" valign="top" width="44.71447144714472%" headers="mcps1.2.4.1.3 "><p id="p1163015226572"><a name="p1163015226572"></a><a name="p1163015226572"></a>myhuaweicloud.com</p>
</td>
</tr>
</tbody>
</table>

