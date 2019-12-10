# Go-EVS<a name="ZH-CN_TOPIC_0090172881"></a>

基于Cinder v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table18312790192017"></a>
<table><thead align="left"><tr id="row16823310192025"><th class="cellrowborder" valign="top" width="19.09190919091909%" id="mcps1.1.4.1.1"><p id="p45879957192652"><a name="p45879957192652"></a><a name="p45879957192652"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="46.24462446244625%" id="mcps1.1.4.1.2"><p id="p1042560192652"><a name="p1042560192652"></a><a name="p1042560192652"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.663466346634664%" id="mcps1.1.4.1.3"><p id="p24514206192652"><a name="p24514206192652"></a><a name="p24514206192652"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row45744883192017"><td class="cellrowborder" rowspan="5" valign="top" width="19.09190919091909%" headers="mcps1.1.4.1.1 "><p id="p40745058192017"><a name="p40745058192017"></a><a name="p40745058192017"></a>Volumes</p>
</td>
<td class="cellrowborder" valign="top" width="46.24462446244625%" headers="mcps1.1.4.1.2 "><p id="p15370023192017"><a name="p15370023192017"></a><a name="p15370023192017"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="34.663466346634664%" headers="mcps1.1.4.1.3 "><p id="p59778613192017"><a name="p59778613192017"></a><a name="p59778613192017"></a>GET /v2/{project_id}/volumes/detail</p>
<p id="p98461249143018"><a name="p98461249143018"></a><a name="p98461249143018"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0058762431.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56484243192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6696444192017"><a name="p6696444192017"></a><a name="p6696444192017"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2594795192017"><a name="p2594795192017"></a><a name="p2594795192017"></a>POST /v2/{project_id}/volumes</p>
<p id="p568914161318"><a name="p568914161318"></a><a name="p568914161318"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0058762427.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39989412192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60747040192017"><a name="p60747040192017"></a><a name="p60747040192017"></a>Get(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5858786192017"><a name="p5858786192017"></a><a name="p5858786192017"></a>GET /v2/{project_id}/volumes/{volume_id}</p>
<p id="p2325917123118"><a name="p2325917123118"></a><a name="p2325917123118"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235170.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7996260192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5767230192017"><a name="p5767230192017"></a><a name="p5767230192017"></a>Delete(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18893346192017"><a name="p18893346192017"></a><a name="p18893346192017"></a>DELETE /v2/{project_id}/volumes/{volume_id}</p>
<p id="p53427196310"><a name="p53427196310"></a><a name="p53427196310"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0058762428.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12250786192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18753795192017"><a name="p18753795192017"></a><a name="p18753795192017"></a>Update(client *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p66558478192017"><a name="p66558478192017"></a><a name="p66558478192017"></a>PUT /v2/{project_id}/volumes/{volume_id}</p>
<p id="p1941162116316"><a name="p1941162116316"></a><a name="p1941162116316"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0058762429.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

