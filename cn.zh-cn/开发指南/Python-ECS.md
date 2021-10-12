# ECS<a name="sdk_12_0004"></a>

基于Nova v2 API的SDK接口如下，调用方式举例如下：conn.compute.create\_server\(\)

<a name="table40336211"></a>
<table><thead align="left"><tr id="row58082052"><th class="cellrowborder" valign="top" width="26.247375262473753%" id="mcps1.1.4.1.1"><p id="p7025744"><a name="p7025744"></a><a name="p7025744"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="41.12588741125888%" id="mcps1.1.4.1.2"><p id="p32214417"><a name="p32214417"></a><a name="p32214417"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.62673732626737%" id="mcps1.1.4.1.3"><p id="p59231023"><a name="p59231023"></a><a name="p59231023"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row32983569"><td class="cellrowborder" rowspan="4" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p54423456"><a name="p54423456"></a><a name="p54423456"></a>Flavor Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p46223811"><a name="p46223811"></a><a name="p46223811"></a>find_flavor(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><a name="ul153094494547"></a><a name="ul153094494547"></a><ul id="ul153094494547"><li>name:<p id="p285918424559"><a name="p285918424559"></a><a name="p285918424559"></a>GET /v2/{project_id}/flavors</p>
<p id="p40191155317"><a name="p40191155317"></a><a name="p40191155317"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0701.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>id:<p id="p68531638115515"><a name="p68531638115515"></a><a name="p68531638115515"></a>GET /v2/{project_id}/flavors/{flavor_id}</p>
<p id="p474119105315"><a name="p474119105315"></a><a name="p474119105315"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0703.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row8508925"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18134306"><a name="p18134306"></a><a name="p18134306"></a>get_flavor(self, flavor)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p59592696"><a name="p59592696"></a><a name="p59592696"></a>GET /v2/{project_id}/flavors/{flavor_id}</p>
<p id="p7622121712532"><a name="p7622121712532"></a><a name="p7622121712532"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0703.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15588116295"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4469112284018"><a name="p4469112284018"></a><a name="p4469112284018"></a>query_flavor_extra_specs(self, flavor_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32521839124012"><a name="p32521839124012"></a><a name="p32521839124012"></a><span>GET /v2/{project_id}/flavors/{flavors_id}/os-extra_specs</span></p>
<p id="p625263984019"><a name="p625263984019"></a><a name="p625263984019"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0704.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row66572221"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p67119913525"><a name="p67119913525"></a><a name="p67119913525"></a><span>flavors(self, details=True, paginated=True, **query)</span></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p35856517"><a name="p35856517"></a><a name="p35856517"></a>GET /v2/{project_id}/flavors/detail</p>
<p id="p1920510242531"><a name="p1920510242531"></a><a name="p1920510242531"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0702.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row54273197"><td class="cellrowborder" rowspan="5" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p34052821"><a name="p34052821"></a><a name="p34052821"></a>Image Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p6815093"><a name="p6815093"></a><a name="p6815093"></a>delete_image(self, image, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p15151670"><a name="p15151670"></a><a name="p15151670"></a>DELETE /v2/{project_id}/images/{image_id}</p>
<p id="p20402113655311"><a name="p20402113655311"></a><a name="p20402113655311"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0505.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2147306"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p39714111"><a name="p39714111"></a><a name="p39714111"></a>find_image(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p81582052205312"><a name="p81582052205312"></a><a name="p81582052205312"></a>name:</p>
<p id="p1515819525533"><a name="p1515819525533"></a><a name="p1515819525533"></a>GET /v2/{project_id}/images</p>
<p id="p415816521533"><a name="p415816521533"></a><a name="p415816521533"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0501.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p19158752115317"><a name="p19158752115317"></a><a name="p19158752115317"></a>Image_id:</p>
<p id="p1515825218534"><a name="p1515825218534"></a><a name="p1515825218534"></a>GET /v2/{project_id}/images/{image_id}</p>
<p id="p141587528537"><a name="p141587528537"></a><a name="p141587528537"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0503.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row27666764"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26415391"><a name="p26415391"></a><a name="p26415391"></a>get_image(self, image)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p59271898"><a name="p59271898"></a><a name="p59271898"></a>GET /v2/{project_id}/images/{image_id}</p>
<p id="p6943515195410"><a name="p6943515195410"></a><a name="p6943515195410"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0503.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row63685038"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58214490"><a name="p58214490"></a><a name="p58214490"></a>images(self, details=True, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17753217"><a name="p17753217"></a><a name="p17753217"></a>GET /v2/{project_id}/images/detail</p>
<p id="p20312325195414"><a name="p20312325195414"></a><a name="p20312325195414"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0502.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row25561231"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p57193853"><a name="p57193853"></a><a name="p57193853"></a>get_image_metadata(self, image)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2190491"><a name="p2190491"></a><a name="p2190491"></a>GET /v2/{project_id}/images/{image_id}/metadata</p>
<p id="p168553114543"><a name="p168553114543"></a><a name="p168553114543"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0504.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19714419"><td class="cellrowborder" rowspan="5" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p53364125"><a name="p53364125"></a><a name="p53364125"></a>Keypair Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p27526859"><a name="p27526859"></a><a name="p27526859"></a>create_keypair(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p15083110"><a name="p15083110"></a><a name="p15083110"></a>POST /v2/{project_id}/os-keypairs</p>
<p id="p11505113805413"><a name="p11505113805413"></a><a name="p11505113805413"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212678.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1530263"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p56842496"><a name="p56842496"></a><a name="p56842496"></a>delete_keypair(self, keypair, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p40839433"><a name="p40839433"></a><a name="p40839433"></a>DELETE /v2/{project_id}/os-keypairs/{keypair_name}</p>
<p id="p102310443547"><a name="p102310443547"></a><a name="p102310443547"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1204.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row32010577"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42719917"><a name="p42719917"></a><a name="p42719917"></a>get_keypair(self, keypair)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p37761278"><a name="p37761278"></a><a name="p37761278"></a>GET /v2/{project_id}/os-keypairs/{keypair_name}</p>
<p id="p1192305416547"><a name="p1192305416547"></a><a name="p1192305416547"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1202.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4307190"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13338129"><a name="p13338129"></a><a name="p13338129"></a>find_keypair(self, name, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19641043155516"><a name="p19641043155516"></a><a name="p19641043155516"></a>Keypair_name:</p>
<p id="p14641943105510"><a name="p14641943105510"></a><a name="p14641943105510"></a>GET /v2/{project_id}/os-keypairs/{keypair_name}</p>
<p id="p116494310550"><a name="p116494310550"></a><a name="p116494310550"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1202.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p18641643105516"><a name="p18641643105516"></a><a name="p18641643105516"></a>Name:</p>
<p id="p5641643105511"><a name="p5641643105511"></a><a name="p5641643105511"></a>GET /v2/{project_id}/os-keypairs</p>
<p id="p8646432552"><a name="p8646432552"></a><a name="p8646432552"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row59820093"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13589360"><a name="p13589360"></a><a name="p13589360"></a>keypairs(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p26996384"><a name="p26996384"></a><a name="p26996384"></a>GET /v2/{project_id}/os-keypairs</p>
<p id="p6837185419556"><a name="p6837185419556"></a><a name="p6837185419556"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row41640866"><td class="cellrowborder" rowspan="16" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p17466967"><a name="p17466967"></a><a name="p17466967"></a>Server Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p5538237"><a name="p5538237"></a><a name="p5538237"></a>create_server(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p45944059"><a name="p45944059"></a><a name="p45944059"></a>POST /v2/{project_id}/servers</p>
<p id="p9646635566"><a name="p9646635566"></a><a name="p9646635566"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10843355"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5896594"><a name="p5896594"></a><a name="p5896594"></a>delete_server(self, server, ignore_missing=True, force=False)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7862068"><a name="p7862068"></a><a name="p7862068"></a>DELETE /v2/{project_id}/servers/{server_id}</p>
<p id="p4242121019566"><a name="p4242121019566"></a><a name="p4242121019566"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0203.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3649754"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p27194634"><a name="p27194634"></a><a name="p27194634"></a>find_server(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p86081325205617"><a name="p86081325205617"></a><a name="p86081325205617"></a>Name:</p>
<p id="p6608202519564"><a name="p6608202519564"></a><a name="p6608202519564"></a>GET /v2/{project_id}/servers</p>
<p id="p16608225145616"><a name="p16608225145616"></a><a name="p16608225145616"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0204.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p6608182512567"><a name="p6608182512567"></a><a name="p6608182512567"></a>Server_id:</p>
<p id="p1960882585615"><a name="p1960882585615"></a><a name="p1960882585615"></a>GET /v2/{project_id}/servers/{server_id}</p>
<p id="p960822575617"><a name="p960822575617"></a><a name="p960822575617"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0206.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row27773751"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p35081372"><a name="p35081372"></a><a name="p35081372"></a>get_server(self, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23018869"><a name="p23018869"></a><a name="p23018869"></a>GET /v2/{project_id}/servers/{server_id}</p>
<p id="p5567133813568"><a name="p5567133813568"></a><a name="p5567133813568"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0206.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5843233"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42601745165212"><a name="p42601745165212"></a><a name="p42601745165212"></a>servers_list(self, details=True, paginated=True, headers=None, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul656255311210"></a><a name="ul656255311210"></a><ul id="ul656255311210"><li>details=True:<p id="p622911311221"><a name="p622911311221"></a><a name="p622911311221"></a>GET /v2/{project_id}/servers/detail</p>
<p id="p041575345611"><a name="p041575345611"></a><a name="p041575345611"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0205.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>details=False:<p id="p1967308223"><a name="p1967308223"></a><a name="p1967308223"></a>GET /v2/{project_id}/servers</p>
<p id="p122194211579"><a name="p122194211579"></a><a name="p122194211579"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0204.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row65099051"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p38531802"><a name="p38531802"></a><a name="p38531802"></a>create_server_image(self, server, name, metadata=None)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34068253"><a name="p34068253"></a><a name="p34068253"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p2186463579"><a name="p2186463579"></a><a name="p2186463579"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0307.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row38178826"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5477191"><a name="p5477191"></a><a name="p5477191"></a>add_floating_ip_to_server(self, server, address, fixed_address=None)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p40999308"><a name="p40999308"></a><a name="p40999308"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p11405175211576"><a name="p11405175211576"></a><a name="p11405175211576"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1301.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row33449458"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p25051543"><a name="p25051543"></a><a name="p25051543"></a>remove_floating_ip_from_server(self, server, address)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15909080"><a name="p15909080"></a><a name="p15909080"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p16430155895711"><a name="p16430155895711"></a><a name="p16430155895711"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1302.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8963999"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54995351"><a name="p54995351"></a><a name="p54995351"></a>lock_server(self, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p25438431"><a name="p25438431"></a><a name="p25438431"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p77247518589"><a name="p77247518589"></a><a name="p77247518589"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0304.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row22569884"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16221316"><a name="p16221316"></a><a name="p16221316"></a>unlock_server(self, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38858233"><a name="p38858233"></a><a name="p38858233"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p20856201125820"><a name="p20856201125820"></a><a name="p20856201125820"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0305.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7711478"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20649961"><a name="p20649961"></a><a name="p20649961"></a>start_server(self, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p62034116"><a name="p62034116"></a><a name="p62034116"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p8351717205818"><a name="p8351717205818"></a><a name="p8351717205818"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0301.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21436136"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58605492"><a name="p58605492"></a><a name="p58605492"></a>stop_server(self, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p49424379"><a name="p49424379"></a><a name="p49424379"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p183823234581"><a name="p183823234581"></a><a name="p183823234581"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0303.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10923387"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12379115"><a name="p12379115"></a><a name="p12379115"></a>wait_for_server(self, server, status='ACTIVE', failures=['ERROR'], interval=2, wait=120)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p63184231"><a name="p63184231"></a><a name="p63184231"></a>GET /v2/{project_id}/servers/{server_id}</p>
<p id="p10185203045814"><a name="p10185203045814"></a><a name="p10185203045814"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0206.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1284921881813"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1184139111916"><a name="p1184139111916"></a><a name="p1184139111916"></a>instance_actions(self, server_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1969420375180"><a name="p1969420375180"></a><a name="p1969420375180"></a>GET /v2/{project_id}/servers/{server_id}/os-instance-actions</p>
<p id="p3419153919586"><a name="p3419153919586"></a><a name="p3419153919586"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1501.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row38663061811"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1525991591911"><a name="p1525991591911"></a><a name="p1525991591911"></a>get_instance_action(self, server_id, request_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1469411378183"><a name="p1469411378183"></a><a name="p1469411378183"></a>GET /v2/{project_id}/servers/{server_id}/os-instance-actions/{request_id}</p>
<p id="p47221948145820"><a name="p47221948145820"></a><a name="p47221948145820"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1502.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1143242214184"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1417317210198"><a name="p1417317210198"></a><a name="p1417317210198"></a>get_server_console_output(self, server_id, lines)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p169417374182"><a name="p169417374182"></a><a name="p169417374182"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p18592057205814"><a name="p18592057205814"></a><a name="p18592057205814"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1601.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31787174"><td class="cellrowborder" rowspan="4" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p24624288"><a name="p24624288"></a><a name="p24624288"></a>Server Interface Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p48410331"><a name="p48410331"></a><a name="p48410331"></a>create_server_interface(self, server, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p28922751"><a name="p28922751"></a><a name="p28922751"></a>POST /v2/{project_id}/servers/{server_id}/os-interface</p>
<p id="p11842182717115"><a name="p11842182717115"></a><a name="p11842182717115"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0803.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row58978167"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12502218"><a name="p12502218"></a><a name="p12502218"></a>delete_server_interface(self, server_interface, server=None, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6046746"><a name="p6046746"></a><a name="p6046746"></a>DELETE /v2/{project_id}/servers/{server_id}/os-interface/{port_id}</p>
<p id="p1062316351215"><a name="p1062316351215"></a><a name="p1062316351215"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0804.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row54420716"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p46001857"><a name="p46001857"></a><a name="p46001857"></a>get_server_interface(self, server_interface, server=None)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p35162951"><a name="p35162951"></a><a name="p35162951"></a>GET /v2/{project_id}/servers/{server_id}/os-interface/{port_id}</p>
<p id="p1157017444116"><a name="p1157017444116"></a><a name="p1157017444116"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0802.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48031108"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p65314517"><a name="p65314517"></a><a name="p65314517"></a>server_interfaces(self, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55984556"><a name="p55984556"></a><a name="p55984556"></a>GET /v2/{project_id}/servers/{server_id}/os-interface</p>
<p id="p1523210539115"><a name="p1523210539115"></a><a name="p1523210539115"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row34098956"><td class="cellrowborder" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p10552036"><a name="p10552036"></a><a name="p10552036"></a>Server IPs Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p49408564"><a name="p49408564"></a><a name="p49408564"></a>server_ips(self, server, network_label=None)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p42670757"><a name="p42670757"></a><a name="p42670757"></a>GET /v2/{project_id}/servers/{server_id}/ips</p>
<p id="p1621583025"><a name="p1621583025"></a><a name="p1621583025"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0402.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48492497"><td class="cellrowborder" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p35578198"><a name="p35578198"></a><a name="p35578198"></a>Availability Zone Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p63261775"><a name="p63261775"></a><a name="p63261775"></a>availability_zones(self, details=False)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p23930149"><a name="p23930149"></a><a name="p23930149"></a>GET /v2/{project_id}/os-availability-zone</p>
<p id="p36824812213"><a name="p36824812213"></a><a name="p36824812213"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14044750"><td class="cellrowborder" rowspan="4" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p63882937"><a name="p63882937"></a><a name="p63882937"></a>Server Group Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p7135413"><a name="p7135413"></a><a name="p7135413"></a>create_server_group(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p41097577"><a name="p41097577"></a><a name="p41097577"></a>POST /v2/{project_id}/os-server-groups</p>
<p id="p186996171212"><a name="p186996171212"></a><a name="p186996171212"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1401.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row34333880"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p29580916"><a name="p29580916"></a><a name="p29580916"></a>delete_server_group(self, server_group, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p47244029"><a name="p47244029"></a><a name="p47244029"></a>DELETE /v2/{project_id}/os-server-groups/{server_group_id}</p>
<p id="p115631241624"><a name="p115631241624"></a><a name="p115631241624"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1404.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row22543082"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14050320"><a name="p14050320"></a><a name="p14050320"></a>find_server_group(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1034903616213"><a name="p1034903616213"></a><a name="p1034903616213"></a>Name:</p>
<p id="p2349153619215"><a name="p2349153619215"></a><a name="p2349153619215"></a>GET /v2/{project_id}/os-server-groups</p>
<p id="p11349736321"><a name="p11349736321"></a><a name="p11349736321"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1402.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p183492361324"><a name="p183492361324"></a><a name="p183492361324"></a>Server_group_id:</p>
<p id="p1734913619212"><a name="p1734913619212"></a><a name="p1734913619212"></a>GET /v2/{project_id}/os-server-groups/{server_group_id}</p>
<p id="p13492365211"><a name="p13492365211"></a><a name="p13492365211"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1403.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42136306"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p57597629"><a name="p57597629"></a><a name="p57597629"></a>get_server_group(self, server_group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34896348"><a name="p34896348"></a><a name="p34896348"></a>GET /v2/{project_id}/os-server-groups/{server_group_id}</p>
<p id="p15364437151418"><a name="p15364437151418"></a><a name="p15364437151418"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1403.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row57001428122210"><td class="cellrowborder" rowspan="3" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p87011828132220"><a name="p87011828132220"></a><a name="p87011828132220"></a>Quota Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p1674319522316"><a name="p1674319522316"></a><a name="p1674319522316"></a>get_limits(self)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p13459184614227"><a name="p13459184614227"></a><a name="p13459184614227"></a>GET /v2/{project_id}/limits</p>
<p id="p2048845101413"><a name="p2048845101413"></a><a name="p2048845101413"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1101.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4293123316220"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2039114114239"><a name="p2039114114239"></a><a name="p2039114114239"></a>query_quota(self, project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34591146142214"><a name="p34591146142214"></a><a name="p34591146142214"></a>GET /v2/{project_id}/os-quota-sets/{project_id}</p>
<p id="p721105118145"><a name="p721105118145"></a><a name="p721105118145"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1102.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row233173832218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6430111610234"><a name="p6430111610234"></a><a name="p6430111610234"></a>query_quota_default(self, project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44603466221"><a name="p44603466221"></a><a name="p44603466221"></a>GET /v2/{project_id}/os-quota-sets/{project_id}/defaults</p>
<p id="p618012597149"><a name="p618012597149"></a><a name="p618012597149"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row929214504239"><td class="cellrowborder" rowspan="4" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p92932050152316"><a name="p92932050152316"></a><a name="p92932050152316"></a>Volume Attachment Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p9417816152413"><a name="p9417816152413"></a><a name="p9417816152413"></a>delete_volume_attachment(self, volume_attachment, server, force_del=False, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><p id="p104531011192415"><a name="p104531011192415"></a><a name="p104531011192415"></a>DELETE /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}</p>
<p id="p233414871517"><a name="p233414871517"></a><a name="p233414871517"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0904.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row818845362313"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1426812262246"><a name="p1426812262246"></a><a name="p1426812262246"></a>volume_attachments(self, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p184534115245"><a name="p184534115245"></a><a name="p184534115245"></a>GET /v2/{project_id}/servers/{server_id}/os-volume_attachments</p>
<p id="p19505815101515"><a name="p19505815101515"></a><a name="p19505815101515"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0901.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1660115513233"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14276113432417"><a name="p14276113432417"></a><a name="p14276113432417"></a>get_volume_attachment(self, volume_attachment, server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p114535112242"><a name="p114535112242"></a><a name="p114535112242"></a>GET /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}</p>
<p id="p1873392112157"><a name="p1873392112157"></a><a name="p1873392112157"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0902.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1880159175812"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3616124295814"><a name="p3616124295814"></a><a name="p3616124295814"></a>create_volume_attachment(self, server, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p980572619584"><a name="p980572619584"></a><a name="p980572619584"></a>POST /v2/{project_id}/servers/{server_id}/os-volume_attachments</p>
<p id="p15130143015153"><a name="p15130143015153"></a><a name="p15130143015153"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_0903.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row166381413162513"><td class="cellrowborder" rowspan="4" valign="top" width="26.247375262473753%" headers="mcps1.1.4.1.1 "><p id="p15940102122512"><a name="p15940102122512"></a><a name="p15940102122512"></a>Metadata Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.12588741125888%" headers="mcps1.1.4.1.2 "><p id="p152310414251"><a name="p152310414251"></a><a name="p152310414251"></a>get_server_metadata(self, server, key=None)</p>
</td>
<td class="cellrowborder" valign="top" width="32.62673732626737%" headers="mcps1.1.4.1.3 "><a name="ul36601488260"></a><a name="ul36601488260"></a><ul id="ul36601488260"><li>Key=None:<p id="p17191133512517"><a name="p17191133512517"></a><a name="p17191133512517"></a>GET /v2/{project_id}/servers/{server_id}/metadata</p>
<p id="p172064510155"><a name="p172064510155"></a><a name="p172064510155"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
<a name="ul751401010262"></a><a name="ul751401010262"></a><ul id="ul751401010262"><li>Key !=None:<p id="p019103572516"><a name="p019103572516"></a><a name="p019103572516"></a>GET /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p141213534156"><a name="p141213534156"></a><a name="p141213534156"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row980091672518"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p799994712251"><a name="p799994712251"></a><a name="p799994712251"></a>update_server_metadata(self, server, key, value)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1019113515259"><a name="p1019113515259"></a><a name="p1019113515259"></a>PUT /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p12769140151613"><a name="p12769140151613"></a><a name="p12769140151613"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row434163192719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3005847"><a name="p3005847"></a><a name="p3005847"></a>set_server_metadata(self, server, **metadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p42147045"><a name="p42147045"></a><a name="p42147045"></a>POST /v2/{project_id}/servers/{server_id}/metadata</p>
<p id="p53317820163"><a name="p53317820163"></a><a name="p53317820163"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row213623522710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p56445345"><a name="p56445345"></a><a name="p56445345"></a>delete_server_metadata(self, server, keys)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8670250"><a name="p8670250"></a><a name="p8670250"></a>DELETE /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p6162104411619"><a name="p6162104411619"></a><a name="p6162104411619"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Nova v2.1 API的SDK接口如下，调用方式举例：conn.ecs.create\_server\_ext\(\)

<a name="table1726118165212"></a>
<table><thead align="left"><tr id="row182612817525"><th class="cellrowborder" valign="top" width="26.25%" id="mcps1.1.4.1.1"><p id="p3273813529"><a name="p3273813529"></a><a name="p3273813529"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="41.23%" id="mcps1.1.4.1.2"><p id="p1274815220"><a name="p1274815220"></a><a name="p1274815220"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.519999999999996%" id="mcps1.1.4.1.3"><p id="p627138105214"><a name="p627138105214"></a><a name="p627138105214"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row12276814529"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p52716819528"><a name="p52716819528"></a><a name="p52716819528"></a>Server Interface Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.23%" headers="mcps1.1.4.1.2 "><p id="p163872446525"><a name="p163872446525"></a><a name="p163872446525"></a>get_vnc_address(headers=headers, server_id=server_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="32.519999999999996%" headers="mcps1.1.4.1.3 "><p id="p7387174415529"><a name="p7387174415529"></a><a name="p7387174415529"></a>POST /v2.1/{project_id}/servers/{server_id}/remote-consoles</p>
<p id="p738714455212"><a name="p738714455212"></a><a name="p738714455212"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_03_1603.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于ECS v1.1 API的SDK接口如下，调用方式举例：conn.ecs.create\_server\_ext\(\)

<a name="table752639153653"></a>
<table><thead align="left"><tr id="row38019639153653"><th class="cellrowborder" valign="top" width="26.25%" id="mcps1.1.4.1.1"><p id="p30369509153737"><a name="p30369509153737"></a><a name="p30369509153737"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="41.23%" id="mcps1.1.4.1.2"><p id="p35471369153737"><a name="p35471369153737"></a><a name="p35471369153737"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.519999999999996%" id="mcps1.1.4.1.3"><p id="p40595810153737"><a name="p40595810153737"></a><a name="p40595810153737"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row19466437153653"><td class="cellrowborder" rowspan="2" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p11440221154023"><a name="p11440221154023"></a><a name="p11440221154023"></a>Server Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.23%" headers="mcps1.1.4.1.2 "><p id="p1832810315382"><a name="p1832810315382"></a><a name="p1832810315382"></a>create_server_ext(self, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="32.519999999999996%" headers="mcps1.1.4.1.3 "><p id="p1631940615382"><a name="p1631940615382"></a><a name="p1631940615382"></a>POST /v1.1/{project_id}/cloudservers</p>
<p id="p15631755191614"><a name="p15631755191614"></a><a name="p15631755191614"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0101.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row38678231153653"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4701324615382"><a name="p4701324615382"></a><a name="p4701324615382"></a>resize_server_ext(self, server_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5177943515382"><a name="p5177943515382"></a><a name="p5177943515382"></a>POST /v1.1/{project_id}/cloudservers/{server_id}/resize</p>
<p id="p191111519176"><a name="p191111519176"></a><a name="p191111519176"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0209.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于ECS v1 API的SDK接口如下，调用方式举例：conn.ecs.get\_server\(\)

<a name="table5621115617409"></a>
<table><thead align="left"><tr id="row176298564403"><th class="cellrowborder" valign="top" width="26.46%" id="mcps1.1.4.1.1"><p id="p863275654010"><a name="p863275654010"></a><a name="p863275654010"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="41.32%" id="mcps1.1.4.1.2"><p id="p56343562401"><a name="p56343562401"></a><a name="p56343562401"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.22%" id="mcps1.1.4.1.3"><p id="p166401565406"><a name="p166401565406"></a><a name="p166401565406"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row3644195618402"><td class="cellrowborder" rowspan="6" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p864665674018"><a name="p864665674018"></a><a name="p864665674018"></a>Server Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.32%" headers="mcps1.1.4.1.2 "><p id="p15323192914213"><a name="p15323192914213"></a><a name="p15323192914213"></a>get_server(self, server_id)</p>
</td>
<td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.1.4.1.3 "><p id="p17712749134211"><a name="p17712749134211"></a><a name="p17712749134211"></a>GET /v1/{project_id}/cloudservers/{server_id}</p>
<p id="p16839101119175"><a name="p16839101119175"></a><a name="p16839101119175"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0104.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19654856144017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6430201118543"><a name="p6430201118543"></a><a name="p6430201118543"></a><span>servers(self, paginated=True, **query)</span></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1571204913428"><a name="p1571204913428"></a><a name="p1571204913428"></a>GET /v1/{project_id}/cloudservers/detail{?flavor,name,status,limit,offset,not-tags,reservation_id,enterprise_project_id}</p>
<p id="p14663218131715"><a name="p14663218131715"></a><a name="p14663218131715"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0094148850.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row81401310115113"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p64982622615"><a name="p64982622615"></a><a name="p64982622615"></a>def batch_change_os_server(self, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p849162615264"><a name="p849162615264"></a><a name="p849162615264"></a>POST/v1/{project_id}/cloudservers/{server_id}/changeos</p>
<p id="p194911269264"><a name="p194911269264"></a><a name="p194911269264"></a>（目前未有接口链接，后续添加）</p>
</td>
</tr>
<tr id="row20978925205117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1557316438286"><a name="p1557316438286"></a><a name="p1557316438286"></a>get_autorecovery(self, server_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1520011378284"><a name="p1520011378284"></a><a name="p1520011378284"></a>GET /v1/{project_id}/cloudservers/{server_id}/autorecovery</p>
<p id="p10731627171716"><a name="p10731627171716"></a><a name="p10731627171716"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0205.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15573182315516"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9364185112814"><a name="p9364185112814"></a><a name="p9364185112814"></a>config_autorecovery(self, server_id, autorecovery)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1200143792811"><a name="p1200143792811"></a><a name="p1200143792811"></a>PUT /v1/{project_id}/cloudservers/{server_id}/autorecovery</p>
<p id="p1555312375176"><a name="p1555312375176"></a><a name="p1555312375176"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0206.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row186269594521"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5627155918523"><a name="p5627155918523"></a><a name="p5627155918523"></a>reset_password(self, server_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1262711594524"><a name="p1262711594524"></a><a name="p1262711594524"></a>PUT /v1/{project_id}/cloudservers/{server_id}/os-reset-password</p>
<p id="p19505173211546"><a name="p19505173211546"></a><a name="p19505173211546"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15019289417"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p313314716438"><a name="p313314716438"></a><a name="p313314716438"></a>Flavor Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.32%" headers="mcps1.1.4.1.2 "><p id="p203233290423"><a name="p203233290423"></a><a name="p203233290423"></a>flavors(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.1.4.1.3 "><p id="p12712194911423"><a name="p12712194911423"></a><a name="p12712194911423"></a>GET /v1/{project_id}/cloudservers/flavors{?availability_zone}</p>
<p id="p14172245121713"><a name="p14172245121713"></a><a name="p14172245121713"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212656.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1191713313413"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p181341578434"><a name="p181341578434"></a><a name="p181341578434"></a>Quota Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.32%" headers="mcps1.1.4.1.2 "><p id="p43231829174214"><a name="p43231829174214"></a><a name="p43231829174214"></a>quotas(self)</p>
</td>
<td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.1.4.1.3 "><p id="p77121949114210"><a name="p77121949114210"></a><a name="p77121949114210"></a>GET /v1/{project_id}/cloudservers/limits</p>
<p id="p088195141714"><a name="p088195141714"></a><a name="p088195141714"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5395015102912"><td class="cellrowborder" rowspan="4" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p139621502914"><a name="p139621502914"></a><a name="p139621502914"></a>Server Tag Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.32%" headers="mcps1.1.4.1.2 "><p id="p173962158298"><a name="p173962158298"></a><a name="p173962158298"></a>create_server_tags(self, server_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.1.4.1.3 "><p id="p33964157290"><a name="p33964157290"></a><a name="p33964157290"></a><span>POST /v1/{project_id}/cloudservers/{server_id}/tags/action</span></p>
<p id="p14941758153720"><a name="p14941758153720"></a><a name="p14941758153720"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row173461524193520"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9347224163511"><a name="p9347224163511"></a><a name="p9347224163511"></a>delete_server_tags(self, server_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17347142417359"><a name="p17347142417359"></a><a name="p17347142417359"></a><span>POST /v1/{project_id}/cloudservers/{server_id}/tags/action</span></p>
<p id="p1836611123717"><a name="p1836611123717"></a><a name="p1836611123717"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row438215417367"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p538214463612"><a name="p538214463612"></a><a name="p538214463612"></a>get_server_tags(self, server_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23821419368"><a name="p23821419368"></a><a name="p23821419368"></a><span>GET /v1/{project_id}/cloudservers/{server_id}/tags</span></p>
<p id="p66045466389"><a name="p66045466389"></a><a name="p66045466389"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1841372023610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p24141820173619"><a name="p24141820173619"></a><a name="p24141820173619"></a>get_project_tags(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p84141920163617"><a name="p84141920163617"></a><a name="p84141920163617"></a><span>GET /v1/{project_id}/cloudservers/tags</span></p>
<p id="p676402823914"><a name="p676402823914"></a><a name="p676402823914"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_1007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row91012427463"><td class="cellrowborder" valign="top" width="26.46%" headers="mcps1.1.4.1.1 "><p id="p61021242184618"><a name="p61021242184618"></a><a name="p61021242184618"></a>Server Interface Operations</p>
</td>
<td class="cellrowborder" valign="top" width="41.32%" headers="mcps1.1.4.1.2 "><p id="p154461658478"><a name="p154461658478"></a><a name="p154461658478"></a>get_vnc_address(server_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="32.22%" headers="mcps1.1.4.1.3 "><p id="p244620594712"><a name="p244620594712"></a><a name="p244620594712"></a>POST /v1/{project_id}/cloudservers/{server_id}/remote_console</p>
<p id="p194461544716"><a name="p194461544716"></a><a name="p194461544716"></a><a href="https://support.huaweicloud.com/api-ecs/ecs_02_0208.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

