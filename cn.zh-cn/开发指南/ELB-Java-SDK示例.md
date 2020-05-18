# ELB Java SDK示例<a name="sdk_01_0021"></a>

SDK与RESTful API一一对应，SDK最新版本支持的接口列表，以及SDK和API的对应关系，请参考[这里](Java-ELB.md)。

在使用ELB SDK的时候，SDK支持的参数细节，请参考ELB API[描述](https://support.huaweicloud.com/api-elb/zh-cn_topic_0022480177.html)。

增强型负载均衡ELB v2 Java SDK支持如下资源对象的操作，资源对象的“增改查删”代码示例如下：

<a name="table136501831193114"></a>
<table><thead align="left"><tr id="row1285453112317"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="p11854113103110"><a name="p11854113103110"></a><a name="p11854113103110"></a>资源对象</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="p12854143123117"><a name="p12854143123117"></a><a name="p12854143123117"></a>“增改查删”代码样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row10854331133111"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p885418316318"><a name="p885418316318"></a><a name="p885418316318"></a>loadbalancer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1785463153113"><a name="p1785463153113"></a><a name="p1785463153113"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/Loadbalancer.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row28541314313"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p485418312316"><a name="p485418312316"></a><a name="p485418312316"></a>listener</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p985423110319"><a name="p985423110319"></a><a name="p985423110319"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/Listener.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1185420311312"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1685483117318"><a name="p1685483117318"></a><a name="p1685483117318"></a>pool</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p168553317319"><a name="p168553317319"></a><a name="p168553317319"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/Pool.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1285503143116"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p985573103118"><a name="p985573103118"></a><a name="p985573103118"></a>member</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p78552312312"><a name="p78552312312"></a><a name="p78552312312"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/Member.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row158551831113120"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p11855103193119"><a name="p11855103193119"></a><a name="p11855103193119"></a>healthmonitor</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p485563123117"><a name="p485563123117"></a><a name="p485563123117"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/Healthmonitor.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row3855731183112"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p48556318312"><a name="p48556318312"></a><a name="p48556318312"></a>certificate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1285514312315"><a name="p1285514312315"></a><a name="p1285514312315"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/Certificate.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row58558310317"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p12855113163115"><a name="p12855113163115"></a><a name="p12855113163115"></a>whitelist</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p15855193116319"><a name="p15855193116319"></a><a name="p15855193116319"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/Whitelist.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1985543110314"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1585583113312"><a name="p1585583113312"></a><a name="p1585583113312"></a>l7policy</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p3855143111314"><a name="p3855143111314"></a><a name="p3855143111314"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/L7policy.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1885583119319"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1285513313318"><a name="p1285513313318"></a><a name="p1285513313318"></a>l7rule</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p12855123110312"><a name="p12855123110312"></a><a name="p12855123110312"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v2/L7rule.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
</tbody>
</table>

经典型负载均衡ELB v1 Java SDK支持如下资源对象的操作，资源对象的“增改查删”代码示例如下：

<a name="table1167963119319"></a>
<table><thead align="left"><tr id="row208554311319"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="p38552031203114"><a name="p38552031203114"></a><a name="p38552031203114"></a>资源对象</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="p1785515315313"><a name="p1785515315313"></a><a name="p1785515315313"></a>“增改查删”代码样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row1585514311319"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p20855203173119"><a name="p20855203173119"></a><a name="p20855203173119"></a>loadbalancer</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1085513317312"><a name="p1085513317312"></a><a name="p1085513317312"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v1/ClassicLoadbalancer.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1185518312317"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p13855203118315"><a name="p13855203118315"></a><a name="p13855203118315"></a>listener</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p17855631153110"><a name="p17855631153110"></a><a name="p17855631153110"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v1/ClassicListener.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1485523111318"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1585543119314"><a name="p1585543119314"></a><a name="p1585543119314"></a>member</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1185514319319"><a name="p1185514319319"></a><a name="p1185514319319"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v1/ClassicMember.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1855123118318"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p685583173111"><a name="p685583173111"></a><a name="p685583173111"></a>healthcheck</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p2085513193117"><a name="p2085513193117"></a><a name="p2085513193117"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v1/ClassicHealthcheck.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1085517314314"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p3855143116312"><a name="p3855143116312"></a><a name="p3855143116312"></a>certificate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1485593114314"><a name="p1485593114314"></a><a name="p1485593114314"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-java/blob/master/examples/elb/v1/ClassicCertificate.java" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
</tbody>
</table>

