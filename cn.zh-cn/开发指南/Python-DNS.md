# Python-DNS<a name="ZH-CN_TOPIC_0072142412"></a>

基于DNS v2 API的SDK接口如下，调用方式举例：conn.dns.create\_zone\(\)

<a name="table34008447"></a>
<table><thead align="left"><tr id="row59665636"><th class="cellrowborder" valign="top" width="18.11%" id="mcps1.1.4.1.1"><p id="p1078370"><a name="p1078370"></a><a name="p1078370"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="43.55%" id="mcps1.1.4.1.2"><p id="p20239120"><a name="p20239120"></a><a name="p20239120"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="38.34%" id="mcps1.1.4.1.3"><p id="p28755990"><a name="p28755990"></a><a name="p28755990"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row47533853"><td class="cellrowborder" rowspan="7" valign="top" width="18.11%" headers="mcps1.1.4.1.1 "><p id="p25036876"><a name="p25036876"></a><a name="p25036876"></a>Zone Operations</p>
</td>
<td class="cellrowborder" valign="top" width="43.55%" headers="mcps1.1.4.1.2 "><p id="p23787231112751"><a name="p23787231112751"></a><a name="p23787231112751"></a>create_zone(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="38.34%" headers="mcps1.1.4.1.3 "><p id="p4124230911054"><a name="p4124230911054"></a><a name="p4124230911054"></a>POST /v2/zones</p>
<p id="p13898135705610"><a name="p13898135705610"></a><a name="p13898135705610"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057310891.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p2018233010402"><a name="p2018233010402"></a><a name="p2018233010402"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311027.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row61373038"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p49305737112751"><a name="p49305737112751"></a><a name="p49305737112751"></a>get_zone(self, zone)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15318330"><a name="p15318330"></a><a name="p15318330"></a>GET /v2/zones/{zone_id}</p>
<p id="p4980239195718"><a name="p4980239195718"></a><a name="p4980239195718"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129973.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p7893185912409"><a name="p7893185912409"></a><a name="p7893185912409"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311028.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row3647249"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42230846112751"><a name="p42230846112751"></a><a name="p42230846112751"></a>zones(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38847270"><a name="p38847270"></a><a name="p38847270"></a>GET /v2/zones</p>
<p id="p838455719575"><a name="p838455719575"></a><a name="p838455719575"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037134402.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p55801020104117"><a name="p55801020104117"></a><a name="p55801020104117"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311029.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row14081115"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p27568838112751"><a name="p27568838112751"></a><a name="p27568838112751"></a>delete_zone(self, zone, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44403789"><a name="p44403789"></a><a name="p44403789"></a>DELETE /v2/zones/{zone_id}</p>
<p id="p194660185813"><a name="p194660185813"></a><a name="p194660185813"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037134403.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p630814914412"><a name="p630814914412"></a><a name="p630814914412"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057311030.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row64089786"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p35802542112751"><a name="p35802542112751"></a><a name="p35802542112751"></a>nameservers(self, zone)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56055356"><a name="p56055356"></a><a name="p56055356"></a>GET /v2/zones/{zone_id}/nameservers</p>
<p id="p16802128155813"><a name="p16802128155813"></a><a name="p16802128155813"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057343056.html" target="_blank" rel="noopener noreferrer">链接</a>（公网）</p>
<p id="p127851352114117"><a name="p127851352114117"></a><a name="p127851352114117"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057342901.html" target="_blank" rel="noopener noreferrer">链接</a>（内网）</p>
</td>
</tr>
<tr id="row46356111741"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p65782031112751"><a name="p65782031112751"></a><a name="p65782031112751"></a>add_router_to_zone(self, zone, **router)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6751147111741"><a name="p6751147111741"></a><a name="p6751147111741"></a>POST /v2/zones/{zone_id}/associaterouter</p>
<p id="p1772169105911"><a name="p1772169105911"></a><a name="p1772169105911"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057329431.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6274943111746"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18759494112751"><a name="p18759494112751"></a><a name="p18759494112751"></a>remove_router_from_zone(self, zone, **router)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55688597111746"><a name="p55688597111746"></a><a name="p55688597111746"></a>POST /v2/zones/{zone_id}/disassociaterouter</p>
<p id="p695661111591"><a name="p695661111591"></a><a name="p695661111591"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0057331452.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20314447"><td class="cellrowborder" rowspan="5" valign="top" width="18.11%" headers="mcps1.1.4.1.1 "><p id="p34857543"><a name="p34857543"></a><a name="p34857543"></a>Recordset Operations</p>
</td>
<td class="cellrowborder" valign="top" width="43.55%" headers="mcps1.1.4.1.2 "><p id="p53698236112751"><a name="p53698236112751"></a><a name="p53698236112751"></a>create_recordset(self, zone, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="38.34%" headers="mcps1.1.4.1.3 "><p id="p60441935"><a name="p60441935"></a><a name="p60441935"></a>POST /v2/zones/{zone_id}/recordsets</p>
<p id="p136791114175919"><a name="p136791114175919"></a><a name="p136791114175919"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037134404.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row55322531111735"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p49002911112751"><a name="p49002911112751"></a><a name="p49002911112751"></a>get_recordset(self, zone, recordset)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46393492111735"><a name="p46393492111735"></a><a name="p46393492111735"></a>GET /v2/zone/{zone_id}/recordsets/{recordset_id}</p>
<p id="p5940141613596"><a name="p5940141613596"></a><a name="p5940141613596"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129968.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7106508"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p25171878112751"><a name="p25171878112751"></a><a name="p25171878112751"></a>all_recordsets(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52250665"><a name="p52250665"></a><a name="p52250665"></a>GET /v2/recordsets</p>
<p id="p83991199597"><a name="p83991199597"></a><a name="p83991199597"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129969.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row493939"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p63375825112751"><a name="p63375825112751"></a><a name="p63375825112751"></a>recordsets(self, zone, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19513753"><a name="p19513753"></a><a name="p19513753"></a>GET /v2/zones/{zone_id}/recordsets</p>
<p id="p7441142120595"><a name="p7441142120595"></a><a name="p7441142120595"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129970.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row41406050"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p24995877112751"><a name="p24995877112751"></a><a name="p24995877112751"></a>delete_recordset(self, zone, recordset, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8414436"><a name="p8414436"></a><a name="p8414436"></a>DELETE /v2/zones/{zone_id}/recordsets/{recordset_id}</p>
<p id="p203731125195910"><a name="p203731125195910"></a><a name="p203731125195910"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0037129971.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8621060"><td class="cellrowborder" rowspan="4" valign="top" width="18.11%" headers="mcps1.1.4.1.1 "><p id="p27217289"><a name="p27217289"></a><a name="p27217289"></a>PTR Record Operations</p>
</td>
<td class="cellrowborder" valign="top" width="43.55%" headers="mcps1.1.4.1.2 "><p id="p14459250112751"><a name="p14459250112751"></a><a name="p14459250112751"></a>create_ptr(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="38.34%" headers="mcps1.1.4.1.3 "><p id="p5860594711258"><a name="p5860594711258"></a><a name="p5860594711258"></a>PATCH /v2/reverse/floatingips/{region}:{floatingip_id}</p>
<p id="p660583075914"><a name="p660583075914"></a><a name="p660583075914"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318613.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row30668413"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p21122320112751"><a name="p21122320112751"></a><a name="p21122320112751"></a>restore_ptr(self, region, floating_ip_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3017953511258"><a name="p3017953511258"></a><a name="p3017953511258"></a>PATCH /v2/reverse/floatingips/{region}:{floatingip_id}</p>
<p id="p4251163312592"><a name="p4251163312592"></a><a name="p4251163312592"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318616.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6466753"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33615517112751"><a name="p33615517112751"></a><a name="p33615517112751"></a>ptrs(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3759833711258"><a name="p3759833711258"></a><a name="p3759833711258"></a>GET /v2/reverse/floatingips</p>
<p id="p243863795910"><a name="p243863795910"></a><a name="p243863795910"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318615.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5908907"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p44194752112751"><a name="p44194752112751"></a><a name="p44194752112751"></a>get_ptr(self, region, floating_ip_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3728940811258"><a name="p3728940811258"></a><a name="p3728940811258"></a>GET /v2/reverse/floatingips/{region}:{floatingip_id}</p>
<p id="p263611398598"><a name="p263611398598"></a><a name="p263611398598"></a><a href="https://support.huaweicloud.com/api-dns/zh-cn_topic_0042318614.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

