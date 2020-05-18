# CDN<a name="sdk_11_0019"></a>

基于CDN v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table1523315114499"></a>
<table><thead align="left"><tr id="row2234951184918"><th class="cellrowborder" valign="top" width="28.372837283728376%" id="mcps1.1.4.1.1"><p id="p62949318403"><a name="p62949318403"></a><a name="p62949318403"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.03360336033604%" id="mcps1.1.4.1.2"><p id="p5098895718403"><a name="p5098895718403"></a><a name="p5098895718403"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.5935593559356%" id="mcps1.1.4.1.3"><p id="p3646482918403"><a name="p3646482918403"></a><a name="p3646482918403"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row523425110494"><td class="cellrowborder" rowspan="26" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p1238710141532"><a name="p1238710141532"></a><a name="p1238710141532"></a>DomainService</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p44361006534"><a name="p44361006534"></a><a name="p44361006534"></a>list(**params)</p>
</td>
<td class="cellrowborder" valign="top" width="35.5935593559356%" headers="mcps1.1.4.1.3 "><p id="p1943600165315"><a name="p1943600165315"></a><a name="p1943600165315"></a>GET /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row8876172513106"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p343615085311"><a name="p343615085311"></a><a name="p343615085311"></a>create(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1943614055312"><a name="p1943614055312"></a><a name="p1943614055312"></a>POST /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row2537755201219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19436908536"><a name="p19436908536"></a><a name="p19436908536"></a>getDetail(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p643614095319"><a name="p643614095319"></a><a name="p643614095319"></a>GET /v1.0/cdn/domains/{domain_id}/detail</p>
</td>
</tr>
<tr id="row16776199141312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p643615065314"><a name="p643615065314"></a><a name="p643615065314"></a>delete(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p0436907537"><a name="p0436907537"></a><a name="p0436907537"></a>DELETE /v1.0/cdn/domains/{domain_id}</p>
</td>
</tr>
<tr id="row1826852514139"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p114368011538"><a name="p114368011538"></a><a name="p114368011538"></a>enable(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p144368055311"><a name="p144368055311"></a><a name="p144368055311"></a>PUT /v1.0/cdn/domains/{domain_id}/enable</p>
</td>
</tr>
<tr id="row14217346141317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4437140165319"><a name="p4437140165319"></a><a name="p4437140165319"></a>disable(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15437904536"><a name="p15437904536"></a><a name="p15437904536"></a>PUT /v1.0/cdn/domains/{domain_id}/disable</p>
</td>
</tr>
<tr id="row92401782145"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11437403539"><a name="p11437403539"></a><a name="p11437403539"></a>setOrigin(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1043730195317"><a name="p1043730195317"></a><a name="p1043730195317"></a>PUT /v1.0/cdn/domains/{domain_id}/origin</p>
</td>
</tr>
<tr id="row13215102212143"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p114371701537"><a name="p114371701537"></a><a name="p114371701537"></a>setOriginHost(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p143770115310"><a name="p143770115310"></a><a name="p143770115310"></a>PUT /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row275592615153"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1843720018534"><a name="p1843720018534"></a><a name="p1843720018534"></a>getOriginHost(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p143780115316"><a name="p143780115316"></a><a name="p143780115316"></a>GET /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row63830433155"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0437180105312"><a name="p0437180105312"></a><a name="p0437180105312"></a>setOriginRange(domainId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p154371903535"><a name="p154371903535"></a><a name="p154371903535"></a>PUT /v1.0/cdn/domains/{domainId}/range-switch</p>
</td>
</tr>
<tr id="row192132198452"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14371206534"><a name="p14371206534"></a><a name="p14371206534"></a>setFollow302(domainId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1743716035311"><a name="p1743716035311"></a><a name="p1743716035311"></a>PUT /v1.0/cdn/domains/{domainId}/follow302-switch</p>
</td>
</tr>
<tr id="row6807131534518"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p194372001532"><a name="p194372001532"></a><a name="p194372001532"></a>setReferer(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p164371025312"><a name="p164371025312"></a><a name="p164371025312"></a>PUT /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row1511016138454"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p124379085312"><a name="p124379085312"></a><a name="p124379085312"></a>getReferer(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p043711085312"><a name="p043711085312"></a><a name="p043711085312"></a>GET /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row94595376199"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p443713045314"><a name="p443713045314"></a><a name="p443713045314"></a>getIpAcl(domainId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19437100145317"><a name="p19437100145317"></a><a name="p19437100145317"></a>GET /v1.0/cdn/domains/{domainId}/ip-acl</p>
</td>
</tr>
<tr id="row83365311916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1437200125315"><a name="p1437200125315"></a><a name="p1437200125315"></a>setIpAcl(domainId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11437902536"><a name="p11437902536"></a><a name="p11437902536"></a>PUT /v1.0/cdn/domains/{domainId}/ip-acl</p>
</td>
</tr>
<tr id="row1979211518470"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3437190105316"><a name="p3437190105316"></a><a name="p3437190105316"></a>setCacheConfig(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44372015530"><a name="p44372015530"></a><a name="p44372015530"></a>PUT /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row1764151242013"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p04371102537"><a name="p04371102537"></a><a name="p04371102537"></a>getCacheConfig(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p184376095315"><a name="p184376095315"></a><a name="p184376095315"></a>GET /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row166913316201"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1743770205313"><a name="p1743770205313"></a><a name="p1743770205313"></a>setHttpsInfo(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12437207534"><a name="p12437207534"></a><a name="p12437207534"></a>PUT /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row873284911202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p143720011532"><a name="p143720011532"></a><a name="p143720011532"></a>getHttpsInfo(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p84381020530"><a name="p84381020530"></a><a name="p84381020530"></a>GET /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row52741617172117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p843817017530"><a name="p843817017530"></a><a name="p843817017530"></a>queryCdnIPs(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2043810015315"><a name="p2043810015315"></a><a name="p2043810015315"></a>GET /v1.0/cdn/ip-info</p>
</td>
</tr>
<tr id="row032673182116"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p184388011539"><a name="p184388011539"></a><a name="p184388011539"></a>setResponseHeader(domainId, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17438607531"><a name="p17438607531"></a><a name="p17438607531"></a>PUT /v1.0/cdn/domains/{domainId}/response-header</p>
</td>
</tr>
<tr id="row9609121122219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1743810015311"><a name="p1743810015311"></a><a name="p1743810015311"></a>getResponseHeader(domainId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p64388014534"><a name="p64388014534"></a><a name="p64388014534"></a>GET /v1.0/cdn/domains/{domainId}/response-header</p>
</td>
</tr>
<tr id="row33951327122216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3438406531"><a name="p3438406531"></a><a name="p3438406531"></a>createRefreshTask(**attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p124389015317"><a name="p124389015317"></a><a name="p124389015317"></a>POST /v1.0/cdn/refreshtasks</p>
</td>
</tr>
<tr id="row9933202916529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13438705535"><a name="p13438705535"></a><a name="p13438705535"></a>createPreheatingTask(**attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10438150185311"><a name="p10438150185311"></a><a name="p10438150185311"></a>POST /v1.0/cdn/preheatingtasks</p>
</td>
</tr>
<tr id="row7218050205218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p84388015318"><a name="p84388015318"></a><a name="p84388015318"></a>queryTasks(**params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p643880165312"><a name="p643880165312"></a><a name="p643880165312"></a>GET /v1.0/cdn/historytasks</p>
</td>
</tr>
<tr id="row6910164785210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1143818095314"><a name="p1143818095314"></a><a name="p1143818095314"></a>getTaskDetail(taskId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p0438202532"><a name="p0438202532"></a><a name="p0438202532"></a>GET /v1.0/cdn/historytasks/{task_id}/detail</p>
</td>
</tr>
<tr id="row19422175445216"><td class="cellrowborder" rowspan="14" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p10473123195318"><a name="p10473123195318"></a><a name="p10473123195318"></a>StatisticService</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p81531131185412"><a name="p81531131185412"></a><a name="p81531131185412"></a>queryTopUrl(**query)</p>
</td>
<td class="cellrowborder" valign="top" width="35.5935593559356%" headers="mcps1.1.4.1.3 "><p id="p10153133155417"><a name="p10153133155417"></a><a name="p10153133155417"></a>GET /v1.0/cdn/statistics/top-url</p>
</td>
</tr>
<tr id="row356024515523"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2015343120541"><a name="p2015343120541"></a><a name="p2015343120541"></a>queryDomainItemDetails(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10153183185419"><a name="p10153183185419"></a><a name="p10153183185419"></a>GET /v1.0/cdn/statistics/domain-item-details</p>
</td>
</tr>
<tr id="row1284621615532"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p915353119546"><a name="p915353119546"></a><a name="p915353119546"></a>queryDomainItemLocationDetails(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p161530319546"><a name="p161530319546"></a><a name="p161530319546"></a>GET /v1.0/cdn/statistics/domain-item-location-details</p>
</td>
</tr>
<tr id="row1666119219545"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11154131105411"><a name="p11154131105411"></a><a name="p11154131105411"></a>queryTotalNetworkTraffic(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p515413105416"><a name="p515413105416"></a><a name="p515413105416"></a>GET /v1.0/cdn/statistics/flux</p>
</td>
</tr>
<tr id="row20542612544"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12154031205416"><a name="p12154031205416"></a><a name="p12154031205416"></a>queryDetailsOfNetworkTraffic(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3154153113548"><a name="p3154153113548"></a><a name="p3154153113548"></a>GET /v1.0/cdn/statistics/flux-detail</p>
</td>
</tr>
<tr id="row7735142546"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16154163155412"><a name="p16154163155412"></a><a name="p16154163155412"></a>queryPeakBandwidth(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4154193115418"><a name="p4154193115418"></a><a name="p4154193115418"></a>GET /v1.0/cdn/statistics/bandwidth</p>
</td>
</tr>
<tr id="row2030871215412"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10154123114543"><a name="p10154123114543"></a><a name="p10154123114543"></a>queryDetailsOfNetworkBandwidth(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p201540314542"><a name="p201540314542"></a><a name="p201540314542"></a>GET /v1.0/cdn/statistics/bandwidth-detail</p>
</td>
</tr>
<tr id="row16831169145420"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5154631115413"><a name="p5154631115413"></a><a name="p5154631115413"></a>queryConsumptionSummary(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p715410316547"><a name="p715410316547"></a><a name="p715410316547"></a>GET /v1.0/cdn/statistics/domain-summary</p>
</td>
</tr>
<tr id="row1695077125416"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p151541631145419"><a name="p151541631145419"></a><a name="p151541631145419"></a>queryConsumptionSummaryDetails(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2154153115415"><a name="p2154153115415"></a><a name="p2154153115415"></a>GET /v1.0/cdn/statistics/domain-summary-detail</p>
</td>
</tr>
<tr id="row960983817534"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p131541531185416"><a name="p131541531185416"></a><a name="p131541531185416"></a>queryDomainConsumptions(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p141541631105415"><a name="p141541631105415"></a><a name="p141541631105415"></a>GET /v1.0/cdn/statistics/domain</p>
</td>
</tr>
<tr id="row1284125755317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5154173175411"><a name="p5154173175411"></a><a name="p5154173175411"></a>queryRegionDetailSummry(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11541331165416"><a name="p11541331165416"></a><a name="p11541331165416"></a>GET /v1.0/cdn/statistics/region-detail-summary</p>
</td>
</tr>
<tr id="row13591003548"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p115443135411"><a name="p115443135411"></a><a name="p115443135411"></a>queryCarrierDetailSummry(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1415415311540"><a name="p1415415311540"></a><a name="p1415415311540"></a>GET /v1.0/cdn/statistics/carrier-detail-summary</p>
</td>
</tr>
<tr id="row12653145814530"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p131541631175410"><a name="p131541631175410"></a><a name="p131541631175410"></a>queryRegionCarrierDomain(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p31541431185411"><a name="p31541431185411"></a><a name="p31541431185411"></a>GET /v1.0/cdn/statistics/region-carrier-domain</p>
</td>
</tr>
<tr id="row11788151045410"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10154131185413"><a name="p10154131185413"></a><a name="p10154131185413"></a>queryRegionCarrierDetail(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p91541231185416"><a name="p91541231185416"></a><a name="p91541231185416"></a>GET /v1.0/cdn/statistics/region-carrier-detail</p>
</td>
</tr>
<tr id="row951404205212"><td class="cellrowborder" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p4759157135412"><a name="p4759157135412"></a><a name="p4759157135412"></a>LogService</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p107593571546"><a name="p107593571546"></a><a name="p107593571546"></a>queryLogs(domainName, queryDate, pageSize, pageNumber, enterpriseProjectId)</p>
</td>
<td class="cellrowborder" valign="top" width="35.5935593559356%" headers="mcps1.1.4.1.3 "><p id="p137591457125420"><a name="p137591457125420"></a><a name="p137591457125420"></a>GET /v1.0/cdn/logs</p>
</td>
</tr>
</tbody>
</table>

