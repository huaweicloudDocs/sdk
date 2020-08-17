# EPS<a name="sdk_12_0027"></a>

基于EPS v1.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table97391636193710"></a>
<table><thead align="left"><tr id="row077663615372"><th class="cellrowborder" valign="top" width="26.40404040404041%" id="mcps1.1.4.1.1"><p id="p137771036123713"><a name="p137771036123713"></a><a name="p137771036123713"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.323232323232325%" id="mcps1.1.4.1.2"><p id="p1177753663717"><a name="p1177753663717"></a><a name="p1177753663717"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.27272727272727%" id="mcps1.1.4.1.3"><p id="p19777836103715"><a name="p19777836103715"></a><a name="p19777836103715"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row069955523211"><td class="cellrowborder" rowspan="8" valign="top" width="26.40404040404041%" headers="mcps1.1.4.1.1 "><p id="p12419816163315"><a name="p12419816163315"></a><a name="p12419816163315"></a>EnterpriseProject</p>
</td>
<td class="cellrowborder" valign="top" width="38.323232323232325%" headers="mcps1.1.4.1.2 "><p id="p11118844113619"><a name="p11118844113619"></a><a name="p11118844113619"></a>create_enterprise_project(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="35.27272727272727%" headers="mcps1.1.4.1.3 "><p id="p1249215818101"><a name="p1249215818101"></a><a name="p1249215818101"></a>POST /v1.0/enterprise-projects</p>
<p id="p47171950141011"><a name="p47171950141011"></a><a name="p47171950141011"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230881.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18430654710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1511894419365"><a name="p1511894419365"></a><a name="p1511894419365"></a>list_enterprise_projects(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1549220814104"><a name="p1549220814104"></a><a name="p1549220814104"></a>GET /v1.0/enterprise-projects</p>
<p id="p101646514115"><a name="p101646514115"></a><a name="p101646514115"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230880.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16710104019389"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p151184444361"><a name="p151184444361"></a><a name="p151184444361"></a>get_enterprise_project(enterpriseProjectId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p849218812108"><a name="p849218812108"></a><a name="p849218812108"></a>GET /v1.0/enterprise-projects/{id}</p>
<p id="p155281812151110"><a name="p155281812151110"></a><a name="p155281812151110"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230883.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52620441388"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0118104412369"><a name="p0118104412369"></a><a name="p0118104412369"></a>update_enterprise_project( enterpriseProjectId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1149298201014"><a name="p1149298201014"></a><a name="p1149298201014"></a>PUT /v1.0/enterprise-projects/{id}</p>
<p id="p71271918151116"><a name="p71271918151116"></a><a name="p71271918151116"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230884.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1678212234510"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41192448362"><a name="p41192448362"></a><a name="p41192448362"></a>enterprise_project_quotas</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34929831011"><a name="p34929831011"></a><a name="p34929831011"></a>GET /v1.0//enterprise-projects/quotas</p>
<p id="p8935162231120"><a name="p8935162231120"></a><a name="p8935162231120"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230886.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row54715712476"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19119844153614"><a name="p19119844153614"></a><a name="p19119844153614"></a>operate_enterprise_project(enterpriseProjectId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p164923821019"><a name="p164923821019"></a><a name="p164923821019"></a>POST/v1.0/enterprise-projects/{id}/action</p>
<p id="p47151328111117"><a name="p47151328111117"></a><a name="p47151328111117"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230885.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1595131216472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13119144473619"><a name="p13119144473619"></a><a name="p13119144473619"></a>filter_resource_enterprise_project(enterpriseProjectId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1049258181013"><a name="p1049258181013"></a><a name="p1049258181013"></a>POST /v1.0/enterprise-projects/{id}/resources/filter</p>
<p id="p3735123315117"><a name="p3735123315117"></a><a name="p3735123315117"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0133254025.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1961062913475"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4119164420365"><a name="p4119164420365"></a><a name="p4119164420365"></a>migrate_resource_enterprise_project(enterpriseProjectId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p74924818101"><a name="p74924818101"></a><a name="p74924818101"></a>POST /v1.0/enterprise-projects/{id} /resources-migrate</p>
<p id="p95521638161114"><a name="p95521638161114"></a><a name="p95521638161114"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0171146929.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

