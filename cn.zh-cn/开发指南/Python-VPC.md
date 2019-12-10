# Python-VPC<a name="ZH-CN_TOPIC_0070868142"></a>

基于VPC v1 API的SDK接口如下，调用方式举例：conn.vpc.create\_network\(\)

<a name="table18849333144717"></a>
<table><thead align="left"><tr id="row284973394714"><th class="cellrowborder" valign="top" width="18.04180418041804%" id="mcps1.1.4.1.1"><p id="p46411415174820"><a name="p46411415174820"></a><a name="p46411415174820"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.59395939593959%" id="mcps1.1.4.1.2"><p id="p86411155486"><a name="p86411155486"></a><a name="p86411155486"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="42.36423642364236%" id="mcps1.1.4.1.3"><p id="p1641111534819"><a name="p1641111534819"></a><a name="p1641111534819"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1585013337473"><td class="cellrowborder" rowspan="6" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p48504335475"><a name="p48504335475"></a><a name="p48504335475"></a>vpc</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p4432184714018"><a name="p4432184714018"></a><a name="p4432184714018"></a>vpcs(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p243234710014"><a name="p243234710014"></a><a name="p243234710014"></a>GET /v1/{project_id}/vpcs</p>
<p id="p4996588403"><a name="p4996588403"></a><a name="p4996588403"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0850193384719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174321547608"><a name="p174321547608"></a><a name="p174321547608"></a>get_vpc(self, vpc)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6432174716017"><a name="p6432174716017"></a><a name="p6432174716017"></a>GET /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p17766351453"><a name="p17766351453"></a><a name="p17766351453"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090618.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2850173317479"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1543211478017"><a name="p1543211478017"></a><a name="p1543211478017"></a>create_vpc(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p154323471209"><a name="p154323471209"></a><a name="p154323471209"></a>POST /v1/{project_id}/vpcs</p>
<p id="p166683864517"><a name="p166683864517"></a><a name="p166683864517"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090608.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1085063314470"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19432154720014"><a name="p19432154720014"></a><a name="p19432154720014"></a>update_vpc(self, vpc, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p24328471807"><a name="p24328471807"></a><a name="p24328471807"></a>PUT /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p1356464015457"><a name="p1356464015457"></a><a name="p1356464015457"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090626.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11850533124715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17432204713011"><a name="p17432204713011"></a><a name="p17432204713011"></a>delete_vpc(self, vpc, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9432144713015"><a name="p9432144713015"></a><a name="p9432144713015"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p5123204312452"><a name="p5123204312452"></a><a name="p5123204312452"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090627.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7850183316478"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p64325471006"><a name="p64325471006"></a><a name="p64325471006"></a>find_vpc(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul93501439101318"></a><a name="ul93501439101318"></a><ul id="ul93501439101318"><li>GET /v1/{project_id}/vpcs/{vpc_id}<p id="p372154517450"><a name="p372154517450"></a><a name="p372154517450"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090618.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/vpcs<p id="p1523335204517"><a name="p1523335204517"></a><a name="p1523335204517"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row1285093394712"><td class="cellrowborder" rowspan="6" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p1485083324720"><a name="p1485083324720"></a><a name="p1485083324720"></a>subnet</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p543212472009"><a name="p543212472009"></a><a name="p543212472009"></a>subnets(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p16432247309"><a name="p16432247309"></a><a name="p16432247309"></a>GET /v1/{project_id}/subnets</p>
<p id="p921415674513"><a name="p921415674513"></a><a name="p921415674513"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090592.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2179141617315"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14333472018"><a name="p14333472018"></a><a name="p14333472018"></a>get_subnet(self, subnet)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1343319473017"><a name="p1343319473017"></a><a name="p1343319473017"></a>GET /v1/{project_id}/subnets/{subnet_id}</p>
<p id="p8695205814455"><a name="p8695205814455"></a><a name="p8695205814455"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090591.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row178501533104717"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p643334719013"><a name="p643334719013"></a><a name="p643334719013"></a>create_subnet(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p24337476019"><a name="p24337476019"></a><a name="p24337476019"></a>POST /v1/{project_id}/subnets</p>
<p id="p61121910469"><a name="p61121910469"></a><a name="p61121910469"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090590.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12850633134719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2043317472011"><a name="p2043317472011"></a><a name="p2043317472011"></a>update_subnet(self, subnet, vpc_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p54331447801"><a name="p54331447801"></a><a name="p54331447801"></a>PUT /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p327818214465"><a name="p327818214465"></a><a name="p327818214465"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090593.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row118511033104711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1843304710014"><a name="p1843304710014"></a><a name="p1843304710014"></a>delete_subnet(self, subnet, vpc_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12433647107"><a name="p12433647107"></a><a name="p12433647107"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p067016172717"><a name="p067016172717"></a><a name="p067016172717"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090594.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row118516338471"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174331947908"><a name="p174331947908"></a><a name="p174331947908"></a>find_subnet(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul35054126149"></a><a name="ul35054126149"></a><ul id="ul35054126149"><li>GET /v1/{project_id}/subnets/{subnet_id}<p id="p1981219818464"><a name="p1981219818464"></a><a name="p1981219818464"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090591.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/subnets<p id="p02911913164616"><a name="p02911913164616"></a><a name="p02911913164616"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090592.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row68518331478"><td class="cellrowborder" rowspan="6" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p9851193374716"><a name="p9851193374716"></a><a name="p9851193374716"></a>public_ip</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p4433447704"><a name="p4433447704"></a><a name="p4433447704"></a>public_ips(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p184332047909"><a name="p184332047909"></a><a name="p184332047909"></a>GET /v1/{project_id}/publicips</p>
<p id="p1763531710469"><a name="p1763531710469"></a><a name="p1763531710469"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6851833134715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p743311471302"><a name="p743311471302"></a><a name="p743311471302"></a>get_public_ip(self, public_ip)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p443316471017"><a name="p443316471017"></a><a name="p443316471017"></a>GET /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p2083514193463"><a name="p2083514193463"></a><a name="p2083514193463"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090597.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1685193312471"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p34333471001"><a name="p34333471001"></a><a name="p34333471001"></a>create_public_ip(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p943374718012"><a name="p943374718012"></a><a name="p943374718012"></a>POST /v1/{project_id}/publicips</p>
<p id="p8108112444619"><a name="p8108112444619"></a><a name="p8108112444619"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090596.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row178511333114720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p84331047409"><a name="p84331047409"></a><a name="p84331047409"></a>update_public_ip(self, public_ip, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p194336471909"><a name="p194336471909"></a><a name="p194336471909"></a>PUT /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p152842269469"><a name="p152842269469"></a><a name="p152842269469"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090600.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row158511334473"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1343313472010"><a name="p1343313472010"></a><a name="p1343313472010"></a>delete_public_ip(self, public_ip, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14338479010"><a name="p14338479010"></a><a name="p14338479010"></a>DELETE /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p196401131194612"><a name="p196401131194612"></a><a name="p196401131194612"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090601.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17851133124718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9433747907"><a name="p9433747907"></a><a name="p9433747907"></a>find_public_ip(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul1417513363469"></a><a name="ul1417513363469"></a><ul id="ul1417513363469"><li>GET /v1/{project_id}/publicips/{publicip_id}<p id="p12768153924617"><a name="p12768153924617"></a><a name="p12768153924617"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090597.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/publicips<p id="p921413445467"><a name="p921413445467"></a><a name="p921413445467"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090598.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row3851203315474"><td class="cellrowborder" rowspan="6" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p14851933144711"><a name="p14851933144711"></a><a name="p14851933144711"></a>private_ip</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p1643418472014"><a name="p1643418472014"></a><a name="p1643418472014"></a>private_ips(self, subnet, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p1343494713016"><a name="p1343494713016"></a><a name="p1343494713016"></a>GET /v1/{project_id}/subnets/{subnet_id}/privateips</p>
<p id="p2275144974613"><a name="p2275144974613"></a><a name="p2275144974613"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090612.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row198511833134715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15434847004"><a name="p15434847004"></a><a name="p15434847004"></a>get_private_ip(self, private_ip)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44341847501"><a name="p44341847501"></a><a name="p44341847501"></a>GET /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p3150155284619"><a name="p3150155284619"></a><a name="p3150155284619"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090611.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19852163319479"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16434114718011"><a name="p16434114718011"></a><a name="p16434114718011"></a>create_private_ip(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44342471208"><a name="p44342471208"></a><a name="p44342471208"></a>POST /v1/{project_id}/privateips</p>
<p id="p10523358124612"><a name="p10523358124612"></a><a name="p10523358124612"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090610.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row58522334479"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p104348471606"><a name="p104348471606"></a><a name="p104348471606"></a>create_private_ips(self, *private_ips)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p94342472006"><a name="p94342472006"></a><a name="p94342472006"></a>POST /v1/{project_id}/privateips</p>
<p id="p54095874612"><a name="p54095874612"></a><a name="p54095874612"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090610.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2852733104713"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p44344471201"><a name="p44344471201"></a><a name="p44344471201"></a>delete_private_ip(self, private_ip, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14434104714016"><a name="p14434104714016"></a><a name="p14434104714016"></a>DELETE /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p118021139474"><a name="p118021139474"></a><a name="p118021139474"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090613.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48520338473"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p043410471406"><a name="p043410471406"></a><a name="p043410471406"></a>find_private_ip(self, name_or_id, subnet_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul1477416914710"></a><a name="ul1477416914710"></a><ul id="ul1477416914710"><li>GET /v1/{project_id}/privateips/{privateip_id}<p id="p84255129471"><a name="p84255129471"></a><a name="p84255129471"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090611.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/subnets/{subnet_id}/privateips<p id="p267411710478"><a name="p267411710478"></a><a name="p267411710478"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090612.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row1285243354720"><td class="cellrowborder" rowspan="6" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p4852933104712"><a name="p4852933104712"></a><a name="p4852933104712"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p1543424710020"><a name="p1543424710020"></a><a name="p1543424710020"></a>ports(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p743413471508"><a name="p743413471508"></a><a name="p743413471508"></a>GET /v1/{project_id}/ports</p>
<p id="p1480722164719"><a name="p1480722164719"></a><a name="p1480722164719"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195888.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row685223311471"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p243424717011"><a name="p243424717011"></a><a name="p243424717011"></a>get_port(self, port)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18434104715010"><a name="p18434104715010"></a><a name="p18434104715010"></a>GET /v1/{project_id}/ports/{port_id}</p>
<p id="p1926814252477"><a name="p1926814252477"></a><a name="p1926814252477"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195887.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1852933164710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1743419471509"><a name="p1743419471509"></a><a name="p1743419471509"></a>create_port(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1343412471703"><a name="p1343412471703"></a><a name="p1343412471703"></a>POST /v1/{project_id}/ports</p>
<p id="p1195222774710"><a name="p1195222774710"></a><a name="p1195222774710"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195886.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11852103312472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13434114714020"><a name="p13434114714020"></a><a name="p13434114714020"></a>update_port(self, port, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1543411471501"><a name="p1543411471501"></a><a name="p1543411471501"></a>PUT /v1/{project_id}/ports/{port_id}</p>
<p id="p1443153018478"><a name="p1443153018478"></a><a name="p1443153018478"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195889.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2852133364710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14347471306"><a name="p14347471306"></a><a name="p14347471306"></a>delete_port(self, port, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p54341147406"><a name="p54341147406"></a><a name="p54341147406"></a>DELETE /v1/{project_id}/ports/{port_id}</p>
<p id="p59461232184713"><a name="p59461232184713"></a><a name="p59461232184713"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195890.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row785316333472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1443414713020"><a name="p1443414713020"></a><a name="p1443414713020"></a>find_port(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul32187384477"></a><a name="ul32187384477"></a><ul id="ul32187384477"><li>GET /v1/{project_id}/ports/{port_id}<p id="p142132422473"><a name="p142132422473"></a><a name="p142132422473"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195887.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/ports<p id="p1317504714477"><a name="p1317504714477"></a><a name="p1317504714477"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0133195888.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row138531133184710"><td class="cellrowborder" rowspan="4" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p38532332479"><a name="p38532332479"></a><a name="p38532332479"></a>bandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p1443517476015"><a name="p1443517476015"></a><a name="p1443517476015"></a>bandwidths(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p1643510475018"><a name="p1643510475018"></a><a name="p1643510475018"></a>GET /v1/{project_id}/bandwidths</p>
<p id="p09556517474"><a name="p09556517474"></a><a name="p09556517474"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090604.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1485353319471"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1843584720019"><a name="p1843584720019"></a><a name="p1843584720019"></a>get_bandwidth(self, bandwidth)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p843504719012"><a name="p843504719012"></a><a name="p843504719012"></a>GET /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p16511185512471"><a name="p16511185512471"></a><a name="p16511185512471"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090603.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12853153319476"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p154355470011"><a name="p154355470011"></a><a name="p154355470011"></a>update_bandwidth(self, bandwidth, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p643513471204"><a name="p643513471204"></a><a name="p643513471204"></a>PUT /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p203641126481"><a name="p203641126481"></a><a name="p203641126481"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090605.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row138532333472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18435847306"><a name="p18435847306"></a><a name="p18435847306"></a>find_bandwidth(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul141351183480"></a><a name="ul141351183480"></a><ul id="ul141351183480"><li>GET /v1/{project_id}/bandwidths/{bandwidth_id<p id="p1670318111485"><a name="p1670318111485"></a><a name="p1670318111485"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090603.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/bandwidths<p id="p258812119485"><a name="p258812119485"></a><a name="p258812119485"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090604.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row11853933164713"><td class="cellrowborder" rowspan="5" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p138531733104710"><a name="p138531733104710"></a><a name="p138531733104710"></a>security_group</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p16435144720010"><a name="p16435144720010"></a><a name="p16435144720010"></a>security_groups(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p643517477017"><a name="p643517477017"></a><a name="p643517477017"></a>GET /v1/{project_id}/security-groups</p>
<p id="p8224132717487"><a name="p8224132717487"></a><a name="p8224132717487"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090617.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18539334470"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1043512471208"><a name="p1043512471208"></a><a name="p1043512471208"></a>create_security_group(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p194356471800"><a name="p194356471800"></a><a name="p194356471800"></a>POST /v1/{project_id}/security-groups</p>
<p id="p79161629114811"><a name="p79161629114811"></a><a name="p79161629114811"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090615.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1853633154714"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1743554713013"><a name="p1743554713013"></a><a name="p1743554713013"></a>delete_security_group(self, security_group, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p443515479010"><a name="p443515479010"></a><a name="p443515479010"></a>DELETE /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p531232194815"><a name="p531232194815"></a><a name="p531232194815"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0086438567.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11854123344716"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174351747808"><a name="p174351747808"></a><a name="p174351747808"></a>get_security_group(self, security_group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p134356471409"><a name="p134356471409"></a><a name="p134356471409"></a>GET /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p38831935184819"><a name="p38831935184819"></a><a name="p38831935184819"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090616.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6854733194715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p743574714010"><a name="p743574714010"></a><a name="p743574714010"></a>find_security_group(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul18910240174812"></a><a name="ul18910240174812"></a><ul id="ul18910240174812"><li>GET /v1/{project_id}/security-groups/{security_group_id}<p id="p105741943164814"><a name="p105741943164814"></a><a name="p105741943164814"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090616.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/security-groups<p id="p1884685064812"><a name="p1884685064812"></a><a name="p1884685064812"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090617.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row17854233104714"><td class="cellrowborder" rowspan="5" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p385417339475"><a name="p385417339475"></a><a name="p385417339475"></a>security_group_rule</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p17435647509"><a name="p17435647509"></a><a name="p17435647509"></a>create_security_group_rule(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p14435164711014"><a name="p14435164711014"></a><a name="p14435164711014"></a>POST /v1/{project_id}/security-group-rules</p>
<p id="p192146545487"><a name="p192146545487"></a><a name="p192146545487"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087451723.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row585453394717"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p194351547800"><a name="p194351547800"></a><a name="p194351547800"></a>delete_security_group_rule(self, security_group_rule, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p24353471407"><a name="p24353471407"></a><a name="p24353471407"></a>DELETE /v1/{project_id}/security-group-rules/{rules_security_groups_id}</p>
<p id="p456685674811"><a name="p456685674811"></a><a name="p456685674811"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467071.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row188543334472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1043624715010"><a name="p1043624715010"></a><a name="p1043624715010"></a>get_security_group_rule(self, security_group_rule)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8436124716015"><a name="p8436124716015"></a><a name="p8436124716015"></a>GET /v1/{project_id}/security-group-rules/{rules_security_groups_id}</p>
<p id="p1965816597487"><a name="p1965816597487"></a><a name="p1965816597487"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row685413339474"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p44360471309"><a name="p44360471309"></a><a name="p44360471309"></a>security_group_rules(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p743674714016"><a name="p743674714016"></a><a name="p743674714016"></a>GET /v1/{project_id}/security-group-rules</p>
<p id="p209429434917"><a name="p209429434917"></a><a name="p209429434917"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467070.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12854103316472"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p114369471208"><a name="p114369471208"></a><a name="p114369471208"></a>find_security_group_rule(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul584269104911"></a><a name="ul584269104911"></a><ul id="ul584269104911"><li>GET /v1/{project_id}/security-group-rules/{rules_security_groups_id}<p id="p1850281217497"><a name="p1850281217497"></a><a name="p1850281217497"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v1/{project_id}/security-group-rules<p id="p191641718154911"><a name="p191641718154911"></a><a name="p191641718154911"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0087467070.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row7855143316475"><td class="cellrowborder" valign="top" width="18.04180418041804%" headers="mcps1.1.4.1.1 "><p id="p5855153313479"><a name="p5855153313479"></a><a name="p5855153313479"></a>quota</p>
</td>
<td class="cellrowborder" valign="top" width="39.59395939593959%" headers="mcps1.1.4.1.2 "><p id="p043604715015"><a name="p043604715015"></a><a name="p043604715015"></a>quotas(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.36423642364236%" headers="mcps1.1.4.1.3 "><p id="p443617470019"><a name="p443617470019"></a><a name="p443617470019"></a>GET /v1/{project_id}/quotas</p>
<p id="p5616922124912"><a name="p5616922124912"></a><a name="p5616922124912"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0020090607.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于VPC v2.0 API的SDK接口如下，调用方式举例：conn.vpc.create\_publicip\_ext\(\)

<a name="table3370552115452"></a>
<table><thead align="left"><tr id="row2159874115452"><th class="cellrowborder" valign="top" width="19.05%" id="mcps1.1.4.1.1"><p id="p47022323154543"><a name="p47022323154543"></a><a name="p47022323154543"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="44.59%" id="mcps1.1.4.1.2"><p id="p16160959154543"><a name="p16160959154543"></a><a name="p16160959154543"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.36%" id="mcps1.1.4.1.3"><p id="p45536893154543"><a name="p45536893154543"></a><a name="p45536893154543"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row16856357054"><td class="cellrowborder" rowspan="5" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p162907175610"><a name="p162907175610"></a><a name="p162907175610"></a>sharebandwidth</p>
</td>
<td class="cellrowborder" valign="top" width="44.59%" headers="mcps1.1.4.1.2 "><p id="p1135783111618"><a name="p1135783111618"></a><a name="p1135783111618"></a>create_sharebandwidth(self, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.36%" headers="mcps1.1.4.1.3 "><p id="p11940163716615"><a name="p11940163716615"></a><a name="p11940163716615"></a>POST /v2.0/{project_id}/bandwidths</p>
<p id="p526465416514"><a name="p526465416514"></a><a name="p526465416514"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0106971318.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row236618619618"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p133576311664"><a name="p133576311664"></a><a name="p133576311664"></a>delete_sharebandwidth(self, bandwidth_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p29401374617"><a name="p29401374617"></a><a name="p29401374617"></a>DELETE /v2.0/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p57941156175115"><a name="p57941156175115"></a><a name="p57941156175115"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0106971320.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2721208869"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p143578311767"><a name="p143578311767"></a><a name="p143578311767"></a>create_batch_sharebandwidth(self, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18940203710617"><a name="p18940203710617"></a><a name="p18940203710617"></a>POST /v2.0/{project_id}/batch-bandwidths</p>
<p id="p125346015525"><a name="p125346015525"></a><a name="p125346015525"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0106971319.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row177391011665"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33577311668"><a name="p33577311668"></a><a name="p33577311668"></a>insert_ip_to_bandwidth(self, bandwidth_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p994015370614"><a name="p994015370614"></a><a name="p994015370614"></a>POST /v2.0/{project_id}/bandwidths/{bandwidth_id}/insert</p>
<p id="p13010355215"><a name="p13010355215"></a><a name="p13010355215"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0106971321.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16310144613"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11357203119616"><a name="p11357203119616"></a><a name="p11357203119616"></a>remove_ip_from_bandwidth(self, bandwidth_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1994043712618"><a name="p1994043712618"></a><a name="p1994043712618"></a>POST /v2.0/{project_id}/bandwidths/{bandwidth_id}/remove</p>
<p id="p135948620521"><a name="p135948620521"></a><a name="p135948620521"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0106971322.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3741561815452"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p1791828115452"><a name="p1791828115452"></a><a name="p1791828115452"></a>Eip Operations</p>
</td>
<td class="cellrowborder" valign="top" width="44.59%" headers="mcps1.1.4.1.2 "><p id="p40602242154614"><a name="p40602242154614"></a><a name="p40602242154614"></a>create_publicip_ext(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.36%" headers="mcps1.1.4.1.3 "><p id="p62123706154614"><a name="p62123706154614"></a><a name="p62123706154614"></a>POST /v2.0/{project_id}/publicips</p>
<p id="p3595586527"><a name="p3595586527"></a><a name="p3595586527"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0097550708.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1093589415452"><td class="cellrowborder" valign="top" width="19.05%" headers="mcps1.1.4.1.1 "><p id="p596240715452"><a name="p596240715452"></a><a name="p596240715452"></a>Bandwidth Operations</p>
</td>
<td class="cellrowborder" valign="top" width="44.59%" headers="mcps1.1.4.1.2 "><p id="p17484278154614"><a name="p17484278154614"></a><a name="p17484278154614"></a>update_bandwidth_ext(self, bandwidth_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.36%" headers="mcps1.1.4.1.3 "><p id="p33701575154614"><a name="p33701575154614"></a><a name="p33701575154614"></a>PUT /v2.0/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p5625101175210"><a name="p5625101175210"></a><a name="p5625101175210"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0107682516.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Neutron v2.0 API的SDK接口如下，调用方式举例：conn.network.create\_network\(\)

<a name="table46007650"></a>
<table><thead align="left"><tr id="row17021380"><th class="cellrowborder" valign="top" width="19.19191919191919%" id="mcps1.1.4.1.1"><p id="p36554565"><a name="p36554565"></a><a name="p36554565"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="48.484848484848484%" id="mcps1.1.4.1.2"><p id="p8129827"><a name="p8129827"></a><a name="p8129827"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.32323232323232%" id="mcps1.1.4.1.3"><p id="p54536261"><a name="p54536261"></a><a name="p54536261"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row55361044"><td class="cellrowborder" rowspan="7" valign="top" width="19.19191919191919%" headers="mcps1.1.4.1.1 "><p id="p55059575"><a name="p55059575"></a><a name="p55059575"></a>Floating IP Operations</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.4.1.2 "><p id="p30640599"><a name="p30640599"></a><a name="p30640599"></a>create_ip(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.32323232323232%" headers="mcps1.1.4.1.3 "><p id="p65969435"><a name="p65969435"></a><a name="p65969435"></a>POST /v2.0/floatingips</p>
<p id="p46112299495"><a name="p46112299495"></a><a name="p46112299495"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333022.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56854006"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41771788"><a name="p41771788"></a><a name="p41771788"></a>delete_ip(self, floating_ip, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p28071674"><a name="p28071674"></a><a name="p28071674"></a>DELETE /v2.0/floatingips/{floatingip_id}</p>
<p id="p156643114919"><a name="p156643114919"></a><a name="p156643114919"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333024.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row51318482"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p63156409"><a name="p63156409"></a><a name="p63156409"></a>find_available_ip(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15395467"><a name="p15395467"></a><a name="p15395467"></a>GET /v2.0/floatingips</p>
<p id="p633411344491"><a name="p633411344491"></a><a name="p633411344491"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4341481"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16115657"><a name="p16115657"></a><a name="p16115657"></a>find_ip(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p30299850"><a name="p30299850"></a><a name="p30299850"></a>GET /v2.0/floatingips</p>
<p id="p842693613497"><a name="p842693613497"></a><a name="p842693613497"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4263198"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9774771"><a name="p9774771"></a><a name="p9774771"></a>get_ip(self, floating_ip)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53558972"><a name="p53558972"></a><a name="p53558972"></a>GET /v2.0/floatingips/{floatingip_id}</p>
<p id="p1693117389493"><a name="p1693117389493"></a><a name="p1693117389493"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333021.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12268704"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54240947"><a name="p54240947"></a><a name="p54240947"></a>ips(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p31440558"><a name="p31440558"></a><a name="p31440558"></a>GET /v2.0/floatingips</p>
<p id="p1290845104915"><a name="p1290845104915"></a><a name="p1290845104915"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14529570"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p36044558"><a name="p36044558"></a><a name="p36044558"></a>update_ip(self, floating_ip, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33928053"><a name="p33928053"></a><a name="p33928053"></a>PUT /v2.0/floatingips/{floatingip_id}</p>
<p id="p1971944819499"><a name="p1971944819499"></a><a name="p1971944819499"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060333023.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row36917027"><td class="cellrowborder" rowspan="6" valign="top" width="19.19191919191919%" headers="mcps1.1.4.1.1 "><p id="p37489233"><a name="p37489233"></a><a name="p37489233"></a>Network Operations</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.4.1.2 "><p id="p16729007"><a name="p16729007"></a><a name="p16729007"></a>create_network(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.32323232323232%" headers="mcps1.1.4.1.3 "><p id="p12872293"><a name="p12872293"></a><a name="p12872293"></a>POST /v2.0/networks</p>
<p id="p8847175017490"><a name="p8847175017490"></a><a name="p8847175017490"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495803.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48741777"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p55769855"><a name="p55769855"></a><a name="p55769855"></a>delete_network(self, network, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21064410"><a name="p21064410"></a><a name="p21064410"></a>DELETE /v2.0/networks/{network_id}</p>
<p id="p673775204910"><a name="p673775204910"></a><a name="p673775204910"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495805.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row55361963"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p55134036"><a name="p55134036"></a><a name="p55134036"></a>find_network(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p36671901"><a name="p36671901"></a><a name="p36671901"></a>GET /v2.0/networks</p>
<p id="p1691195417494"><a name="p1691195417494"></a><a name="p1691195417494"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row61611653"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p24487969"><a name="p24487969"></a><a name="p24487969"></a>get_network(self, network)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p37368498"><a name="p37368498"></a><a name="p37368498"></a>GET /v2.0/networks/{network_id}</p>
<p id="p4191957144910"><a name="p4191957144910"></a><a name="p4191957144910"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495802.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row772170"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p62545829"><a name="p62545829"></a><a name="p62545829"></a>networks(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33047401"><a name="p33047401"></a><a name="p33047401"></a>GET /v2.0/networks</p>
<p id="p208208592498"><a name="p208208592498"></a><a name="p208208592498"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row28991153"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66582052"><a name="p66582052"></a><a name="p66582052"></a>update_network(self, network, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p24437140"><a name="p24437140"></a><a name="p24437140"></a>PUT /v2.0/networks/{network_id}</p>
<p id="p2143213508"><a name="p2143213508"></a><a name="p2143213508"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495804.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18607670"><td class="cellrowborder" rowspan="6" valign="top" width="19.19191919191919%" headers="mcps1.1.4.1.1 "><p id="p30826283"><a name="p30826283"></a><a name="p30826283"></a>Port Operations</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.4.1.2 "><p id="p13901009"><a name="p13901009"></a><a name="p13901009"></a>create_port(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.32323232323232%" headers="mcps1.1.4.1.3 "><p id="p52239951"><a name="p52239951"></a><a name="p52239951"></a>POST /v2.0/ports</p>
<p id="p18959933505"><a name="p18959933505"></a><a name="p18959933505"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207808.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row397519"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32199110"><a name="p32199110"></a><a name="p32199110"></a>delete_port(self, port, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p57991080"><a name="p57991080"></a><a name="p57991080"></a>DELETE /v2.0/ports/{port_id}</p>
<p id="p1281613655012"><a name="p1281613655012"></a><a name="p1281613655012"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207810.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52157678"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p64022366"><a name="p64022366"></a><a name="p64022366"></a>find_port(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18429167"><a name="p18429167"></a><a name="p18429167"></a>GET /v2.0/ports</p>
<p id="p3644915504"><a name="p3644915504"></a><a name="p3644915504"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207806.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31644779"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13090320"><a name="p13090320"></a><a name="p13090320"></a>get_port(self, port)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53682985"><a name="p53682985"></a><a name="p53682985"></a>GET /v2.0/ports/{port_id}</p>
<p id="p14315314115019"><a name="p14315314115019"></a><a name="p14315314115019"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207807.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13384821"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10428696"><a name="p10428696"></a><a name="p10428696"></a>ports(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p39418019"><a name="p39418019"></a><a name="p39418019"></a>GET /v2.0/ports</p>
<p id="p55551118115017"><a name="p55551118115017"></a><a name="p55551118115017"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207806.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19217855"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13142459"><a name="p13142459"></a><a name="p13142459"></a>update_port(self, port, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p57906226"><a name="p57906226"></a><a name="p57906226"></a>PUT /v2.0/ports/{port_id}</p>
<p id="p52719219501"><a name="p52719219501"></a><a name="p52719219501"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207809.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row51393992"><td class="cellrowborder" rowspan="8" valign="top" width="19.19191919191919%" headers="mcps1.1.4.1.1 "><p id="p2163846"><a name="p2163846"></a><a name="p2163846"></a>Router Operations</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.4.1.2 "><p id="p41053812"><a name="p41053812"></a><a name="p41053812"></a>create_router(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.32323232323232%" headers="mcps1.1.4.1.3 "><p id="p37024442"><a name="p37024442"></a><a name="p37024442"></a>POST /v2.0/router</p>
<p id="p2097252355019"><a name="p2097252355019"></a><a name="p2097252355019"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495815.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row64784526"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13055244"><a name="p13055244"></a><a name="p13055244"></a>delete_router(self, router, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p50841847"><a name="p50841847"></a><a name="p50841847"></a>DELETE /v2.0/routers/{router_id}</p>
<p id="p2869182625019"><a name="p2869182625019"></a><a name="p2869182625019"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495817.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row54923440"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19613673"><a name="p19613673"></a><a name="p19613673"></a>find_router(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p45203650"><a name="p45203650"></a><a name="p45203650"></a>GET /v2.0/routers</p>
<p id="p9224132915504"><a name="p9224132915504"></a><a name="p9224132915504"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062224579.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4179666"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3008638"><a name="p3008638"></a><a name="p3008638"></a>get_router(self, router)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p42373151"><a name="p42373151"></a><a name="p42373151"></a>GET /v2.0/routers/{router_id}</p>
<p id="p1768143214508"><a name="p1768143214508"></a><a name="p1768143214508"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495814.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row45814047"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19950346"><a name="p19950346"></a><a name="p19950346"></a>routers(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5365342"><a name="p5365342"></a><a name="p5365342"></a>GET /v2.0/routers</p>
<p id="p1684311346506"><a name="p1684311346506"></a><a name="p1684311346506"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062224579.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48288078"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19020241"><a name="p19020241"></a><a name="p19020241"></a>update_router(self, router, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p64244561"><a name="p64244561"></a><a name="p64244561"></a>PUT /v2.0/routers/{router_id}</p>
<p id="p3260123920509"><a name="p3260123920509"></a><a name="p3260123920509"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495816.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row41330139"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p59406944"><a name="p59406944"></a><a name="p59406944"></a>add_interface_to_router(self, router, subnet_id=None, port_id=None)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p47233174"><a name="p47233174"></a><a name="p47233174"></a>PUT /v2.0/routers/{router_id}/add_router_interface</p>
<p id="p2412204215018"><a name="p2412204215018"></a><a name="p2412204215018"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495818.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row22445387"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6137036"><a name="p6137036"></a><a name="p6137036"></a>remove_interface_from_router(self, router, subnet_id=None, port_id=None)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p27337939"><a name="p27337939"></a><a name="p27337939"></a>PUT /v2.0/routers/{router_id}/remove_router_interface</p>
<p id="p1282364435012"><a name="p1282364435012"></a><a name="p1282364435012"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060495819.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row44714859"><td class="cellrowborder" rowspan="13" valign="top" width="19.19191919191919%" headers="mcps1.1.4.1.1 "><p id="p65133811"><a name="p65133811"></a><a name="p65133811"></a>Security Group Operations</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.4.1.2 "><p id="p41347315"><a name="p41347315"></a><a name="p41347315"></a>create_security_group(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.32323232323232%" headers="mcps1.1.4.1.3 "><p id="p60798228"><a name="p60798228"></a><a name="p60798228"></a>POST /v2.0/security-groups</p>
<p id="p63444710503"><a name="p63444710503"></a><a name="p63444710503"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595533.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10313144"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p30058349"><a name="p30058349"></a><a name="p30058349"></a>delete_security_group(self, security_group, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18807190"><a name="p18807190"></a><a name="p18807190"></a>DELETE /v2.0/security-groups/{security_group_id}</p>
<p id="p1116810495502"><a name="p1116810495502"></a><a name="p1116810495502"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595555.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row35046986"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20233597"><a name="p20233597"></a><a name="p20233597"></a>find_security_group(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p28308632"><a name="p28308632"></a><a name="p28308632"></a>GET /v2.0/security-groups</p>
<p id="p191418497507"><a name="p191418497507"></a><a name="p191418497507"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595064.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row53451100"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p34571880"><a name="p34571880"></a><a name="p34571880"></a>get_security_group(self, security_group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p48858863"><a name="p48858863"></a><a name="p48858863"></a>GET /v2.0/security-groups/{security_group_id}</p>
<p id="p10148185265017"><a name="p10148185265017"></a><a name="p10148185265017"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595065.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row37076589"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p50413755"><a name="p50413755"></a><a name="p50413755"></a>security_groups(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56982329"><a name="p56982329"></a><a name="p56982329"></a>GET /v2.0/security-groups</p>
<p id="p112549553504"><a name="p112549553504"></a><a name="p112549553504"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595064.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row43078913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66839947"><a name="p66839947"></a><a name="p66839947"></a>update_security_group(self, security_group, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p45326617"><a name="p45326617"></a><a name="p45326617"></a>PUT /v2.0/security-groups/{security_group_id}</p>
<p id="p17713157175018"><a name="p17713157175018"></a><a name="p17713157175018"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595534.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5286373"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p25543093"><a name="p25543093"></a><a name="p25543093"></a>security_group_open_port(self, sgid, port, protocol='tcp')</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55724670"><a name="p55724670"></a><a name="p55724670"></a>POST /v2.0/security-group-rules</p>
<p id="p18732200185115"><a name="p18732200185115"></a><a name="p18732200185115"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595558.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31759983"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p22421791"><a name="p22421791"></a><a name="p22421791"></a>security_group_allow_ping(self, sgid)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4225755"><a name="p4225755"></a><a name="p4225755"></a>POST /v2.0/security-group-rules</p>
<p id="p919773175120"><a name="p919773175120"></a><a name="p919773175120"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595558.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row38031802"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60677108"><a name="p60677108"></a><a name="p60677108"></a>create_security_group_rule(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15898735"><a name="p15898735"></a><a name="p15898735"></a>POST /v2.0/security-group-rules</p>
<p id="p13375168105119"><a name="p13375168105119"></a><a name="p13375168105119"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595558.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8870892"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p47453675"><a name="p47453675"></a><a name="p47453675"></a>delete_security_group_rule(self, security_group_rule, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18542462"><a name="p18542462"></a><a name="p18542462"></a>DELETE /v2.0/security-group-rules/{security_group_rule_id}</p>
<p id="p56095104511"><a name="p56095104511"></a><a name="p56095104511"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595559.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row32664435"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p28573568"><a name="p28573568"></a><a name="p28573568"></a>find_security_group_rule(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32757653"><a name="p32757653"></a><a name="p32757653"></a>GET /v2.0/security-group-rules</p>
<p id="p202021585114"><a name="p202021585114"></a><a name="p202021585114"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595556.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row26383427"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p56682808"><a name="p56682808"></a><a name="p56682808"></a>get_security_group_rule(self, security_group_rule)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p27904713"><a name="p27904713"></a><a name="p27904713"></a>GET /v2.0/security-group-rules/{security_group_rule_id}</p>
<p id="p136781620115117"><a name="p136781620115117"></a><a name="p136781620115117"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595557.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row49815832"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8550624"><a name="p8550624"></a><a name="p8550624"></a>security_group_rules(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21511928"><a name="p21511928"></a><a name="p21511928"></a>GET /v2.0/security-group-rules</p>
<p id="p55891326155118"><a name="p55891326155118"></a><a name="p55891326155118"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0060595556.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row59389625"><td class="cellrowborder" rowspan="7" valign="top" width="19.19191919191919%" headers="mcps1.1.4.1.1 "><p id="p45830349"><a name="p45830349"></a><a name="p45830349"></a>Subnet Operations</p>
</td>
<td class="cellrowborder" valign="top" width="48.484848484848484%" headers="mcps1.1.4.1.2 "><p id="p21270789"><a name="p21270789"></a><a name="p21270789"></a>create_subnet(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.32323232323232%" headers="mcps1.1.4.1.3 "><p id="p45212362"><a name="p45212362"></a><a name="p45212362"></a>POST /v2.0/subnets</p>
<p id="p1655242918519"><a name="p1655242918519"></a><a name="p1655242918519"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160180.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4258076"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9359903"><a name="p9359903"></a><a name="p9359903"></a>delete_subnet(self, subnet, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19954658"><a name="p19954658"></a><a name="p19954658"></a>DELETE /v2.0/subnets/{subnet_id}</p>
<p id="p1955653325118"><a name="p1955653325118"></a><a name="p1955653325118"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160182.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row45374195"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p51431161"><a name="p51431161"></a><a name="p51431161"></a>find_subnet(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5174549"><a name="p5174549"></a><a name="p5174549"></a>GET /v2.0/subnets</p>
<p id="p1470983517513"><a name="p1470983517513"></a><a name="p1470983517513"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160178.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46570941"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14149906"><a name="p14149906"></a><a name="p14149906"></a>get_subnet(self, subnet)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5291760"><a name="p5291760"></a><a name="p5291760"></a>GET /v2.0/subnets/{subnet_id}</p>
<p id="p108949372517"><a name="p108949372517"></a><a name="p108949372517"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160179.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row47625841"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32487918"><a name="p32487918"></a><a name="p32487918"></a>subnets(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14275720"><a name="p14275720"></a><a name="p14275720"></a>GET /v2.0/subnets</p>
<p id="p0558184114511"><a name="p0558184114511"></a><a name="p0558184114511"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160178.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row61372619"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5126234"><a name="p5126234"></a><a name="p5126234"></a>get_subnet_ports(self, subnet_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12571834"><a name="p12571834"></a><a name="p12571834"></a>GET /v2.0/ports</p>
<p id="p1785284365117"><a name="p1785284365117"></a><a name="p1785284365117"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062207806.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46037648"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p38061996"><a name="p38061996"></a><a name="p38061996"></a>update_subnet(self, subnet, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p63122796"><a name="p63122796"></a><a name="p63122796"></a>PUT /v2.0/subnets/{subnet_id}</p>
<p id="p102584810517"><a name="p102584810517"></a><a name="p102584810517"></a><a href="https://support.huaweicloud.com/api-vpc/zh-cn_topic_0062160181.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

