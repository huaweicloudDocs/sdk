# Java-ECS<a name="ZH-CN_TOPIC_0070867954"></a>

基于Nova v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table34008447"></a>
<table><thead align="left"><tr id="row59665636"><th class="cellrowborder" valign="top" width="22.92929292929293%" id="mcps1.1.4.1.1"><p id="p1078370"><a name="p1078370"></a><a name="p1078370"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="44.74747474747475%" id="mcps1.1.4.1.2"><p id="p20239120"><a name="p20239120"></a><a name="p20239120"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.323232323232325%" id="mcps1.1.4.1.3"><p id="p28755990"><a name="p28755990"></a><a name="p28755990"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row47533853"><td class="cellrowborder" rowspan="6" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p25036876"><a name="p25036876"></a><a name="p25036876"></a>ComputeFloatingIPService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p14721100"><a name="p14721100"></a><a name="p14721100"></a>ActionResponse addFloatingIP(Server server, String ipAddress)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p51558469"><a name="p51558469"></a><a name="p51558469"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p14157057121719"><a name="p14157057121719"></a><a name="p14157057121719"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817718.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row61373038"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5160142"><a name="p5160142"></a><a name="p5160142"></a>ActionResponse addFloatingIP(Server server, String fixedIpAddress, String ipAddress)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15318330"><a name="p15318330"></a><a name="p15318330"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p176441120194"><a name="p176441120194"></a><a name="p176441120194"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817718.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3647249"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26991739"><a name="p26991739"></a><a name="p26991739"></a>FloatingIP allocateIP(String pool)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38847270"><a name="p38847270"></a><a name="p38847270"></a>POST /v2/{project_id}/os-floating-ips</p>
<p id="p48017801913"><a name="p48017801913"></a><a name="p48017801913"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820816.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14081115"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66828554"><a name="p66828554"></a><a name="p66828554"></a>ActionResponse deallocateIP(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44403789"><a name="p44403789"></a><a name="p44403789"></a>DELETE /v2/{project_id}/os-floating-ips/{floating_ip_id}</p>
<p id="p8569151518190"><a name="p8569151518190"></a><a name="p8569151518190"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820819.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row64089786"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p23890167"><a name="p23890167"></a><a name="p23890167"></a>List&lt;? extends FloatingIP&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56055356"><a name="p56055356"></a><a name="p56055356"></a>GET /v2/{project_id}/os-floating-ips</p>
<p id="p18881127121920"><a name="p18881127121920"></a><a name="p18881127121920"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820817.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row34736162"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p62165703"><a name="p62165703"></a><a name="p62165703"></a>ActionResponse removeFloatingIP(Server server, String ipAddress)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2257160"><a name="p2257160"></a><a name="p2257160"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p1199492682012"><a name="p1199492682012"></a><a name="p1199492682012"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817719.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20314447"><td class="cellrowborder" rowspan="4" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p34857543"><a name="p34857543"></a><a name="p34857543"></a>ComputeImageService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p4888719"><a name="p4888719"></a><a name="p4888719"></a>ActionResponse delete(String imageId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p60441935"><a name="p60441935"></a><a name="p60441935"></a>DELETE /v2/{project_id}/images/{image_id}</p>
<p id="p15284143782012"><a name="p15284143782012"></a><a name="p15284143782012"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817699.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7106508"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p38756276"><a name="p38756276"></a><a name="p38756276"></a>Image get(String imageId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52250665"><a name="p52250665"></a><a name="p52250665"></a>GET /v2/{project_id}/images/{image_id}</p>
<p id="p9269135082013"><a name="p9269135082013"></a><a name="p9269135082013"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817697.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row493939"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p40009126"><a name="p40009126"></a><a name="p40009126"></a>List&lt;? extends Image&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19513753"><a name="p19513753"></a><a name="p19513753"></a>GET /v2/{project_id}/images/detail</p>
<p id="p067913565204"><a name="p067913565204"></a><a name="p067913565204"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817696.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row41406050"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p65555736"><a name="p65555736"></a><a name="p65555736"></a>List&lt;? extends Image&gt; list(boolean detailed)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul1046717178597"></a><a name="ul1046717178597"></a><ul id="ul1046717178597"><li>detailed=true:<p id="p1017672615594"><a name="p1017672615594"></a><a name="p1017672615594"></a>GET /v2/{project_id}/images/detail</p>
<p id="p147311712114"><a name="p147311712114"></a><a name="p147311712114"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817696.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>detailed=false:<p id="p1317818307590"><a name="p1317818307590"></a><a name="p1317818307590"></a>GET /v2/{project_id}/images</p>
<p id="p896181214216"><a name="p896181214216"></a><a name="p896181214216"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817695.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row8621060"><td class="cellrowborder" rowspan="7" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p27217289"><a name="p27217289"></a><a name="p27217289"></a>ComputeSecurityGroupService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p57116823"><a name="p57116823"></a><a name="p57116823"></a>SecGroupExtension create(String name, String description)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p63059925"><a name="p63059925"></a><a name="p63059925"></a>POST /v2/{project_id}/os-security-groups</p>
<p id="p156224222215"><a name="p156224222215"></a><a name="p156224222215"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0090187680.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row30668413"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1113543"><a name="p1113543"></a><a name="p1113543"></a>SecGroupExtension.Rule createRule(SecGroupExtension.Rule rule)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23088149"><a name="p23088149"></a><a name="p23088149"></a>POST /v2/{project_id}/os-security-group-rules</p>
<p id="p112118292213"><a name="p112118292213"></a><a name="p112118292213"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817703.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6466753"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54045009"><a name="p54045009"></a><a name="p54045009"></a>ActionResponse delete(String securityGroupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15569626"><a name="p15569626"></a><a name="p15569626"></a>DELETE /v2/{project_id}/os-security-groups/{security_group}</p>
<p id="p127720424213"><a name="p127720424213"></a><a name="p127720424213"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817701.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5908907"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8859419"><a name="p8859419"></a><a name="p8859419"></a>ActionResponse deleteRule(String ruleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46524311"><a name="p46524311"></a><a name="p46524311"></a>DELETE /v2/{project_id}/os-security-group-rules/{security_group_rule_id}</p>
<p id="p7139155052117"><a name="p7139155052117"></a><a name="p7139155052117"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817704.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16065622"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26246992"><a name="p26246992"></a><a name="p26246992"></a>SecGroupExtension get(String securityGroupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p45631627"><a name="p45631627"></a><a name="p45631627"></a>GET /v2/{project_id}/os-security-groups/{security_group_id}</p>
<p id="p1262993132219"><a name="p1262993132219"></a><a name="p1262993132219"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0090187681.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8031464"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p46568871"><a name="p46568871"></a><a name="p46568871"></a>List&lt;? extends SecGroupExtension&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13982202"><a name="p13982202"></a><a name="p13982202"></a>GET /v2/{project_id}/os-security-groups</p>
<p id="p643641192218"><a name="p643641192218"></a><a name="p643641192218"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0090187679.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13898105093515"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1470913214366"><a name="p1470913214366"></a><a name="p1470913214366"></a>SecGroupExtension update(String securityGroupId, String name, String description)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17709422369"><a name="p17709422369"></a><a name="p17709422369"></a>PUT /v2/{project_id}/os-security-groups/{security_group_id}</p>
<p id="p14662179220"><a name="p14662179220"></a><a name="p14662179220"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817700.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row58730959"><td class="cellrowborder" rowspan="4" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p59587228"><a name="p59587228"></a><a name="p59587228"></a>FlavorService</p>
<p id="p10171746933"><a name="p10171746933"></a><a name="p10171746933"></a></p>
<p id="p01145501632"><a name="p01145501632"></a><a name="p01145501632"></a></p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p61836145"><a name="p61836145"></a><a name="p61836145"></a>Flavor get(String flavorId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p42671863"><a name="p42671863"></a><a name="p42671863"></a>GET /v2/{project_id}/flavors/{flavor_id}</p>
<p id="p1690020225225"><a name="p1690020225225"></a><a name="p1690020225225"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212659.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48502452"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p36384517"><a name="p36384517"></a><a name="p36384517"></a>List&lt;? extends Flavor&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p61464796"><a name="p61464796"></a><a name="p61464796"></a>GET /v2/{project_id}/flavors/detail</p>
<p id="p2780162718228"><a name="p2780162718228"></a><a name="p2780162718228"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212658.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row81703461931"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 ">&nbsp;</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 ">&nbsp;</td>
</tr>
<tr id="row151141050932"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 ">&nbsp;</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 ">&nbsp;</td>
</tr>
<tr id="row16312252"><td class="cellrowborder" rowspan="4" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p46224020"><a name="p46224020"></a><a name="p46224020"></a>KeypairService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p53158116"><a name="p53158116"></a><a name="p53158116"></a>Keypair create(String name, String publicKey)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p10840149"><a name="p10840149"></a><a name="p10840149"></a>POST /v2/{project_id}/os-keypairs</p>
<p id="p898093572217"><a name="p898093572217"></a><a name="p898093572217"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212678.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row30452481"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p50731910"><a name="p50731910"></a><a name="p50731910"></a>ActionResponse delete(String name)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15644031"><a name="p15644031"></a><a name="p15644031"></a>DELETE /v2/{project_id}/os-keypairs/{keypair_name}</p>
<p id="p37077414224"><a name="p37077414224"></a><a name="p37077414224"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212680.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6578555"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p63100926"><a name="p63100926"></a><a name="p63100926"></a>Keypair get(String name)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10901353"><a name="p10901353"></a><a name="p10901353"></a>GET /v2/{project_id}/os-keypairs/{keypair_name}</p>
<p id="p67413489226"><a name="p67413489226"></a><a name="p67413489226"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212677.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31003317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p28240785"><a name="p28240785"></a><a name="p28240785"></a>List&lt;? extends Keypair&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5802216"><a name="p5802216"></a><a name="p5802216"></a>GET /v2/{project_id}/os-keypairs</p>
<p id="p5753145412219"><a name="p5753145412219"></a><a name="p5753145412219"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212676.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row57651333133019"><td class="cellrowborder" rowspan="2" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p5765134916303"><a name="p5765134916303"></a><a name="p5765134916303"></a>InstanceActionsService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p031384463016"><a name="p031384463016"></a><a name="p031384463016"></a>List&lt;? extends InstanceAction&gt; list(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p173131544163015"><a name="p173131544163015"></a><a name="p173131544163015"></a>GET /v2/{project_id}/servers/{server_id}/os-instance-actions</p>
<p id="p552616594223"><a name="p552616594223"></a><a name="p552616594223"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817692.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row09091353305"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6313144443011"><a name="p6313144443011"></a><a name="p6313144443011"></a>InstanceAction get(String serverId, String requestId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p143132044143010"><a name="p143132044143010"></a><a name="p143132044143010"></a>GET /v2/{project_id}/servers/{server_id}/os-instance-actions/{request_id}</p>
<p id="p1141581592318"><a name="p1141581592318"></a><a name="p1141581592318"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817693.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52219950"><td class="cellrowborder" rowspan="4" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p1957580"><a name="p1957580"></a><a name="p1957580"></a>QuotaSetService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p24346266"><a name="p24346266"></a><a name="p24346266"></a>QuotaSet get(String tenantId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p25890496"><a name="p25890496"></a><a name="p25890496"></a>GET /v2/{project_id}/os-quota-sets/{project_id}</p>
<p id="p1719862372313"><a name="p1719862372313"></a><a name="p1719862372313"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0067298110.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15306111710314"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p850993412317"><a name="p850993412317"></a><a name="p850993412317"></a>QuotaSet get(String tenantId, String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15509034123118"><a name="p15509034123118"></a><a name="p15509034123118"></a>GET /v2/{project_id}/os-quota-sets/{project_id}?user_id={user_id}</p>
<p id="p736682914236"><a name="p736682914236"></a><a name="p736682914236"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0067298110.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31687876"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16581154"><a name="p16581154"></a><a name="p16581154"></a>Limits limits()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p896237"><a name="p896237"></a><a name="p896237"></a>GET /v2/{project_id}/limits</p>
<p id="p1247053811236"><a name="p1247053811236"></a><a name="p1247053811236"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817717.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row126271720173117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18460154312312"><a name="p18460154312312"></a><a name="p18460154312312"></a>getDefault(String tenantId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1046054317313"><a name="p1046054317313"></a><a name="p1046054317313"></a>GET /v2/{project_id}/os-quota-sets/{project_id}/defaults</p>
<p id="p12175134510233"><a name="p12175134510233"></a><a name="p12175134510233"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817716.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8066134"><td class="cellrowborder" rowspan="4" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p49377135"><a name="p49377135"></a><a name="p49377135"></a>ServerGroupService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p40124968"><a name="p40124968"></a><a name="p40124968"></a>ServerGroup create(String name, String policy)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p28896937"><a name="p28896937"></a><a name="p28896937"></a>POST /v2/{project_id}/os-server-groups</p>
<p id="p52971351122315"><a name="p52971351122315"></a><a name="p52971351122315"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817720.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row58745844"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60792949"><a name="p60792949"></a><a name="p60792949"></a>ActionResponse delete(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p25281875"><a name="p25281875"></a><a name="p25281875"></a>DELETE /v2/{project_id}/os-server-groups/{server_group_id}</p>
<p id="p1190355711236"><a name="p1190355711236"></a><a name="p1190355711236"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817723.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row26210288"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42658596"><a name="p42658596"></a><a name="p42658596"></a>ServerGroup get(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32794215"><a name="p32794215"></a><a name="p32794215"></a>GET /v2/{project_id}/os-server-groups/{server_group_id}</p>
<p id="p1397512418241"><a name="p1397512418241"></a><a name="p1397512418241"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817722.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row26712487"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16227847"><a name="p16227847"></a><a name="p16227847"></a>List&lt;? extends ServerGroup&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p39387211"><a name="p39387211"></a><a name="p39387211"></a>GET /v2/{project_id}/os-server-groups</p>
<p id="p1360155152714"><a name="p1360155152714"></a><a name="p1360155152714"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817721.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row290591014019"><td class="cellrowborder" rowspan="28" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p57792188"><a name="p57792188"></a><a name="p57792188"></a>ServerService</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p1313210366271"><a name="p1313210366271"></a><a name="p1313210366271"></a>VolumeAttachment getAttachVolume(String serverId, String volumeId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p10132193618271"><a name="p10132193618271"></a><a name="p10132193618271"></a>GET /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}</p>
<p id="p559014952811"><a name="p559014952811"></a><a name="p559014952811"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212672.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1082481200"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p82971615183513"><a name="p82971615183513"></a><a name="p82971615183513"></a>List&lt;? extends VolumeAttachment&gt; listAttachedVolumes(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p102971815143518"><a name="p102971815143518"></a><a name="p102971815143518"></a>GET /v2/{project_id}/servers/{server_id}/os-volume_attachments</p>
<p id="p8483324102813"><a name="p8483324102813"></a><a name="p8483324102813"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212671.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18940582"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p50655658"><a name="p50655658"></a><a name="p50655658"></a>ActionResponse action(String serverId, Action action)</p>
<p id="p53247746"><a name="p53247746"></a><a name="p53247746"></a>Executes the specified Action such as RESUME, PAUSE, START, STOP …</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18100201"><a name="p18100201"></a><a name="p18100201"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p83691938192918"><a name="p83691938192918"></a><a name="p83691938192918"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212648.html" target="_blank" rel="noopener noreferrer">链接</a>（START）</p>
<p id="p1036920387290"><a name="p1036920387290"></a><a name="p1036920387290"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212652.html" target="_blank" rel="noopener noreferrer">链接</a>（STOP）</p>
</td>
</tr>
<tr id="row19534171613912"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1853610161592"><a name="p1853610161592"></a><a name="p1853610161592"></a>ActionResponse stop(String serverId, StopType type)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2053610161397"><a name="p2053610161397"></a><a name="p2053610161397"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p1710344411292"><a name="p1710344411292"></a><a name="p1710344411292"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212652.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row23002745"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p51283066"><a name="p51283066"></a><a name="p51283066"></a>VolumeAttachment attachVolume(String serverId, String volumeId, String device)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p60287683"><a name="p60287683"></a><a name="p60287683"></a>POST /v2/{project_id}/servers/{server_id}/os-volume_attachments</p>
<p id="p8962194962912"><a name="p8962194962912"></a><a name="p8962194962912"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0031167350.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5718243"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60524524"><a name="p60524524"></a><a name="p60524524"></a>Server boot(ServerCreate server)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3539410"><a name="p3539410"></a><a name="p3539410"></a>POST /v2/{project_id}/servers</p>
<p id="p92021658102916"><a name="p92021658102916"></a><a name="p92021658102916"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0068473331.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31854691"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p30093150"><a name="p30093150"></a><a name="p30093150"></a>Server bootAndWaitActive(ServerCreate server, int maxWaitTime)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21626090"><a name="p21626090"></a><a name="p21626090"></a>POST /v2/{project_id}/servers</p>
<p id="p1524214103303"><a name="p1524214103303"></a><a name="p1524214103303"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0068473331.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p60417086"><a name="p60417086"></a><a name="p60417086"></a>GET /v2/{project_id}/servers/{server_id}</p>
<p id="p636621518305"><a name="p636621518305"></a><a name="p636621518305"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212690.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6882862"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20640979"><a name="p20640979"></a><a name="p20640979"></a>ActionResponse confirmResize(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p61306625"><a name="p61306625"></a><a name="p61306625"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p1399224113014"><a name="p1399224113014"></a><a name="p1399224113014"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0028714262.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row66889567"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p49345813"><a name="p49345813"></a><a name="p49345813"></a>String createSnapshot(String serverId, String snapshotName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p37587916"><a name="p37587916"></a><a name="p37587916"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p4396132610309"><a name="p4396132610309"></a><a name="p4396132610309"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817694.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21174538"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p37415993"><a name="p37415993"></a><a name="p37415993"></a>ActionResponse delete(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10796581"><a name="p10796581"></a><a name="p10796581"></a>DELETE /v2/{project_id}/servers/{server_id}</p>
<p id="p1760133733015"><a name="p1760133733015"></a><a name="p1760133733015"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0025560296.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row30060365"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18970462"><a name="p18970462"></a><a name="p18970462"></a>ActionResponse deleteMetadataItem(String serverId, String key)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p60212448"><a name="p60212448"></a><a name="p60212448"></a>DELETE /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p11761643123012"><a name="p11761643123012"></a><a name="p11761643123012"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0025560299.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7190103044019"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5677776"><a name="p5677776"></a><a name="p5677776"></a>ActionResponse detachVolume(String serverId, String attachmentId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p57246722"><a name="p57246722"></a><a name="p57246722"></a>DELETE /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}</p>
<p id="p46577497303"><a name="p46577497303"></a><a name="p46577497303"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817707.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row165718519562"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2080392719561"><a name="p2080392719561"></a><a name="p2080392719561"></a>ActionResponse detachVolume(String serverId, String volumeId, int deleteFlag)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12803172713563"><a name="p12803172713563"></a><a name="p12803172713563"></a>DELETE /v2/{project_id}/servers/{server_id}/os-volume_attachments/{volume_id}?delete_flag={delete_flag}</p>
<p id="p125160461536"><a name="p125160461536"></a><a name="p125160461536"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817707.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row45458457"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58256364"><a name="p58256364"></a><a name="p58256364"></a>Server get(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21145081"><a name="p21145081"></a><a name="p21145081"></a>GET /v2/{project_id}/servers/{server_id}</p>
<p id="p32070234319"><a name="p32070234319"></a><a name="p32070234319"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212690.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56088004"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p46834456"><a name="p46834456"></a><a name="p46834456"></a>Map&lt;String,String&gt; getMetadata(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p35494585"><a name="p35494585"></a><a name="p35494585"></a>GET /v2/{project_id}/servers/{server_id}/metadata</p>
<p id="p1236103073115"><a name="p1236103073115"></a><a name="p1236103073115"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817713.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row51015809"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p38639871"><a name="p38639871"></a><a name="p38639871"></a>List&lt;? extends Server&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p42821886"><a name="p42821886"></a><a name="p42821886"></a>GET /v2/{project_id}/servers/detail</p>
<p id="p242213371316"><a name="p242213371316"></a><a name="p242213371316"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212689.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row49852662"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11533784"><a name="p11533784"></a><a name="p11533784"></a>List&lt;? extends Server&gt; list(boolean detail)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul5933125165812"></a><a name="ul5933125165812"></a><ul id="ul5933125165812"><li>detail=true:<p id="p18603449135816"><a name="p18603449135816"></a><a name="p18603449135816"></a>GET /v2/{project_id}/servers/detail</p>
<p id="p1421815455318"><a name="p1421815455318"></a><a name="p1421815455318"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212689.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>detail=false:<p id="p144811444145818"><a name="p144811444145818"></a><a name="p144811444145818"></a>GET /v2/{project_id}/servers</p>
<p id="p11441185314313"><a name="p11441185314313"></a><a name="p11441185314313"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212688.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row19521038"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p37700255"><a name="p37700255"></a><a name="p37700255"></a>List&lt;? extends Server&gt; list(Map&lt;String,String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33821816"><a name="p33821816"></a><a name="p33821816"></a>GET /v2/{project_id}/servers/detail{?changes-since,image,flavor,name,status,host,limit,marker}</p>
<p id="p1563213011322"><a name="p1563213011322"></a><a name="p1563213011322"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212689.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row35960896"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p27151449"><a name="p27151449"></a><a name="p27151449"></a>ActionResponse reboot(String serverId, RebootType type)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p51783759"><a name="p51783759"></a><a name="p51783759"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p276615673216"><a name="p276615673216"></a><a name="p276615673216"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212650.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row54392930"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p43751230"><a name="p43751230"></a><a name="p43751230"></a>ActionResponse resize(String serverId, String flavorId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p54188775"><a name="p54188775"></a><a name="p54188775"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p17874101614322"><a name="p17874101614322"></a><a name="p17874101614322"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0028714261.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row27214660"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p56903870"><a name="p56903870"></a><a name="p56903870"></a>ActionResponse revertResize(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p45810748"><a name="p45810748"></a><a name="p45810748"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p22652022123220"><a name="p22652022123220"></a><a name="p22652022123220"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0028714263.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42930272"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54800025"><a name="p54800025"></a><a name="p54800025"></a>Server update(String serverId, ServerUpdateOptions options)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9617010"><a name="p9617010"></a><a name="p9617010"></a>PUT /v2/{project_id}/servers/{server_id}</p>
<p id="p1649018281329"><a name="p1649018281329"></a><a name="p1649018281329"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212692.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19444226"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p31478446"><a name="p31478446"></a><a name="p31478446"></a>Map&lt;String,String&gt; updateMetadata(String serverId, Map&lt;String,String&gt; metadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p66726223"><a name="p66726223"></a><a name="p66726223"></a>PUT /v2/{project_id}/servers/{server_id}/metadata</p>
<p id="p1531883633220"><a name="p1531883633220"></a><a name="p1531883633220"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0077847902.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row63665103"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p56599738"><a name="p56599738"></a><a name="p56599738"></a>Server waitForServerStatus(String serverId, Server.Status status, int maxWait, TimeUnit maxWaitUnit)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21176078"><a name="p21176078"></a><a name="p21176078"></a>GET /v2/{project_id}/servers/{server_id}</p>
<p id="p13881043173218"><a name="p13881043173218"></a><a name="p13881043173218"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212690.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row55791526133216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p184106513332"><a name="p184106513332"></a><a name="p184106513332"></a>List&lt;? extends Server&gt; list(boolean detail , Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul1410654331"></a><a name="ul1410654331"></a><ul id="ul1410654331"><li>detail = true:</li></ul>
<p id="p184101513332"><a name="p184101513332"></a><a name="p184101513332"></a>GET /v2/{project_id}/servers/detail{?changes-since,image,flavor,name,status,limit,marker,not-tags,reservation_id,ip}</p>
<p id="p10797553103212"><a name="p10797553103212"></a><a name="p10797553103212"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212689.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<a name="ul14410857335"></a><a name="ul14410857335"></a><ul id="ul14410857335"><li>detail = false:</li></ul>
<p id="p34105583312"><a name="p34105583312"></a><a name="p34105583312"></a>GET /v2/{project_id}/servers{?changes-since,image,flavor,name,status,limit,marker,not-tags,reservation_id}</p>
<p id="p8637175953210"><a name="p8637175953210"></a><a name="p8637175953210"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212688.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1250732173213"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14101555335"><a name="p14101555335"></a><a name="p14101555335"></a>String getConsoleOutput(String serverId, int numLines)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7410451330"><a name="p7410451330"></a><a name="p7410451330"></a>POST /v2/{project_id}/servers/{server_id}/action</p>
<p id="p8712051339"><a name="p8712051339"></a><a name="p8712051339"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817689.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1661015354321"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174101057336"><a name="p174101057336"></a><a name="p174101057336"></a>Map&lt;String, String&gt; getMetadataItem(String serverId, String key)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44101057338"><a name="p44101057338"></a><a name="p44101057338"></a>GET /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p19277611153317"><a name="p19277611153317"></a><a name="p19277611153317"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817714.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15420129123212"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15411145143315"><a name="p15411145143315"></a><a name="p15411145143315"></a>Map&lt;String, String&gt; setMetadataItem(String serverId, String key, String value)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10411453334"><a name="p10411453334"></a><a name="p10411453334"></a>PUT /v2/{project_id}/servers/{server_id}/metadata/{key}</p>
<p id="p79581417173317"><a name="p79581417173317"></a><a name="p79581417173317"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0025567413.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56366974"><td class="cellrowborder" rowspan="5" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p2322177"><a name="p2322177"></a><a name="p2322177"></a>InterfaceService (ext)</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p53878657"><a name="p53878657"></a><a name="p53878657"></a>InterfaceAttachment create(String serverId, String portId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p2095077"><a name="p2095077"></a><a name="p2095077"></a>POST /v2/{project_id}/servers/{server_id}/os-interface</p>
<p id="p222942510339"><a name="p222942510339"></a><a name="p222942510339"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212664.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2731161844216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p867873084217"><a name="p867873084217"></a><a name="p867873084217"></a>InterfaceAttachment create(String serverId, NovaInterfaceAttachmentCreate novaInterfaceAttachmentCreate)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p567813017423"><a name="p567813017423"></a><a name="p567813017423"></a>POST /v2/{project_id}/servers/{server_id}/os-interface</p>
<p id="p882623163314"><a name="p882623163314"></a><a name="p882623163314"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212664.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18855696"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p50916422"><a name="p50916422"></a><a name="p50916422"></a>ActionResponse detach(String serverId, String attachmentId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p30589524"><a name="p30589524"></a><a name="p30589524"></a>DELETE /v2/{project_id}/servers/{server_id}/os-interface/{port_id}</p>
<p id="p13676163793317"><a name="p13676163793317"></a><a name="p13676163793317"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212666.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6870268"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19620867"><a name="p19620867"></a><a name="p19620867"></a>InterfaceAttachment get(String serverId, String attachmentId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p45786357"><a name="p45786357"></a><a name="p45786357"></a>GET /v2/{project_id}/servers/{server_id}/os-interface/{port_id}</p>
<p id="p20661946143311"><a name="p20661946143311"></a><a name="p20661946143311"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212662.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9424035"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p25149347"><a name="p25149347"></a><a name="p25149347"></a>List&lt;? extends InterfaceAttachment&gt; list(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23831236"><a name="p23831236"></a><a name="p23831236"></a>GET /v2/{project_id}/servers/{server_id}/os-interface</p>
<p id="p1629765203320"><a name="p1629765203320"></a><a name="p1629765203320"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212661.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13154536"><td class="cellrowborder" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p58884509"><a name="p58884509"></a><a name="p58884509"></a>ZoneService(ext)</p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p4915910"><a name="p4915910"></a><a name="p4915910"></a>List&lt;? extends AvailabilityZone&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p62644428"><a name="p62644428"></a><a name="p62644428"></a>GET /v2/{project_id}/os-availability-zone</p>
<p id="p1510759153310"><a name="p1510759153310"></a><a name="p1510759153310"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065817728.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13309318153410"><td class="cellrowborder" rowspan="6" valign="top" width="22.92929292929293%" headers="mcps1.1.4.1.1 "><p id="p780704983417"><a name="p780704983417"></a><a name="p780704983417"></a>ServerTagService<a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820823.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
<td class="cellrowborder" valign="top" width="44.74747474747475%" headers="mcps1.1.4.1.2 "><p id="p1421641173411"><a name="p1421641173411"></a><a name="p1421641173411"></a>NovaServerTag list(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.323232323232325%" headers="mcps1.1.4.1.3 "><p id="p92114112344"><a name="p92114112344"></a><a name="p92114112344"></a>GET /v2.1/{project_id}/servers/{server_id}/tags</p>
<p id="p145101437142711"><a name="p145101437142711"></a><a name="p145101437142711"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820822.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19296152011346"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0274193410"><a name="p0274193410"></a><a name="p0274193410"></a>NovaServerTag addTags(String serverId, NovaServerTag tags)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p172174133410"><a name="p172174133410"></a><a name="p172174133410"></a>PUT /v2.1/{project_id}/servers/{server_id}/tags</p>
<p id="p102961136132812"><a name="p102961136132812"></a><a name="p102961136132812"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820822.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19844122413349"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p112841193413"><a name="p112841193413"></a><a name="p112841193413"></a>ActionResponse delete(String serverId, String tag)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1429415348"><a name="p1429415348"></a><a name="p1429415348"></a>DELETE /v2.1/{project_id}/servers/{server_id}/tags</p>
<p id="p151031637152813"><a name="p151031637152813"></a><a name="p151031637152813"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820824.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14475122103416"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1214114344"><a name="p1214114344"></a><a name="p1214114344"></a>ActionResponse check(String serverId, String tag)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12174153410"><a name="p12174153410"></a><a name="p12174153410"></a>GET /v2.1/{project_id}/servers/{server_id}/tags/{tag}</p>
<p id="p4234538112815"><a name="p4234538112815"></a><a name="p4234538112815"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820826.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row04492280346"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p121141153415"><a name="p121141153415"></a><a name="p121141153415"></a>ActionResponse addSingle(String serverId, String tag)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p182194114346"><a name="p182194114346"></a><a name="p182194114346"></a>PUT /v2.1/{project_id}/servers/{server_id}/tags/{tag}</p>
<p id="p1216163932815"><a name="p1216163932815"></a><a name="p1216163932815"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820825.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row147992030153412"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p152134163410"><a name="p152134163410"></a><a name="p152134163410"></a>ActionResponse deleteAll(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p112441113415"><a name="p112441113415"></a><a name="p112441113415"></a>DELETE /v2.1/{project_id}/servers/{server_id}/tags/{tag}</p>
<p id="p4991039102820"><a name="p4991039102820"></a><a name="p4991039102820"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0065820827.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于ECS v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table49365540155514"></a>
<table><thead align="left"><tr id="row8867585155514"><th class="cellrowborder" valign="top" width="17.46%" id="mcps1.1.4.1.1"><p id="p46565096155656"><a name="p46565096155656"></a><a name="p46565096155656"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="50.14999999999999%" id="mcps1.1.4.1.2"><p id="p61305001155656"><a name="p61305001155656"></a><a name="p61305001155656"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.39%" id="mcps1.1.4.1.3"><p id="p40467695155656"><a name="p40467695155656"></a><a name="p40467695155656"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row32630553155514"><td class="cellrowborder" rowspan="16" valign="top" width="17.46%" headers="mcps1.1.4.1.1 "><p id="p55982254155638"><a name="p55982254155638"></a><a name="p55982254155638"></a>CloudServerService</p>
<p id="p17117407424"><a name="p17117407424"></a><a name="p17117407424"></a></p>
</td>
<td class="cellrowborder" valign="top" width="50.14999999999999%" headers="mcps1.1.4.1.2 "><p id="p1657518308283"><a name="p1657518308283"></a><a name="p1657518308283"></a>String create(ServerCreate creation)</p>
</td>
<td class="cellrowborder" valign="top" width="32.39%" headers="mcps1.1.4.1.3 "><p id="p32188077155614"><a name="p32188077155614"></a><a name="p32188077155614"></a>POST /v1/{project_id}/cloudservers</p>
<p id="p1463192143518"><a name="p1463192143518"></a><a name="p1463192143518"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212668.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row27006953155514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12845081155614"><a name="p12845081155614"></a><a name="p12845081155614"></a>List&lt;CloudServer&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2393671155614"><a name="p2393671155614"></a><a name="p2393671155614"></a>GET /v1/{project_id}/cloudservers/detail</p>
<p id="p1163183011355"><a name="p1163183011355"></a><a name="p1163183011355"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0094148850.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row67171013816"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p169510980"><a name="p169510980"></a><a name="p169510980"></a>CloudServers listWithCount()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p179131015816"><a name="p179131015816"></a><a name="p179131015816"></a>GET /v1/{project_id}/cloudservers/detail</p>
<p id="p670573610357"><a name="p670573610357"></a><a name="p670573610357"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0094148850.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56202892155514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p48025421155614"><a name="p48025421155614"></a><a name="p48025421155614"></a>CloudServer get(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p24063778155614"><a name="p24063778155614"></a><a name="p24063778155614"></a>GET /v1/{project_id}/cloudservers/{server_id}</p>
<p id="p245264210355"><a name="p245264210355"></a><a name="p245264210355"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0094148849.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row47965757155514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10885174862813"><a name="p10885174862813"></a><a name="p10885174862813"></a>String resize(ResizeServer resize,String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p62593397155614"><a name="p62593397155614"></a><a name="p62593397155614"></a>POST /v1/{project_id}/cloudservers/{server_id}/resize</p>
<p id="p73737133611"><a name="p73737133611"></a><a name="p73737133611"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212653.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row33366200155514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3965162118306"><a name="p3965162118306"></a><a name="p3965162118306"></a>String delete(List&lt;String&gt; serverIds, boolean deletePublicIp, boolean deleteVolume)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5887225155614"><a name="p5887225155614"></a><a name="p5887225155614"></a>POST /v1/{project_id}/cloudservers/delete</p>
<p id="p131810113612"><a name="p131810113612"></a><a name="p131810113612"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212679.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17105222155514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p06546473303"><a name="p06546473303"></a><a name="p06546473303"></a>String stop(List&lt;String&gt; serverIds, StopType type)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8026483155614"><a name="p8026483155614"></a><a name="p8026483155614"></a>POST /v1/{project_id}/cloudservers/action</p>
<p id="p1446131463612"><a name="p1446131463612"></a><a name="p1446131463612"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212651.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1790041155514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19968261155614"><a name="p19968261155614"></a><a name="p19968261155614"></a>String reboot(List&lt;String&gt; serverIds, RebootType type)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23241832155614"><a name="p23241832155614"></a><a name="p23241832155614"></a>POST /v1/{project_id}/cloudservers/action</p>
<p id="p872772263617"><a name="p872772263617"></a><a name="p872772263617"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212649.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7498077155542"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14216110103119"><a name="p14216110103119"></a><a name="p14216110103119"></a>String start(List&lt;String&gt; serverIds)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9327458155614"><a name="p9327458155614"></a><a name="p9327458155614"></a>POST /v1/{project_id}/cloudservers/action</p>
<p id="p858133183613"><a name="p858133183613"></a><a name="p858133183613"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212207.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row121065017501"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1851221915511"><a name="p1851221915511"></a><a name="p1851221915511"></a>List&lt;CloudServer&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17188913103311"><a name="p17188913103311"></a><a name="p17188913103311"></a>GET /v1/{project_id}/cloudservers/detail{?flavor,name,status,limit,offset,not-tags,reservation_id,enterprise_project_id}</p>
<p id="p1789073712367"><a name="p1789073712367"></a><a name="p1789073712367"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0094148850.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row181498301799"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11501030298"><a name="p11501030298"></a><a name="p11501030298"></a>CloudServers listWithCount(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p915083019914"><a name="p915083019914"></a><a name="p915083019914"></a>GET /v1/{project_id}/cloudservers/detail{?flavor,name,status,limit,offset,not-tags,reservation_id,enterprise_project_id}</p>
<p id="p104061122143716"><a name="p104061122143716"></a><a name="p104061122143716"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0094148850.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row322831155116"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8512111914516"><a name="p8512111914516"></a><a name="p8512111914516"></a>List&lt;Flavor&gt; getSpecifications(String availabilityZone)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p75121219185115"><a name="p75121219185115"></a><a name="p75121219185115"></a>GET /v1/{project_id}/cloudservers/flavors{?availability_zone}</p>
<p id="p8219530173712"><a name="p8219530173712"></a><a name="p8219530173712"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212656.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row53361754185016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p195131619135113"><a name="p195131619135113"></a><a name="p195131619135113"></a>CloudAbsoluteLimit limits()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p155131019165112"><a name="p155131019165112"></a><a name="p155131019165112"></a>GET /v1/{project_id}/cloudservers/limits</p>
<p id="p31831239103710"><a name="p31831239103710"></a><a name="p31831239103710"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0020212674.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row181161565350"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p109994288350"><a name="p109994288350"></a><a name="p109994288350"></a>SupportAutoRecovery getAutoRecovery(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19999172814353"><a name="p19999172814353"></a><a name="p19999172814353"></a>GET /v1/{project_id}/cloudservers/{server_id}/autorecovery</p>
<p id="p68775513373"><a name="p68775513373"></a><a name="p68775513373"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0067600148.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1274568163516"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p149994283357"><a name="p149994283357"></a><a name="p149994283357"></a>ActionResponse manageAutoRecovery(String serverId, SupportAutoRecovery supportAutoRecovery)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9999828123518"><a name="p9999828123518"></a><a name="p9999828123518"></a>PUT /v1/{project_id}/cloudservers/{server_id}/autorecovery</p>
<p id="p254511016388"><a name="p254511016388"></a><a name="p254511016388"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0067600284.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6709406426"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 ">&nbsp;</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 ">&nbsp;</td>
</tr>
<tr id="row14618038155548"><td class="cellrowborder" valign="top" width="17.46%" headers="mcps1.1.4.1.1 "><p id="p13653662155548"><a name="p13653662155548"></a><a name="p13653662155548"></a>JobService</p>
</td>
<td class="cellrowborder" valign="top" width="50.14999999999999%" headers="mcps1.1.4.1.2 "><p id="p380091773112"><a name="p380091773112"></a><a name="p380091773112"></a>Job get(String jobId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.39%" headers="mcps1.1.4.1.3 "><p id="p6077593155614"><a name="p6077593155614"></a><a name="p6077593155614"></a>GET /v1/{project_id}/jobs/{job_id}</p>
<p id="p1884812719385"><a name="p1884812719385"></a><a name="p1884812719385"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0022225398.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1275312154198"><td class="cellrowborder" rowspan="4" valign="top" width="17.46%" headers="mcps1.1.4.1.1 "><p id="p28443211918"><a name="p28443211918"></a><a name="p28443211918"></a>TagService</p>
</td>
<td class="cellrowborder" valign="top" width="50.14999999999999%" headers="mcps1.1.4.1.2 "><p id="p81581556171919"><a name="p81581556171919"></a><a name="p81581556171919"></a>ActionResponse add(String serverId, List&lt;ServerTags&gt;</p>
<p id="p1215815612197"><a name="p1215815612197"></a><a name="p1215815612197"></a>serverTags)</p>
</td>
<td class="cellrowborder" valign="top" width="32.39%" headers="mcps1.1.4.1.3 "><p id="p1415912568194"><a name="p1415912568194"></a><a name="p1415912568194"></a>POST /v1/{project_id}/cloudservers/{server_id}/tags/action</p>
<p id="p1615935691917"><a name="p1615935691917"></a><a name="p1615935691917"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0167811963.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9877183282014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1959034492013"><a name="p1959034492013"></a><a name="p1959034492013"></a>ActionResponse delete(String serverId, List&lt;ServerTags&gt;</p>
<p id="p359054472013"><a name="p359054472013"></a><a name="p359054472013"></a>serverTags)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p35901444162017"><a name="p35901444162017"></a><a name="p35901444162017"></a>POST /v1/{project_id}/cloudservers/{server_id}/tags/action</p>
<p id="p11590124411208"><a name="p11590124411208"></a><a name="p11590124411208"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0167811964.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13524137192016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p195916442203"><a name="p195916442203"></a><a name="p195916442203"></a>CloudServerTag list(String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p105914441207"><a name="p105914441207"></a><a name="p105914441207"></a>GET /v1/{project_id}/cloudservers/{server_id}/tags</p>
<p id="p1591184413206"><a name="p1591184413206"></a><a name="p1591184413206"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0167811967.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row882912802010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p75912441205"><a name="p75912441205"></a><a name="p75912441205"></a>ProjectTag listProjectTags()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p759104442014"><a name="p759104442014"></a><a name="p759104442014"></a>GET /v1/{project_id}/cloudservers/tags</p>
<p id="p16591164417200"><a name="p16591164417200"></a><a name="p16591164417200"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0167811966.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于ECS v2 API的SDK接口如下,调用方式请参考示例代码。

<a name="table1329917498352"></a>
<table><thead align="left"><tr id="row20348849193511"><th class="cellrowborder" valign="top" width="19.788021197880212%" id="mcps1.1.4.1.1"><p id="p23481449123512"><a name="p23481449123512"></a><a name="p23481449123512"></a><strong id="b33481849143516"><a name="b33481849143516"></a><a name="b33481849143516"></a>Interface</strong></p>
</th>
<th class="cellrowborder" valign="top" width="33.87661233876612%" id="mcps1.1.4.1.2"><p id="p14348124918357"><a name="p14348124918357"></a><a name="p14348124918357"></a><strong id="b534864917351"><a name="b534864917351"></a><a name="b534864917351"></a>Method</strong></p>
</th>
<th class="cellrowborder" valign="top" width="46.33536646335366%" id="mcps1.1.4.1.3"><p id="p43481949163513"><a name="p43481949163513"></a><a name="p43481949163513"></a><strong id="b11348194933520"><a name="b11348194933520"></a><a name="b11348194933520"></a>API</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row1834818490359"><td class="cellrowborder" valign="top" width="19.788021197880212%" headers="mcps1.1.4.1.1 "><p id="p143494492358"><a name="p143494492358"></a><a name="p143494492358"></a>CloudServerV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="33.87661233876612%" headers="mcps1.1.4.1.2 "><p id="p33490493358"><a name="p33490493358"></a><a name="p33490493358"></a>AsyncJobEntity reinstallOS(OSReinstall osReinstall, String serverId)</p>
</td>
<td class="cellrowborder" valign="top" width="46.33536646335366%" headers="mcps1.1.4.1.3 "><p id="p12349124918355"><a name="p12349124918355"></a><a name="p12349124918355"></a>POST /v2/{project_id}/cloudservers/{server_id}/reinstallos</p>
<p id="p191445204381"><a name="p191445204381"></a><a name="p191445204381"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0067876349.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于ECS v1.1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table57097423155751"></a>
<table><thead align="left"><tr id="row47498298155751"><th class="cellrowborder" valign="top" width="18.85811418858114%" id="mcps1.1.4.1.1"><p id="p6718160155853"><a name="p6718160155853"></a><a name="p6718160155853"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="41.2058794120588%" id="mcps1.1.4.1.2"><p id="p3247442155853"><a name="p3247442155853"></a><a name="p3247442155853"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="39.93600639936006%" id="mcps1.1.4.1.3"><p id="p16563973155853"><a name="p16563973155853"></a><a name="p16563973155853"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row14919882155751"><td class="cellrowborder" rowspan="2" valign="top" width="18.85811418858114%" headers="mcps1.1.4.1.1 "><p id="p7838072155819"><a name="p7838072155819"></a><a name="p7838072155819"></a>CloudServerService</p>
</td>
<td class="cellrowborder" valign="top" width="41.2058794120588%" headers="mcps1.1.4.1.2 "><p id="p2255444415586"><a name="p2255444415586"></a><a name="p2255444415586"></a>AsyncRespEntity create(ServerCreate creation)</p>
</td>
<td class="cellrowborder" valign="top" width="39.93600639936006%" headers="mcps1.1.4.1.3 "><p id="p695731615586"><a name="p695731615586"></a><a name="p695731615586"></a>POST /v1.1/{project_id}/cloudservers</p>
<p id="p168392613816"><a name="p168392613816"></a><a name="p168392613816"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0093055772.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row66644417155751"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6710630143118"><a name="p6710630143118"></a><a name="p6710630143118"></a>AsyncRespEntity resize(ResizeServer resize,String serverId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4520846015586"><a name="p4520846015586"></a><a name="p4520846015586"></a>POST /v1.1/{project_id}/cloudservers/{server_id}/resize</p>
<p id="p1288563114389"><a name="p1288563114389"></a><a name="p1288563114389"></a><a href="https://support.huaweicloud.com/api-ecs/zh-cn_topic_0093298376.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

