# EVS<a name="sdk_13_0002"></a>

基于Cinder v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table18312790192017"></a>
<table><thead align="left"><tr id="row16823310192025"><th class="cellrowborder" valign="top" width="26.672667266726673%" id="mcps1.1.4.1.1"><p id="p45879957192652"><a name="p45879957192652"></a><a name="p45879957192652"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.263826382638264%" id="mcps1.1.4.1.2"><p id="p1042560192652"><a name="p1042560192652"></a><a name="p1042560192652"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="p24514206192652"><a name="p24514206192652"></a><a name="p24514206192652"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row45744883192017"><td class="cellrowborder" rowspan="5" valign="top" width="26.672667266726673%" headers="mcps1.1.4.1.1 "><p id="p40745058192017"><a name="p40745058192017"></a><a name="p40745058192017"></a>Volumes</p>
</td>
<td class="cellrowborder" valign="top" width="38.263826382638264%" headers="mcps1.1.4.1.2 "><p id="p15370023192017"><a name="p15370023192017"></a><a name="p15370023192017"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p1828019165517"><a name="p1828019165517"></a><a name="p1828019165517"></a>GET /v2/{project_id}/volumes/detail</p>
<p id="p62805945515"><a name="p62805945515"></a><a name="p62805945515"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56484243192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6696444192017"><a name="p6696444192017"></a><a name="p6696444192017"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p628020965519"><a name="p628020965519"></a><a name="p628020965519"></a>POST /v2/{project_id}/volumes</p>
<p id="p1728018913557"><a name="p1728018913557"></a><a name="p1728018913557"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2065.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39989412192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60747040192017"><a name="p60747040192017"></a><a name="p60747040192017"></a>Get(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p132807914553"><a name="p132807914553"></a><a name="p132807914553"></a>GET /v2/{project_id}/volumes/{volume_id}</p>
<p id="p6280189205513"><a name="p6280189205513"></a><a name="p6280189205513"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2070.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7996260192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5767230192017"><a name="p5767230192017"></a><a name="p5767230192017"></a>Delete(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5280179195517"><a name="p5280179195517"></a><a name="p5280179195517"></a>DELETE /v2/{project_id}/volumes/{volume_id}</p>
<p id="p122801925515"><a name="p122801925515"></a><a name="p122801925515"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2066.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12250786192017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18753795192017"><a name="p18753795192017"></a><a name="p18753795192017"></a>Update(client *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12280696551"><a name="p12280696551"></a><a name="p12280696551"></a>PUT /v2/{project_id}/volumes/{volume_id}</p>
<p id="p1828018955514"><a name="p1828018955514"></a><a name="p1828018955514"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2067.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

