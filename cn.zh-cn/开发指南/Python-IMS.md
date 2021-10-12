# IMS<a name="sdk_12_0002"></a>

基于Glance v2 API的SDK接口如下，调用方式举例：conn.image.upload\_image\(\)

<a name="table35632194"></a>
<table><thead align="left"><tr id="row48861387"><th class="cellrowborder" valign="top" width="25.82258225822582%" id="mcps1.1.4.1.1"><p id="p65458312"><a name="p65458312"></a><a name="p65458312"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="40.384038403840385%" id="mcps1.1.4.1.2"><p id="p523045"><a name="p523045"></a><a name="p523045"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.79337933793379%" id="mcps1.1.4.1.3"><p id="p42366666"><a name="p42366666"></a><a name="p42366666"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row9147936"><td class="cellrowborder" rowspan="7" valign="top" width="25.82258225822582%" headers="mcps1.1.4.1.1 "><p id="p2785358"><a name="p2785358"></a><a name="p2785358"></a>Image Operations</p>
</td>
<td class="cellrowborder" valign="top" width="40.384038403840385%" headers="mcps1.1.4.1.2 "><p id="p24287485"><a name="p24287485"></a><a name="p24287485"></a>upload_image(self, container_format=None, disk_format=None, data=None, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="33.79337933793379%" headers="mcps1.1.4.1.3 "><p id="p8910195962614"><a name="p8910195962614"></a><a name="p8910195962614"></a>POST /v2/images</p>
<p id="p21129301"><a name="p21129301"></a><a name="p21129301"></a>PUT /v2/images/{image_id}/file</p>
</td>
</tr>
<tr id="row55945983"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p35330790"><a name="p35330790"></a><a name="p35330790"></a>delete_image(self, image,  ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p43221770"><a name="p43221770"></a><a name="p43221770"></a>DELETE /v2/images/{image_id}</p>
</td>
</tr>
<tr id="row53451614"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p34613479"><a name="p34613479"></a><a name="p34613479"></a>find_image(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52228449"><a name="p52228449"></a><a name="p52228449"></a>GET /v2/images</p>
</td>
</tr>
<tr id="row294000"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p23814038"><a name="p23814038"></a><a name="p23814038"></a>get_image(self, image)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p49888896"><a name="p49888896"></a><a name="p49888896"></a>GET /v2/images/{image_id}</p>
</td>
</tr>
<tr id="row46346882"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p63109966"><a name="p63109966"></a><a name="p63109966"></a>images(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11633618"><a name="p11633618"></a><a name="p11633618"></a>GET /v2/images</p>
</td>
</tr>
<tr id="row37593705"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p25191285"><a name="p25191285"></a><a name="p25191285"></a>add_tag(self, image, tag)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p27228238"><a name="p27228238"></a><a name="p27228238"></a>PUT /v2/images/{image_id}/tags/{tag}</p>
</td>
</tr>
<tr id="row43727555"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p52271033"><a name="p52271033"></a><a name="p52271033"></a>remove_tag(self, image, tag)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6095280"><a name="p6095280"></a><a name="p6095280"></a>DELETE /v2/images/{image_id}/tags/{tag}</p>
</td>
</tr>
<tr id="row54857523"><td class="cellrowborder" rowspan="6" valign="top" width="25.82258225822582%" headers="mcps1.1.4.1.1 "><p id="p14274382"><a name="p14274382"></a><a name="p14274382"></a>Member Operations</p>
</td>
<td class="cellrowborder" valign="top" width="40.384038403840385%" headers="mcps1.1.4.1.2 "><p id="p15374269"><a name="p15374269"></a><a name="p15374269"></a>add_member(self, image, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="33.79337933793379%" headers="mcps1.1.4.1.3 "><p id="p37356265"><a name="p37356265"></a><a name="p37356265"></a>POST /v2/images/{image_id}/members</p>
</td>
</tr>
<tr id="row662065"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p53627266"><a name="p53627266"></a><a name="p53627266"></a>remove_member(self, member, image, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p48841284"><a name="p48841284"></a><a name="p48841284"></a>DELETE /v2/images/{image_id}/members/{member_id}</p>
</td>
</tr>
<tr id="row36918374"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p37598356"><a name="p37598356"></a><a name="p37598356"></a>find_member(self, name_or_id, image, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p25568006"><a name="p25568006"></a><a name="p25568006"></a>GET /v2/images/{image_id}/members</p>
</td>
</tr>
<tr id="row28785469"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p49921616"><a name="p49921616"></a><a name="p49921616"></a>get_member(self, member, image)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17119133"><a name="p17119133"></a><a name="p17119133"></a>GET /v2/images/{image_id}/members/{member_id}</p>
</td>
</tr>
<tr id="row19854472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p64708380"><a name="p64708380"></a><a name="p64708380"></a>members(self, image)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6887421"><a name="p6887421"></a><a name="p6887421"></a>GET /v2/images/{image_id}/members</p>
</td>
</tr>
<tr id="row61986789"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54874019"><a name="p54874019"></a><a name="p54874019"></a>update_member(self, member, image, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15610594"><a name="p15610594"></a><a name="p15610594"></a>PUT /v2/images/{image_id}/members/{member_id}</p>
</td>
</tr>
</tbody>
</table>

基于IMS v2 API的SDK接口如下，调用方式举例：conn.ims.create\_cloudimage\(\)

<a name="table1398913118454"></a>
<table><thead align="left"><tr id="row139901012459"><th class="cellrowborder" valign="top" width="25.722572257225725%" id="mcps1.1.4.1.1"><p id="p94789469457"><a name="p94789469457"></a><a name="p94789469457"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="40.59405940594059%" id="mcps1.1.4.1.2"><p id="p8480134617458"><a name="p8480134617458"></a><a name="p8480134617458"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.68336833683368%" id="mcps1.1.4.1.3"><p id="p104815463459"><a name="p104815463459"></a><a name="p104815463459"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row199118110451"><td class="cellrowborder" rowspan="4" valign="top" width="25.722572257225725%" headers="mcps1.1.4.1.1 "><p id="p12158182504611"><a name="p12158182504611"></a><a name="p12158182504611"></a>Cloudimage Operations</p>
<p id="p1166342514194"><a name="p1166342514194"></a><a name="p1166342514194"></a></p>
</td>
<td class="cellrowborder" valign="top" width="40.59405940594059%" headers="mcps1.1.4.1.2 "><p id="p514312420453"><a name="p514312420453"></a><a name="p514312420453"></a>cloudimages(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="33.68336833683368%" headers="mcps1.1.4.1.3 "><p id="p4535435184513"><a name="p4535435184513"></a><a name="p4535435184513"></a>GET /v2/cloudimages</p>
</td>
</tr>
<tr id="row299112124519"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1414319242452"><a name="p1414319242452"></a><a name="p1414319242452"></a>update_cloudimage(self, cloudimage_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1753633516459"><a name="p1753633516459"></a><a name="p1753633516459"></a>PATCH /v2/cloudimages/{image_id}</p>
</td>
</tr>
<tr id="row299111174511"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11143424194510"><a name="p11143424194510"></a><a name="p11143424194510"></a>create_cloudimage(self, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18536153510450"><a name="p18536153510450"></a><a name="p18536153510450"></a>POST /v2/cloudimages/action</p>
</td>
</tr>
<tr id="row866182521920"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p36633254196"><a name="p36633254196"></a><a name="p36633254196"></a>get_job(self, job_id):</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10663725121913"><a name="p10663725121913"></a><a name="p10663725121913"></a>GET /v1/{project_id}/jobs/{job_id}</p>
</td>
</tr>
</tbody>
</table>

