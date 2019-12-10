# Go-ELB<a name="ZH-CN_TOPIC_0149280948"></a>

基于ELB v2 Go SDK的SDK接口如下，调用方式请参考示例代码。

<a name="table13788732172917"></a>
<table><thead align="left"><tr id="row04401185303"><th class="cellrowborder" valign="top" width="11.86%" id="mcps1.1.4.1.1"><p id="p3763296319273"><a name="p3763296319273"></a><a name="p3763296319273"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="47.15%" id="mcps1.1.4.1.2"><p id="p950753419273"><a name="p950753419273"></a><a name="p950753419273"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="40.99%" id="mcps1.1.4.1.3"><p id="p2230708619273"><a name="p2230708619273"></a><a name="p2230708619273"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row37533162911"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p1877335297"><a name="p1877335297"></a><a name="p1877335297"></a>policy</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p197103311292"><a name="p197103311292"></a><a name="p197103311292"></a>func List(sc *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p57153312294"><a name="p57153312294"></a><a name="p57153312294"></a>GET /v2.0/lbaas/l7policies</p>
<p id="p101883583620"><a name="p101883583620"></a><a name="p101883583620"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0136295315.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row187143372920"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1675332296"><a name="p1675332296"></a><a name="p1675332296"></a>func Get(sc *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p117193313297"><a name="p117193313297"></a><a name="p117193313297"></a>GET /v2.0/lbaas/l7policies/{policy_id}</p>
<p id="p1299120487363"><a name="p1299120487363"></a><a name="p1299120487363"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0136295316.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17203372917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1671433102912"><a name="p1671433102912"></a><a name="p1671433102912"></a>func Create(sc *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p20723372910"><a name="p20723372910"></a><a name="p20723372910"></a>POST /v2.0/lbaas/l7policies</p>
<p id="p497205016364"><a name="p497205016364"></a><a name="p497205016364"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0136295317.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5793372913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p47833132919"><a name="p47833132919"></a><a name="p47833132919"></a>func Update(sc *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3713362914"><a name="p3713362914"></a><a name="p3713362914"></a>PUT /v2.0/lbaas/l7policies/{policy_id}</p>
<p id="p3962652123611"><a name="p3962652123611"></a><a name="p3962652123611"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0136295318.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19763382910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16773319295"><a name="p16773319295"></a><a name="p16773319295"></a>func Delete(sc *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p57153342910"><a name="p57153342910"></a><a name="p57153342910"></a>DELETE /v2.0/lbaas/l7policies/{policy_id}</p>
<p id="p121617553368"><a name="p121617553368"></a><a name="p121617553368"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0136295319.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row67193352915"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p1471033152914"><a name="p1471033152914"></a><a name="p1471033152914"></a>certificate</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p077337295"><a name="p077337295"></a><a name="p077337295"></a>func List(c *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p878332296"><a name="p878332296"></a><a name="p878332296"></a>GET /v2.0/lbaas/certificates</p>
<p id="p17873125820368"><a name="p17873125820368"></a><a name="p17873125820368"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561582.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1271233102916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20712331293"><a name="p20712331293"></a><a name="p20712331293"></a>func Get(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p671533102915"><a name="p671533102915"></a><a name="p671533102915"></a>GET /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p146799223717"><a name="p146799223717"></a><a name="p146799223717"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561583.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row207173313297"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7710336291"><a name="p7710336291"></a><a name="p7710336291"></a>func Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p177933152916"><a name="p177933152916"></a><a name="p177933152916"></a>POST /v2.0/lbaas/certificates</p>
<p id="p111787593719"><a name="p111787593719"></a><a name="p111787593719"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561584.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1571433112910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6743312295"><a name="p6743312295"></a><a name="p6743312295"></a>func Update(c *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2717336298"><a name="p2717336298"></a><a name="p2717336298"></a>PUT /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p929218133710"><a name="p929218133710"></a><a name="p929218133710"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561585.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row971339290"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1671933202919"><a name="p1671933202919"></a><a name="p1671933202919"></a>func Delete(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1072338299"><a name="p1072338299"></a><a name="p1072338299"></a>DELETE /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p10622310183710"><a name="p10622310183710"></a><a name="p10622310183710"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561586.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9723314299"><td class="cellrowborder" rowspan="6" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p1371033112911"><a name="p1371033112911"></a><a name="p1371033112911"></a>loadbalancer</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p6733315296"><a name="p6733315296"></a><a name="p6733315296"></a>func List(c *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p957154194913"><a name="p957154194913"></a><a name="p957154194913"></a>GET /v2.0/lbaas/loadbalancers</p>
<p id="p154351147375"><a name="p154351147375"></a><a name="p154351147375"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561531.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row873333297"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p379331291"><a name="p379331291"></a><a name="p379331291"></a>func Get(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1671533152916"><a name="p1671533152916"></a><a name="p1671533152916"></a>GET /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p514121743710"><a name="p514121743710"></a><a name="p514121743710"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0141008271.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row87533162913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p177113332920"><a name="p177113332920"></a><a name="p177113332920"></a>func Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p127153352910"><a name="p127153352910"></a><a name="p127153352910"></a>POST /v2.0/lbaas/loadbalancers</p>
<p id="p122226192377"><a name="p122226192377"></a><a name="p122226192377"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561535.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row97133312913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20753332914"><a name="p20753332914"></a><a name="p20753332914"></a>func Update(c *gophercloud.ServiceClient, id string, opts UpdateOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p773337298"><a name="p773337298"></a><a name="p773337298"></a>PUT /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p104891821193717"><a name="p104891821193717"></a><a name="p104891821193717"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0141008274.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row157113382913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p47233172912"><a name="p47233172912"></a><a name="p47233172912"></a>func Delete(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1777336296"><a name="p1777336296"></a><a name="p1777336296"></a>DELETE /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p20528724143716"><a name="p20528724143716"></a><a name="p20528724143716"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0141008275.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1672033172912"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1471334296"><a name="p1471334296"></a><a name="p1471334296"></a>func GetStatuses(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p137233172919"><a name="p137233172919"></a><a name="p137233172919"></a>GET /v2.0/lbaas/loadbalancers/{loadbalancer_id}/statuses</p>
<p id="p98137261377"><a name="p98137261377"></a><a name="p98137261377"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0141008272.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row271133192910"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p127833162913"><a name="p127833162913"></a><a name="p127833162913"></a>listener</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p7720331295"><a name="p7720331295"></a><a name="p7720331295"></a>func List(c *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p127533192913"><a name="p127533192913"></a><a name="p127533192913"></a>GET /v2.0/lbaas/listeners</p>
<p id="p168122913372"><a name="p168122913372"></a><a name="p168122913372"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561541.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row37163312910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17203362914"><a name="p17203362914"></a><a name="p17203362914"></a>func Get(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p147123392910"><a name="p147123392910"></a><a name="p147123392910"></a>GET /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p1111313123711"><a name="p1111313123711"></a><a name="p1111313123711"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561540.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row07433112920"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p871233132912"><a name="p871233132912"></a><a name="p871233132912"></a>func Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p127833182920"><a name="p127833182920"></a><a name="p127833182920"></a>POST /v2.0/lbaas/listeners</p>
<p id="p1562093310370"><a name="p1562093310370"></a><a name="p1562093310370"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561483.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19743382910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p37183342917"><a name="p37183342917"></a><a name="p37183342917"></a>func Update(c *gophercloud.ServiceClient, id string, opts UpdateOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p77193310299"><a name="p77193310299"></a><a name="p77193310299"></a>PUT /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p07265359374"><a name="p07265359374"></a><a name="p07265359374"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561544.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10723392917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17723312920"><a name="p17723312920"></a><a name="p17723312920"></a>func Delete(c *gophercloud.ServiceClient, id string) (r DeleteResult)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6773319298"><a name="p6773319298"></a><a name="p6773319298"></a>DELETE /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p1578738133715"><a name="p1578738133715"></a><a name="p1578738133715"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561543.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1371533102913"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p18703312919"><a name="p18703312919"></a><a name="p18703312919"></a>pool</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p197203312299"><a name="p197203312299"></a><a name="p197203312299"></a>func List(c *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p771133122917"><a name="p771133122917"></a><a name="p771133122917"></a>GET /v2.0/lbaas/pools</p>
<p id="p4871194110377"><a name="p4871194110377"></a><a name="p4871194110377"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561547.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row571233152919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p981333112912"><a name="p981333112912"></a><a name="p981333112912"></a>func Get(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8873392914"><a name="p8873392914"></a><a name="p8873392914"></a>GET /v2.0/lbaas/pools/{pool_id}</p>
<p id="p590164483713"><a name="p590164483713"></a><a name="p590164483713"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561548.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16843320291"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18433102913"><a name="p18433102913"></a><a name="p18433102913"></a>func Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p188173382916"><a name="p188173382916"></a><a name="p188173382916"></a>POST /v2.0/lbaas/pools</p>
<p id="p2010644617374"><a name="p2010644617374"></a><a name="p2010644617374"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561549.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16873316293"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18853362911"><a name="p18853362911"></a><a name="p18853362911"></a>func Update(c *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p188153319292"><a name="p188153319292"></a><a name="p188153319292"></a>PUT /v2.0/lbaas/pools/{pool_id}</p>
<p id="p19252184814376"><a name="p19252184814376"></a><a name="p19252184814376"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561550.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row158173352911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3883311295"><a name="p3883311295"></a><a name="p3883311295"></a>func Delete(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13833342912"><a name="p13833342912"></a><a name="p13833342912"></a>DELETE /v2.0/lbaas/pools/{pool_id}</p>
<p id="p1242925083711"><a name="p1242925083711"></a><a name="p1242925083711"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561551.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row540655345510"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p586469175615"><a name="p586469175615"></a><a name="p586469175615"></a>Member</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p445763717565"><a name="p445763717565"></a><a name="p445763717565"></a>func ListMembers(c *gophercloud.ServiceClient, poolID string, opts ListMembersOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p164573375566"><a name="p164573375566"></a><a name="p164573375566"></a>GET /v2.0/lbaas/pools/{pool_id}/members</p>
<p id="p1841745314568"><a name="p1841745314568"></a><a name="p1841745314568"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561554.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row577113365610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p645812378561"><a name="p645812378561"></a><a name="p645812378561"></a>func GetMember(c *gophercloud.ServiceClient, poolID string, memberID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34586375567"><a name="p34586375567"></a><a name="p34586375567"></a>GET /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p10506109575"><a name="p10506109575"></a><a name="p10506109575"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561555.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row191776195610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174589371564"><a name="p174589371564"></a><a name="p174589371564"></a>func CreateMember(c *gophercloud.ServiceClient, poolID string, opts CreateMemberOpts)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p345863713560"><a name="p345863713560"></a><a name="p345863713560"></a>POST /v2.0/lbaas/pools/{pool_id}/members</p>
<p id="p19235231576"><a name="p19235231576"></a><a name="p19235231576"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561556.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0889658165517"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p64581937125611"><a name="p64581937125611"></a><a name="p64581937125611"></a>func UpdateMember(c *gophercloud.ServiceClient, poolID string, memberID string, opts UpdateMemberOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p145815375564"><a name="p145815375564"></a><a name="p145815375564"></a>PUT /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p478176205719"><a name="p478176205719"></a><a name="p478176205719"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561557.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1264825613559"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1345813712562"><a name="p1345813712562"></a><a name="p1345813712562"></a>func DeleteMember(c *gophercloud.ServiceClient, poolID string, memberID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p745815377560"><a name="p745815377560"></a><a name="p745815377560"></a>DELETE /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p192288165714"><a name="p192288165714"></a><a name="p192288165714"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561558.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19893392915"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p1484338295"><a name="p1484338295"></a><a name="p1484338295"></a>healthmonitor</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p148633132914"><a name="p148633132914"></a><a name="p148633132914"></a>func List(c *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p1687332296"><a name="p1687332296"></a><a name="p1687332296"></a>GET /v2.0/lbaas/healthmonitors</p>
<p id="p1255605213379"><a name="p1255605213379"></a><a name="p1255605213379"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561561.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1181333292"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p681533102911"><a name="p681533102911"></a><a name="p681533102911"></a>func Get(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18143352913"><a name="p18143352913"></a><a name="p18143352913"></a>GET /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p451517550378"><a name="p451517550378"></a><a name="p451517550378"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561562.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row188833172910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1781833172910"><a name="p1781833172910"></a><a name="p1781833172910"></a>func Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13812332292"><a name="p13812332292"></a><a name="p13812332292"></a>POST /v2.0/lbaas/healthmonitors</p>
<p id="p188771657173716"><a name="p188771657173716"></a><a name="p188771657173716"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561563.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6818331296"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10833392916"><a name="p10833392916"></a><a name="p10833392916"></a>func Update(c *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p58203310297"><a name="p58203310297"></a><a name="p58203310297"></a>PUT /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p1991385910379"><a name="p1991385910379"></a><a name="p1991385910379"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561564.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row148103315293"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p48143342914"><a name="p48143342914"></a><a name="p48143342914"></a>func Delete(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p159123315297"><a name="p159123315297"></a><a name="p159123315297"></a>DELETE /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p1127712163818"><a name="p1127712163818"></a><a name="p1127712163818"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561565.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11911333290"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p19953315297"><a name="p19953315297"></a><a name="p19953315297"></a>whitelist</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p1983392911"><a name="p1983392911"></a><a name="p1983392911"></a>func List(c *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p15943319294"><a name="p15943319294"></a><a name="p15943319294"></a>GET /v2.0/lbaas/whitelists</p>
<p id="p2435165193814"><a name="p2435165193814"></a><a name="p2435165193814"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0143878052.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row891533172916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1891333142916"><a name="p1891333142916"></a><a name="p1891333142916"></a>func Get(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p119033182910"><a name="p119033182910"></a><a name="p119033182910"></a>GET /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p68611878381"><a name="p68611878381"></a><a name="p68611878381"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0143878051.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row139203332916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p99163312291"><a name="p99163312291"></a><a name="p99163312291"></a>func Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p39173322914"><a name="p39173322914"></a><a name="p39173322914"></a>POST /v2.0/lbaas/whitelists</p>
<p id="p18635983814"><a name="p18635983814"></a><a name="p18635983814"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0143878053.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row499338297"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1691333192910"><a name="p1691333192910"></a><a name="p1691333192910"></a>func Update(c *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p179933102918"><a name="p179933102918"></a><a name="p179933102918"></a>PUT /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p15243101420383"><a name="p15243101420383"></a><a name="p15243101420383"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0143878054.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1691233102913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9943372915"><a name="p9943372915"></a><a name="p9943372915"></a>func Delete(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2923313293"><a name="p2923313293"></a><a name="p2923313293"></a>DELETE /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p1913563114386"><a name="p1913563114386"></a><a name="p1913563114386"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0143878055.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8933382911"><td class="cellrowborder" rowspan="5" valign="top" width="11.86%" headers="mcps1.1.4.1.1 "><p id="p19133392916"><a name="p19133392916"></a><a name="p19133392916"></a>rule</p>
</td>
<td class="cellrowborder" valign="top" width="47.15%" headers="mcps1.1.4.1.2 "><p id="p091339290"><a name="p091339290"></a><a name="p091339290"></a>func List(c *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p199332295"><a name="p199332295"></a><a name="p199332295"></a>GET /v2.0/lbaas/l7policies/{l7policy_id}/rules</p>
<p id="p7562123510384"><a name="p7562123510384"></a><a name="p7562123510384"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0116649234.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row993332295"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p179123315298"><a name="p179123315298"></a><a name="p179123315298"></a>func Get(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p49133122910"><a name="p49133122910"></a><a name="p49133122910"></a>GET /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p9365238193820"><a name="p9365238193820"></a><a name="p9365238193820"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0116649235.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row29113313293"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1963382911"><a name="p1963382911"></a><a name="p1963382911"></a>func Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p131069483810"><a name="p131069483810"></a><a name="p131069483810"></a>POST /v2.0/lbaas/l7policies/{l7policy_id}/rules</p>
<p id="p287918471387"><a name="p287918471387"></a><a name="p287918471387"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0116649236.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14919332295"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13943316291"><a name="p13943316291"></a><a name="p13943316291"></a>func Update(c *gophercloud.ServiceClient, id string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p121183312920"><a name="p121183312920"></a><a name="p121183312920"></a>PUT /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p13385150133810"><a name="p13385150133810"></a><a name="p13385150133810"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0116649237.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1311143318299"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13115336299"><a name="p13115336299"></a><a name="p13115336299"></a>func Delete(c *gophercloud.ServiceClient, id string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p125508548386"><a name="p125508548386"></a><a name="p125508548386"></a>DELETE /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p1895104043910"><a name="p1895104043910"></a><a name="p1895104043910"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0116649238.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

