# ELB<a name="sdk_11_0010"></a>

基于ELB v2.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table1523315114499"></a>
<table><thead align="left"><tr id="row2234951184918"><th class="cellrowborder" valign="top" width="28.162816281628167%" id="mcps1.1.4.1.1"><p id="p62949318403"><a name="p62949318403"></a><a name="p62949318403"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.62376237623762%" id="mcps1.1.4.1.2"><p id="p5098895718403"><a name="p5098895718403"></a><a name="p5098895718403"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.21342134213422%" id="mcps1.1.4.1.3"><p id="p3646482918403"><a name="p3646482918403"></a><a name="p3646482918403"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row023445114496"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p19234185184920"><a name="p19234185184920"></a><a name="p19234185184920"></a>LbRuleV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p116551649195013"><a name="p116551649195013"></a><a name="p116551649195013"></a>NeutronRules list(String l7policyId)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p9655164917504"><a name="p9655164917504"></a><a name="p9655164917504"></a>GET /v2.0/lbaas/l7policies/{l7policy_id}/rules</p>
<p id="p1326514383366"><a name="p1326514383366"></a><a name="p1326514383366"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row023465119499"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p265584916506"><a name="p265584916506"></a><a name="p265584916506"></a>NeutronRule get(String l7policyId, String ruleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17655749175010"><a name="p17655749175010"></a><a name="p17655749175010"></a>GET /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p184371457195413"><a name="p184371457195413"></a><a name="p184371457195413"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1234185116493"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p865510492502"><a name="p865510492502"></a><a name="p865510492502"></a>NeutronRule create(NeutronRule ruleModel, String l7policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1365524995017"><a name="p1365524995017"></a><a name="p1365524995017"></a>POST /v2.0/lbaas/l7policies/{l7policy_id}/rules</p>
<p id="p932020105510"><a name="p932020105510"></a><a name="p932020105510"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17234851114912"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4655204935017"><a name="p4655204935017"></a><a name="p4655204935017"></a>NeutronRule update(NeutronRuleUpdate updateModel, String l7policyId, String ruleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p465519490505"><a name="p465519490505"></a><a name="p465519490505"></a>PUT /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p16917102195520"><a name="p16917102195520"></a><a name="p16917102195520"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row523425110494"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1965534913509"><a name="p1965534913509"></a><a name="p1965534913509"></a>ActionResponse delete(String l7policyId, String ruleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1655104955016"><a name="p1655104955016"></a><a name="p1655104955016"></a>DELETE /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p66171255555"><a name="p66171255555"></a><a name="p66171255555"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row132358512493"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p947663314207"><a name="p947663314207"></a><a name="p947663314207"></a>LbWhitelistV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p1665564925015"><a name="p1665564925015"></a><a name="p1665564925015"></a>NeutronWhitelists list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p565519492506"><a name="p565519492506"></a><a name="p565519492506"></a>GET /v2.0/lbaas/whitelists</p>
<p id="p14902970558"><a name="p14902970558"></a><a name="p14902970558"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9235125124912"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p165510492509"><a name="p165510492509"></a><a name="p165510492509"></a>NeutronWhitelist get(String whitelistId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2655114915502"><a name="p2655114915502"></a><a name="p2655114915502"></a>GET /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p959912118553"><a name="p959912118553"></a><a name="p959912118553"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1723585154911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18655174919505"><a name="p18655174919505"></a><a name="p18655174919505"></a>NeutronWhitelist create(NeutronWhitelist model)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p26551649115020"><a name="p26551649115020"></a><a name="p26551649115020"></a>POST /v2.0/lbaas/whitelists</p>
<p id="p133114144555"><a name="p133114144555"></a><a name="p133114144555"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8235151194912"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2655249165018"><a name="p2655249165018"></a><a name="p2655249165018"></a>NeutronWhitelist update(NeutronWhitelist model,String whitelistId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p146551949185018"><a name="p146551949185018"></a><a name="p146551949185018"></a>PUT /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p1828181695518"><a name="p1828181695518"></a><a name="p1828181695518"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7235145119497"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p86551349115014"><a name="p86551349115014"></a><a name="p86551349115014"></a>ActionResponse delete(String whitelistId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5655949125018"><a name="p5655949125018"></a><a name="p5655949125018"></a>DELETE /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p429021819551"><a name="p429021819551"></a><a name="p429021819551"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17235115124911"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p1123545113495"><a name="p1123545113495"></a><a name="p1123545113495"></a>LbCertificateV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p10655164913503"><a name="p10655164913503"></a><a name="p10655164913503"></a>NeutronCertificates list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p065504916506"><a name="p065504916506"></a><a name="p065504916506"></a>GET /v2.0/lbaas/certificates</p>
<p id="p7254202085513"><a name="p7254202085513"></a><a name="p7254202085513"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1235155154918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p565524925011"><a name="p565524925011"></a><a name="p565524925011"></a>NeutronCertificate get(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p965544935015"><a name="p965544935015"></a><a name="p965544935015"></a>GET /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p112913233551"><a name="p112913233551"></a><a name="p112913233551"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2235145154912"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p206552049135013"><a name="p206552049135013"></a><a name="p206552049135013"></a>NeutronCertificate create(NeutronCertificate model)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15655134915019"><a name="p15655134915019"></a><a name="p15655134915019"></a>POST /v2.0/lbaas/certificates</p>
<p id="p132711258554"><a name="p132711258554"></a><a name="p132711258554"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4235125194917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1965564913509"><a name="p1965564913509"></a><a name="p1965564913509"></a>NeutronCertificate update(NeutronCertificateUpdate model, String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p365513493502"><a name="p365513493502"></a><a name="p365513493502"></a>PUT /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p6401027145517"><a name="p6401027145517"></a><a name="p6401027145517"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3235351154915"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1065511493502"><a name="p1065511493502"></a><a name="p1065511493502"></a>ActionResponse delete(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56553491504"><a name="p56553491504"></a><a name="p56553491504"></a>DELETE /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p12958129165514"><a name="p12958129165514"></a><a name="p12958129165514"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row92351516498"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p72219537224"><a name="p72219537224"></a><a name="p72219537224"></a>LbPolicyV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p565518499505"><a name="p565518499505"></a><a name="p565518499505"></a>NeutronL7Policies list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p18655194985011"><a name="p18655194985011"></a><a name="p18655194985011"></a>GET /v2.0/lbaas/l7policies</p>
<p id="p13920193115555"><a name="p13920193115555"></a><a name="p13920193115555"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9235551174911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p765511499505"><a name="p765511499505"></a><a name="p765511499505"></a>NeutronL7Policy get(String policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1365534913509"><a name="p1365534913509"></a><a name="p1365534913509"></a>GET /v2.0/lbaas/l7policies/{policy_id}</p>
<p id="p123429345555"><a name="p123429345555"></a><a name="p123429345555"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1023705174917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1165534915503"><a name="p1165534915503"></a><a name="p1165534915503"></a>NeutronL7Policy create(NeutronL7Policy model)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5655449165017"><a name="p5655449165017"></a><a name="p5655449165017"></a>POST /v2.0/lbaas/l7policies</p>
<p id="p1039653817554"><a name="p1039653817554"></a><a name="p1039653817554"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16237051194910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13655104913503"><a name="p13655104913503"></a><a name="p13655104913503"></a>NeutronL7Policy update(NeutronL7PolicyUpdate l7PolicyUpdate, String l7policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1365519492506"><a name="p1365519492506"></a><a name="p1365519492506"></a>PUT /v2.0/lbaas/l7policies/{policy_id}</p>
<p id="p919753865510"><a name="p919753865510"></a><a name="p919753865510"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row122379516490"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1655164918506"><a name="p1655164918506"></a><a name="p1655164918506"></a>ActionResponse delete(String l7policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15655204911506"><a name="p15655204911506"></a><a name="p15655204911506"></a>DELETE /v2.0/lbaas/l7policies/{policy_id}</p>
<p id="p1160384019558"><a name="p1160384019558"></a><a name="p1160384019558"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9237351144914"><td class="cellrowborder" rowspan="6" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p2972142211237"><a name="p2972142211237"></a><a name="p2972142211237"></a>LoadBalancerV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p86552498501"><a name="p86552498501"></a><a name="p86552498501"></a>List&lt;? extends LoadBalancerV2&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p6655174965013"><a name="p6655174965013"></a><a name="p6655174965013"></a>GET /v2.0/lbaas/loadbalancers</p>
<p id="p185401445145510"><a name="p185401445145510"></a><a name="p185401445145510"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row123719513496"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p46556499504"><a name="p46556499504"></a><a name="p46556499504"></a>LoadBalancerV2 get(String loadbalancerId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1765514918500"><a name="p1765514918500"></a><a name="p1765514918500"></a>GET /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p1762716518554"><a name="p1762716518554"></a><a name="p1762716518554"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0141008271.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row423795194914"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1065584925018"><a name="p1065584925018"></a><a name="p1065584925018"></a>LoadBalancerV2 create(LoadBalancerV2 loadbalancer)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46551749135018"><a name="p46551749135018"></a><a name="p46551749135018"></a>POST /v2.0/lbaas/loadbalancers</p>
<p id="p1127055710550"><a name="p1127055710550"></a><a name="p1127055710550"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561535.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62371751104917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26559493503"><a name="p26559493503"></a><a name="p26559493503"></a>LoadBalancerV2 update(String loadbalancerId, LoadBalancerV2Update loadbalancer)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p06551349135020"><a name="p06551349135020"></a><a name="p06551349135020"></a>PUT /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p19770190145612"><a name="p19770190145612"></a><a name="p19770190145612"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16237115124918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13655549105018"><a name="p13655549105018"></a><a name="p13655549105018"></a>ActionResponse delete(String loadbalancerId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p96551649105011"><a name="p96551649105011"></a><a name="p96551649105011"></a>DELETE /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p14151184165619"><a name="p14151184165619"></a><a name="p14151184165619"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row182371651184913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66552499502"><a name="p66552499502"></a><a name="p66552499502"></a>LoadBalancerV2StatusTree statusTree(String loadbalancerId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p465524919502"><a name="p465524919502"></a><a name="p465524919502"></a>GET /v2.0/lbaas/loadbalancers/{loadbalancer_id}/statuses</p>
<p id="p811516813563"><a name="p811516813563"></a><a name="p811516813563"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row132371751134911"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p16237155112494"><a name="p16237155112494"></a><a name="p16237155112494"></a>ListenerV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p16572494502"><a name="p16572494502"></a><a name="p16572494502"></a>List&lt;? extends ListenerV2&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p1065794919506"><a name="p1065794919506"></a><a name="p1065794919506"></a>GET /v2.0/lbaas/listeners</p>
<p id="p933721116568"><a name="p933721116568"></a><a name="p933721116568"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3237165184918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p265719498501"><a name="p265719498501"></a><a name="p265719498501"></a>ListenerV2 get(String listenerId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46571749125014"><a name="p46571749125014"></a><a name="p46571749125014"></a>GET /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p126031814125618"><a name="p126031814125618"></a><a name="p126031814125618"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10237125144918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p365774935012"><a name="p365774935012"></a><a name="p365774935012"></a>ListenerV2 create(ListenerV2 listener)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p465713492505"><a name="p465713492505"></a><a name="p465713492505"></a>POST /v2.0/lbaas/listeners</p>
<p id="p854541715618"><a name="p854541715618"></a><a name="p854541715618"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42371511496"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4657849175016"><a name="p4657849175016"></a><a name="p4657849175016"></a>ListenerV2 update(String listenerId, ListenerV2Update listener)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1565784935016"><a name="p1565784935016"></a><a name="p1565784935016"></a>PUT /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p13705112015568"><a name="p13705112015568"></a><a name="p13705112015568"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2023745114916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19657249195012"><a name="p19657249195012"></a><a name="p19657249195012"></a>ActionResponse delete(String listenerId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15657114985015"><a name="p15657114985015"></a><a name="p15657114985015"></a>DELETE /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p396302255614"><a name="p396302255614"></a><a name="p396302255614"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row723785119490"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p1623795144917"><a name="p1623795144917"></a><a name="p1623795144917"></a>LbPoolV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p26576499503"><a name="p26576499503"></a><a name="p26576499503"></a>List&lt;? extends LbPoolV2&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p20657114917508"><a name="p20657114917508"></a><a name="p20657114917508"></a>GET /v2.0/lbaas/pools</p>
<p id="p16938425105610"><a name="p16938425105610"></a><a name="p16938425105610"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561547.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row523715114491"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18657154995014"><a name="p18657154995014"></a><a name="p18657154995014"></a>LbPoolV2 get(String lbPoolId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p196571749125013"><a name="p196571749125013"></a><a name="p196571749125013"></a>GET /v2.0/lbaas/pools/{pool_id}</p>
<p id="p1182582885613"><a name="p1182582885613"></a><a name="p1182582885613"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9237205114490"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p96571349135011"><a name="p96571349135011"></a><a name="p96571349135011"></a>LbPoolV2 create(LbPoolV2 lbPool)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p116571449205019"><a name="p116571449205019"></a><a name="p116571449205019"></a>POST /v2.0/lbaas/pools</p>
<p id="p13515163217567"><a name="p13515163217567"></a><a name="p13515163217567"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row223755114917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p865713496505"><a name="p865713496505"></a><a name="p865713496505"></a>LbPoolV2 update(String lbPoolId, LbPoolV2Update lbPool)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p065734915019"><a name="p065734915019"></a><a name="p065734915019"></a>PUT /v2.0/lbaas/pools/{pool_id}</p>
<p id="p9829163410565"><a name="p9829163410565"></a><a name="p9829163410565"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20237551154914"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p106571749105018"><a name="p106571749105018"></a><a name="p106571749105018"></a>ActionResponse delete(String lbPoolId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9657749135019"><a name="p9657749135019"></a><a name="p9657749135019"></a>DELETE /v2.0/lbaas/pools/{pool_id}</p>
<p id="p1245413418566"><a name="p1245413418566"></a><a name="p1245413418566"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1623745174918"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p824903542420"><a name="p824903542420"></a><a name="p824903542420"></a>HealthMonitorV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p116574496507"><a name="p116574496507"></a><a name="p116574496507"></a>List&lt;? extends HealthMonitorV2&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p1765714917509"><a name="p1765714917509"></a><a name="p1765714917509"></a>GET /v2.0/lbaas/healthmonitors</p>
<p id="p66001836165618"><a name="p66001836165618"></a><a name="p66001836165618"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1237105111497"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2657154917508"><a name="p2657154917508"></a><a name="p2657154917508"></a>HealthMonitorV2 get(String healthMonitorId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8657164914503"><a name="p8657164914503"></a><a name="p8657164914503"></a>GET /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p1480144316561"><a name="p1480144316561"></a><a name="p1480144316561"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16237185119498"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6657134965014"><a name="p6657134965014"></a><a name="p6657134965014"></a>HealthMonitorV2 create(HealthMonitorV2 healthMonitor)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p665714912506"><a name="p665714912506"></a><a name="p665714912506"></a>POST /v2.0/lbaas/healthmonitors</p>
<p id="p05671445105614"><a name="p05671445105614"></a><a name="p05671445105614"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16237451204910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16571149135012"><a name="p16571149135012"></a><a name="p16571149135012"></a>HealthMonitorV2 update(String healthMonitorId, HealthMonitorV2Update healthMonitor)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p165724911509"><a name="p165724911509"></a><a name="p165724911509"></a>PUT /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p1246850195610"><a name="p1246850195610"></a><a name="p1246850195610"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row82371951164911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6657249155014"><a name="p6657249155014"></a><a name="p6657249155014"></a>ActionResponse delete(String healthMonitorId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14657184985015"><a name="p14657184985015"></a><a name="p14657184985015"></a>DELETE /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p2058685285619"><a name="p2058685285619"></a><a name="p2058685285619"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16237125118496"><td class="cellrowborder" rowspan="5" valign="top" width="28.162816281628167%" headers="mcps1.1.4.1.1 "><p id="p10938193702520"><a name="p10938193702520"></a><a name="p10938193702520"></a>LbPoolV2Service</p>
</td>
<td class="cellrowborder" valign="top" width="37.62376237623762%" headers="mcps1.1.4.1.2 "><p id="p265734911507"><a name="p265734911507"></a><a name="p265734911507"></a>List&lt;? extends MemberV2&gt; listMembers(String lbPoolId)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p1065734985013"><a name="p1065734985013"></a><a name="p1065734985013"></a>GET /v2.0/lbaas/pools/{pool_id}/members</p>
<p id="p107411554105618"><a name="p107411554105618"></a><a name="p107411554105618"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0237185124916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p106571449165015"><a name="p106571449165015"></a><a name="p106571449165015"></a>MemberV2 getMember(String lbPoolId, String memberId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p26571049195010"><a name="p26571049195010"></a><a name="p26571049195010"></a>GET /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p3928856185616"><a name="p3928856185616"></a><a name="p3928856185616"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13237195134911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16582049205019"><a name="p16582049205019"></a><a name="p16582049205019"></a>MemberV2 createMember(String lbPoolId, MemberV2 member)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15658449125010"><a name="p15658449125010"></a><a name="p15658449125010"></a>POST /v2.0/lbaas/pools/{pool_id}/members</p>
<p id="p139075593567"><a name="p139075593567"></a><a name="p139075593567"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row172371251114918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p76581949125012"><a name="p76581949125012"></a><a name="p76581949125012"></a>MemberV2 updateMember(String lbPoolId, String memberId, MemberV2Update member)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1165864985015"><a name="p1165864985015"></a><a name="p1165864985015"></a>PUT /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p172766211571"><a name="p172766211571"></a><a name="p172766211571"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7237175144919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13658154916506"><a name="p13658154916506"></a><a name="p13658154916506"></a>ActionResponse deleteMember(String lbPoolId, String memberId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13850143620433"><a name="p13850143620433"></a><a name="p13850143620433"></a>DELETE /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p8658104925013"><a name="p8658104925013"></a><a name="p8658104925013"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

