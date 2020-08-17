# EPS<a name="sdk_11_0027"></a>

基于EPS v1.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table8484916201010"></a>
<table><thead align="left"><tr id="row157021316171019"><th class="cellrowborder" valign="top" width="25.722572257225725%" id="mcps1.1.4.1.1"><p id="p157026162107"><a name="p157026162107"></a><a name="p157026162107"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.43394339433943%" id="mcps1.1.4.1.2"><p id="p370211618107"><a name="p370211618107"></a><a name="p370211618107"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.84348434843484%" id="mcps1.1.4.1.3"><p id="p1670231681013"><a name="p1670231681013"></a><a name="p1670231681013"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row970281614107"><td class="cellrowborder" rowspan="9" valign="top" width="25.722572257225725%" headers="mcps1.1.4.1.1 "><p id="p16397124734818"><a name="p16397124734818"></a><a name="p16397124734818"></a>EPService</p>
</td>
<td class="cellrowborder" valign="top" width="39.43394339433943%" headers="mcps1.1.4.1.2 "><p id="p15157154134616"><a name="p15157154134616"></a><a name="p15157154134616"></a>EPCreateResponse create(EPCreateRequest createRequest)</p>
</td>
<td class="cellrowborder" valign="top" width="34.84348434843484%" headers="mcps1.1.4.1.3 "><p id="p131581149463"><a name="p131581149463"></a><a name="p131581149463"></a>POST/v1.0/enterprise-projects</p>
<p id="p856681014714"><a name="p856681014714"></a><a name="p856681014714"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230881.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11702121671016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1158184184619"><a name="p1158184184619"></a><a name="p1158184184619"></a>EPListResponse list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p81586474610"><a name="p81586474610"></a><a name="p81586474610"></a>GET/v1.0/enterprise-projects</p>
<p id="p133391815778"><a name="p133391815778"></a><a name="p133391815778"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230880.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row370341612101"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p161585464613"><a name="p161585464613"></a><a name="p161585464613"></a>EPListResponse list(Map&lt;String, String&gt; queryParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10158144134613"><a name="p10158144134613"></a><a name="p10158144134613"></a>GET/v1.0/enterprise-projects</p>
<p id="p1226213200710"><a name="p1226213200710"></a><a name="p1226213200710"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230880.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19703716191017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41583494615"><a name="p41583494615"></a><a name="p41583494615"></a>EPQueryResponse get(String epID)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p161587494613"><a name="p161587494613"></a><a name="p161587494613"></a>GET/v1.0/enterprise-projects/{id}</p>
<p id="p88711252714"><a name="p88711252714"></a><a name="p88711252714"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230883.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1070320164101"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1315810414611"><a name="p1315810414611"></a><a name="p1315810414611"></a>EPQueryResponse modify(String epID, EPModifyRequest modifyRequest)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1715854124619"><a name="p1715854124619"></a><a name="p1715854124619"></a>PUT/v1.0/enterprise-projects/{id}</p>
<p id="p07745291178"><a name="p07745291178"></a><a name="p07745291178"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230884.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row797185710453"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11158240467"><a name="p11158240467"></a><a name="p11158240467"></a>EPQuotaResponse quotas()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1415817411468"><a name="p1415817411468"></a><a name="p1415817411468"></a>GET/v1.0//enterprise-projects/quotas</p>
<p id="p1580819341179"><a name="p1580819341179"></a><a name="p1580819341179"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230886.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1755210544455"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p161582484614"><a name="p161582484614"></a><a name="p161582484614"></a>ActionResponse action(String epID, EPActionRequest actionRequest)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1158184184613"><a name="p1158184184613"></a><a name="p1158184184613"></a>POST/v1.0/enterprise-projects/{id}/action</p>
<p id="p13505183913719"><a name="p13505183913719"></a><a name="p13505183913719"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0121230885.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15551051174514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1915817414612"><a name="p1915817414612"></a><a name="p1915817414612"></a>EPResourceFilterResponse filterResource(String epID, EPResourceFilterRequest filterRequest)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p71585484612"><a name="p71585484612"></a><a name="p71585484612"></a>POST/v1.0/enterprise-projects/{id}/resources/filter</p>
<p id="p1220411451272"><a name="p1220411451272"></a><a name="p1220411451272"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0133254025.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10507184820457"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p515817434615"><a name="p515817434615"></a><a name="p515817434615"></a>ActionResponse migrateResource(String epID, EPResourceActionRequest actionRequest)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p515920413463"><a name="p515920413463"></a><a name="p515920413463"></a>POST/v1.0/enterprise-projects/{id} /resources-migrate</p>
<p id="p193082500712"><a name="p193082500712"></a><a name="p193082500712"></a><a href="https://support.huaweicloud.com/api-em/zh-cn_topic_0171146929.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

