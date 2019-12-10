# Go-VPC<a name="ZH-CN_TOPIC_0090172882"></a>

基于VPC v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table52914471212"></a>
<table><thead align="left"><tr id="row1122515441212"><th class="cellrowborder" valign="top" width="18.39%" id="mcps1.1.4.1.1"><p id="p522564171210"><a name="p522564171210"></a><a name="p522564171210"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="44.41%" id="mcps1.1.4.1.2"><p id="p10225164161215"><a name="p10225164161215"></a><a name="p10225164161215"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="37.2%" id="mcps1.1.4.1.3"><p id="p1622516413121"><a name="p1622516413121"></a><a name="p1622516413121"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row122511412123"><td class="cellrowborder" rowspan="3" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p22251643120"><a name="p22251643120"></a><a name="p22251643120"></a>Bandwidths</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p18159152291014"><a name="p18159152291014"></a><a name="p18159152291014"></a>Get(client *gophercloud.ServiceClient, bandwidthId string)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p174421434019"><a name="p174421434019"></a><a name="p174421434019"></a>GET /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p15442932006"><a name="p15442932006"></a><a name="p15442932006"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090603.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row152259419129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p815914226106"><a name="p815914226106"></a><a name="p815914226106"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14421636015"><a name="p14421636015"></a><a name="p14421636015"></a>GET /v1/{project_id}/bandwidths</p>
<p id="p124421035015"><a name="p124421035015"></a><a name="p124421035015"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090604.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1822504101214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12159152221011"><a name="p12159152221011"></a><a name="p12159152221011"></a>Update(client *gophercloud.ServiceClient, bandwidthId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1944320311019"><a name="p1944320311019"></a><a name="p1944320311019"></a>PUT /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p10443338015"><a name="p10443338015"></a><a name="p10443338015"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090605.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10225124131215"><td class="cellrowborder" rowspan="5" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p132257415120"><a name="p132257415120"></a><a name="p132257415120"></a>Ports</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p1816014228107"><a name="p1816014228107"></a><a name="p1816014228107"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p14443131304"><a name="p14443131304"></a><a name="p14443131304"></a>POST /v1/{project_id}/ports</p>
<p id="p5443331305"><a name="p5443331305"></a><a name="p5443331305"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195886.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row722619412129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17160122191019"><a name="p17160122191019"></a><a name="p17160122191019"></a>Delete(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11443123001"><a name="p11443123001"></a><a name="p11443123001"></a>DELETE /v1/{project_id}/ports/{port_id}</p>
<p id="p74431233012"><a name="p74431233012"></a><a name="p74431233012"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195890.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row822684151214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p916015224106"><a name="p916015224106"></a><a name="p916015224106"></a>Get(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p189143118218"><a name="p189143118218"></a><a name="p189143118218"></a>GET /v1/{project_id}/ports/{port_id}</p>
<p id="p19146119216"><a name="p19146119216"></a><a name="p19146119216"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195887.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1222674181213"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p151601322121012"><a name="p151601322121012"></a><a name="p151601322121012"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4546102512217"><a name="p4546102512217"></a><a name="p4546102512217"></a>GET /v1/{project_id}/ports</p>
<p id="p1654617251222"><a name="p1654617251222"></a><a name="p1654617251222"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195888.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7228146124"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p91601223105"><a name="p91601223105"></a><a name="p91601223105"></a>Update(client *gophercloud.ServiceClient, portId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p35466251926"><a name="p35466251926"></a><a name="p35466251926"></a>PUT /v1/{project_id}/ports/{port_id}</p>
<p id="p3546225926"><a name="p3546225926"></a><a name="p3546225926"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195889.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8228114121213"><td class="cellrowborder" rowspan="4" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p178432495419"><a name="p178432495419"></a><a name="p178432495419"></a>PrivateIps</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p1616062217104"><a name="p1616062217104"></a><a name="p1616062217104"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p1254632516213"><a name="p1254632516213"></a><a name="p1254632516213"></a>POST /v1/{project_id}/privateips</p>
<p id="p154632514214"><a name="p154632514214"></a><a name="p154632514214"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090610.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2228144191218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p131607228107"><a name="p131607228107"></a><a name="p131607228107"></a>Delete(client *gophercloud.ServiceClient, privateipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p108753586216"><a name="p108753586216"></a><a name="p108753586216"></a>DELETE /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p6875115819210"><a name="p6875115819210"></a><a name="p6875115819210"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090613.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42284415122"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15160182219104"><a name="p15160182219104"></a><a name="p15160182219104"></a>Get(client *gophercloud.ServiceClient, privateipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p58751558727"><a name="p58751558727"></a><a name="p58751558727"></a>GET /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p128755581023"><a name="p128755581023"></a><a name="p128755581023"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090611.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10229174131219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p141609225100"><a name="p141609225100"></a><a name="p141609225100"></a>List(client *gophercloud.ServiceClient, subnetId string, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11876658125"><a name="p11876658125"></a><a name="p11876658125"></a>GET /v1/{project_id}/subnets/{subnet_id}/privateips</p>
<p id="p148761858926"><a name="p148761858926"></a><a name="p148761858926"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090612.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row182299471214"><td class="cellrowborder" rowspan="5" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p14981935115410"><a name="p14981935115410"></a><a name="p14981935115410"></a>PublicIps</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p12160162251020"><a name="p12160162251020"></a><a name="p12160162251020"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p839216732"><a name="p839216732"></a><a name="p839216732"></a>POST /v1/{project_id}/publicips</p>
<p id="p18391916233"><a name="p18391916233"></a><a name="p18391916233"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090596.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10229448122"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6160122121016"><a name="p6160122121016"></a><a name="p6160122121016"></a>Delete(client *gophercloud.ServiceClient, publicipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p143915161036"><a name="p143915161036"></a><a name="p143915161036"></a>DELETE /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p13971619310"><a name="p13971619310"></a><a name="p13971619310"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090601.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row152299411129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p81601222109"><a name="p81601222109"></a><a name="p81601222109"></a>Get(client *gophercloud.ServiceClient, publicipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p183911161332"><a name="p183911161332"></a><a name="p183911161332"></a>GET /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p103991615318"><a name="p103991615318"></a><a name="p103991615318"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090597.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9229114201216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1516062271012"><a name="p1516062271012"></a><a name="p1516062271012"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18401816936"><a name="p18401816936"></a><a name="p18401816936"></a>GET /v1/{project_id}/publicips</p>
<p id="p104012161436"><a name="p104012161436"></a><a name="p104012161436"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row202295417123"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p101609228109"><a name="p101609228109"></a><a name="p101609228109"></a>Update(client *gophercloud.ServiceClient, publicipId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1640121611318"><a name="p1640121611318"></a><a name="p1640121611318"></a>PUT /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p114010162036"><a name="p114010162036"></a><a name="p114010162036"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090600.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row112291249122"><td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p42299416129"><a name="p42299416129"></a><a name="p42299416129"></a>Quotas</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p181601122141019"><a name="p181601122141019"></a><a name="p181601122141019"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p14413261236"><a name="p14413261236"></a><a name="p14413261236"></a>GET /v1/{project_id}/quotas</p>
<p id="p164410261833"><a name="p164410261833"></a><a name="p164410261833"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090607.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row322915481215"><td class="cellrowborder" rowspan="4" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p11487194145916"><a name="p11487194145916"></a><a name="p11487194145916"></a>SecurityGroupRules</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p1016092212106"><a name="p1016092212106"></a><a name="p1016092212106"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p28661951537"><a name="p28661951537"></a><a name="p28661951537"></a>POST /v1/security-group-rules</p>
<p id="p128661951133"><a name="p128661951133"></a><a name="p128661951133"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087451723.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row922912415126"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1716015228102"><a name="p1716015228102"></a><a name="p1716015228102"></a>Delete(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13867951537"><a name="p13867951537"></a><a name="p13867951537"></a>DELETE /v1/security-group-rules/{security-groups-rules-id}</p>
<p id="p88675517310"><a name="p88675517310"></a><a name="p88675517310"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467071.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1422919401220"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4160172271017"><a name="p4160172271017"></a><a name="p4160172271017"></a>Get(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p128671751335"><a name="p128671751335"></a><a name="p128671751335"></a>GET /v1/security-group-rules/{security-groups-rules-id}</p>
<p id="p58671351937"><a name="p58671351937"></a><a name="p58671351937"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row162299411128"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19161822101011"><a name="p19161822101011"></a><a name="p19161822101011"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p186712510312"><a name="p186712510312"></a><a name="p186712510312"></a>GET /v1/security-group-rules</p>
<p id="p1986765112315"><a name="p1986765112315"></a><a name="p1986765112315"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467070.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62301341122"><td class="cellrowborder" rowspan="4" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p54116475415"><a name="p54116475415"></a><a name="p54116475415"></a>SecurityGroups</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p4161102217109"><a name="p4161102217109"></a><a name="p4161102217109"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p1986725113312"><a name="p1986725113312"></a><a name="p1986725113312"></a>POST /v1/{project_id}/security-groups</p>
<p id="p108676511537"><a name="p108676511537"></a><a name="p108676511537"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090615.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row192307481210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1916142261012"><a name="p1916142261012"></a><a name="p1916142261012"></a>Delete(client *gophercloud.ServiceClient, securityGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4868105110314"><a name="p4868105110314"></a><a name="p4868105110314"></a>DELETE /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p10868351431"><a name="p10868351431"></a><a name="p10868351431"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0086438567.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row202303419124"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1016172210104"><a name="p1016172210104"></a><a name="p1016172210104"></a>Get(client *gophercloud.ServiceClient, securityGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15868125114311"><a name="p15868125114311"></a><a name="p15868125114311"></a>GET /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p10868105116318"><a name="p10868105116318"></a><a name="p10868105116318"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090616.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1823013411120"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18161112231020"><a name="p18161112231020"></a><a name="p18161112231020"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p786815511931"><a name="p786815511931"></a><a name="p786815511931"></a>GET /v1/{project_id}/security-groups</p>
<p id="p1868125110318"><a name="p1868125110318"></a><a name="p1868125110318"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090617.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1123012461218"><td class="cellrowborder" rowspan="5" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p223012481211"><a name="p223012481211"></a><a name="p223012481211"></a>Subnets</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p11161322191013"><a name="p11161322191013"></a><a name="p11161322191013"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p153457197411"><a name="p153457197411"></a><a name="p153457197411"></a>POST /v1/{project_id}/subnets</p>
<p id="p16345419549"><a name="p16345419549"></a><a name="p16345419549"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090590.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8230444129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1016122261013"><a name="p1016122261013"></a><a name="p1016122261013"></a>Delete(client *gophercloud.ServiceClient, vpcId string, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16978185812414"><a name="p16978185812414"></a><a name="p16978185812414"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p134512191541"><a name="p134512191541"></a><a name="p134512191541"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090594.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row192301241125"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p61616224101"><a name="p61616224101"></a><a name="p61616224101"></a>Get(client *gophercloud.ServiceClient, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33457191045"><a name="p33457191045"></a><a name="p33457191045"></a>GET /v1/{project_id}/subnets/{subnet_id}</p>
<p id="p9345819541"><a name="p9345819541"></a><a name="p9345819541"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090591.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18230104191218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p860418346507"><a name="p860418346507"></a><a name="p860418346507"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53451119945"><a name="p53451119945"></a><a name="p53451119945"></a>GET /v1/{project_id}/subnets</p>
<p id="p113459191147"><a name="p113459191147"></a><a name="p113459191147"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090592.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1623054141215"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1716172218108"><a name="p1716172218108"></a><a name="p1716172218108"></a>Update(client *gophercloud.ServiceClient, vpcId string, subnetId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14346101917419"><a name="p14346101917419"></a><a name="p14346101917419"></a>PUT /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p73461519342"><a name="p73461519342"></a><a name="p73461519342"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090593.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row523015419128"><td class="cellrowborder" rowspan="5" valign="top" width="18.39%" headers="mcps1.1.4.1.1 "><p id="p1123110411126"><a name="p1123110411126"></a><a name="p1123110411126"></a>Vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="44.41%" headers="mcps1.1.4.1.2 "><p id="p3161112213102"><a name="p3161112213102"></a><a name="p3161112213102"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="37.2%" headers="mcps1.1.4.1.3 "><p id="p119211028541"><a name="p119211028541"></a><a name="p119211028541"></a>POST /v1/{project_id}/vpcs</p>
<p id="p169211628049"><a name="p169211628049"></a><a name="p169211628049"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090608.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12231134191211"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15161722141015"><a name="p15161722141015"></a><a name="p15161722141015"></a>Delete(client *gophercloud.ServiceClient, vpcId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1192110281243"><a name="p1192110281243"></a><a name="p1192110281243"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p14921228247"><a name="p14921228247"></a><a name="p14921228247"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090627.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row182310416129"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2161622161016"><a name="p2161622161016"></a><a name="p2161622161016"></a>Get(client *gophercloud.ServiceClient, vpcId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p892110281847"><a name="p892110281847"></a><a name="p892110281847"></a>GET /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p29213282417"><a name="p29213282417"></a><a name="p29213282417"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090618.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row523164131210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p116132281015"><a name="p116132281015"></a><a name="p116132281015"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p149215287414"><a name="p149215287414"></a><a name="p149215287414"></a>GET /v1/{project_id}/vpcs</p>
<p id="p169217281347"><a name="p169217281347"></a><a name="p169217281347"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12312471212"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1816211225101"><a name="p1816211225101"></a><a name="p1816211225101"></a>Update(client *gophercloud.ServiceClient, vpcId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1692112281044"><a name="p1692112281044"></a><a name="p1692112281044"></a>PUT /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p9921228146"><a name="p9921228146"></a><a name="p9921228146"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090626.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Neutron v2.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table992328719225"></a>
<table><thead align="left"><tr id="row17099872192215"><th class="cellrowborder" valign="top" width="12.761276127612762%" id="mcps1.1.4.1.1"><p id="p3836953192658"><a name="p3836953192658"></a><a name="p3836953192658"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="51.03510351035104%" id="mcps1.1.4.1.2"><p id="p34036061192658"><a name="p34036061192658"></a><a name="p34036061192658"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.203620362036204%" id="mcps1.1.4.1.3"><p id="p38415708192658"><a name="p38415708192658"></a><a name="p38415708192658"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1456033119225"><td class="cellrowborder" rowspan="5" valign="top" width="12.761276127612762%" headers="mcps1.1.4.1.1 "><p id="p3607449719225"><a name="p3607449719225"></a><a name="p3607449719225"></a>Networks</p>
</td>
<td class="cellrowborder" valign="top" width="51.03510351035104%" headers="mcps1.1.4.1.2 "><p id="p10202225165314"><a name="p10202225165314"></a><a name="p10202225165314"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.203620362036204%" headers="mcps1.1.4.1.3 "><p id="p3840433619225"><a name="p3840433619225"></a><a name="p3840433619225"></a>POST /v2.0/networks</p>
<p id="p4996588403"><a name="p4996588403"></a><a name="p4996588403"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495803.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1483347619225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p102023255537"><a name="p102023255537"></a><a name="p102023255537"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5886338419225"><a name="p5886338419225"></a><a name="p5886338419225"></a>GET /v2.0/networks</p>
<p id="p9994152355213"><a name="p9994152355213"></a><a name="p9994152355213"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3847678719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32028255532"><a name="p32028255532"></a><a name="p32028255532"></a>Get(client *gophercloud.ServiceClient, networkId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4254010119225"><a name="p4254010119225"></a><a name="p4254010119225"></a>GET /v2.0/networks/{network_id}</p>
<p id="p12329142617524"><a name="p12329142617524"></a><a name="p12329142617524"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495802.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6391532719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10202112565312"><a name="p10202112565312"></a><a name="p10202112565312"></a>Update(client *gophercloud.ServiceClient, networkId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4853299119225"><a name="p4853299119225"></a><a name="p4853299119225"></a>PUT /v2.0/networks/{network_id)</p>
<p id="p134810289522"><a name="p134810289522"></a><a name="p134810289522"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495804.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1727432519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p620218257531"><a name="p620218257531"></a><a name="p620218257531"></a>Delete(client *gophercloud.ServiceClient, networkId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3274348619225"><a name="p3274348619225"></a><a name="p3274348619225"></a>DELETE /v2.0/networks/{network_id}</p>
<p id="p453573017525"><a name="p453573017525"></a><a name="p453573017525"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495805.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2524536719225"><td class="cellrowborder" rowspan="5" valign="top" width="12.761276127612762%" headers="mcps1.1.4.1.1 "><p id="p4204824119225"><a name="p4204824119225"></a><a name="p4204824119225"></a>Subnets</p>
</td>
<td class="cellrowborder" valign="top" width="51.03510351035104%" headers="mcps1.1.4.1.2 "><p id="p716014477536"><a name="p716014477536"></a><a name="p716014477536"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.203620362036204%" headers="mcps1.1.4.1.3 "><p id="p5573045319225"><a name="p5573045319225"></a><a name="p5573045319225"></a>POST /v2.0/subnets</p>
<p id="p1022011334522"><a name="p1022011334522"></a><a name="p1022011334522"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160180.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1554961919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p81601247125313"><a name="p81601247125313"></a><a name="p81601247125313"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6590919719225"><a name="p6590919719225"></a><a name="p6590919719225"></a>GET /v2.0/subnets</p>
<p id="p12330153565219"><a name="p12330153565219"></a><a name="p12330153565219"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160178.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2264872619225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p151601647185316"><a name="p151601647185316"></a><a name="p151601647185316"></a>Get(client *gophercloud.ServiceClient, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1645214719225"><a name="p1645214719225"></a><a name="p1645214719225"></a>GET /v2.0/subnets/{subnet_id}</p>
<p id="p13238441185216"><a name="p13238441185216"></a><a name="p13238441185216"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160179.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5365471919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5160134745310"><a name="p5160134745310"></a><a name="p5160134745310"></a>Update(client *gophercloud.ServiceClient, subnetId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4376008319225"><a name="p4376008319225"></a><a name="p4376008319225"></a>PUT /v2.0/subnets/{subnet_id}</p>
<p id="p5189184645216"><a name="p5189184645216"></a><a name="p5189184645216"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160181.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4315595719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18160847135314"><a name="p18160847135314"></a><a name="p18160847135314"></a>Delete(client *gophercloud.ServiceClient, subnetId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2950294819225"><a name="p2950294819225"></a><a name="p2950294819225"></a>DELETE /v2.0/subnets/{subnet_id}</p>
<p id="p7250114914525"><a name="p7250114914525"></a><a name="p7250114914525"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160182.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5941967519225"><td class="cellrowborder" rowspan="5" valign="top" width="12.761276127612762%" headers="mcps1.1.4.1.1 "><p id="p109045619225"><a name="p109045619225"></a><a name="p109045619225"></a>Ports</p>
</td>
<td class="cellrowborder" valign="top" width="51.03510351035104%" headers="mcps1.1.4.1.2 "><p id="p1116094785317"><a name="p1116094785317"></a><a name="p1116094785317"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.203620362036204%" headers="mcps1.1.4.1.3 "><p id="p4928554019225"><a name="p4928554019225"></a><a name="p4928554019225"></a>POST /v2.0/ports</p>
<p id="p627255155214"><a name="p627255155214"></a><a name="p627255155214"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207808.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2015247919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19160104713535"><a name="p19160104713535"></a><a name="p19160104713535"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5011504219225"><a name="p5011504219225"></a><a name="p5011504219225"></a>GET /v2.0/ports</p>
<p id="p09571253195210"><a name="p09571253195210"></a><a name="p09571253195210"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207806.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3018735219225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1616044715534"><a name="p1616044715534"></a><a name="p1616044715534"></a>Get(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4484185619225"><a name="p4484185619225"></a><a name="p4484185619225"></a>GET /v2.0/ports/{port_id}</p>
<p id="p34213566523"><a name="p34213566523"></a><a name="p34213566523"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207807.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row954305419225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17160184713535"><a name="p17160184713535"></a><a name="p17160184713535"></a>Update(client *gophercloud.ServiceClient, portId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2674882319225"><a name="p2674882319225"></a><a name="p2674882319225"></a>PUT /v2.0/ports/{port_id}</p>
<p id="p933315910528"><a name="p933315910528"></a><a name="p933315910528"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207809.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row461260119225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6160547195312"><a name="p6160547195312"></a><a name="p6160547195312"></a>Delete(client *gophercloud.ServiceClient, portId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4990133719225"><a name="p4990133719225"></a><a name="p4990133719225"></a>DELETE /v2.0/ports/{port_id}</p>
<p id="p4184123165310"><a name="p4184123165310"></a><a name="p4184123165310"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207810.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1031281219225"><td class="cellrowborder" rowspan="4" valign="top" width="12.761276127612762%" headers="mcps1.1.4.1.1 "><p id="p783249019225"><a name="p783249019225"></a><a name="p783249019225"></a>SecurityGroup</p>
</td>
<td class="cellrowborder" valign="top" width="51.03510351035104%" headers="mcps1.1.4.1.2 "><p id="p1054841516549"><a name="p1054841516549"></a><a name="p1054841516549"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.203620362036204%" headers="mcps1.1.4.1.3 "><p id="p2819753219225"><a name="p2819753219225"></a><a name="p2819753219225"></a>POST /v2.0/security-groups</p>
<p id="p292626195315"><a name="p292626195315"></a><a name="p292626195315"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595533.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row512484819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11548201513544"><a name="p11548201513544"></a><a name="p11548201513544"></a>Update(client *gophercloud.ServiceClient, securityGroupId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4780904319225"><a name="p4780904319225"></a><a name="p4780904319225"></a>PUT /v2.0/security-groups/{security_group_id}</p>
<p id="p34629965316"><a name="p34629965316"></a><a name="p34629965316"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595534.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1705601819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15548191545419"><a name="p15548191545419"></a><a name="p15548191545419"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4305593219225"><a name="p4305593219225"></a><a name="p4305593219225"></a>GET /v2.0/security-groups</p>
<p id="p0826612165311"><a name="p0826612165311"></a><a name="p0826612165311"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595064.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4477878219225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p654814156547"><a name="p654814156547"></a><a name="p654814156547"></a>Get(client *gophercloud.ServiceClient, securityGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1011827019225"><a name="p1011827019225"></a><a name="p1011827019225"></a>GET /v2.0/security-groups/{security_group_id}</p>
<p id="p438551675314"><a name="p438551675314"></a><a name="p438551675314"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595065.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row147508319225"><td class="cellrowborder" rowspan="4" valign="top" width="12.761276127612762%" headers="mcps1.1.4.1.1 "><p id="p731533019225"><a name="p731533019225"></a><a name="p731533019225"></a>SecurityGroupRules</p>
</td>
<td class="cellrowborder" valign="top" width="51.03510351035104%" headers="mcps1.1.4.1.2 "><p id="p2090193218545"><a name="p2090193218545"></a><a name="p2090193218545"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.203620362036204%" headers="mcps1.1.4.1.3 "><p id="p2195377719225"><a name="p2195377719225"></a><a name="p2195377719225"></a>POST /v2.0/security-group-rules</p>
<p id="p3372171825316"><a name="p3372171825316"></a><a name="p3372171825316"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595558.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2843541519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p790203217542"><a name="p790203217542"></a><a name="p790203217542"></a>Delete(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p653142119225"><a name="p653142119225"></a><a name="p653142119225"></a>DELETE /v2.0/security-group-rules/{security-groups-rules-id}</p>
<p id="p411822214535"><a name="p411822214535"></a><a name="p411822214535"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595559.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row344244919225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18901532155419"><a name="p18901532155419"></a><a name="p18901532155419"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p491542919225"><a name="p491542919225"></a><a name="p491542919225"></a>GET /v2.0/security-group-rules</p>
<p id="p1257792412537"><a name="p1257792412537"></a><a name="p1257792412537"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595556.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5448175519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12911832115411"><a name="p12911832115411"></a><a name="p12911832115411"></a>Get(client *gophercloud.ServiceClient, securityGroupsRulesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2814441819225"><a name="p2814441819225"></a><a name="p2814441819225"></a>GET /v2.0/security-group-rules/{security-groups-rules-id}</p>
<p id="p2184125452113"><a name="p2184125452113"></a><a name="p2184125452113"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595557.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18523019225"><td class="cellrowborder" rowspan="7" valign="top" width="12.761276127612762%" headers="mcps1.1.4.1.1 "><p id="p5855323719225"><a name="p5855323719225"></a><a name="p5855323719225"></a>Routers</p>
</td>
<td class="cellrowborder" valign="top" width="51.03510351035104%" headers="mcps1.1.4.1.2 "><p id="p91571147115411"><a name="p91571147115411"></a><a name="p91571147115411"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.203620362036204%" headers="mcps1.1.4.1.3 "><p id="p5896305719225"><a name="p5896305719225"></a><a name="p5896305719225"></a>POST /v2.0/routers</p>
<p id="p111194294534"><a name="p111194294534"></a><a name="p111194294534"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495815.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4774639619225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2157947115417"><a name="p2157947115417"></a><a name="p2157947115417"></a>Delete(client *gophercloud.ServiceClient, routerId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2823684719225"><a name="p2823684719225"></a><a name="p2823684719225"></a>DELETE /v2.0/routers/{router_id}</p>
<p id="p152521531175319"><a name="p152521531175319"></a><a name="p152521531175319"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495817.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row878108319225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p01571347175413"><a name="p01571347175413"></a><a name="p01571347175413"></a>Update(client *gophercloud.ServiceClient, routerId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2233436919225"><a name="p2233436919225"></a><a name="p2233436919225"></a>PUT /v2.0/routers/{router_id}</p>
<p id="p293614364531"><a name="p293614364531"></a><a name="p293614364531"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495816.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6383039819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9157134745415"><a name="p9157134745415"></a><a name="p9157134745415"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5616315719225"><a name="p5616315719225"></a><a name="p5616315719225"></a>GET /v2.0/routers</p>
<p id="p7146123915315"><a name="p7146123915315"></a><a name="p7146123915315"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062224579.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5579110719225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1115716474541"><a name="p1115716474541"></a><a name="p1115716474541"></a>Get(client *gophercloud.ServiceClient, routerId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5956394819225"><a name="p5956394819225"></a><a name="p5956394819225"></a>GET /v2.0/routers/{router_id}</p>
<p id="p16521541145314"><a name="p16521541145314"></a><a name="p16521541145314"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495814.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3652040119225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3157154713543"><a name="p3157154713543"></a><a name="p3157154713543"></a>AddInterface(client *gophercloud.ServiceClient, routerId string, opts AddInterfaceOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3372757519225"><a name="p3372757519225"></a><a name="p3372757519225"></a>PUT /v2.0/routers/{router_id}/add_router_interface</p>
<p id="p41759419531"><a name="p41759419531"></a><a name="p41759419531"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495818.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4965676819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14157144755414"><a name="p14157144755414"></a><a name="p14157144755414"></a>RemoveInterface(client *gophercloud.ServiceClient, routerId string, opts RemoveInterfaceOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5758809519225"><a name="p5758809519225"></a><a name="p5758809519225"></a>PUT /v2.0/routers/{router_id}/remove_router_interface</p>
<p id="p799674410537"><a name="p799674410537"></a><a name="p799674410537"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495819.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5409263219225"><td class="cellrowborder" rowspan="5" valign="top" width="12.761276127612762%" headers="mcps1.1.4.1.1 "><p id="p42887394176"><a name="p42887394176"></a><a name="p42887394176"></a>FloatingIps</p>
</td>
<td class="cellrowborder" valign="top" width="51.03510351035104%" headers="mcps1.1.4.1.2 "><p id="p53894195513"><a name="p53894195513"></a><a name="p53894195513"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.203620362036204%" headers="mcps1.1.4.1.3 "><p id="p419543119225"><a name="p419543119225"></a><a name="p419543119225"></a>POST /v2.0/floatingips</p>
<p id="p147844472536"><a name="p147844472536"></a><a name="p147844472536"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333022.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5463078019225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p938912112558"><a name="p938912112558"></a><a name="p938912112558"></a>Delete(client *gophercloud.ServiceClient, floatingipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2252190619225"><a name="p2252190619225"></a><a name="p2252190619225"></a>DELETE /v2.0/floatingips/{floatingip_id}</p>
<p id="p726665365310"><a name="p726665365310"></a><a name="p726665365310"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333024.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1416256519225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8389111125514"><a name="p8389111125514"></a><a name="p8389111125514"></a>Update(client *gophercloud.ServiceClient, floatingipId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p420931819225"><a name="p420931819225"></a><a name="p420931819225"></a>PUT /v2.0/floatingips/{floatingip_id}</p>
<p id="p19940655135319"><a name="p19940655135319"></a><a name="p19940655135319"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333023.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5592232019225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17389111145513"><a name="p17389111145513"></a><a name="p17389111145513"></a>List(client *gophercloud.ServiceClient, opts ListOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1779393719225"><a name="p1779393719225"></a><a name="p1779393719225"></a>GET /v2.0/floatingips</p>
<p id="p1374665995313"><a name="p1374665995313"></a><a name="p1374665995313"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4422341819225"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20390151155518"><a name="p20390151155518"></a><a name="p20390151155518"></a>Get(client *gophercloud.ServiceClient, floatingipId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p328004019225"><a name="p328004019225"></a><a name="p328004019225"></a>GET /v2.0/floatingips/{floatingip_id}</p>
<p id="p1596119225410"><a name="p1596119225410"></a><a name="p1596119225410"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333021.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

