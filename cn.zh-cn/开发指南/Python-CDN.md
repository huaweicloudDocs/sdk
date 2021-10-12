# CDN<a name="sdk_12_0020"></a>

基于CDN v1.0 API的SDK接口如下，调用方式举例：conn.cdn.domains\(\)

<a name="table61508492"></a>
<table><thead align="left"><tr id="row30905118"><th class="cellrowborder" valign="top" width="26.99269926992699%" id="mcps1.1.4.1.1"><p id="p20286624"><a name="p20286624"></a><a name="p20286624"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.03360336033604%" id="mcps1.1.4.1.2"><p id="p32603834"><a name="p32603834"></a><a name="p32603834"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.97369736973697%" id="mcps1.1.4.1.3"><p id="p23664917"><a name="p23664917"></a><a name="p23664917"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row11657666"><td class="cellrowborder" rowspan="38" valign="top" width="26.99269926992699%" headers="mcps1.1.4.1.1 "><p id="p2674132855811"><a name="p2674132855811"></a><a name="p2674132855811"></a><span>Acceleration domain name</span> Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p59810509373"><a name="p59810509373"></a><a name="p59810509373"></a>domains(enterprise_project_id='ALL', page_size=100, page_number=1, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p8981850153718"><a name="p8981850153718"></a><a name="p8981850153718"></a>GET /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row53875622"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1299125093712"><a name="p1299125093712"></a><a name="p1299125093712"></a>create_domain(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1399195018372"><a name="p1399195018372"></a><a name="p1399195018372"></a>POST /v1.0/cdn/domains</p>
</td>
</tr>
<tr id="row5921358"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p29925063710"><a name="p29925063710"></a><a name="p29925063710"></a>get_domain(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1299165012376"><a name="p1299165012376"></a><a name="p1299165012376"></a>GET /v1.0/cdn/domains/{domain_id}/detail</p>
</td>
</tr>
<tr id="row553513572615"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14991650173710"><a name="p14991650173710"></a><a name="p14991650173710"></a>get_domain_detail_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2991650173711"><a name="p2991650173711"></a><a name="p2991650173711"></a>GET /v1.0/cdn/domains/{domain_id}/detail</p>
</td>
</tr>
<tr id="row13100134"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p599850133717"><a name="p599850133717"></a><a name="p599850133717"></a>delete_domain(domain_id), ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p799125053720"><a name="p799125053720"></a><a name="p799125053720"></a>DELETE /v1.0/cdn/domains/{domain_id}</p>
</td>
</tr>
<tr id="row112651787572"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p189925053718"><a name="p189925053718"></a><a name="p189925053718"></a>delete_domain_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1499185015374"><a name="p1499185015374"></a><a name="p1499185015374"></a>DELETE /v1.0/cdn/domains/{domain_id}</p>
</td>
</tr>
<tr id="row53063747"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p119915083718"><a name="p119915083718"></a><a name="p119915083718"></a>enable_domain(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p89985020376"><a name="p89985020376"></a><a name="p89985020376"></a>PUT /v1.0/cdn/domains/{domain_id}/enable</p>
</td>
</tr>
<tr id="row112281638135720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9991450173712"><a name="p9991450173712"></a><a name="p9991450173712"></a>enable_domain_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p79916506375"><a name="p79916506375"></a><a name="p79916506375"></a>PUT /v1.0/cdn/domains/{domain_id}/enable</p>
</td>
</tr>
<tr id="row48366082"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1499350143714"><a name="p1499350143714"></a><a name="p1499350143714"></a>disable_domain(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p149995012371"><a name="p149995012371"></a><a name="p149995012371"></a>PUT /v1.0/cdn/domains/{domain_id}/disable</p>
</td>
</tr>
<tr id="row18687553115714"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1799155013715"><a name="p1799155013715"></a><a name="p1799155013715"></a>disable_domain_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12991150143715"><a name="p12991150143715"></a><a name="p12991150143715"></a>PUT /v1.0/cdn/domains/{domain_id}/disable</p>
</td>
</tr>
<tr id="row16899785"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14992050103715"><a name="p14992050103715"></a><a name="p14992050103715"></a>set_domain_sources(domain_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11991650103714"><a name="p11991650103714"></a><a name="p11991650103714"></a>PUT /v1.0/cdn/domains/{domain_id}/origin</p>
</td>
</tr>
<tr id="row1499708155819"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p179965018379"><a name="p179965018379"></a><a name="p179965018379"></a>set_domain_sources_by_enterprise_project_id(domain_id, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p999195013712"><a name="p999195013712"></a><a name="p999195013712"></a>PUT /v1.0/cdn/domains/{domain_id}/origin</p>
</td>
</tr>
<tr id="row6613507"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p109975043718"><a name="p109975043718"></a><a name="p109975043718"></a>set_domain_origin_host(domain_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1199125013715"><a name="p1199125013715"></a><a name="p1199125013715"></a>PUT /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row155818343591"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p179914506371"><a name="p179914506371"></a><a name="p179914506371"></a>set_domain_origin_host_by_enterprise_project_id(domain_id, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p169925020378"><a name="p169925020378"></a><a name="p169925020378"></a>PUT /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row14546087"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p129965073717"><a name="p129965073717"></a><a name="p129965073717"></a>get_domain_origin_host(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p299165033712"><a name="p299165033712"></a><a name="p299165033712"></a>GET /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row11225251576"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p910045043715"><a name="p910045043715"></a><a name="p910045043715"></a>get_domain_origin_host_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1610018503371"><a name="p1610018503371"></a><a name="p1610018503371"></a>GET /v1.0/cdn/domains/{domain_id}/originhost</p>
</td>
</tr>
<tr id="row5574257"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p61001504372"><a name="p61001504372"></a><a name="p61001504372"></a>set_domain_range_status(domain_id,**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p510015508370"><a name="p510015508370"></a><a name="p510015508370"></a>PUT /v1.0/cdn/domains/{domainId}/range-switch</p>
</td>
</tr>
<tr id="row6540957125919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1910065033711"><a name="p1910065033711"></a><a name="p1910065033711"></a>set_domain_follow302_switch(domain_id,**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p20100135083720"><a name="p20100135083720"></a><a name="p20100135083720"></a>PUT /v1.0/cdn/domains/{domainId}/follow302-switch</p>
</td>
</tr>
<tr id="row52455718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0100135017376"><a name="p0100135017376"></a><a name="p0100135017376"></a>set_domain_referer(domain_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p110014507379"><a name="p110014507379"></a><a name="p110014507379"></a>PUT /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row321118481975"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19100195043711"><a name="p19100195043711"></a><a name="p19100195043711"></a>set_domain_referer_by_enterprise_project_id(domain_id, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1110015011373"><a name="p1110015011373"></a><a name="p1110015011373"></a>PUT /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row48094675"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1010095013377"><a name="p1010095013377"></a><a name="p1010095013377"></a>get_domain_referer(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p410035063713"><a name="p410035063713"></a><a name="p410035063713"></a>GET /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row15604541155"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p910035011370"><a name="p910035011370"></a><a name="p910035011370"></a>get_domain_referer_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p810011502376"><a name="p810011502376"></a><a name="p810011502376"></a>GET /v1.0/cdn/domains/{domain_id}/referer</p>
</td>
</tr>
<tr id="row29582349"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p61009502376"><a name="p61009502376"></a><a name="p61009502376"></a>get_domain_ip_acl(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17100175083712"><a name="p17100175083712"></a><a name="p17100175083712"></a>GET /v1.0/cdn/domains/{domainId}/ip-acl</p>
</td>
</tr>
<tr id="row583319084"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p121001950173717"><a name="p121001950173717"></a><a name="p121001950173717"></a>set_domain_ip_acl(domain_id,**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p31001350133719"><a name="p31001350133719"></a><a name="p31001350133719"></a>PUT /v1.0/cdn/domains/{domainId}/ip-acl</p>
</td>
</tr>
<tr id="row31542065"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1010085013377"><a name="p1010085013377"></a><a name="p1010085013377"></a>set_domain_cache_rules(domain_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3100650193717"><a name="p3100650193717"></a><a name="p3100650193717"></a>PUT /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row13483135017512"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1100350153714"><a name="p1100350153714"></a><a name="p1100350153714"></a>set_domain_cache_rules_by_enterprise_project_id(domain_id, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p71004500371"><a name="p71004500371"></a><a name="p71004500371"></a>PUT /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row55149989"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1610065063720"><a name="p1610065063720"></a><a name="p1610065063720"></a>get_domain_cache_rules(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1310015043720"><a name="p1310015043720"></a><a name="p1310015043720"></a>GET /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row1987182716816"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12100195012373"><a name="p12100195012373"></a><a name="p12100195012373"></a>get_domain_cache_rules_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1410013504379"><a name="p1410013504379"></a><a name="p1410013504379"></a>GET /v1.0/cdn/domains/{domain_id}/cache</p>
</td>
</tr>
<tr id="row26990100"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5100105019378"><a name="p5100105019378"></a><a name="p5100105019378"></a>set_domain_https(domain_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4101145015371"><a name="p4101145015371"></a><a name="p4101145015371"></a>PUT /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row37170869"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13101135016373"><a name="p13101135016373"></a><a name="p13101135016373"></a>set_domain_https_by_enterprise_project_id(domain_id, enterprise_project_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3101185023716"><a name="p3101185023716"></a><a name="p3101185023716"></a>PUT /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row40178308"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1101205011379"><a name="p1101205011379"></a><a name="p1101205011379"></a>get_domain_https(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p31011250153718"><a name="p31011250153718"></a><a name="p31011250153718"></a>GET /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row56379526"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17101205018378"><a name="p17101205018378"></a><a name="p17101205018378"></a>get_domain_https_by_enterprise_project_id(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p910118506375"><a name="p910118506375"></a><a name="p910118506375"></a>GET /v1.0/cdn/domains/{domain_id}/https-info</p>
</td>
</tr>
<tr id="row18133256"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16101850163714"><a name="p16101850163714"></a><a name="p16101850163714"></a>get_cdn_ips(ips)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10101115016371"><a name="p10101115016371"></a><a name="p10101115016371"></a>GET /v1.0/cdn/ip-info</p>
</td>
</tr>
<tr id="row46305995"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5101135083718"><a name="p5101135083718"></a><a name="p5101135083718"></a>get_cdn_ips_enterprise(ips, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p710185083712"><a name="p710185083712"></a><a name="p710185083712"></a>GET /v1.0/cdn/ip-info</p>
</td>
</tr>
<tr id="row39197567"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13101050163710"><a name="p13101050163710"></a><a name="p13101050163710"></a>set_domain_response_header(domain_id,**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19101135015374"><a name="p19101135015374"></a><a name="p19101135015374"></a>PUT /v1.0/cdn/domains/{domainId}/response-header</p>
</td>
</tr>
<tr id="row59552004"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2010285015372"><a name="p2010285015372"></a><a name="p2010285015372"></a>set_domain_response_header_enterprise(domain_id, enterprise_project_id,**attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17102350203713"><a name="p17102350203713"></a><a name="p17102350203713"></a>PUT /v1.0/cdn/domains/{domainId}/response-header</p>
</td>
</tr>
<tr id="row2062181214593"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1810265015379"><a name="p1810265015379"></a><a name="p1810265015379"></a>get_domain_response_header(domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7102155073713"><a name="p7102155073713"></a><a name="p7102155073713"></a>GET /v1.0/cdn/domains/{domainId}/response-header</p>
</td>
</tr>
<tr id="row48930647"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9102150103720"><a name="p9102150103720"></a><a name="p9102150103720"></a>get_domain_response_header_enterprise(domain_id, enterprise_project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p141021950193720"><a name="p141021950193720"></a><a name="p141021950193720"></a>GET /v1.0/cdn/domains/{domainId}/response-header</p>
</td>
</tr>
<tr id="row860783410219"><td class="cellrowborder" rowspan="14" valign="top" width="26.99269926992699%" headers="mcps1.1.4.1.1 "><p id="p1860753418220"><a name="p1860753418220"></a><a name="p1860753418220"></a>Statistic Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p610255073715"><a name="p610255073715"></a><a name="p610255073715"></a>query_top_url(**query)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p12102145053711"><a name="p12102145053711"></a><a name="p12102145053711"></a>GET /v1.0/cdn/statistics/top-url</p>
</td>
</tr>
<tr id="row967091012220"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1510295023711"><a name="p1510295023711"></a><a name="p1510295023711"></a>query_domain_item_details(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3102350133717"><a name="p3102350133717"></a><a name="p3102350133717"></a>GET /v1.0/cdn/statistics/domain-item-details</p>
</td>
</tr>
<tr id="row666410181227"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20102155033716"><a name="p20102155033716"></a><a name="p20102155033716"></a>query_domain_item_location_details(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21021450173710"><a name="p21021450173710"></a><a name="p21021450173710"></a>GET /v1.0/cdn/statistics/domain-item-location-details</p>
</td>
</tr>
<tr id="row1539515195915"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2102105093718"><a name="p2102105093718"></a><a name="p2102105093718"></a>query_network_traffic(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p0102175023715"><a name="p0102175023715"></a><a name="p0102175023715"></a>GET /v1.0/cdn/statistics/flux</p>
</td>
</tr>
<tr id="row137051214225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p161025505371"><a name="p161025505371"></a><a name="p161025505371"></a>query_network_traffic_detail(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1310295015371"><a name="p1310295015371"></a><a name="p1310295015371"></a>GET /v1.0/cdn/statistics/flux-detail</p>
</td>
</tr>
<tr id="row790373618214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4102850103720"><a name="p4102850103720"></a><a name="p4102850103720"></a>query_bandwidth_peak(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p111031550103711"><a name="p111031550103711"></a><a name="p111031550103711"></a>GET /v1.0/cdn/statistics/bandwidth</p>
</td>
</tr>
<tr id="row16961012228"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1510325083719"><a name="p1510325083719"></a><a name="p1510325083719"></a>query_bandwidth(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1110312501377"><a name="p1110312501377"></a><a name="p1110312501377"></a>GET /v1.0/cdn/statistics/bandwidth-detail</p>
</td>
</tr>
<tr id="row13787207226"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p191030500378"><a name="p191030500378"></a><a name="p191030500378"></a>query_summary(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1510365063710"><a name="p1510365063710"></a><a name="p1510365063710"></a>GET /v1.0/cdn/statistics/domain-summary</p>
</td>
</tr>
<tr id="row47252515212"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p110385013378"><a name="p110385013378"></a><a name="p110385013378"></a>query_summary_detail(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p910355033710"><a name="p910355033710"></a><a name="p910355033710"></a>GET /v1.0/cdn/statistics/domain-summary-detail</p>
</td>
</tr>
<tr id="row7423193325"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p710335016371"><a name="p710335016371"></a><a name="p710335016371"></a>summaries(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12103195011374"><a name="p12103195011374"></a><a name="p12103195011374"></a>GET /v1.0/cdn/statistics/domain</p>
</td>
</tr>
<tr id="row384718615915"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12103175016373"><a name="p12103175016373"></a><a name="p12103175016373"></a>query_region_detail_summary(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1010355014372"><a name="p1010355014372"></a><a name="p1010355014372"></a>GET /v1.0/cdn/statistics/region-detail-summary</p>
</td>
</tr>
<tr id="row370121015590"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p110311501378"><a name="p110311501378"></a><a name="p110311501378"></a>query_carrier_detail_summary(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18103950113712"><a name="p18103950113712"></a><a name="p18103950113712"></a>GET /v1.0/cdn/statistics/carrier-detail-summary</p>
</td>
</tr>
<tr id="row377018285214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16103450193713"><a name="p16103450193713"></a><a name="p16103450193713"></a>query_region_carrier_domain(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14103135023718"><a name="p14103135023718"></a><a name="p14103135023718"></a>GET /v1.0/cdn/statistics/region-carrier-domain</p>
</td>
</tr>
<tr id="row1149133019211"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20103135012376"><a name="p20103135012376"></a><a name="p20103135012376"></a>query_region_carrier_detail(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7103205011377"><a name="p7103205011377"></a><a name="p7103205011377"></a>GET /v1.0/cdn/statistics/region-carrier-detail</p>
</td>
</tr>
<tr id="row1086418266215"><td class="cellrowborder" rowspan="2" valign="top" width="26.99269926992699%" headers="mcps1.1.4.1.1 "><p id="p986414267216"><a name="p986414267216"></a><a name="p986414267216"></a>Log Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p2010318501373"><a name="p2010318501373"></a><a name="p2010318501373"></a>logs(domain_name, query_date,</p>
<p id="p010315018373"><a name="p010315018373"></a><a name="p010315018373"></a>page_size=100, page_number=1)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p61031750133711"><a name="p61031750133711"></a><a name="p61031750133711"></a>GET /v1.0/cdn/logs</p>
</td>
</tr>
<tr id="row1164571785910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p51051500371"><a name="p51051500371"></a><a name="p51051500371"></a>logs_by_enterprise_project_id（domain_name, query_date,</p>
<p id="p510515043714"><a name="p510515043714"></a><a name="p510515043714"></a>page_size=100, page_number=1, enterprise_project_id）</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p191058500372"><a name="p191058500372"></a><a name="p191058500372"></a>GET /v1.0/cdn/logs</p>
</td>
</tr>
<tr id="row745084"><td class="cellrowborder" valign="top" width="26.99269926992699%" headers="mcps1.1.4.1.1 "><p id="p185281636774"><a name="p185281636774"></a><a name="p185281636774"></a><span>Preheating task </span>Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p16105650183720"><a name="p16105650183720"></a><a name="p16105650183720"></a>create_preheat_task(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p5106185053714"><a name="p5106185053714"></a><a name="p5106185053714"></a>POST /v1.0/cdn/preheatingtasks</p>
</td>
</tr>
<tr id="row40216515"><td class="cellrowborder" valign="top" width="26.99269926992699%" headers="mcps1.1.4.1.1 "><p id="p852843620714"><a name="p852843620714"></a><a name="p852843620714"></a><span>Refreshing task </span>Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p3106195019378"><a name="p3106195019378"></a><a name="p3106195019378"></a>create_refresh_task(**attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p1010695018371"><a name="p1010695018371"></a><a name="p1010695018371"></a>POST /v1.0/cdn/refreshtasks</p>
</td>
</tr>
<tr id="row109961723113210"><td class="cellrowborder" rowspan="2" valign="top" width="26.99269926992699%" headers="mcps1.1.4.1.1 "><p id="p45296361672"><a name="p45296361672"></a><a name="p45296361672"></a><span>Query task </span>Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p710618509373"><a name="p710618509373"></a><a name="p710618509373"></a>tasks(page_size=100, page_number=1, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p61061450143715"><a name="p61061450143715"></a><a name="p61061450143715"></a>GET /v1.0/cdn/historytasks</p>
</td>
</tr>
<tr id="row30735614"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1110685093717"><a name="p1110685093717"></a><a name="p1110685093717"></a>get_task(task_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p131069500371"><a name="p131069500371"></a><a name="p131069500371"></a>GET /v1.0/cdn/historytasks/{task_id}/detail</p>
</td>
</tr>
</tbody>
</table>

