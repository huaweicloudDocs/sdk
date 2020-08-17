# IAM<a name="sdk_13_0004"></a>

基于Keystone v3 API的SDK接口如下，调用方式请参考示例代码。

<a name="table48873717191826"></a>
<table><thead align="left"><tr id="row50709260191826"><th class="cellrowborder" valign="top" width="26.46%" id="mcps1.1.4.1.1"><p id="p6497830191826"><a name="p6497830191826"></a><a name="p6497830191826"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.51%" id="mcps1.1.4.1.2"><p id="p29613179191826"><a name="p29613179191826"></a><a name="p29613179191826"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.03%" id="mcps1.1.4.1.3"><p id="p36961635191826"><a name="p36961635191826"></a><a name="p36961635191826"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row14879992191826"><td class="cellrowborder" rowspan="2" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p57433218191826"><a name="p57433218191826"></a><a name="p57433218191826"></a>Tokens</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.4.1.2 "><p id="p96831191826"><a name="p96831191826"></a><a name="p96831191826"></a>Create(c *gophercloud.ServiceClient, opts AuthOptionsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.03%" headers="mcps1.1.4.1.3 "><p id="p32188195191826"><a name="p32188195191826"></a><a name="p32188195191826"></a>POST /v3/auth/tokens</p>
<p id="p19562030101510"><a name="p19562030101510"></a><a name="p19562030101510"></a><a href="https://support.huaweicloud.com/api-iam/iam_30_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row40712197191826"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p28423540191826"><a name="p28423540191826"></a><a name="p28423540191826"></a>Validate(c *gophercloud.ServiceClient, token string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15435251191826"><a name="p15435251191826"></a><a name="p15435251191826"></a>GET /v3/auth/tokens</p>
<p id="p5497174761510"><a name="p5497174761510"></a><a name="p5497174761510"></a><a href="https://support.huaweicloud.com/api-iam/iam_30_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row26192232191826"><td class="cellrowborder" rowspan="2" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p54065268191826"><a name="p54065268191826"></a><a name="p54065268191826"></a>Service catalog</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.4.1.2 "><p id="p63048526191826"><a name="p63048526191826"></a><a name="p63048526191826"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.03%" headers="mcps1.1.4.1.3 "><p id="p47186510191826"><a name="p47186510191826"></a><a name="p47186510191826"></a>GET /v3/services</p>
<p id="p066934971511"><a name="p066934971511"></a><a name="p066934971511"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row26269345191826"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4564051191826"><a name="p4564051191826"></a><a name="p4564051191826"></a>Get(client *gophercloud.ServiceClient, serviceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14466014191826"><a name="p14466014191826"></a><a name="p14466014191826"></a>GET /v3/services/{service_id}</p>
<p id="p12789527158"><a name="p12789527158"></a><a name="p12789527158"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3162064191826"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p30528489191826"><a name="p30528489191826"></a><a name="p30528489191826"></a>Endpoints</p>
</td>
<td class="cellrowborder" valign="top" width="37.51%" headers="mcps1.1.4.1.2 "><p id="p34633359191826"><a name="p34633359191826"></a><a name="p34633359191826"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.03%" headers="mcps1.1.4.1.3 "><p id="p37066825191826"><a name="p37066825191826"></a><a name="p37066825191826"></a>GET /v3/endpoints</p>
<p id="p63293546156"><a name="p63293546156"></a><a name="p63293546156"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

