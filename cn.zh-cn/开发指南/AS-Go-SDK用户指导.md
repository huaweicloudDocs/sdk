# AS Go SDK用户指导<a name="sdk_03_0020"></a>

SDK与RESTful API一一对应，SDK最新版本支持的接口列表，以及SDK和API的对应关系，请参考[AS](GO-AS.md)。

在使用AS SDK的时候，SDK支持的参数细节，请参考AS API[描述](https://support.huaweicloud.com/api-as/zh-cn_topic_0045219159.html)。

AS v1 Go SDK支持如下资源对象的操作，资源对象的“增改查删”代码示例如下：

<a name="table1827067191917"></a>
<table><thead align="left"><tr id="row1239047151914"><th class="cellrowborder" valign="top" width="32.25%" id="mcps1.1.3.1.1"><p id="p1839057171910"><a name="p1839057171910"></a><a name="p1839057171910"></a>资源对象</p>
</th>
<th class="cellrowborder" valign="top" width="67.75%" id="mcps1.1.3.1.2"><p id="p1039217171913"><a name="p1039217171913"></a><a name="p1039217171913"></a>“增改查删”代码样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row2039217201917"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p142171711459"><a name="p142171711459"></a><a name="p142171711459"></a>configration</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p3413194413318"><a name="p3413194413318"></a><a name="p3413194413318"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/configrations.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row18392674191"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p1539297171916"><a name="p1539297171916"></a><a name="p1539297171916"></a>group</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p323013118475"><a name="p323013118475"></a><a name="p323013118475"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/groups.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row03925741913"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p18868242154519"><a name="p18868242154519"></a><a name="p18868242154519"></a>instance</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p311372518418"><a name="p311372518418"></a><a name="p311372518418"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/instances.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row439219712195"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p3454855154518"><a name="p3454855154518"></a><a name="p3454855154518"></a>lifecyclehook</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p12113925445"><a name="p12113925445"></a><a name="p12113925445"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/lifecyclehooks.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row16392207131915"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p1539416153463"><a name="p1539416153463"></a><a name="p1539416153463"></a>log</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p1655014301646"><a name="p1655014301646"></a><a name="p1655014301646"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/logs.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row183926716196"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p15865142384611"><a name="p15865142384611"></a><a name="p15865142384611"></a>notification</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p175591230547"><a name="p175591230547"></a><a name="p175591230547"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/notifications.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row939215791918"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p9578244134613"><a name="p9578244134613"></a><a name="p9578244134613"></a>policy</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p155626304410"><a name="p155626304410"></a><a name="p155626304410"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/policies.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row203933710195"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p16233141144712"><a name="p16233141144712"></a><a name="p16233141144712"></a>policylog</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p1156593017419"><a name="p1156593017419"></a><a name="p1156593017419"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/policylogs.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1379018617482"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p157917624815"><a name="p157917624815"></a><a name="p157917624815"></a>quota</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p19568113013410"><a name="p19568113013410"></a><a name="p19568113013410"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/quotas.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1139387131916"><td class="cellrowborder" valign="top" width="32.25%" headers="mcps1.1.3.1.1 "><p id="p677342113478"><a name="p677342113478"></a><a name="p677342113478"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="67.75%" headers="mcps1.1.3.1.2 "><p id="p155721830646"><a name="p155721830646"></a><a name="p155721830646"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-go/blob/master/examples/as/v1/tags.go" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
</tbody>
</table>

