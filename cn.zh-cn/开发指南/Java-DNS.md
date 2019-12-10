# Java-DNS<a name="ZH-CN_TOPIC_0072142405"></a>

基于DNS v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table34008447"></a>
<table><thead align="left"><tr id="row59665636"><th class="cellrowborder" valign="top" width="18.48%" id="mcps1.1.4.1.1"><p id="p1078370"><a name="p1078370"></a><a name="p1078370"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="44.68%" id="mcps1.1.4.1.2"><p id="p20239120"><a name="p20239120"></a><a name="p20239120"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.84%" id="mcps1.1.4.1.3"><p id="p28755990"><a name="p28755990"></a><a name="p28755990"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row47533853"><td class="cellrowborder" rowspan="7" valign="top" width="18.48%" headers="mcps1.1.4.1.1 "><p id="p1177111197241"><a name="p1177111197241"></a><a name="p1177111197241"></a>ZoneService</p>
</td>
<td class="cellrowborder" valign="top" width="44.68%" headers="mcps1.1.4.1.2 "><p id="p6779622115"><a name="p6779622115"></a><a name="p6779622115"></a>Zone create(Zone zone)</p>
</td>
<td class="cellrowborder" valign="top" width="36.84%" headers="mcps1.1.4.1.3 "><p id="p4124230911054"><a name="p4124230911054"></a><a name="p4124230911054"></a>POST /v2/zones</p>
<p id="p13898135705610"><a name="p13898135705610"></a><a name="p13898135705610"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057310891.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p2018233010402"><a name="p2018233010402"></a><a name="p2018233010402"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311027.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row61373038"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1580951213118"><a name="p1580951213118"></a><a name="p1580951213118"></a>Zone get(String zoneId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15318330"><a name="p15318330"></a><a name="p15318330"></a>GET /v2/zones/{zone_id}</p>
<p id="p4980239195718"><a name="p4980239195718"></a><a name="p4980239195718"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129973.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p7893185912409"><a name="p7893185912409"></a><a name="p7893185912409"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311028.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row3647249"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p183801919310"><a name="p183801919310"></a><a name="p183801919310"></a>List&lt;? extends Zone&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38847270"><a name="p38847270"></a><a name="p38847270"></a>GET /v2/zones</p>
<p id="p838455719575"><a name="p838455719575"></a><a name="p838455719575"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037134402.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p55801020104117"><a name="p55801020104117"></a><a name="p55801020104117"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311029.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row14081115"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p425722813112"><a name="p425722813112"></a><a name="p425722813112"></a>Zone delete(String zoneId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44403789"><a name="p44403789"></a><a name="p44403789"></a>DELETE /v2/zones/{zone_id}</p>
<p id="p194660185813"><a name="p194660185813"></a><a name="p194660185813"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037134403.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p630814914412"><a name="p630814914412"></a><a name="p630814914412"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311030.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row64089786"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p23890167"><a name="p23890167"></a><a name="p23890167"></a>List&lt;? extends Nameserver&gt; listNameservers(String zoneId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56055356"><a name="p56055356"></a><a name="p56055356"></a>GET /v2/zones/{zone_id}/nameservers</p>
<p id="p16802128155813"><a name="p16802128155813"></a><a name="p16802128155813"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057343056.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p127851352114117"><a name="p127851352114117"></a><a name="p127851352114117"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057342901.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row46356111741"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p35709040111741"><a name="p35709040111741"></a><a name="p35709040111741"></a>DesignateZone.Router associateRouter(String zoneId, DesignateZone.Router router)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6751147111741"><a name="p6751147111741"></a><a name="p6751147111741"></a>POST /v2/zones/{zone_id}/associaterouter</p>
<p id="p14657911165819"><a name="p14657911165819"></a><a name="p14657911165819"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057329431.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6274943111746"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32170684111746"><a name="p32170684111746"></a><a name="p32170684111746"></a>DesignateZone.Router disassociateRouter(String zoneId, DesignateZone.Router router)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55688597111746"><a name="p55688597111746"></a><a name="p55688597111746"></a>POST /v2/zones/{zone_id}/disassociaterouter</p>
<p id="p84071621145815"><a name="p84071621145815"></a><a name="p84071621145815"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057331452.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20314447"><td class="cellrowborder" rowspan="5" valign="top" width="18.48%" headers="mcps1.1.4.1.1 "><p id="p121153642417"><a name="p121153642417"></a><a name="p121153642417"></a>RecordsetService</p>
</td>
<td class="cellrowborder" valign="top" width="44.68%" headers="mcps1.1.4.1.2 "><p id="p131061381227"><a name="p131061381227"></a><a name="p131061381227"></a>Recordset create(String zoneId, Recordset recordSet)</p>
</td>
<td class="cellrowborder" valign="top" width="36.84%" headers="mcps1.1.4.1.3 "><p id="p60441935"><a name="p60441935"></a><a name="p60441935"></a>POST /v2/zones/{zone_id}/recordsets</p>
<p id="p42041726185810"><a name="p42041726185810"></a><a name="p42041726185810"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037134404.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row55322531111735"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p516215244213"><a name="p516215244213"></a><a name="p516215244213"></a>Recordset get(String zoneId, String recordsetId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46393492111735"><a name="p46393492111735"></a><a name="p46393492111735"></a>GET /v2/zone/{zone_id}/recordsets/{recordset_id}</p>
<p id="p43601928185811"><a name="p43601928185811"></a><a name="p43601928185811"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129968.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7106508"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1425873019212"><a name="p1425873019212"></a><a name="p1425873019212"></a>List&lt;? extends Recordset&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52250665"><a name="p52250665"></a><a name="p52250665"></a>GET /v2/recordsets</p>
<p id="p1599103015585"><a name="p1599103015585"></a><a name="p1599103015585"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129969.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row493939"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p169851362215"><a name="p169851362215"></a><a name="p169851362215"></a>List&lt;? extends Recordset&gt; list(RecordsetListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19513753"><a name="p19513753"></a><a name="p19513753"></a>GET /v2/zones/{zone_id}/recordsets</p>
<p id="p72898336584"><a name="p72898336584"></a><a name="p72898336584"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129970.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row41406050"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p65555736"><a name="p65555736"></a><a name="p65555736"></a>Recordset delete(String zoneId, String recordsetId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8414436"><a name="p8414436"></a><a name="p8414436"></a>DELETE /v2/zones/{zone_id}/recordsets/{recordset_id}</p>
<p id="p14121153817589"><a name="p14121153817589"></a><a name="p14121153817589"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129971.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8621060"><td class="cellrowborder" rowspan="4" valign="top" width="18.48%" headers="mcps1.1.4.1.1 "><p id="p1630013816252"><a name="p1630013816252"></a><a name="p1630013816252"></a>PTRService</p>
</td>
<td class="cellrowborder" valign="top" width="44.68%" headers="mcps1.1.4.1.2 "><p id="p1374311511025"><a name="p1374311511025"></a><a name="p1374311511025"></a>DesignatePTR setup(DesignatePTR record)</p>
</td>
<td class="cellrowborder" valign="top" width="36.84%" headers="mcps1.1.4.1.3 "><p id="p5860594711258"><a name="p5860594711258"></a><a name="p5860594711258"></a>PATCH /v2/reverse/floatingips/{region}:{floatingip_id}</p>
<p id="p182431240115815"><a name="p182431240115815"></a><a name="p182431240115815"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318613.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row30668413"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16481059920"><a name="p16481059920"></a><a name="p16481059920"></a>ActionResponse restore(String region, String floatingIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3017953511258"><a name="p3017953511258"></a><a name="p3017953511258"></a>PATCH /v2/reverse/floatingips/{region}:{floatingip_id}</p>
<p id="p7929184235820"><a name="p7929184235820"></a><a name="p7929184235820"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318616.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6466753"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1841218519314"><a name="p1841218519314"></a><a name="p1841218519314"></a>List&lt;? extends PTR&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3759833711258"><a name="p3759833711258"></a><a name="p3759833711258"></a>GET /v2/reverse/floatingips</p>
<p id="p55252045175811"><a name="p55252045175811"></a><a name="p55252045175811"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318615.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5908907"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8859419"><a name="p8859419"></a><a name="p8859419"></a>DesignatePTR get(String region, String floatingIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3728940811258"><a name="p3728940811258"></a><a name="p3728940811258"></a>GET /v2/reverse/floatingips/{region}:{floatingip_id}</p>
<p id="p27666479586"><a name="p27666479586"></a><a name="p27666479586"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318614.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

