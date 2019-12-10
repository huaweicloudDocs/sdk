# Java-CDN<a name="ZH-CN_TOPIC_0140531507"></a>

基于CDN v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table1523315114499"></a>
<table><thead align="left"><tr id="row2234951184918"><th class="cellrowborder" valign="top" width="17.52175217521752%" id="mcps1.1.4.1.1"><p id="p62949318403"><a name="p62949318403"></a><a name="p62949318403"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.15391539153916%" id="mcps1.1.4.1.2"><p id="p5098895718403"><a name="p5098895718403"></a><a name="p5098895718403"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="43.32433243324332%" id="mcps1.1.4.1.3"><p id="p3646482918403"><a name="p3646482918403"></a><a name="p3646482918403"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row523425110494"><td class="cellrowborder" rowspan="7" valign="top" width="17.52175217521752%" headers="mcps1.1.4.1.1 "><p id="p159581830203112"><a name="p159581830203112"></a><a name="p159581830203112"></a>StatisticService</p>
</td>
<td class="cellrowborder" valign="top" width="39.15391539153916%" headers="mcps1.1.4.1.2 "><p id="p173541628163119"><a name="p173541628163119"></a><a name="p173541628163119"></a>queryTotalNetworkTraffic(**query)</p>
</td>
<td class="cellrowborder" valign="top" width="43.32433243324332%" headers="mcps1.1.4.1.3 "><p id="p1655104955016"><a name="p1655104955016"></a><a name="p1655104955016"></a>GET /v1.0/cdn/statistics/flux</p>
</td>
</tr>
<tr id="row8876172513106"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1288032571010"><a name="p1288032571010"></a><a name="p1288032571010"></a>queryDetailsOfNetworkTraffic(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18880425151014"><a name="p18880425151014"></a><a name="p18880425151014"></a>GET /v1.0/cdn/statistics/flux-detail</p>
</td>
</tr>
<tr id="row2537755201219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1253717554125"><a name="p1253717554125"></a><a name="p1253717554125"></a>queryPeakBandwidth(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1053705520123"><a name="p1053705520123"></a><a name="p1053705520123"></a>GET /v1.0/cdn/statistics/bandwidth</p>
</td>
</tr>
<tr id="row16776199141312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p07781921317"><a name="p07781921317"></a><a name="p07781921317"></a>queryDetailsOfNetworkBandwidth(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2778129161311"><a name="p2778129161311"></a><a name="p2778129161311"></a>GET /v1.0/cdn/statistics/bandwidth-detail</p>
</td>
</tr>
<tr id="row1826852514139"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8269152531316"><a name="p8269152531316"></a><a name="p8269152531316"></a>queryConsumptionSummary(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1726920257137"><a name="p1726920257137"></a><a name="p1726920257137"></a>GET /v1.0/cdn/statistics/domain-summary</p>
</td>
</tr>
<tr id="row14217346141317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p918774617131"><a name="p918774617131"></a><a name="p918774617131"></a>queryConsumptionSummaryDetails(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1118874613133"><a name="p1118874613133"></a><a name="p1118874613133"></a>GET /v1.0/cdn/statistics/domain-summary-detail</p>
</td>
</tr>
<tr id="row92401782145"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p112418851411"><a name="p112418851411"></a><a name="p112418851411"></a>queryDomainConsumptions(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3241118171410"><a name="p3241118171410"></a><a name="p3241118171410"></a>GET /v1.0/cdn/statistics/domain</p>
</td>
</tr>
<tr id="row13215102212143"><td class="cellrowborder" rowspan="19" valign="top" width="17.52175217521752%" headers="mcps1.1.4.1.1 "><p id="p52151222111419"><a name="p52151222111419"></a><a name="p52151222111419"></a>DomainService</p>
</td>
<td class="cellrowborder" valign="top" width="39.15391539153916%" headers="mcps1.1.4.1.2 "><p id="p1421542291416"><a name="p1421542291416"></a><a name="p1421542291416"></a>list(**params)</p>
</td>
<td class="cellrowborder" valign="top" width="43.32433243324332%" headers="mcps1.1.4.1.3 "><p id="p132151922141414"><a name="p132151922141414"></a><a name="p132151922141414"></a>GET /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row275592615153"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1275512611151"><a name="p1275512611151"></a><a name="p1275512611151"></a>create(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1275672661510"><a name="p1275672661510"></a><a name="p1275672661510"></a>POST /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row63830433155"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1838424321515"><a name="p1838424321515"></a><a name="p1838424321515"></a>getDetail(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16384164319155"><a name="p16384164319155"></a><a name="p16384164319155"></a>GET /v1.0/cdn/domains/{domain_id}/detail</p>
</td>
</tr>
<tr id="row94595376199"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1046018371190"><a name="p1046018371190"></a><a name="p1046018371190"></a>setOrigin(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1946073721911"><a name="p1946073721911"></a><a name="p1946073721911"></a>PUT /v1.0/cdn/domains/{domain_id}/origin</p>
</td>
</tr>
<tr id="row83365311916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p433125314192"><a name="p433125314192"></a><a name="p433125314192"></a>delete(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9338539199"><a name="p9338539199"></a><a name="p9338539199"></a>DELETE /v1.0/cdn/domains/{domain_id}</p>
</td>
</tr>
<tr id="row1764151242013"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p965612122015"><a name="p965612122015"></a><a name="p965612122015"></a>enable(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16651123208"><a name="p16651123208"></a><a name="p16651123208"></a>PUT /v1.0/cdn/domains/{domain_id}/enable</p>
</td>
</tr>
<tr id="row166913316201"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p166973316202"><a name="p166973316202"></a><a name="p166973316202"></a>disable(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p869533112010"><a name="p869533112010"></a><a name="p869533112010"></a>PUT /v1.0/cdn/domains/{domain_id}/disable</p>
</td>
</tr>
<tr id="row873284911202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4732124942010"><a name="p4732124942010"></a><a name="p4732124942010"></a>setOriginHost(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p57325498204"><a name="p57325498204"></a><a name="p57325498204"></a>PUT /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row52741617172117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2274191782120"><a name="p2274191782120"></a><a name="p2274191782120"></a>getOriginHost(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1227441702111"><a name="p1227441702111"></a><a name="p1227441702111"></a>GET /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row032673182116"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1332619317213"><a name="p1332619317213"></a><a name="p1332619317213"></a>setReferer(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p183261131142112"><a name="p183261131142112"></a><a name="p183261131142112"></a>PUT /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row9609121122219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1561011114226"><a name="p1561011114226"></a><a name="p1561011114226"></a>getReferer(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p961001162213"><a name="p961001162213"></a><a name="p961001162213"></a>GET /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row33951327122216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p739792722214"><a name="p739792722214"></a><a name="p739792722214"></a>setCacheConfig(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1397172722212"><a name="p1397172722212"></a><a name="p1397172722212"></a>PUT /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row9933202916529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17934172918522"><a name="p17934172918522"></a><a name="p17934172918522"></a>getCacheConfig(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17934152935217"><a name="p17934152935217"></a><a name="p17934152935217"></a>GET /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row19422175445216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1542335413528"><a name="p1542335413528"></a><a name="p1542335413528"></a>setHttpsInfo(domainId, **attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p842305495219"><a name="p842305495219"></a><a name="p842305495219"></a>PUT /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row1284621615532"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p178475166539"><a name="p178475166539"></a><a name="p178475166539"></a>getHttpsInfo(domainId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p384711625316"><a name="p384711625316"></a><a name="p384711625316"></a>GET /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row960983817534"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16610173805317"><a name="p16610173805317"></a><a name="p16610173805317"></a>createRefreshTask(**attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56101438155310"><a name="p56101438155310"></a><a name="p56101438155310"></a>POST /v1.0/cdn/refreshtasks</p>
</td>
</tr>
<tr id="row1284125755317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p728505715310"><a name="p728505715310"></a><a name="p728505715310"></a>createPreheatingTask(**attrs, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4285195775315"><a name="p4285195775315"></a><a name="p4285195775315"></a>POST /v1.0/cdn/preheatingtasks</p>
</td>
</tr>
<tr id="row11788151045410"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p378951011544"><a name="p378951011544"></a><a name="p378951011544"></a>queryTasks(**params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p178991085411"><a name="p178991085411"></a><a name="p178991085411"></a>GET /v1.0/cdn/historytasks</p>
</td>
</tr>
<tr id="row470012374544"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p177003373541"><a name="p177003373541"></a><a name="p177003373541"></a>getTaskDetail(taskId, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1170017378547"><a name="p1170017378547"></a><a name="p1170017378547"></a>GET /v1.0/cdn/historytasks/{task_id}/detail</p>
</td>
</tr>
<tr id="row15822191885520"><td class="cellrowborder" valign="top" width="17.52175217521752%" headers="mcps1.1.4.1.1 "><p id="p282251805511"><a name="p282251805511"></a><a name="p282251805511"></a>LogService</p>
</td>
<td class="cellrowborder" valign="top" width="39.15391539153916%" headers="mcps1.1.4.1.2 "><p id="p1082251835520"><a name="p1082251835520"></a><a name="p1082251835520"></a>queryLogs(domainName, queryDate, pageSize, pageNumber, enterpriseProjectId, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="43.32433243324332%" headers="mcps1.1.4.1.3 "><p id="p14822181819558"><a name="p14822181819558"></a><a name="p14822181819558"></a>GET /v1.0/cdn/logs</p>
</td>
</tr>
</tbody>
</table>

