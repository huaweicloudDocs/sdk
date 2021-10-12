# IMS<a name="sdk_11_0002"></a>

基于Glance v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table1963786"></a>
<table><thead align="left"><tr id="row26485815"><th class="cellrowborder" valign="top" width="29.44294429442944%" id="mcps1.1.4.1.1"><p id="p64976233"><a name="p64976233"></a><a name="p64976233"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.493549354935496%" id="mcps1.1.4.1.2"><p id="p28583536"><a name="p28583536"></a><a name="p28583536"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="p33565108"><a name="p33565108"></a><a name="p33565108"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row34419228"><td class="cellrowborder" rowspan="12" valign="top" width="29.44294429442944%" headers="mcps1.1.4.1.1 "><p id="p36494097"><a name="p36494097"></a><a name="p36494097"></a>ImageService</p>
<p id="p1327118161118"><a name="p1327118161118"></a><a name="p1327118161118"></a></p>
</td>
<td class="cellrowborder" valign="top" width="35.493549354935496%" headers="mcps1.1.4.1.2 "><p id="p3231866"><a name="p3231866"></a><a name="p3231866"></a>Image create(Image image)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p162011834193216"><a name="p162011834193216"></a><a name="p162011834193216"></a>POST /v2/images</p>
</td>
</tr>
<tr id="row7220417"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p47982876"><a name="p47982876"></a><a name="p47982876"></a>ActionResponse upload(String imageId, Payload payload, Image image)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p61407752"><a name="p61407752"></a><a name="p61407752"></a>PUT /v2/images/{image_id}/file</p>
</td>
</tr>
<tr id="row26571327"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4793853"><a name="p4793853"></a><a name="p4793853"></a>ActionResponse delete(String imageId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52757779"><a name="p52757779"></a><a name="p52757779"></a>DELETE /v2/images/{image_id}</p>
</td>
</tr>
<tr id="row5057967"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7042173"><a name="p7042173"></a><a name="p7042173"></a>List&lt;? extends Image&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33545144"><a name="p33545144"></a><a name="p33545144"></a>GET /v2/images</p>
</td>
</tr>
<tr id="row33470841"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26783618"><a name="p26783618"></a><a name="p26783618"></a>Image get(String imageId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21989419"><a name="p21989419"></a><a name="p21989419"></a>GET /v2/images/{image_id}</p>
</td>
</tr>
<tr id="row51053199"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41668450"><a name="p41668450"></a><a name="p41668450"></a>ActionResponse updateTag(String imageId, String tagkeyvalue)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19701298"><a name="p19701298"></a><a name="p19701298"></a>PUT /v2/images/{image_id}/tags/{tag}</p>
</td>
</tr>
<tr id="row43093956"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p949529"><a name="p949529"></a><a name="p949529"></a>ActionResponse deleteTag(String imageId, String tagkey)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9803039"><a name="p9803039"></a><a name="p9803039"></a>DELETE /v2/images/{image_id}/tags/{tag}</p>
</td>
</tr>
<tr id="row21118492"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32876269"><a name="p32876269"></a><a name="p32876269"></a>List&lt;? extends Member&gt; listMembers(String imageId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p45732164"><a name="p45732164"></a><a name="p45732164"></a>GET /v2/images/{image_id}/members</p>
</td>
</tr>
<tr id="row8936292"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p52751036"><a name="p52751036"></a><a name="p52751036"></a>Member getMember(String imageId, memberId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44975500"><a name="p44975500"></a><a name="p44975500"></a>GET /v2/images/{image_id}/members/{member_id}</p>
</td>
</tr>
<tr id="row2126321"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p38014313"><a name="p38014313"></a><a name="p38014313"></a>ActionResponse deleteMember(String imageId, String memberId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p59260526"><a name="p59260526"></a><a name="p59260526"></a>DELETE /v2/images/{image_id}/members/{member_id}</p>
</td>
</tr>
<tr id="row35373287"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p46663997"><a name="p46663997"></a><a name="p46663997"></a>Member updateMember(String imageId, String memberId, Member.MemberStatus.ACCEPTED)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21687383"><a name="p21687383"></a><a name="p21687383"></a>PUT /v2/images/{image_id}/members/{member_id}</p>
</td>
</tr>
<tr id="row1326684113"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20666125713121"><a name="p20666125713121"></a><a name="p20666125713121"></a>Member createMember(String imageId, String memberId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2327380119"><a name="p2327380119"></a><a name="p2327380119"></a>POST /v2/images/{image_id}/members</p>
</td>
</tr>
</tbody>
</table>

基于IMS v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table411442315562"></a>
<table><thead align="left"><tr id="row311582365611"><th class="cellrowborder" valign="top" width="29.332933293329333%" id="mcps1.1.4.1.1"><p id="p7275744145815"><a name="p7275744145815"></a><a name="p7275744145815"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.81358135813581%" id="mcps1.1.4.1.2"><p id="p42761644205819"><a name="p42761644205819"></a><a name="p42761644205819"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.85348534853485%" id="mcps1.1.4.1.3"><p id="p727634455818"><a name="p727634455818"></a><a name="p727634455818"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1411522385618"><td class="cellrowborder" rowspan="4" valign="top" width="29.332933293329333%" headers="mcps1.1.4.1.1 "><p id="p1115162385612"><a name="p1115162385612"></a><a name="p1115162385612"></a>ImageService</p>
</td>
<td class="cellrowborder" valign="top" width="35.81358135813581%" headers="mcps1.1.4.1.2 "><p id="p438414291575"><a name="p438414291575"></a><a name="p438414291575"></a>String create(ImageCreateByInstance imageCreateByInstance)</p>
</td>
<td class="cellrowborder" valign="top" width="34.85348534853485%" headers="mcps1.1.4.1.3 "><p id="p16384102925711"><a name="p16384102925711"></a><a name="p16384102925711"></a>POST /v2/cloudimages/action</p>
</td>
</tr>
<tr id="row31151323205613"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8384152995714"><a name="p8384152995714"></a><a name="p8384152995714"></a>String create(ImageCreateByExternalImage imageCreateByExternalImage)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p0384929165716"><a name="p0384929165716"></a><a name="p0384929165716"></a>POST /v2/cloudimages/action</p>
</td>
</tr>
<tr id="row5116152375611"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33846292579"><a name="p33846292579"></a><a name="p33846292579"></a>List&lt;Image&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p63841729185713"><a name="p63841729185713"></a><a name="p63841729185713"></a>GET /v2/cloudimages</p>
</td>
</tr>
<tr id="row1411682335618"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1038519290574"><a name="p1038519290574"></a><a name="p1038519290574"></a>Image update(List&lt;ImageUpdate&gt; updateModel, String imageId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3385122965714"><a name="p3385122965714"></a><a name="p3385122965714"></a>PATCH /v2/cloudimages/{image_id}</p>
</td>
</tr>
</tbody>
</table>

基于IMS v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table1563512445565"></a>
<table><thead align="left"><tr id="row1263618443565"><th class="cellrowborder" valign="top" width="29.762976297629763%" id="mcps1.1.4.1.1"><p id="p24265995"><a name="p24265995"></a><a name="p24265995"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.6035603560356%" id="mcps1.1.4.1.2"><p id="p19388612"><a name="p19388612"></a><a name="p19388612"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.63346334633463%" id="mcps1.1.4.1.3"><p id="p26973745"><a name="p26973745"></a><a name="p26973745"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row18637124411567"><td class="cellrowborder" rowspan="5" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p4637444115610"><a name="p4637444115610"></a><a name="p4637444115610"></a>ImageService</p>
</td>
<td class="cellrowborder" valign="top" width="35.6035603560356%" headers="mcps1.1.4.1.2 "><p id="p364210506575"><a name="p364210506575"></a><a name="p364210506575"></a>String create(ImageCreateByOBS imageCreateByOBS)</p>
</td>
<td class="cellrowborder" valign="top" width="34.63346334633463%" headers="mcps1.1.4.1.3 "><p id="p12642165015712"><a name="p12642165015712"></a><a name="p12642165015712"></a>POST /v1/cloudimages/dataimages/action</p>
</td>
</tr>
<tr id="row663794415563"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p864285085719"><a name="p864285085719"></a><a name="p864285085719"></a>String regist(RegistImage image, String imageId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46421250105713"><a name="p46421250105713"></a><a name="p46421250105713"></a>PUT /v1/cloudimages/{image_id}/upload</p>
</td>
</tr>
<tr id="row13637184420562"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p136422050145717"><a name="p136422050145717"></a><a name="p136422050145717"></a>String export(ExportImage image, String imageId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1164265018579"><a name="p1164265018579"></a><a name="p1164265018579"></a>POST /v1/cloudimages/{image_id}/file</p>
</td>
</tr>
<tr id="row463720445564"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p864235045717"><a name="p864235045717"></a><a name="p864235045717"></a>String create(ImageCreateByExternalImage imageCreateByExternalImage)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46428501571"><a name="p46428501571"></a><a name="p46428501571"></a>POST /v1/cloudimages/wholeimages/action</p>
</td>
</tr>
<tr id="row1163714411563"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1864216507572"><a name="p1864216507572"></a><a name="p1864216507572"></a>String create(ImageCreateByInstance imageCreateByInstance)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p464345075712"><a name="p464345075712"></a><a name="p464345075712"></a>POST /v1/cloudimages/wholeimages/action</p>
</td>
</tr>
<tr id="row1363894417567"><td class="cellrowborder" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p9638154414569"><a name="p9638154414569"></a><a name="p9638154414569"></a>Jobservice</p>
</td>
<td class="cellrowborder" valign="top" width="35.6035603560356%" headers="mcps1.1.4.1.2 "><p id="p93111131582"><a name="p93111131582"></a><a name="p93111131582"></a>Job get(String jobId)</p>
</td>
<td class="cellrowborder" valign="top" width="34.63346334633463%" headers="mcps1.1.4.1.3 "><p id="p133171320582"><a name="p133171320582"></a><a name="p133171320582"></a>GET /v1/{project_id}/jobs/{job_id}</p>
</td>
</tr>
</tbody>
</table>

