# VPC<a name="sdk_13_0003"></a>

基于VPC v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table52914471212"></a>
<table><thead align="left"><tr id="row1122515441212"><th class="cellrowborder" valign="top" width="26.25%" id="mcps1.1.4.1.1"><p id="p522564171210"><a name="p522564171210"></a><a name="p522564171210"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.58%" id="mcps1.1.4.1.2"><p id="p10225164161215"><a name="p10225164161215"></a><a name="p10225164161215"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.17%" id="mcps1.1.4.1.3"><p id="p1622516413121"><a name="p1622516413121"></a><a name="p1622516413121"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row122511412123"><td class="cellrowborder" rowspan="3" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p22251643120"><a name="p22251643120"></a><a name="p22251643120"></a>Bandwidths</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p18159152291014"><a name="p18159152291014"></a><a name="p18159152291014"></a>Get(client *gophercloud.ServiceClient, bandwidthId string)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p14958174311113"><a name="p14958174311113"></a><a name="p14958174311113"></a>GET /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p5958643181112"><a name="p5958643181112"></a><a name="p5958643181112"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row152259419129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p815914226106"><a name="p815914226106"></a><a name="p815914226106"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p295814435119"><a name="p295814435119"></a><a name="p295814435119"></a>GET /v1/{project_id}/bandwidths</p>
<p id="p395884310119"><a name="p395884310119"></a><a name="p395884310119"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1822504101214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12159152221011"><a name="p12159152221011"></a><a name="p12159152221011"></a>Update(client *gophercloud.ServiceClient, bandwidthId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19958204318112"><a name="p19958204318112"></a><a name="p19958204318112"></a>PUT /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p17958543101114"><a name="p17958543101114"></a><a name="p17958543101114"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10225124131215"><td class="cellrowborder" rowspan="5" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p132257415120"><a name="p132257415120"></a><a name="p132257415120"></a>Ports</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p1816014228107"><a name="p1816014228107"></a><a name="p1816014228107"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p1514917191214"><a name="p1514917191214"></a><a name="p1514917191214"></a>POST /v1/{project_id}/ports</p>
<p id="p2149107151213"><a name="p2149107151213"></a><a name="p2149107151213"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row722619412129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17160122191019"><a name="p17160122191019"></a><a name="p17160122191019"></a>Delete(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1714918718121"><a name="p1714918718121"></a><a name="p1714918718121"></a>DELETE /v1/{project_id}/ports/{port_id}</p>
<p id="p151499711128"><a name="p151499711128"></a><a name="p151499711128"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row822684151214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p916015224106"><a name="p916015224106"></a><a name="p916015224106"></a>Get(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p114915741212"><a name="p114915741212"></a><a name="p114915741212"></a>GET /v1/{project_id}/ports/{port_id}</p>
<p id="p214907191211"><a name="p214907191211"></a><a name="p214907191211"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1222674181213"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p151601322121012"><a name="p151601322121012"></a><a name="p151601322121012"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p414915721217"><a name="p414915721217"></a><a name="p414915721217"></a>GET /v1/{project_id}/ports</p>
<p id="p9149271124"><a name="p9149271124"></a><a name="p9149271124"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7228146124"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p91601223105"><a name="p91601223105"></a><a name="p91601223105"></a>Update(client *gophercloud.ServiceClient, portId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1014910714120"><a name="p1014910714120"></a><a name="p1014910714120"></a>PUT /v1/{project_id}/ports/{port_id}</p>
<p id="p1514987181215"><a name="p1514987181215"></a><a name="p1514987181215"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8228114121213"><td class="cellrowborder" rowspan="4" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p178432495419"><a name="p178432495419"></a><a name="p178432495419"></a>PrivateIps</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p1616062217104"><a name="p1616062217104"></a><a name="p1616062217104"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p1413511283128"><a name="p1413511283128"></a><a name="p1413511283128"></a>POST /v1/{project_id}/privateips</p>
<p id="p6135142812125"><a name="p6135142812125"></a><a name="p6135142812125"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2228144191218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p131607228107"><a name="p131607228107"></a><a name="p131607228107"></a>Delete(client *gophercloud.ServiceClient, privateipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18135182851218"><a name="p18135182851218"></a><a name="p18135182851218"></a>DELETE /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p12135182831212"><a name="p12135182831212"></a><a name="p12135182831212"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42284415122"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15160182219104"><a name="p15160182219104"></a><a name="p15160182219104"></a>Get(client *gophercloud.ServiceClient, privateipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7135102851211"><a name="p7135102851211"></a><a name="p7135102851211"></a>GET /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p6135142817124"><a name="p6135142817124"></a><a name="p6135142817124"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10229174131219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p141609225100"><a name="p141609225100"></a><a name="p141609225100"></a>List(client *gophercloud.ServiceClient, subnetId string, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p101353285126"><a name="p101353285126"></a><a name="p101353285126"></a>GET /v1/{project_id}/subnets/{subnet_id}/privateips</p>
<p id="p1413518284124"><a name="p1413518284124"></a><a name="p1413518284124"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row182299471214"><td class="cellrowborder" rowspan="5" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p14981935115410"><a name="p14981935115410"></a><a name="p14981935115410"></a>PublicIps</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p12160162251020"><a name="p12160162251020"></a><a name="p12160162251020"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p839216732"><a name="p839216732"></a><a name="p839216732"></a>POST /v1/{project_id}/publicips</p>
<p id="p18391916233"><a name="p18391916233"></a><a name="p18391916233"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10229448122"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6160122121016"><a name="p6160122121016"></a><a name="p6160122121016"></a>Delete(client *gophercloud.ServiceClient, publicipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6629768137"><a name="p6629768137"></a><a name="p6629768137"></a>DELETE /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p36291162132"><a name="p36291162132"></a><a name="p36291162132"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row152299411129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p81601222109"><a name="p81601222109"></a><a name="p81601222109"></a>Get(client *gophercloud.ServiceClient, publicipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p146291664136"><a name="p146291664136"></a><a name="p146291664136"></a>GET /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p762913681313"><a name="p762913681313"></a><a name="p762913681313"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9229114201216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1516062271012"><a name="p1516062271012"></a><a name="p1516062271012"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p206291065130"><a name="p206291065130"></a><a name="p206291065130"></a>GET /v1/{project_id}/publicips</p>
<p id="p15629862137"><a name="p15629862137"></a><a name="p15629862137"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row202295417123"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p101609228109"><a name="p101609228109"></a><a name="p101609228109"></a>Update(client *gophercloud.ServiceClient, publicipId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p462912621311"><a name="p462912621311"></a><a name="p462912621311"></a>PUT /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p3629196151317"><a name="p3629196151317"></a><a name="p3629196151317"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row112291249122"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p42299416129"><a name="p42299416129"></a><a name="p42299416129"></a>Quotas</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p181601122141019"><a name="p181601122141019"></a><a name="p181601122141019"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p1362913661318"><a name="p1362913661318"></a><a name="p1362913661318"></a>GET /v1/{project_id}/quotas</p>
<p id="p136298618130"><a name="p136298618130"></a><a name="p136298618130"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_quota_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row322915481215"><td class="cellrowborder" rowspan="4" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p11487194145916"><a name="p11487194145916"></a><a name="p11487194145916"></a>SecurityGroupRules</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p1016092212106"><a name="p1016092212106"></a><a name="p1016092212106"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p9423287135"><a name="p9423287135"></a><a name="p9423287135"></a>POST /v1/security-group-rules</p>
<p id="p1342102811315"><a name="p1342102811315"></a><a name="p1342102811315"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row922912415126"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1716015228102"><a name="p1716015228102"></a><a name="p1716015228102"></a>Delete(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2042112821315"><a name="p2042112821315"></a><a name="p2042112821315"></a>DELETE /v1/security-group-rules/{security-groups-rules-id}</p>
<p id="p8426285138"><a name="p8426285138"></a><a name="p8426285138"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1422919401220"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4160172271017"><a name="p4160172271017"></a><a name="p4160172271017"></a>Get(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p20421128161312"><a name="p20421128161312"></a><a name="p20421128161312"></a>GET /v1/security-group-rules/{security-groups-rules-id}</p>
<p id="p442172851319"><a name="p442172851319"></a><a name="p442172851319"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row162299411128"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19161822101011"><a name="p19161822101011"></a><a name="p19161822101011"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p743192881312"><a name="p743192881312"></a><a name="p743192881312"></a>GET /v1/security-group-rules</p>
<p id="p343142811312"><a name="p343142811312"></a><a name="p343142811312"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62301341122"><td class="cellrowborder" rowspan="4" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p54116475415"><a name="p54116475415"></a><a name="p54116475415"></a>SecurityGroups</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p4161102217109"><a name="p4161102217109"></a><a name="p4161102217109"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p16076219147"><a name="p16076219147"></a><a name="p16076219147"></a>POST /v1/{project_id}/security-groups</p>
<p id="p5607182111419"><a name="p5607182111419"></a><a name="p5607182111419"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row192307481210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1916142261012"><a name="p1916142261012"></a><a name="p1916142261012"></a>Delete(client *gophercloud.ServiceClient, securityGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p106074214144"><a name="p106074214144"></a><a name="p106074214144"></a>DELETE /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p560782181411"><a name="p560782181411"></a><a name="p560782181411"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row202303419124"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1016172210104"><a name="p1016172210104"></a><a name="p1016172210104"></a>Get(client *gophercloud.ServiceClient, securityGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1860718211414"><a name="p1860718211414"></a><a name="p1860718211414"></a>GET /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p1860717218142"><a name="p1860717218142"></a><a name="p1860717218142"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1823013411120"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18161112231020"><a name="p18161112231020"></a><a name="p18161112231020"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6607827142"><a name="p6607827142"></a><a name="p6607827142"></a>GET /v1/{project_id}/security-groups</p>
<p id="p96076212143"><a name="p96076212143"></a><a name="p96076212143"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1123012461218"><td class="cellrowborder" rowspan="5" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p223012481211"><a name="p223012481211"></a><a name="p223012481211"></a>Subnets</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p11161322191013"><a name="p11161322191013"></a><a name="p11161322191013"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p1672173114141"><a name="p1672173114141"></a><a name="p1672173114141"></a>POST /v1/{project_id}/subnets</p>
<p id="p1972203151419"><a name="p1972203151419"></a><a name="p1972203151419"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8230444129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1016122261013"><a name="p1016122261013"></a><a name="p1016122261013"></a>Delete(client *gophercloud.ServiceClient, vpcId string, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p97293121415"><a name="p97293121415"></a><a name="p97293121415"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p1772631181418"><a name="p1772631181418"></a><a name="p1772631181418"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row192301241125"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p61616224101"><a name="p61616224101"></a><a name="p61616224101"></a>Get(client *gophercloud.ServiceClient, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p197283114147"><a name="p197283114147"></a><a name="p197283114147"></a>GET /v1/{project_id}/subnets/{subnet_id}</p>
<p id="p177273113143"><a name="p177273113143"></a><a name="p177273113143"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18230104191218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p860418346507"><a name="p860418346507"></a><a name="p860418346507"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1972831151414"><a name="p1972831151414"></a><a name="p1972831151414"></a>GET /v1/{project_id}/subnets</p>
<p id="p1372173113142"><a name="p1372173113142"></a><a name="p1372173113142"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1623054141215"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1716172218108"><a name="p1716172218108"></a><a name="p1716172218108"></a>Update(client *gophercloud.ServiceClient, vpcId string, subnetId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1372331161417"><a name="p1372331161417"></a><a name="p1372331161417"></a>PUT /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p197263111415"><a name="p197263111415"></a><a name="p197263111415"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row523015419128"><td class="cellrowborder" rowspan="5" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p1123110411126"><a name="p1123110411126"></a><a name="p1123110411126"></a>Vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p3161112213102"><a name="p3161112213102"></a><a name="p3161112213102"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p117495271416"><a name="p117495271416"></a><a name="p117495271416"></a>POST /v1/{project_id}/vpcs</p>
<p id="p17411524146"><a name="p17411524146"></a><a name="p17411524146"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12231134191211"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15161722141015"><a name="p15161722141015"></a><a name="p15161722141015"></a>Delete(client *gophercloud.ServiceClient, vpcId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1074125281420"><a name="p1074125281420"></a><a name="p1074125281420"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p187435214145"><a name="p187435214145"></a><a name="p187435214145"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row182310416129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2161622161016"><a name="p2161622161016"></a><a name="p2161622161016"></a>Get(client *gophercloud.ServiceClient, vpcId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p167475220143"><a name="p167475220143"></a><a name="p167475220143"></a>GET /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p1774152111416"><a name="p1774152111416"></a><a name="p1774152111416"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row523164131210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p116132281015"><a name="p116132281015"></a><a name="p116132281015"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p47413524143"><a name="p47413524143"></a><a name="p47413524143"></a>GET /v1/{project_id}/vpcs</p>
<p id="p19746521145"><a name="p19746521145"></a><a name="p19746521145"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12312471212"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1816211225101"><a name="p1816211225101"></a><a name="p1816211225101"></a>Update(client *gophercloud.ServiceClient, vpcId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1574165216149"><a name="p1574165216149"></a><a name="p1574165216149"></a>PUT /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p177455281410"><a name="p177455281410"></a><a name="p177455281410"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Neutron v2.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table992328719225"></a>
<table><thead align="left"><tr id="row17099872192215"><th class="cellrowborder" valign="top" width="26.572657265726573%" id="mcps1.1.4.1.1"><p id="p3836953192658"><a name="p3836953192658"></a><a name="p3836953192658"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.62376237623762%" id="mcps1.1.4.1.2"><p id="p34036061192658"><a name="p34036061192658"></a><a name="p34036061192658"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.80358035803581%" id="mcps1.1.4.1.3"><p id="p38415708192658"><a name="p38415708192658"></a><a name="p38415708192658"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1456033119225"><td class="cellrowborder" rowspan="5" valign="top" width="26.572657265726573%" headers="mcps1.1.4.1.1 "><p id="p3607449719225"><a name="p3607449719225"></a><a name="p3607449719225"></a>Networks</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p10202225165314"><a name="p10202225165314"></a><a name="p10202225165314"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.4.1.3 "><p id="p1438034961510"><a name="p1438034961510"></a><a name="p1438034961510"></a>POST /v2.0/networks</p>
<p id="p2038064951518"><a name="p2038064951518"></a><a name="p2038064951518"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1483347619225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p102023255537"><a name="p102023255537"></a><a name="p102023255537"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p0380949121510"><a name="p0380949121510"></a><a name="p0380949121510"></a>GET /v2.0/networks</p>
<p id="p10380949181510"><a name="p10380949181510"></a><a name="p10380949181510"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3847678719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32028255532"><a name="p32028255532"></a><a name="p32028255532"></a>Get(client *gophercloud.ServiceClient, networkId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1380449131516"><a name="p1380449131516"></a><a name="p1380449131516"></a>GET /v2.0/networks/{network_id}</p>
<p id="p1538014496154"><a name="p1538014496154"></a><a name="p1538014496154"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6391532719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10202112565312"><a name="p10202112565312"></a><a name="p10202112565312"></a>Update(client *gophercloud.ServiceClient, networkId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12380649171516"><a name="p12380649171516"></a><a name="p12380649171516"></a>PUT /v2.0/networks/{network_id)</p>
<p id="p6380114971519"><a name="p6380114971519"></a><a name="p6380114971519"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1727432519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p620218257531"><a name="p620218257531"></a><a name="p620218257531"></a>Delete(client *gophercloud.ServiceClient, networkId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17380049181520"><a name="p17380049181520"></a><a name="p17380049181520"></a>DELETE /v2.0/networks/{network_id}</p>
<p id="p038017498155"><a name="p038017498155"></a><a name="p038017498155"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2524536719225"><td class="cellrowborder" rowspan="5" valign="top" width="26.572657265726573%" headers="mcps1.1.4.1.1 "><p id="p4204824119225"><a name="p4204824119225"></a><a name="p4204824119225"></a>Subnets</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p716014477536"><a name="p716014477536"></a><a name="p716014477536"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.4.1.3 "><p id="p338034941510"><a name="p338034941510"></a><a name="p338034941510"></a>POST /v2.0/subnets</p>
<p id="p1638014910152"><a name="p1638014910152"></a><a name="p1638014910152"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1554961919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p81601247125313"><a name="p81601247125313"></a><a name="p81601247125313"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p93801849111510"><a name="p93801849111510"></a><a name="p93801849111510"></a>GET /v2.0/subnets</p>
<p id="p23808499157"><a name="p23808499157"></a><a name="p23808499157"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2264872619225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p151601647185316"><a name="p151601647185316"></a><a name="p151601647185316"></a>Get(client *gophercloud.ServiceClient, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9380114931511"><a name="p9380114931511"></a><a name="p9380114931511"></a>GET /v2.0/subnets/{subnet_id}</p>
<p id="p19380194921516"><a name="p19380194921516"></a><a name="p19380194921516"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5365471919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5160134745310"><a name="p5160134745310"></a><a name="p5160134745310"></a>Update(client *gophercloud.ServiceClient, subnetId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p133801449181511"><a name="p133801449181511"></a><a name="p133801449181511"></a>PUT /v2.0/subnets/{subnet_id}</p>
<p id="p138020490159"><a name="p138020490159"></a><a name="p138020490159"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4315595719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18160847135314"><a name="p18160847135314"></a><a name="p18160847135314"></a>Delete(client *gophercloud.ServiceClient, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1538011495158"><a name="p1538011495158"></a><a name="p1538011495158"></a>DELETE /v2.0/subnets/{subnet_id}</p>
<p id="p838054981510"><a name="p838054981510"></a><a name="p838054981510"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5941967519225"><td class="cellrowborder" rowspan="5" valign="top" width="26.572657265726573%" headers="mcps1.1.4.1.1 "><p id="p109045619225"><a name="p109045619225"></a><a name="p109045619225"></a>Ports</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p1116094785317"><a name="p1116094785317"></a><a name="p1116094785317"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.4.1.3 "><p id="p4316312191617"><a name="p4316312191617"></a><a name="p4316312191617"></a>POST /v2.0/ports</p>
<p id="p5316161211620"><a name="p5316161211620"></a><a name="p5316161211620"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2015247919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19160104713535"><a name="p19160104713535"></a><a name="p19160104713535"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p731612127163"><a name="p731612127163"></a><a name="p731612127163"></a>GET /v2.0/ports</p>
<p id="p9316131216166"><a name="p9316131216166"></a><a name="p9316131216166"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3018735219225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1616044715534"><a name="p1616044715534"></a><a name="p1616044715534"></a>Get(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p83161012161619"><a name="p83161012161619"></a><a name="p83161012161619"></a>GET /v2.0/ports/{port_id}</p>
<p id="p183161712121611"><a name="p183161712121611"></a><a name="p183161712121611"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row954305419225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17160184713535"><a name="p17160184713535"></a><a name="p17160184713535"></a>Update(client *gophercloud.ServiceClient, portId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1931631216161"><a name="p1931631216161"></a><a name="p1931631216161"></a>PUT /v2.0/ports/{port_id}</p>
<p id="p113166123162"><a name="p113166123162"></a><a name="p113166123162"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row461260119225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6160547195312"><a name="p6160547195312"></a><a name="p6160547195312"></a>Delete(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19316171218168"><a name="p19316171218168"></a><a name="p19316171218168"></a>DELETE /v2.0/ports/{port_id}</p>
<p id="p731661271613"><a name="p731661271613"></a><a name="p731661271613"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1031281219225"><td class="cellrowborder" rowspan="4" valign="top" width="26.572657265726573%" headers="mcps1.1.4.1.1 "><p id="p783249019225"><a name="p783249019225"></a><a name="p783249019225"></a>SecurityGroup</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p1054841516549"><a name="p1054841516549"></a><a name="p1054841516549"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.4.1.3 "><p id="p1327513334166"><a name="p1327513334166"></a><a name="p1327513334166"></a>POST /v2.0/security-groups</p>
<p id="p11275933101620"><a name="p11275933101620"></a><a name="p11275933101620"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row512484819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11548201513544"><a name="p11548201513544"></a><a name="p11548201513544"></a>Update(client *gophercloud.ServiceClient, securityGroupId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1427511336165"><a name="p1427511336165"></a><a name="p1427511336165"></a>PUT /v2.0/security-groups/{security_group_id}</p>
<p id="p72751833101617"><a name="p72751833101617"></a><a name="p72751833101617"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1705601819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15548191545419"><a name="p15548191545419"></a><a name="p15548191545419"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p152751433201612"><a name="p152751433201612"></a><a name="p152751433201612"></a>GET /v2.0/security-groups</p>
<p id="p52758339166"><a name="p52758339166"></a><a name="p52758339166"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4477878219225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p654814156547"><a name="p654814156547"></a><a name="p654814156547"></a>Get(client *gophercloud.ServiceClient, securityGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p42761339161"><a name="p42761339161"></a><a name="p42761339161"></a>GET /v2.0/security-groups/{security_group_id}</p>
<p id="p127693317161"><a name="p127693317161"></a><a name="p127693317161"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row147508319225"><td class="cellrowborder" rowspan="4" valign="top" width="26.572657265726573%" headers="mcps1.1.4.1.1 "><p id="p731533019225"><a name="p731533019225"></a><a name="p731533019225"></a>SecurityGroupRules</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p2090193218545"><a name="p2090193218545"></a><a name="p2090193218545"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.4.1.3 "><p id="p952917541165"><a name="p952917541165"></a><a name="p952917541165"></a>POST /v2.0/security-group-rules</p>
<p id="p652985410161"><a name="p652985410161"></a><a name="p652985410161"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2843541519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p790203217542"><a name="p790203217542"></a><a name="p790203217542"></a>Delete(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12529195411613"><a name="p12529195411613"></a><a name="p12529195411613"></a>DELETE /v2.0/security-group-rules/{security-groups-rules-id}</p>
<p id="p4529354151610"><a name="p4529354151610"></a><a name="p4529354151610"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row344244919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18901532155419"><a name="p18901532155419"></a><a name="p18901532155419"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p95291954131619"><a name="p95291954131619"></a><a name="p95291954131619"></a>GET /v2.0/security-group-rules</p>
<p id="p352914548166"><a name="p352914548166"></a><a name="p352914548166"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5448175519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12911832115411"><a name="p12911832115411"></a><a name="p12911832115411"></a>Get(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p165295541167"><a name="p165295541167"></a><a name="p165295541167"></a>GET /v2.0/security-group-rules/{security-groups-rules-id}</p>
<p id="p35291354111610"><a name="p35291354111610"></a><a name="p35291354111610"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18523019225"><td class="cellrowborder" rowspan="7" valign="top" width="26.572657265726573%" headers="mcps1.1.4.1.1 "><p id="p5855323719225"><a name="p5855323719225"></a><a name="p5855323719225"></a>Routers</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p91571147115411"><a name="p91571147115411"></a><a name="p91571147115411"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.4.1.3 "><p id="p27377193172"><a name="p27377193172"></a><a name="p27377193172"></a>POST /v2.0/routers</p>
<p id="p1173719194171"><a name="p1173719194171"></a><a name="p1173719194171"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4774639619225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2157947115417"><a name="p2157947115417"></a><a name="p2157947115417"></a>Delete(client *gophercloud.ServiceClient, routerId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p117371819131714"><a name="p117371819131714"></a><a name="p117371819131714"></a>DELETE /v2.0/routers/{router_id}</p>
<p id="p17737719121714"><a name="p17737719121714"></a><a name="p17737719121714"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row878108319225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p01571347175413"><a name="p01571347175413"></a><a name="p01571347175413"></a>Update(client *gophercloud.ServiceClient, routerId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p137381819161710"><a name="p137381819161710"></a><a name="p137381819161710"></a>PUT /v2.0/routers/{router_id}</p>
<p id="p4738619161717"><a name="p4738619161717"></a><a name="p4738619161717"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6383039819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9157134745415"><a name="p9157134745415"></a><a name="p9157134745415"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p187381419201714"><a name="p187381419201714"></a><a name="p187381419201714"></a>GET /v2.0/routers</p>
<p id="p373812193172"><a name="p373812193172"></a><a name="p373812193172"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5579110719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1115716474541"><a name="p1115716474541"></a><a name="p1115716474541"></a>Get(client *gophercloud.ServiceClient, routerId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16738319101715"><a name="p16738319101715"></a><a name="p16738319101715"></a>GET /v2.0/routers/{router_id}</p>
<p id="p1073801918170"><a name="p1073801918170"></a><a name="p1073801918170"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3652040119225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3157154713543"><a name="p3157154713543"></a><a name="p3157154713543"></a>AddInterface(client *gophercloud.ServiceClient, routerId string, opts AddInterfaceOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3738519101714"><a name="p3738519101714"></a><a name="p3738519101714"></a>PUT /v2.0/routers/{router_id}/add_router_interface</p>
<p id="p4738619181712"><a name="p4738619181712"></a><a name="p4738619181712"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4965676819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14157144755414"><a name="p14157144755414"></a><a name="p14157144755414"></a>RemoveInterface(client *gophercloud.ServiceClient, routerId string, opts RemoveInterfaceOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11738101914171"><a name="p11738101914171"></a><a name="p11738101914171"></a>PUT /v2.0/routers/{router_id}/remove_router_interface</p>
<p id="p87387193175"><a name="p87387193175"></a><a name="p87387193175"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5409263219225"><td class="cellrowborder" rowspan="5" valign="top" width="26.572657265726573%" headers="mcps1.1.4.1.1 "><p id="p42887394176"><a name="p42887394176"></a><a name="p42887394176"></a>FloatingIps</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p53894195513"><a name="p53894195513"></a><a name="p53894195513"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="35.80358035803581%" headers="mcps1.1.4.1.3 "><p id="p7177185017170"><a name="p7177185017170"></a><a name="p7177185017170"></a>POST /v2.0/floatingips</p>
<p id="p15177125011712"><a name="p15177125011712"></a><a name="p15177125011712"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5463078019225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p938912112558"><a name="p938912112558"></a><a name="p938912112558"></a>Delete(client *gophercloud.ServiceClient, floatingipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16178165051720"><a name="p16178165051720"></a><a name="p16178165051720"></a>DELETE /v2.0/floatingips/{floatingip_id}</p>
<p id="p617819502173"><a name="p617819502173"></a><a name="p617819502173"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1416256519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8389111125514"><a name="p8389111125514"></a><a name="p8389111125514"></a>Update(client *gophercloud.ServiceClient, floatingipId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1917811506175"><a name="p1917811506175"></a><a name="p1917811506175"></a>PUT /v2.0/floatingips/{floatingip_id}</p>
<p id="p41788503178"><a name="p41788503178"></a><a name="p41788503178"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5592232019225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17389111145513"><a name="p17389111145513"></a><a name="p17389111145513"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p517816505173"><a name="p517816505173"></a><a name="p517816505173"></a>GET /v2.0/floatingips</p>
<p id="p131784504170"><a name="p131784504170"></a><a name="p131784504170"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4422341819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20390151155518"><a name="p20390151155518"></a><a name="p20390151155518"></a>Get(client *gophercloud.ServiceClient, floatingipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p017825071715"><a name="p017825071715"></a><a name="p017825071715"></a>GET /v2.0/floatingips/{floatingip_id}</p>
<p id="p617814507177"><a name="p617814507177"></a><a name="p617814507177"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

