# Python-CDN<a name="ZH-CN_TOPIC_0119046158"></a>

基于CDN v1.0 API的SDK接口如下，调用方式举例：conn.cdn.domains\(\)

<a name="table61508492"></a>
<table><thead align="left"><tr id="row30905118"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="p20286624"><a name="p20286624"></a><a name="p20286624"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="p32603834"><a name="p32603834"></a><a name="p32603834"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="p23664917"><a name="p23664917"></a><a name="p23664917"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row11657666"><td class="cellrowborder" rowspan="32" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p4746913"><a name="p4746913"></a><a name="p4746913"></a>Domain Operations</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p10301551195613"><a name="p10301551195613"></a><a name="p10301551195613"></a>domains(enterprise_project_id='ALL', page_size=100, page_number=1, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p5986180"><a name="p5986180"></a><a name="p5986180"></a>GET /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row53875622"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1849243"><a name="p1849243"></a><a name="p1849243"></a>create_domain(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15571009"><a name="p15571009"></a><a name="p15571009"></a>POST /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row5921358"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9867967"><a name="p9867967"></a><a name="p9867967"></a>get_domain(domain)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p61107894"><a name="p61107894"></a><a name="p61107894"></a>GET /v1.0/cdn/domains/{domain_id}/detail</p>
</td>
</tr>
<tr id="row553513572615"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7535357964"><a name="p7535357964"></a><a name="p7535357964"></a>get_domain_detail_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p124121136710"><a name="p124121136710"></a><a name="p124121136710"></a>GET /v1.0/cdn/domains/{domain_id}/detail</p>
</td>
</tr>
<tr id="row13100134"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54477918"><a name="p54477918"></a><a name="p54477918"></a>set_domain_sources(domain, *sources)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p50635214"><a name="p50635214"></a><a name="p50635214"></a>PUT /v1.0/cdn/domains/{domain_id}/origin</p>
</td>
</tr>
<tr id="row112651787572"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18265178115720"><a name="p18265178115720"></a><a name="p18265178115720"></a>set_domain_sources_by_enterprise_project_id(domain, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1126613811576"><a name="p1126613811576"></a><a name="p1126613811576"></a>PUT /v1.0/cdn/domains/{domain_id}/origin</p>
</td>
</tr>
<tr id="row53063747"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3196251"><a name="p3196251"></a><a name="p3196251"></a>delete_domain(domain, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p57569792"><a name="p57569792"></a><a name="p57569792"></a>DELETE /v1.0/cdn/domains/{domain_id}</p>
</td>
</tr>
<tr id="row112281638135720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p152285387572"><a name="p152285387572"></a><a name="p152285387572"></a>delete_domain_by_enterprise_project_id(domain, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6793134225715"><a name="p6793134225715"></a><a name="p6793134225715"></a>DELETE /v1.0/cdn/domains/{domain_id}</p>
</td>
</tr>
<tr id="row48366082"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p25338597"><a name="p25338597"></a><a name="p25338597"></a>enable_domain(domain)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p39160456"><a name="p39160456"></a><a name="p39160456"></a>PUT /v1.0/cdn/domains/{domain_id}/enable</p>
</td>
</tr>
<tr id="row18687553115714"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p116881653165712"><a name="p116881653165712"></a><a name="p116881653165712"></a>enable_domain_by_enterprise_project_id(domain, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1368825316578"><a name="p1368825316578"></a><a name="p1368825316578"></a>PUT /v1.0/cdn/domains/{domain_id}/enable</p>
</td>
</tr>
<tr id="row16899785"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26705327"><a name="p26705327"></a><a name="p26705327"></a>disable_domain(domain)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15647915"><a name="p15647915"></a><a name="p15647915"></a>PUT /v1.0/cdn/domains/{domain_id}/disable</p>
</td>
</tr>
<tr id="row1499708155819"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0998184587"><a name="p0998184587"></a><a name="p0998184587"></a>disable_domain_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18460151415589"><a name="p18460151415589"></a><a name="p18460151415589"></a>PUT /v1.0/cdn/domains/{domain_id}/disable</p>
</td>
</tr>
<tr id="row6613507"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p65932088"><a name="p65932088"></a><a name="p65932088"></a>set_domain_origin_host(domain, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38898934"><a name="p38898934"></a><a name="p38898934"></a>PUT /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row155818343591"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p259203475913"><a name="p259203475913"></a><a name="p259203475913"></a>set_domain_origin_host_by_enterprise_project_id(domain, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p65973411598"><a name="p65973411598"></a><a name="p65973411598"></a>PUT /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row14546087"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p37382404"><a name="p37382404"></a><a name="p37382404"></a>get_domain_origin_host(domain)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8075902"><a name="p8075902"></a><a name="p8075902"></a>GET /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row11225251576"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1512316251073"><a name="p1512316251073"></a><a name="p1512316251073"></a>get_domain_origin_host_by_enterprise_project_id(domain, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1121183016718"><a name="p1121183016718"></a><a name="p1121183016718"></a>GET /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row5574257"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p48861664"><a name="p48861664"></a><a name="p48861664"></a>set_domain_referer(domain, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p65480736"><a name="p65480736"></a><a name="p65480736"></a>PUT /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row6540957125919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10542757165912"><a name="p10542757165912"></a><a name="p10542757165912"></a>set_domain_referer_by_enterprise_project_id(domain, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4120534013"><a name="p4120534013"></a><a name="p4120534013"></a>PUT /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row52455718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p21054754"><a name="p21054754"></a><a name="p21054754"></a>get_domain_referer(domain)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p27713474"><a name="p27713474"></a><a name="p27713474"></a>GET /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row321118481975"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p102121648176"><a name="p102121648176"></a><a name="p102121648176"></a>get_domain_referer_by_enterprise_project_id(domain, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13409752576"><a name="p13409752576"></a><a name="p13409752576"></a>GET /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row48094675"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3354597"><a name="p3354597"></a><a name="p3354597"></a>set_domain_cache_rules(domain, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3286927"><a name="p3286927"></a><a name="p3286927"></a>PUT /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row15604541155"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10606541955"><a name="p10606541955"></a><a name="p10606541955"></a>set_domain_cache_rules_by_enterprise_project_id(domain, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1582715458514"><a name="p1582715458514"></a><a name="p1582715458514"></a>PUT /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row29582349"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p47360079"><a name="p47360079"></a><a name="p47360079"></a>get_domain_cache_rules(domain)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10961214"><a name="p10961214"></a><a name="p10961214"></a>GET /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row583319084"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6833189688"><a name="p6833189688"></a><a name="p6833189688"></a>get_domain_cache_rules_by_enterprise_project_id(domain, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p176727151083"><a name="p176727151083"></a><a name="p176727151083"></a>GET /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row31542065"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4770510"><a name="p4770510"></a><a name="p4770510"></a>set_domain_https(domain, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p50867019"><a name="p50867019"></a><a name="p50867019"></a>PUT /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row13483135017512"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p648412501453"><a name="p648412501453"></a><a name="p648412501453"></a>set_domain_https_by_enterprise_project_id(domain, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p931912362"><a name="p931912362"></a><a name="p931912362"></a>PUT /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row55149989"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p37964118"><a name="p37964118"></a><a name="p37964118"></a>get_domain_https(domain)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55194683"><a name="p55194683"></a><a name="p55194683"></a>GET /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row1987182716816"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1488112715820"><a name="p1488112715820"></a><a name="p1488112715820"></a>get_domain_https_by_enterprise_project_id(domain, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1849420335817"><a name="p1849420335817"></a><a name="p1849420335817"></a>GET /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row26990100"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p38714531"><a name="p38714531"></a><a name="p38714531"></a>create_refresh_task(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p48869339"><a name="p48869339"></a><a name="p48869339"></a>POST /v1.0/cdn/refreshtasks</p>
</td>
</tr>
<tr id="row37170869"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58050428"><a name="p58050428"></a><a name="p58050428"></a>create_preheat_task(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4464256"><a name="p4464256"></a><a name="p4464256"></a>POST /v1.0/cdn/preheatingtasks</p>
</td>
</tr>
<tr id="row40178308"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33217517"><a name="p33217517"></a><a name="p33217517"></a>tasks(page_size=100, page_number=1, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6264391"><a name="p6264391"></a><a name="p6264391"></a>GET /v1.0/cdn/historytasks</p>
</td>
</tr>
<tr id="row56379526"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3338892"><a name="p3338892"></a><a name="p3338892"></a>get_task(task)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2014806"><a name="p2014806"></a><a name="p2014806"></a>GET /v1.0/cdn/historytasks/{task_id}/detail</p>
</td>
</tr>
<tr id="row18133256"><td class="cellrowborder" rowspan="7" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p59507636"><a name="p59507636"></a><a name="p59507636"></a>Statistic Operations</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p55389208"><a name="p55389208"></a><a name="p55389208"></a>query_network_traffic(**query)</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p57340893"><a name="p57340893"></a><a name="p57340893"></a>GET /v1.0/cdn/statistics/flux</p>
</td>
</tr>
<tr id="row46305995"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p59798148"><a name="p59798148"></a><a name="p59798148"></a>query_network_traffic_detail(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11811825"><a name="p11811825"></a><a name="p11811825"></a>GET /v1.0/cdn/statistics/flux-detail</p>
</td>
</tr>
<tr id="row39197567"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20886358"><a name="p20886358"></a><a name="p20886358"></a>query_bandwidth_peak(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14073429"><a name="p14073429"></a><a name="p14073429"></a>GET /v1.0/cdn/statistics/bandwidth</p>
</td>
</tr>
<tr id="row59552004"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58982995"><a name="p58982995"></a><a name="p58982995"></a>query_bandwidth(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12893279"><a name="p12893279"></a><a name="p12893279"></a>GET /v1.0/cdn/statistics/bandwidth-detail</p>
</td>
</tr>
<tr id="row48930647"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3959432"><a name="p3959432"></a><a name="p3959432"></a>query_summary(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52278570"><a name="p52278570"></a><a name="p52278570"></a>GET /v1.0/cdn/statistics/domain-summary</p>
</td>
</tr>
<tr id="row745084"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60351882"><a name="p60351882"></a><a name="p60351882"></a>query_summary_detail(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56664284"><a name="p56664284"></a><a name="p56664284"></a>GET /v1.0/cdn/statistics/domain-summary-detail</p>
</td>
</tr>
<tr id="row40216515"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p36312246"><a name="p36312246"></a><a name="p36312246"></a>summaries(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55610851"><a name="p55610851"></a><a name="p55610851"></a>GET /v1.0/cdn/statistics/domain</p>
</td>
</tr>
<tr id="row30735614"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p6556786"><a name="p6556786"></a><a name="p6556786"></a>Log Operations</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p61337651"><a name="p61337651"></a><a name="p61337651"></a>logs(domain_name, query_date,</p>
<p id="p15167947"><a name="p15167947"></a><a name="p15167947"></a>page_size=100, page_number=1, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p20644201"><a name="p20644201"></a><a name="p20644201"></a>GET /v1.0/cdn/logs</p>
</td>
</tr>
</tbody>
</table>

