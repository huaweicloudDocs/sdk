# VPC Go SDK用户指导<a name="sdk_03_0015"></a>

SDK与RESTful API一一对应，SDK最新版本支持的接口列表，以及SDK和API的对应关系，请参考[这里](Python-VPC.md)。

在使用VPC SDK的时候，SDK支持的参数细节，请参考VPC API[描述](https://support.huaweicloud.com/api-vpc/zh-cn_topic_0050065465.html)。

VPC v1 Go SDK支持如下资源对象的操作，资源对象的“增改查删”代码示例如下：

<a name="table621354644113"></a>
<table><thead align="left"><tr id="row15293846114110"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="p1829319468418"><a name="p1829319468418"></a><a name="p1829319468418"></a>资源对象</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="p2029318463417"><a name="p2029318463417"></a><a name="p2029318463417"></a>“增改查删”代码样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row152931446134114"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p17293134618411"><a name="p17293134618411"></a><a name="p17293134618411"></a>bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1129316467419"><a name="p1129316467419"></a><a name="p1129316467419"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/bandwidths.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row12938467412"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p729320469418"><a name="p729320469418"></a><a name="p729320469418"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p729314614417"><a name="p729314614417"></a><a name="p729314614417"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/ports.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row17293144634117"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p9293946134117"><a name="p9293946134117"></a><a name="p9293946134117"></a>private ip</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p122931846144119"><a name="p122931846144119"></a><a name="p122931846144119"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/privateips.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row16293204644111"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p16293144664119"><a name="p16293144664119"></a><a name="p16293144664119"></a>public ip</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p3293104634118"><a name="p3293104634118"></a><a name="p3293104634118"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/publicips.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row929344619412"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p2294946154116"><a name="p2294946154116"></a><a name="p2294946154116"></a>quota</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p16294546154110"><a name="p16294546154110"></a><a name="p16294546154110"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/quotas.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row2294124616415"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p11294184664119"><a name="p11294184664119"></a><a name="p11294184664119"></a>security group</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p429414616418"><a name="p429414616418"></a><a name="p429414616418"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/securitygroups.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row02942046144115"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p629420469417"><a name="p629420469417"></a><a name="p629420469417"></a>security group rule</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1329415468417"><a name="p1329415468417"></a><a name="p1329415468417"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/securitygrouprules.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row7294134611413"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1294114624117"><a name="p1294114624117"></a><a name="p1294114624117"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p162946468416"><a name="p162946468416"></a><a name="p162946468416"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/subnets.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row19294134613415"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p72941446164119"><a name="p72941446164119"></a><a name="p72941446164119"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p11294184610417"><a name="p11294184610417"></a><a name="p11294184610417"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/vpc/v1/vpcs.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
</tbody>
</table>

