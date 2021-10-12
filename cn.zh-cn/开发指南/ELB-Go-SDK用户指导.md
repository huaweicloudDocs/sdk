# ELB Go SDK用户指导<a name="sdk_03_0019"></a>

SDK与RESTful API一一对应，SDK最新版本支持的接口列表，以及SDK和API的对应关系，请参考[A.2.9 ELB](GO-ELB.md)。

在使用ELB SDK的时候，SDK支持的参数细节，请参考ELB API[描述](https://support.huaweicloud.com/api-elb/zh-cn_topic_0022480177.html)。

增强型负载均衡ELB v2 Go SDK支持如下资源对象的操作，资源对象的“增改查删”代码示例如下：

<a name="table1827067191917"></a>
<table><thead align="left"><tr id="row1239047151914"><th class="cellrowborder" valign="top" width="32.25%" id="mcps1.1.3.1.1"><p id="p1839057171910"><a name="p1839057171910"></a><a name="p1839057171910"></a>资源对象</p>
</th>
<th class="cellrowborder" valign="top" width="67.75%" id="mcps1.1.3.1.2"><p id="p1039217171913"><a name="p1039217171913"></a><a name="p1039217171913"></a>“增改查删”代码样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row2039217201917"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p173921731920"><a name="p173921731920"></a><a name="p173921731920"></a>loadbalacner</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p5392177131912"><a name="p5392177131912"></a><a name="p5392177131912"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/loadbalancer.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row18392674191"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p1539297171916"><a name="p1539297171916"></a><a name="p1539297171916"></a>listener</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p639237191911"><a name="p639237191911"></a><a name="p639237191911"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/listener.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row03925741913"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p1639297151916"><a name="p1639297151916"></a><a name="p1639297151916"></a>pool</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p439297201919"><a name="p439297201919"></a><a name="p439297201919"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/pool.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row439219712195"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p5392379191"><a name="p5392379191"></a><a name="p5392379191"></a>member</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p163925751913"><a name="p163925751913"></a><a name="p163925751913"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/member.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row16392207131915"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p1539216712196"><a name="p1539216712196"></a><a name="p1539216712196"></a>healthmonitor</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p1339211751918"><a name="p1339211751918"></a><a name="p1339211751918"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/healthmonitor.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row183926716196"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p17392197131910"><a name="p17392197131910"></a><a name="p17392197131910"></a>certificate</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p12392176197"><a name="p12392176197"></a><a name="p12392176197"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/certificate.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row939215791918"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p14392167121910"><a name="p14392167121910"></a><a name="p14392167121910"></a>l7policy</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p1339277191919"><a name="p1339277191919"></a><a name="p1339277191919"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/policy.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row203933710195"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p43939719190"><a name="p43939719190"></a><a name="p43939719190"></a>l7rule</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p739320731913"><a name="p739320731913"></a><a name="p739320731913"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/rule.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1139387131916"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p173932071196"><a name="p173932071196"></a><a name="p173932071196"></a>whitelist</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p13934712193"><a name="p13934712193"></a><a name="p13934712193"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/elb/v2/whitelist.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
</tbody>
</table>

