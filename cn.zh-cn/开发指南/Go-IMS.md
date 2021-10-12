# IMS<a name="sdk_13_0005"></a>

基于Glance v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table23186431192059"></a>
<table><thead align="left"><tr id="row6232965719213"><th class="cellrowborder" valign="top" width="26.142614261426147%" id="mcps1.1.4.1.1"><p id="p3763296319273"><a name="p3763296319273"></a><a name="p3763296319273"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.19371937193719%" id="mcps1.1.4.1.2"><p id="p950753419273"><a name="p950753419273"></a><a name="p950753419273"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.66366636663666%" id="mcps1.1.4.1.3"><p id="p2230708619273"><a name="p2230708619273"></a><a name="p2230708619273"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row18496463192059"><td class="cellrowborder" rowspan="5" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p55486927192059"><a name="p55486927192059"></a><a name="p55486927192059"></a>images</p>
</td>
<td class="cellrowborder" valign="top" width="37.19371937193719%" headers="mcps1.1.4.1.2 "><p id="p10952728192059"><a name="p10952728192059"></a><a name="p10952728192059"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.66366636663666%" headers="mcps1.1.4.1.3 "><p id="p39540342192059"><a name="p39540342192059"></a><a name="p39540342192059"></a>POST /v2/images</p>
</td>
</tr>
<tr id="row53373202192059"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p52645891192059"><a name="p52645891192059"></a><a name="p52645891192059"></a>Delete(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p671317192059"><a name="p671317192059"></a><a name="p671317192059"></a>DELETE /v2/images/{image_id}</p>
</td>
</tr>
<tr id="row62432560192059"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8189604192059"><a name="p8189604192059"></a><a name="p8189604192059"></a>List(c *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32038883192059"><a name="p32038883192059"></a><a name="p32038883192059"></a>GET /v2/images</p>
</td>
</tr>
<tr id="row26826111192059"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9588077192059"><a name="p9588077192059"></a><a name="p9588077192059"></a>Update(client *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p47832421192059"><a name="p47832421192059"></a><a name="p47832421192059"></a>PATCH /v2/images/{image_id}</p>
</td>
</tr>
<tr id="row19230130192059"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42990172192059"><a name="p42990172192059"></a><a name="p42990172192059"></a>Get(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38896745192059"><a name="p38896745192059"></a><a name="p38896745192059"></a>GET /v2/images/{image_id}</p>
</td>
</tr>
</tbody>
</table>

