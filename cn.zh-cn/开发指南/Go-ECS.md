# ECS<a name="sdk_13_0001"></a>

基于ECS v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table97391636193710"></a>
<table><thead align="left"><tr id="row077663615372"><th class="cellrowborder" valign="top" width="26.515151515151516%" id="mcps1.1.4.1.1"><p id="p137771036123713"><a name="p137771036123713"></a><a name="p137771036123713"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.535353535353536%" id="mcps1.1.4.1.2"><p id="p1177753663717"><a name="p1177753663717"></a><a name="p1177753663717"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.94949494949495%" id="mcps1.1.4.1.3"><p id="p19777836103715"><a name="p19777836103715"></a><a name="p19777836103715"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row18430654710"><td class="cellrowborder" rowspan="9" valign="top" width="26.515151515151516%" headers="mcps1.1.4.1.1 "><p id="p12419816163315"><a name="p12419816163315"></a><a name="p12419816163315"></a>CloudServers</p>
</td>
<td class="cellrowborder" valign="top" width="38.535353535353536%" headers="mcps1.1.4.1.2 "><p id="p15950021079"><a name="p15950021079"></a><a name="p15950021079"></a>GetJobResult(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" width="34.94949494949495%" headers="mcps1.1.4.1.3 "><p id="p29502211574"><a name="p29502211574"></a><a name="p29502211574"></a>GET /v1/{project_id}/jobs/{job_id}</p>
<p id="p117622031154813"><a name="p117622031154813"></a><a name="p117622031154813"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0901.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16710104019389"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p735433211396"><a name="p735433211396"></a><a name="p735433211396"></a>GetServerRecoveryStatus(client *gophercloud.ServiceClient, serverID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1611135718381"><a name="p1611135718381"></a><a name="p1611135718381"></a>GET /v1/{project_id}/cloudservers/{server_id}/autorecovery</p>
<p id="p312574124812"><a name="p312574124812"></a><a name="p312574124812"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0205.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52620441388"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7427142710399"><a name="p7427142710399"></a><a name="p7427142710399"></a>ConfigServerRecovery(client *gophercloud.ServiceClient, serverID string, opts string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1211105773811"><a name="p1211105773811"></a><a name="p1211105773811"></a>PUT /v1/{project_id}/cloudservers/{server_id}/autorecovery</p>
<p id="p121221852144812"><a name="p121221852144812"></a><a name="p121221852144812"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0206.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1678212234510"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p59681839659"><a name="p59681839659"></a><a name="p59681839659"></a>Get(client *gophercloud.ServiceClient, serverID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18968539655"><a name="p18968539655"></a><a name="p18968539655"></a>GET /v1/{project_id}/cloudservers/{server_id}</p>
<p id="p31611458104818"><a name="p31611458104818"></a><a name="p31611458104818"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0104.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row54715712476"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p169683390518"><a name="p169683390518"></a><a name="p169683390518"></a>ListDetail(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1496883915511"><a name="p1496883915511"></a><a name="p1496883915511"></a>GET /v1/{project_id}/cloudservers/detail{?flavor,name,status,limit,offset,not-tags,reservation_id,enterprise_project_id,tags}</p>
<p id="p720812684913"><a name="p720812684913"></a><a name="p720812684913"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0094148850.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1595131216472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1214405164711"><a name="p1214405164711"></a><a name="p1214405164711"></a>BatchStart(client *gophercloud.ServiceClient, opts BatchStartOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5144125134710"><a name="p5144125134710"></a><a name="p5144125134710"></a>POST /v1/{project_id}/cloudservers/action</p>
<p id="p151451451154711"><a name="p151451451154711"></a><a name="p151451451154711"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0301.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1961062913475"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17145751184720"><a name="p17145751184720"></a><a name="p17145751184720"></a>BatchReboot(client *gophercloud.ServiceClient, opts BatchRebootOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16145165116479"><a name="p16145165116479"></a><a name="p16145165116479"></a>POST /v1/{project_id}/cloudservers/action</p>
<p id="p12145351184718"><a name="p12145351184718"></a><a name="p12145351184718"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0302.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62701025164715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1514555119472"><a name="p1514555119472"></a><a name="p1514555119472"></a>BatchStop(client *gophercloud.ServiceClient, opts BatchStopOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p414585114712"><a name="p414585114712"></a><a name="p414585114712"></a>POST /v1/{project_id}/cloudservers/action</p>
<p id="p1914535111476"><a name="p1914535111476"></a><a name="p1914535111476"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0303.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row72191261856"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1514519517478"><a name="p1514519517478"></a><a name="p1514519517478"></a>BatchUpdate(client *gophercloud.ServiceClient, opts BatchUpdateOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2146145112479"><a name="p2146145112479"></a><a name="p2146145112479"></a>PUT /v1/{project_id}/cloudservers/server-name</p>
<p id="p214655104716"><a name="p214655104716"></a><a name="p214655104716"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0305.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row554762819514"><td class="cellrowborder" rowspan="4" valign="top" width="26.515151515151516%" headers="mcps1.1.4.1.1 "><p id="p131691747145116"><a name="p131691747145116"></a><a name="p131691747145116"></a>Tags</p>
</td>
<td class="cellrowborder" valign="top" width="38.535353535353536%" headers="mcps1.1.4.1.2 "><p id="p51793719529"><a name="p51793719529"></a><a name="p51793719529"></a>BatchCreateServerTags(client *gophercloud.ServiceClient, serverID string, opts BatchTagCreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="34.94949494949495%" headers="mcps1.1.4.1.3 "><p id="p617957175213"><a name="p617957175213"></a><a name="p617957175213"></a>POST /v1/{project_id}/cloudservers/{server_id}/tags/action</p>
<p id="p4179078528"><a name="p4179078528"></a><a name="p4179078528"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9399115105111"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p817915715220"><a name="p817915715220"></a><a name="p817915715220"></a>BatchDeleteServerTags(client *gophercloud.ServiceClient, serverID string, opts BatchTagDeleteOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p517912765214"><a name="p517912765214"></a><a name="p517912765214"></a>POST /v1/{project_id}/cloudservers/{server_id}/tags/action</p>
<p id="p1517917785219"><a name="p1517917785219"></a><a name="p1517917785219"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20570165575117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p161797755216"><a name="p161797755216"></a><a name="p161797755216"></a>ListProjectTags(client *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p417916719522"><a name="p417916719522"></a><a name="p417916719522"></a>GET /v1/{project_id}/cloudservers/tags</p>
<p id="p9179207125216"><a name="p9179207125216"></a><a name="p9179207125216"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62897379515"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p181806795218"><a name="p181806795218"></a><a name="p181806795218"></a>ListServerTags(client *gophercloud.ServiceClient, serverID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p01804775214"><a name="p01804775214"></a><a name="p01804775214"></a>GET /v1/{project_id}/cloudservers/{server_id}/tags</p>
<p id="p1180137185219"><a name="p1180137185219"></a><a name="p1180137185219"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于ECS v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table152111026409"></a>
<table><thead align="left"><tr id="row22979219408"><th class="cellrowborder" valign="top" width="26.669999999999998%" id="mcps1.1.4.1.1"><p id="p929732124019"><a name="p929732124019"></a><a name="p929732124019"></a><strong id="b202971225408"><a name="b202971225408"></a><a name="b202971225408"></a>Interface</strong></p>
</th>
<th class="cellrowborder" valign="top" width="38.58%" id="mcps1.1.4.1.2"><p id="p729716234016"><a name="p729716234016"></a><a name="p729716234016"></a><strong id="b192972217408"><a name="b192972217408"></a><a name="b192972217408"></a>Method</strong></p>
</th>
<th class="cellrowborder" valign="top" width="34.75%" id="mcps1.1.4.1.3"><p id="p629712134015"><a name="p629712134015"></a><a name="p629712134015"></a><strong id="b7297924406"><a name="b7297924406"></a><a name="b7297924406"></a>API</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row22971624409"><td class="cellrowborder" valign="top" width="26.669999999999998%" headers="mcps1.1.4.1.1 "><p id="p1029732134019"><a name="p1029732134019"></a><a name="p1029732134019"></a>CloudServers</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p1297122400"><a name="p1297122400"></a><a name="p1297122400"></a>ReinstallOS(client *gophercloud.ServiceClient, serverID string, opts ReinstallOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="34.75%" headers="mcps1.1.4.1.3 "><p id="p429718284014"><a name="p429718284014"></a><a name="p429718284014"></a>POST /v2/{project_id}/cloudservers/{server_id}/reinstallos</p>
<p id="p054172418141"><a name="p054172418141"></a><a name="p054172418141"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Nova v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table6059935319245"></a>
<table><thead align="left"><tr id="row36038990192419"><th class="cellrowborder" valign="top" width="26.352635263526352%" id="mcps1.1.4.1.1"><p id="p23494012192648"><a name="p23494012192648"></a><a name="p23494012192648"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.58385838583858%" id="mcps1.1.4.1.2"><p id="p61183056192648"><a name="p61183056192648"></a><a name="p61183056192648"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.063506350635066%" id="mcps1.1.4.1.3"><p id="p18860867192648"><a name="p18860867192648"></a><a name="p18860867192648"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1622153919245"><td class="cellrowborder" rowspan="20" valign="top" width="26.352635263526352%" headers="mcps1.1.4.1.1 "><p id="p4256762019245"><a name="p4256762019245"></a><a name="p4256762019245"></a>Servers</p>
</td>
<td class="cellrowborder" valign="top" width="38.58385838583858%" headers="mcps1.1.4.1.2 "><p id="p811869319245"><a name="p811869319245"></a><a name="p811869319245"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p2271036619245"><a name="p2271036619245"></a><a name="p2271036619245"></a>POST /v2/{project_id}/servers</p>
<p id="p1877834614911"><a name="p1877834614911"></a><a name="p1877834614911"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3168926119245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5869025619245"><a name="p5869025619245"></a><a name="p5869025619245"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p58090319245"><a name="p58090319245"></a><a name="p58090319245"></a>GET /v2/{project_id}/servers/detail</p>
<p id="p177101851154910"><a name="p177101851154910"></a><a name="p177101851154910"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0205.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5402404219245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4354553319245"><a name="p4354553319245"></a><a name="p4354553319245"></a>Get(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1037785319245"><a name="p1037785319245"></a><a name="p1037785319245"></a>GET /v2/{project_id}/servers/{server_id}</p>
<p id="p1397925617496"><a name="p1397925617496"></a><a name="p1397925617496"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0206.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2561627819245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3172661119245"><a name="p3172661119245"></a><a name="p3172661119245"></a>Update(client *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6242899519245"><a name="p6242899519245"></a><a name="p6242899519245"></a>PUT /v2/{project_id}/servers/{server_id}</p>
<p id="p17133238505"><a name="p17133238505"></a><a name="p17133238505"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0202.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3453425119245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5462557819245"><a name="p5462557819245"></a><a name="p5462557819245"></a>Delete(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1022845519245"><a name="p1022845519245"></a><a name="p1022845519245"></a>DELETE /v2/{project_id}/servers/{server_id}</p>
<p id="p79112175501"><a name="p79112175501"></a><a name="p79112175501"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0203.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6154711819245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2041781419245"><a name="p2041781419245"></a><a name="p2041781419245"></a>Resize(client *gophercloud.ServiceClient, id string, opts ResizeOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3025602219245"><a name="p3025602219245"></a><a name="p3025602219245"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p1329503316508"><a name="p1329503316508"></a><a name="p1329503316508"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0308.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6234667219245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p283242319245"><a name="p283242319245"></a><a name="p283242319245"></a>ConfirmResize(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p289603319245"><a name="p289603319245"></a><a name="p289603319245"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p16655174014509"><a name="p16655174014509"></a><a name="p16655174014509"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0309.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row89566219245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5986889019245"><a name="p5986889019245"></a><a name="p5986889019245"></a>RevertResize(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6115128419245"><a name="p6115128419245"></a><a name="p6115128419245"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p1993916467509"><a name="p1993916467509"></a><a name="p1993916467509"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0310.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4992485419245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5714631619245"><a name="p5714631619245"></a><a name="p5714631619245"></a>Start(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p170453619245"><a name="p170453619245"></a><a name="p170453619245"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p1032115325010"><a name="p1032115325010"></a><a name="p1032115325010"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0301.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2430414919245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5488755419245"><a name="p5488755419245"></a><a name="p5488755419245"></a>Stop(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6145961019245"><a name="p6145961019245"></a><a name="p6145961019245"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p11444858145019"><a name="p11444858145019"></a><a name="p11444858145019"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0303.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1149034619245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4855265019245"><a name="p4855265019245"></a><a name="p4855265019245"></a>Create(client *gophercloud.ServiceClient, opts servers.CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3171104619245"><a name="p3171104619245"></a><a name="p3171104619245"></a>POST /v2/{project_id}/os-volumes_boot</p>
<p id="p1779045919171"><a name="p1779045919171"></a><a name="p1779045919171"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6344620419245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4889325319245"><a name="p4889325319245"></a><a name="p4889325319245"></a>Reboot(client *gophercloud.ServiceClient, id string, opts RebootOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2480110719245"><a name="p2480110719245"></a><a name="p2480110719245"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p4461191612519"><a name="p4461191612519"></a><a name="p4461191612519"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0302.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2480164619245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p663114019245"><a name="p663114019245"></a><a name="p663114019245"></a>ResetMetadata(client *gophercloud.ServiceClient, id string, opts ResetMetadataOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4176351919245"><a name="p4176351919245"></a><a name="p4176351919245"></a>PUT /v2/{project_id}/servers/{server_id}/metadata</p>
<p id="p7350112755119"><a name="p7350112755119"></a><a name="p7350112755119"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5880203019245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5288142419245"><a name="p5288142419245"></a><a name="p5288142419245"></a>Metadata(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2453301719245"><a name="p2453301719245"></a><a name="p2453301719245"></a>GET /v2/{project_id}/servers/{server_id}/metadata</p>
<p id="p4129194355511"><a name="p4129194355511"></a><a name="p4129194355511"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6697813119245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3538823619245"><a name="p3538823619245"></a><a name="p3538823619245"></a>UpdateMetadata(client *gophercloud.ServiceClient, id string, opts UpdateMetadataOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5643494719245"><a name="p5643494719245"></a><a name="p5643494719245"></a>POST /v2/{project_id}/servers/{server_id}/metadata</p>
<p id="p3841164814556"><a name="p3841164814556"></a><a name="p3841164814556"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1395869319245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2404812319245"><a name="p2404812319245"></a><a name="p2404812319245"></a>Metadatum(client *gophercloud.ServiceClient, id, key string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2185480619245"><a name="p2185480619245"></a><a name="p2185480619245"></a>GET /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p3707155914559"><a name="p3707155914559"></a><a name="p3707155914559"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1923106819245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1907229119245"><a name="p1907229119245"></a><a name="p1907229119245"></a>DeleteMetadatum(client *gophercloud.ServiceClient, id, key string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p266336419245"><a name="p266336419245"></a><a name="p266336419245"></a>DELETE /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p163501171563"><a name="p163501171563"></a><a name="p163501171563"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row513972716710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p143630451774"><a name="p143630451774"></a><a name="p143630451774"></a>ListInstanceActions(client *gophercloud.ServiceClient, serverID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p153631145471"><a name="p153631145471"></a><a name="p153631145471"></a>GET /v2/{project_id}/servers/{server_id}/os-instance-actions</p>
<p id="p12767173065615"><a name="p12767173065615"></a><a name="p12767173065615"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1501.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11167830771"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p63633451979"><a name="p63633451979"></a><a name="p63633451979"></a>GetInstanceActions(client *gophercloud.ServiceClient, serverID string, RequestID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p113642459715"><a name="p113642459715"></a><a name="p113642459715"></a>GET /v2/{project_id}/servers/{server_id}/os-instance-actions/{request_id}</p>
<p id="p154651737175618"><a name="p154651737175618"></a><a name="p154651737175618"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1502.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1698110570467"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8655013154718"><a name="p8655013154718"></a><a name="p8655013154718"></a>GetConsoleLog(client *gophercloud.ServiceClient, id string, length string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p665571317477"><a name="p665571317477"></a><a name="p665571317477"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p185871843195617"><a name="p185871843195617"></a><a name="p185871843195617"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1601.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1665134103211"><td class="cellrowborder" rowspan="4" valign="top" width="26.352635263526352%" headers="mcps1.1.4.1.1 "><p id="p96526413321"><a name="p96526413321"></a><a name="p96526413321"></a>Interface</p>
</td>
<td class="cellrowborder" valign="top" width="38.58385838583858%" headers="mcps1.1.4.1.2 "><p id="p6551163419245"><a name="p6551163419245"></a><a name="p6551163419245"></a>List(client *gophercloud.ServiceClient, serverID string)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p998493119245"><a name="p998493119245"></a><a name="p998493119245"></a>GET /v2/{project_id}/servers/{server_id}/os-interface</p>
<p id="p465513508568"><a name="p465513508568"></a><a name="p465513508568"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row03632288358"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p173631289357"><a name="p173631289357"></a><a name="p173631289357"></a>Get(client *gophercloud.ServiceClient, serverID, portID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19782175564115"><a name="p19782175564115"></a><a name="p19782175564115"></a>GET /v2/{project_id}/servers/{server_id}/os-interface/{id}</p>
<p id="p0979145585617"><a name="p0979145585617"></a><a name="p0979145585617"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0802.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1140814361352"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15408113617355"><a name="p15408113617355"></a><a name="p15408113617355"></a>Create(client *gophercloud.ServiceClient, serverID string, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7363162820353"><a name="p7363162820353"></a><a name="p7363162820353"></a>POST /v2/{project_id}/servers/{server_id}/os-interface</p>
<p id="p166989015579"><a name="p166989015579"></a><a name="p166989015579"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0803.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row360233253519"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17603732113520"><a name="p17603732113520"></a><a name="p17603732113520"></a>Delete(client *gophercloud.ServiceClient, serverID, portID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p677855133715"><a name="p677855133715"></a><a name="p677855133715"></a>DELETE /v2/{project_id}/servers/{server_id}/os-interface/{id}</p>
<p id="p1611610717574"><a name="p1611610717574"></a><a name="p1611610717574"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0804.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5618341919245"><td class="cellrowborder" rowspan="2" valign="top" width="26.352635263526352%" headers="mcps1.1.4.1.1 "><p id="p6221827519245"><a name="p6221827519245"></a><a name="p6221827519245"></a>Flavors</p>
</td>
<td class="cellrowborder" valign="top" width="38.58385838583858%" headers="mcps1.1.4.1.2 "><p id="p4699135719245"><a name="p4699135719245"></a><a name="p4699135719245"></a>ListDetail(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p1696631019245"><a name="p1696631019245"></a><a name="p1696631019245"></a>GET /v2/{project_id}/flavors/detail</p>
<p id="p147890129577"><a name="p147890129577"></a><a name="p147890129577"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0702.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3436300119245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2659572519245"><a name="p2659572519245"></a><a name="p2659572519245"></a>Get(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4434900319245"><a name="p4434900319245"></a><a name="p4434900319245"></a>GET /v2/{project_id}/flavors/{flavor_id}</p>
<p id="p1970891815717"><a name="p1970891815717"></a><a name="p1970891815717"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0703.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3081665719245"><td class="cellrowborder" rowspan="3" valign="top" width="26.352635263526352%" headers="mcps1.1.4.1.1 "><p id="p4397474819245"><a name="p4397474819245"></a><a name="p4397474819245"></a>Images</p>
</td>
<td class="cellrowborder" valign="top" width="38.58385838583858%" headers="mcps1.1.4.1.2 "><p id="p3166370619245"><a name="p3166370619245"></a><a name="p3166370619245"></a>ListDetail(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p5522834519245"><a name="p5522834519245"></a><a name="p5522834519245"></a>GET /v2/{project_id}/images/detail</p>
<p id="p183071125175711"><a name="p183071125175711"></a><a name="p183071125175711"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0502.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3596249019245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6307912619245"><a name="p6307912619245"></a><a name="p6307912619245"></a>Delete(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4341140019245"><a name="p4341140019245"></a><a name="p4341140019245"></a>DELETE /v2/{project_id}/images/{image_id}</p>
<p id="p2913300572"><a name="p2913300572"></a><a name="p2913300572"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0505.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1072843419245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4749470019245"><a name="p4749470019245"></a><a name="p4749470019245"></a>Get(client *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p831078419245"><a name="p831078419245"></a><a name="p831078419245"></a>GET /v2/{project_id}/images/{image_id}</p>
<p id="p32621136105716"><a name="p32621136105716"></a><a name="p32621136105716"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0503.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3470548019245"><td class="cellrowborder" rowspan="4" valign="top" width="26.352635263526352%" headers="mcps1.1.4.1.1 "><p id="p5686252419245"><a name="p5686252419245"></a><a name="p5686252419245"></a>Key Pairs</p>
</td>
<td class="cellrowborder" valign="top" width="38.58385838583858%" headers="mcps1.1.4.1.2 "><p id="p3021914519245"><a name="p3021914519245"></a><a name="p3021914519245"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p4346963619245"><a name="p4346963619245"></a><a name="p4346963619245"></a>POST /v2/{project_id}/os-keypairs</p>
<p id="p14091443579"><a name="p14091443579"></a><a name="p14091443579"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212678.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1614435019245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3981551119245"><a name="p3981551119245"></a><a name="p3981551119245"></a>Get(client *gophercloud.ServiceClient, name string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2877642919245"><a name="p2877642919245"></a><a name="p2877642919245"></a>GET /v2/{project_id}/os-keypairs/{keypair_name}</p>
<p id="p74839537571"><a name="p74839537571"></a><a name="p74839537571"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1202.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5896225319245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3433195019245"><a name="p3433195019245"></a><a name="p3433195019245"></a>Delete(client *gophercloud.ServiceClient, name string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4742351219245"><a name="p4742351219245"></a><a name="p4742351219245"></a>DELETE /v2/{project_id}/os-keypairs/{keypair_name}</p>
<p id="p473362116584"><a name="p473362116584"></a><a name="p473362116584"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1204.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4831053519245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5018884319245"><a name="p5018884319245"></a><a name="p5018884319245"></a>List(client *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2317616219245"><a name="p2317616219245"></a><a name="p2317616219245"></a>GET /v2/{project_id}/os-keypairs</p>
<p id="p278910314587"><a name="p278910314587"></a><a name="p278910314587"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row29940500366"><td class="cellrowborder" rowspan="3" valign="top" width="26.352635263526352%" headers="mcps1.1.4.1.1 "><p id="p9198151343713"><a name="p9198151343713"></a><a name="p9198151343713"></a>Quotas</p>
</td>
<td class="cellrowborder" valign="top" width="38.58385838583858%" headers="mcps1.1.4.1.2 "><p id="p163541520183719"><a name="p163541520183719"></a><a name="p163541520183719"></a>GetLimits(client *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p121636123717"><a name="p121636123717"></a><a name="p121636123717"></a>GET /v2/{project_id}/limits</p>
<p id="p29554015129"><a name="p29554015129"></a><a name="p29554015129"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1101.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11417195783610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1288852493711"><a name="p1288852493711"></a><a name="p1288852493711"></a>Get(client *gophercloud.ServiceClient, tenantID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1116126173712"><a name="p1116126173712"></a><a name="p1116126173712"></a>GET /v2/{project_id}/os-quota-sets/{project_id}</p>
<p id="p19780104513126"><a name="p19780104513126"></a><a name="p19780104513126"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1102.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5902359153617"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2321112933717"><a name="p2321112933717"></a><a name="p2321112933717"></a>GetDefault(client *gophercloud.ServiceClient, ProjectID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p616156113711"><a name="p616156113711"></a><a name="p616156113711"></a>GET /v2/{project_id}/os-quota-sets/{project_id}/defaults</p>
<p id="p18851551131217"><a name="p18851551131217"></a><a name="p18851551131217"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row789942619245"><td class="cellrowborder" rowspan="5" valign="top" width="26.352635263526352%" headers="mcps1.1.4.1.1 "><p id="p531827519245"><a name="p531827519245"></a><a name="p531827519245"></a>Volumeattach</p>
</td>
<td class="cellrowborder" valign="top" width="38.58385838583858%" headers="mcps1.1.4.1.2 "><p id="p2818931219245"><a name="p2818931219245"></a><a name="p2818931219245"></a>List(client *gophercloud.ServiceClient, serverID string)</p>
</td>
<td class="cellrowborder" valign="top" width="35.063506350635066%" headers="mcps1.1.4.1.3 "><p id="p285806419245"><a name="p285806419245"></a><a name="p285806419245"></a>GET /v2/{project_id}/servers/{server_id}/os-volume_attachments</p>
<p id="p7522058111211"><a name="p7522058111211"></a><a name="p7522058111211"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0901.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6447336119245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3707799519245"><a name="p3707799519245"></a><a name="p3707799519245"></a>Create(client *gophercloud.ServiceClient, serverID string, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4143224019245"><a name="p4143224019245"></a><a name="p4143224019245"></a>POST /v2/{project_id}/servers/{server_id}/os-volume_attachments</p>
<p id="p189813311138"><a name="p189813311138"></a><a name="p189813311138"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0903.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2799310619245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2615140019245"><a name="p2615140019245"></a><a name="p2615140019245"></a>Get(client *gophercloud.ServiceClient, serverID, attachmentID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2659408319245"><a name="p2659408319245"></a><a name="p2659408319245"></a>GET /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}</p>
<p id="p1582015912130"><a name="p1582015912130"></a><a name="p1582015912130"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0902.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5733070019245"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2503866519245"><a name="p2503866519245"></a><a name="p2503866519245"></a>Delete(client *gophercloud.ServiceClient, serverID, attachmentID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6622210619245"><a name="p6622210619245"></a><a name="p6622210619245"></a>DELETE /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}</p>
<p id="p396913175132"><a name="p396913175132"></a><a name="p396913175132"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0904.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4475181316019"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1279310281302"><a name="p1279310281302"></a><a name="p1279310281302"></a>DeleteWithFlag(client *gophercloud.ServiceClient, serverID, volumeID string, deleteFlag int)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7793128401"><a name="p7793128401"></a><a name="p7793128401"></a>DELETE /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}?delete_flag={delete_flag}</p>
<p id="p2329202319133"><a name="p2329202319133"></a><a name="p2329202319133"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0904.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

