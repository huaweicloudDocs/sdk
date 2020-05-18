# ELB<a name="sdk_12_0010"></a>

基于ELB v2.0 API的SDK接口如下，调用方式举例：conn.network.loadbalancers\(\)

<a name="table436253365517"></a>
<table><thead align="left"><tr id="row1236213319551"><th class="cellrowborder" valign="top" width="25.356435643564357%" id="mcps1.1.4.1.1"><p id="p103770113344"><a name="p103770113344"></a><a name="p103770113344"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="42.4059405940594%" id="mcps1.1.4.1.2"><p id="p1837915110346"><a name="p1837915110346"></a><a name="p1837915110346"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.23762376237624%" id="mcps1.1.4.1.3"><p id="p17380311113412"><a name="p17380311113412"></a><a name="p17380311113412"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row103639336554"><td class="cellrowborder" rowspan="6" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p936343315512"><a name="p936343315512"></a><a name="p936343315512"></a>Loadbalancer Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p10363183375517"><a name="p10363183375517"></a><a name="p10363183375517"></a>loadbalancers(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p4363143355510"><a name="p4363143355510"></a><a name="p4363143355510"></a>GET /v2.0/lbaas/loadbalancers</p>
<p id="p1326514383366"><a name="p1326514383366"></a><a name="p1326514383366"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19363153318557"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p936353385512"><a name="p936353385512"></a><a name="p936353385512"></a>get_loadbalancer(self, lb)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17363153315520"><a name="p17363153315520"></a><a name="p17363153315520"></a>GET /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p175401284586"><a name="p175401284586"></a><a name="p175401284586"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0141008271.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row113637336553"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1236383318556"><a name="p1236383318556"></a><a name="p1236383318556"></a>create_loadbalancer(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p43631533185516"><a name="p43631533185516"></a><a name="p43631533185516"></a>POST /v2.0/lbaas/loadbalancers</p>
<p id="p11673183115586"><a name="p11673183115586"></a><a name="p11673183115586"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561535.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row203634339552"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p153633331552"><a name="p153633331552"></a><a name="p153633331552"></a>update_loadbalancer(self, lb, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13363183310551"><a name="p13363183310551"></a><a name="p13363183310551"></a>PUT /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p14570163285818"><a name="p14570163285818"></a><a name="p14570163285818"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row136313338559"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4363933105517"><a name="p4363933105517"></a><a name="p4363933105517"></a>delete_loadbalancer(self, lb, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1936353319559"><a name="p1936353319559"></a><a name="p1936353319559"></a>DELETE /v2.0/lbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p177264346589"><a name="p177264346589"></a><a name="p177264346589"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11363103313553"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13631633125513"><a name="p13631633125513"></a><a name="p13631633125513"></a>get_loadbalancer_status_stree(self, lb)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p173631433185511"><a name="p173631433185511"></a><a name="p173631433185511"></a>GET /v2.0/lbaas/loadbalancers/{loadbalancer_id}/statuses</p>
<p id="p11436153805818"><a name="p11436153805818"></a><a name="p11436153805818"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_fz_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12363133395513"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p16363113345518"><a name="p16363113345518"></a><a name="p16363113345518"></a>Listener Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p133631833135517"><a name="p133631833135517"></a><a name="p133631833135517"></a>listeners(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p18363103311552"><a name="p18363103311552"></a><a name="p18363103311552"></a>GET /v2.0/lbaas/listeners</p>
<p id="p13341154475820"><a name="p13341154475820"></a><a name="p13341154475820"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row123631233165514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19363143375511"><a name="p19363143375511"></a><a name="p19363143375511"></a>get_listener(self, lsn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p836393310555"><a name="p836393310555"></a><a name="p836393310555"></a>GET /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p15356104725819"><a name="p15356104725819"></a><a name="p15356104725819"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row93631833155510"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1436513385519"><a name="p1436513385519"></a><a name="p1436513385519"></a>create_listener(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4365123395517"><a name="p4365123395517"></a><a name="p4365123395517"></a>POST /v2.0/lbaas/listeners</p>
<p id="p206795095813"><a name="p206795095813"></a><a name="p206795095813"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row173655335555"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18365183313558"><a name="p18365183313558"></a><a name="p18365183313558"></a>update_listener(self, lsn, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1936553395515"><a name="p1936553395515"></a><a name="p1936553395515"></a>PUT /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p153541452135819"><a name="p153541452135819"></a><a name="p153541452135819"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1336563313555"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p736543317555"><a name="p736543317555"></a><a name="p736543317555"></a>delete_listener(self, lsn, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p136543313550"><a name="p136543313550"></a><a name="p136543313550"></a>DELETE /v2.0/lbaas/listeners/{listener_id}</p>
<p id="p33641456155814"><a name="p33641456155814"></a><a name="p33641456155814"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jt_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1236513335510"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p16365193314551"><a name="p16365193314551"></a><a name="p16365193314551"></a>Pool Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p9365833105510"><a name="p9365833105510"></a><a name="p9365833105510"></a>pools(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p1365033205511"><a name="p1365033205511"></a><a name="p1365033205511"></a>GET /v2.0/lbaas/pools</p>
<p id="p14927446590"><a name="p14927446590"></a><a name="p14927446590"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561547.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row836513365520"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p173652335553"><a name="p173652335553"></a><a name="p173652335553"></a>get_pool(self, pol)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1236516332553"><a name="p1236516332553"></a><a name="p1236516332553"></a>GET /v2.0/lbaas/pools/{pool_id}</p>
<p id="p153321273590"><a name="p153321273590"></a><a name="p153321273590"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row163657333558"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p636511339551"><a name="p636511339551"></a><a name="p636511339551"></a>create_pool(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1136523375518"><a name="p1136523375518"></a><a name="p1136523375518"></a>POST /v2.0/lbaas/pools</p>
<p id="p5464179195915"><a name="p5464179195915"></a><a name="p5464179195915"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row436514336558"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1536563311552"><a name="p1536563311552"></a><a name="p1536563311552"></a>update_pool(self, pol, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p136583313550"><a name="p136583313550"></a><a name="p136583313550"></a>PUT /v2.0/lbaas/pools/{pool_id}</p>
<p id="p2079312115920"><a name="p2079312115920"></a><a name="p2079312115920"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row636593325514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12365193312555"><a name="p12365193312555"></a><a name="p12365193312555"></a>delete_pool(self, pol, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1736503335513"><a name="p1736503335513"></a><a name="p1736503335513"></a>DELETE /v2.0/lbaas/pools/{pool_id}</p>
<p id="p9907314205914"><a name="p9907314205914"></a><a name="p9907314205914"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hz_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row83651233155515"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p2036553315510"><a name="p2036553315510"></a><a name="p2036553315510"></a>Member Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p3365433185519"><a name="p3365433185519"></a><a name="p3365433185519"></a>members(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p0365333185513"><a name="p0365333185513"></a><a name="p0365333185513"></a>GET /v2.0/lbaas/pools/{pool_id}/members</p>
<p id="p01511917145918"><a name="p01511917145918"></a><a name="p01511917145918"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row836516336552"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p183651333555"><a name="p183651333555"></a><a name="p183651333555"></a>get_member(self, mem, pool = None)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4365113385510"><a name="p4365113385510"></a><a name="p4365113385510"></a>GET /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p015042125914"><a name="p015042125914"></a><a name="p015042125914"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9365173365518"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1536553315553"><a name="p1536553315553"></a><a name="p1536553315553"></a>create_member(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6365133195513"><a name="p6365133195513"></a><a name="p6365133195513"></a>POST /v2.0/lbaas/pools/{pool_id}/members</p>
<p id="p1198019236597"><a name="p1198019236597"></a><a name="p1198019236597"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18365143315516"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4365233195510"><a name="p4365233195510"></a><a name="p4365233195510"></a>update_member(self, mem, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p636543385517"><a name="p636543385517"></a><a name="p636543385517"></a>PUT /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p20487329165913"><a name="p20487329165913"></a><a name="p20487329165913"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1836517338552"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p636553365514"><a name="p636553365514"></a><a name="p636553365514"></a>delete_member(self, mem, pool = None, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9365163316558"><a name="p9365163316558"></a><a name="p9365163316558"></a>DELETE /v2.0/lbaas/pools/{pool_id}/members/{member_id}</p>
<p id="p154029292594"><a name="p154029292594"></a><a name="p154029292594"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_hd_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20365113313554"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p63651733145513"><a name="p63651733145513"></a><a name="p63651733145513"></a>Healthmonitor Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p113659331555"><a name="p113659331555"></a><a name="p113659331555"></a>healthmonitors(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p17365103311550"><a name="p17365103311550"></a><a name="p17365103311550"></a>GET /v2.0/lbaas/healthmonitors</p>
<p id="p17891431135910"><a name="p17891431135910"></a><a name="p17891431135910"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16365203317558"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p113651033125511"><a name="p113651033125511"></a><a name="p113651033125511"></a>get_healthmonitor(self, hlth)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1436503310556"><a name="p1436503310556"></a><a name="p1436503310556"></a>GET /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p62741934105915"><a name="p62741934105915"></a><a name="p62741934105915"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13365183319550"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p133651433165519"><a name="p133651433165519"></a><a name="p133651433165519"></a>create_healthmonitor(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p336503314550"><a name="p336503314550"></a><a name="p336503314550"></a>POST /v2.0/lbaas/healthmonitors</p>
<p id="p18497173615915"><a name="p18497173615915"></a><a name="p18497173615915"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17365633195512"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1836519339559"><a name="p1836519339559"></a><a name="p1836519339559"></a>update_healthmonitor(self, hlth, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2365103315556"><a name="p2365103315556"></a><a name="p2365103315556"></a>PUT /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p126422383594"><a name="p126422383594"></a><a name="p126422383594"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row113651733145516"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18365733145512"><a name="p18365733145512"></a><a name="p18365733145512"></a>delete_healthmonitor(self, hlth, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p43651533115511"><a name="p43651533115511"></a><a name="p43651533115511"></a>DELETE /v2.0/lbaas/healthmonitors/{healthmonitor_id}</p>
<p id="p4610184519593"><a name="p4610184519593"></a><a name="p4610184519593"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_jk_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6365933135520"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p3365433165520"><a name="p3365433165520"></a><a name="p3365433165520"></a>Policy Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p836523345516"><a name="p836523345516"></a><a name="p836523345516"></a>poliycies(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p10366633125511"><a name="p10366633125511"></a><a name="p10366633125511"></a>GET /v2.0/lbaas/l7policies</p>
<p id="p9382350145920"><a name="p9382350145920"></a><a name="p9382350145920"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11152172310112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6152162321113"><a name="p6152162321113"></a><a name="p6152162321113"></a>get_policy(self, plc)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1915220238116"><a name="p1915220238116"></a><a name="p1915220238116"></a>GET /v2.0/lbaas/l7policies/{l7policy_id}</p>
<p id="p210125335912"><a name="p210125335912"></a><a name="p210125335912"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5366533105518"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6366153385510"><a name="p6366153385510"></a><a name="p6366153385510"></a>create_policy(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1936611338559"><a name="p1936611338559"></a><a name="p1936611338559"></a>POST /v2.0/lbaas/l7policies</p>
<p id="p8418555185918"><a name="p8418555185918"></a><a name="p8418555185918"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5956143851113"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2095653801114"><a name="p2095653801114"></a><a name="p2095653801114"></a>update_policy(self, plc, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1195618388111"><a name="p1195618388111"></a><a name="p1195618388111"></a>PUT /v2.0/lbaas/l7policies/{l7policy_id}</p>
<p id="p1598435835910"><a name="p1598435835910"></a><a name="p1598435835910"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1827514714114"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17275184721111"><a name="p17275184721111"></a><a name="p17275184721111"></a>delete_policy(self, plc, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11275124711115"><a name="p11275124711115"></a><a name="p11275124711115"></a>DELETE /v2.0/lbaas/l7policies/{l7policy_id}</p>
<p id="p9283111014"><a name="p9283111014"></a><a name="p9283111014"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zf_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5898951111118"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p13898551151114"><a name="p13898551151114"></a><a name="p13898551151114"></a>Rule Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p1689895113114"><a name="p1689895113114"></a><a name="p1689895113114"></a>rules(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p118981251101119"><a name="p118981251101119"></a><a name="p118981251101119"></a>GET /v2.0/lbaas/l7policies/{l7policy_id}/rules</p>
<p id="p11835718018"><a name="p11835718018"></a><a name="p11835718018"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row478405331120"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p87841353151112"><a name="p87841353151112"></a><a name="p87841353151112"></a>get_rule(self, rul, policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2784135314119"><a name="p2784135314119"></a><a name="p2784135314119"></a>GET /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p13862592005"><a name="p13862592005"></a><a name="p13862592005"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5268185815117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2268175810118"><a name="p2268175810118"></a><a name="p2268175810118"></a>create_rule(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p62681158181115"><a name="p62681158181115"></a><a name="p62681158181115"></a>POST /v2.0/lbaas/l7policies/{l7policy_id}/rules</p>
<p id="p1291071413014"><a name="p1291071413014"></a><a name="p1291071413014"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4351154914116"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p133511849131113"><a name="p133511849131113"></a><a name="p133511849131113"></a>update_rule(self, rul, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p935184916117"><a name="p935184916117"></a><a name="p935184916117"></a>PUT /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p2809183018"><a name="p2809183018"></a><a name="p2809183018"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1246565617118"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10465656191119"><a name="p10465656191119"></a><a name="p10465656191119"></a>delete_rule(self, rul, policy, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p04654566111"><a name="p04654566111"></a><a name="p04654566111"></a>DELETE /v2.0/lbaas/l7policies/{l7policy_id}/rules/{l7rule_id}</p>
<p id="p1132582017018"><a name="p1132582017018"></a><a name="p1132582017018"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zg_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1453024181119"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p65301441101111"><a name="p65301441101111"></a><a name="p65301441101111"></a>Whitelist Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p1530154161113"><a name="p1530154161113"></a><a name="p1530154161113"></a>whitelists(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p192216818332"><a name="p192216818332"></a><a name="p192216818332"></a>GET /v2.0/lbaas/whitelists</p>
<p id="p154561022903"><a name="p154561022903"></a><a name="p154561022903"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7567133419118"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p125671834161116"><a name="p125671834161116"></a><a name="p125671834161116"></a>get_whitelist(self, wl)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p118612260333"><a name="p118612260333"></a><a name="p118612260333"></a>GET /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p10816162419012"><a name="p10816162419012"></a><a name="p10816162419012"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16884114401117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1488514451115"><a name="p1488514451115"></a><a name="p1488514451115"></a>create_whitelist(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5885134418116"><a name="p5885134418116"></a><a name="p5885134418116"></a>POST /v2.0/lbaas/whitelists</p>
<p id="p17395526604"><a name="p17395526604"></a><a name="p17395526604"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0743123620116"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7743936171111"><a name="p7743936171111"></a><a name="p7743936171111"></a>update_whitelist(self, wl, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p97431036131117"><a name="p97431036131117"></a><a name="p97431036131117"></a>PUT /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p108203288016"><a name="p108203288016"></a><a name="p108203288016"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row03721632171117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p937253201111"><a name="p937253201111"></a><a name="p937253201111"></a>delete_whitelist(self, wl, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7372153261113"><a name="p7372153261113"></a><a name="p7372153261113"></a>DELETE /v2.0/lbaas/whitelists/{whitelist_id}</p>
<p id="p87019311207"><a name="p87019311207"></a><a name="p87019311207"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_bm_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1125622881116"><td class="cellrowborder" rowspan="5" valign="top" width="25.356435643564357%" headers="mcps1.1.4.1.1 "><p id="p9256182851119"><a name="p9256182851119"></a><a name="p9256182851119"></a>Certificate Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.4059405940594%" headers="mcps1.1.4.1.2 "><p id="p10257122841113"><a name="p10257122841113"></a><a name="p10257122841113"></a>certificates(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="32.23762376237624%" headers="mcps1.1.4.1.3 "><p id="p125722811117"><a name="p125722811117"></a><a name="p125722811117"></a>GET /v2.0/lbaas/certificates</p>
<p id="p313973310016"><a name="p313973310016"></a><a name="p313973310016"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1395132515119"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p295162512116"><a name="p295162512116"></a><a name="p295162512116"></a>get_certificate(self, cf)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1595172591112"><a name="p1595172591112"></a><a name="p1595172591112"></a>GET /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p17492136509"><a name="p17492136509"></a><a name="p17492136509"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7695152018119"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p176951920171115"><a name="p176951920171115"></a><a name="p176951920171115"></a>create_certificate(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p469517209111"><a name="p469517209111"></a><a name="p469517209111"></a>POST /v2.0/lbaas/certificates</p>
<p id="p15886163814016"><a name="p15886163814016"></a><a name="p15886163814016"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7733191713114"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p373791781118"><a name="p373791781118"></a><a name="p373791781118"></a>update_certificate(self, cf, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10737181711115"><a name="p10737181711115"></a><a name="p10737181711115"></a>PUT /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p36356421105"><a name="p36356421105"></a><a name="p36356421105"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10366833105519"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p936616331554"><a name="p936616331554"></a><a name="p936616331554"></a>delete_certificate(self, cf, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1736623319551"><a name="p1736623319551"></a><a name="p1736623319551"></a>DELETE /v2.0/lbaas/certificates/{certificate_id}</p>
<p id="p386451013"><a name="p386451013"></a><a name="p386451013"></a><a href="https://support.huaweicloud.com/api-elb/elb_zq_zs_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于ELB v1.0 API的SDK接口如下，调用方法举例：conn.load\_balancer.create\_load\_balancer\(\)

<a name="table22377509173456"></a>
<table><thead align="left"><tr id="row31280221173456"><th class="cellrowborder" valign="top" width="25.4%" id="mcps1.1.4.1.1"><p id="p50669961173456"><a name="p50669961173456"></a><a name="p50669961173456"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="42.3%" id="mcps1.1.4.1.2"><p id="p10626137173456"><a name="p10626137173456"></a><a name="p10626137173456"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.300000000000004%" id="mcps1.1.4.1.3"><p id="p55410741173456"><a name="p55410741173456"></a><a name="p55410741173456"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row59085062173456"><td class="cellrowborder" rowspan="5" valign="top" width="25.4%" headers="mcps1.1.4.1.1 "><p id="p56380605175740"><a name="p56380605175740"></a><a name="p56380605175740"></a>LoadBalancer Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.3%" headers="mcps1.1.4.1.2 "><p id="p62963525193239"><a name="p62963525193239"></a><a name="p62963525193239"></a>create_load_balancer(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.300000000000004%" headers="mcps1.1.4.1.3 "><p id="p5703528192631"><a name="p5703528192631"></a><a name="p5703528192631"></a>POST /v1.0/{project_id}/elbaas/loadbalancers</p>
<p id="p6752649301"><a name="p6752649301"></a><a name="p6752649301"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_fz_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39651246175759"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12087402193258"><a name="p12087402193258"></a><a name="p12087402193258"></a>get_load_balancer(self, load_balancer)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3741660192646"><a name="p3741660192646"></a><a name="p3741660192646"></a>GET /v1.0/{project_id}/elbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p12205165219015"><a name="p12205165219015"></a><a name="p12205165219015"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_fz_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3700652418010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33444519193313"><a name="p33444519193313"></a><a name="p33444519193313"></a>load_balancers(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3703625192653"><a name="p3703625192653"></a><a name="p3703625192653"></a>GET /v1.0/{project_id}/elbaas/loadbalancers</p>
<p id="p1799911544014"><a name="p1799911544014"></a><a name="p1799911544014"></a><a href="https://support.huaweicloud.com/api-elb/zh-cn_topic_0096561504.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5729000518014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p35593450193327"><a name="p35593450193327"></a><a name="p35593450193327"></a>update_load_balancer(self, load_balancer, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1036102119270"><a name="p1036102119270"></a><a name="p1036102119270"></a>PUT /v1.0/{project_id}/elbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p49083578017"><a name="p49083578017"></a><a name="p49083578017"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_fz_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3088701173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10560758193341"><a name="p10560758193341"></a><a name="p10560758193341"></a>delete_load_balancer(self, load_balancer, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6317238619276"><a name="p6317238619276"></a><a name="p6317238619276"></a>DELETE /v1.0/{project_id}/elbaas/loadbalancers/{loadbalancer_id}</p>
<p id="p18122160418"><a name="p18122160418"></a><a name="p18122160418"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_fz_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row35075245173456"><td class="cellrowborder" rowspan="5" valign="top" width="25.4%" headers="mcps1.1.4.1.1 "><p id="p1083981918115"><a name="p1083981918115"></a><a name="p1083981918115"></a>Listener Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.3%" headers="mcps1.1.4.1.2 "><p id="p6978898193355"><a name="p6978898193355"></a><a name="p6978898193355"></a>create_listener(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.300000000000004%" headers="mcps1.1.4.1.3 "><p id="p46324010192714"><a name="p46324010192714"></a><a name="p46324010192714"></a>POST /v1.0/{project_id}/elbaas/listeners</p>
<p id="p45812213113"><a name="p45812213113"></a><a name="p45812213113"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jt_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42544890173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3273425819348"><a name="p3273425819348"></a><a name="p3273425819348"></a>get_listener(self, listener)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18852868192724"><a name="p18852868192724"></a><a name="p18852868192724"></a>GET /v1.0/{project_id}/elbaas/listeners/{listener_id}</p>
<p id="p139182041711"><a name="p139182041711"></a><a name="p139182041711"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jt_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48955445173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p25225651193429"><a name="p25225651193429"></a><a name="p25225651193429"></a>listeners(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p66628182192732"><a name="p66628182192732"></a><a name="p66628182192732"></a>GET /v1.0/{project_id}/elbaas/listeners?loadbalancer_id={loadbalancer_id}</p>
<p id="p21868314"><a name="p21868314"></a><a name="p21868314"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jt_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1022652718232"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11510383193441"><a name="p11510383193441"></a><a name="p11510383193441"></a>update_listener(self, listener, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6496982192742"><a name="p6496982192742"></a><a name="p6496982192742"></a>PUT /v1.0/{project_id}/elbaas/listeners/{listener_id}</p>
<p id="p1058416132016"><a name="p1058416132016"></a><a name="p1058416132016"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jt_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6515000718253"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p57368937193452"><a name="p57368937193452"></a><a name="p57368937193452"></a>delete_listener(self, listener, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p37329587192749"><a name="p37329587192749"></a><a name="p37329587192749"></a>DELETE /v1.0/{project_id}/elbaas/listeners/{listener_id}</p>
<p id="p793116813"><a name="p793116813"></a><a name="p793116813"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jt_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row144860671831"><td class="cellrowborder" rowspan="4" valign="top" width="25.4%" headers="mcps1.1.4.1.1 "><p id="p4664355718332"><a name="p4664355718332"></a><a name="p4664355718332"></a>HealthCheck Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.3%" headers="mcps1.1.4.1.2 "><p id="p3927811219357"><a name="p3927811219357"></a><a name="p3927811219357"></a>create_health_check(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.300000000000004%" headers="mcps1.1.4.1.3 "><p id="p41895993192841"><a name="p41895993192841"></a><a name="p41895993192841"></a>POST /v1.0/{project_id}/elbaas/healthcheck</p>
<p id="p1254520213117"><a name="p1254520213117"></a><a name="p1254520213117"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jk_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row638903301846"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p44145262193523"><a name="p44145262193523"></a><a name="p44145262193523"></a>get_health_check(self, health_check)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46856802192855"><a name="p46856802192855"></a><a name="p46856802192855"></a>GET /v1.0/{project_id}/elbaas/healthcheck/{healthcheck_id}</p>
<p id="p14852112320112"><a name="p14852112320112"></a><a name="p14852112320112"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jk_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3166059718354"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42770293193540"><a name="p42770293193540"></a><a name="p42770293193540"></a>update_health_check(self, health_check, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5335645919297"><a name="p5335645919297"></a><a name="p5335645919297"></a>PUT /v1.0/{project_id}/elbaas/healthcheck/{healthcheck_id}</p>
<p id="p1394232317117"><a name="p1394232317117"></a><a name="p1394232317117"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jk_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row241237431849"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p22743539193553"><a name="p22743539193553"></a><a name="p22743539193553"></a>delete_health_check(self, health_check, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33686504192917"><a name="p33686504192917"></a><a name="p33686504192917"></a>DELETE /v1.0/{project_id}/elbaas/healthcheck/{healthcheck_id}</p>
<p id="p177012261515"><a name="p177012261515"></a><a name="p177012261515"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_jk_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row296146318412"><td class="cellrowborder" rowspan="3" valign="top" width="25.4%" headers="mcps1.1.4.1.1 "><p id="p2907311018454"><a name="p2907311018454"></a><a name="p2907311018454"></a>Member Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.3%" headers="mcps1.1.4.1.2 "><p id="p1175745319369"><a name="p1175745319369"></a><a name="p1175745319369"></a>add_members_to_listener(self, listener, members)</p>
</td>
<td class="cellrowborder" valign="top" width="32.300000000000004%" headers="mcps1.1.4.1.3 "><p id="p894630192927"><a name="p894630192927"></a><a name="p894630192927"></a>POST /v1.0/{project_id}/elbaas/listeners/{listener_id}/members</p>
<p id="p494915281611"><a name="p494915281611"></a><a name="p494915281611"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_hd_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row732382918414"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12520113193621"><a name="p12520113193621"></a><a name="p12520113193621"></a>remove_members_of_listener(self, listener, members)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7360492192938"><a name="p7360492192938"></a><a name="p7360492192938"></a>POST /v1.0/{project_id}/elbaas/listeners/{listener_id}/members/action</p>
<p id="p1719611315114"><a name="p1719611315114"></a><a name="p1719611315114"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_hd_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row394420831843"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p57465850193633"><a name="p57465850193633"></a><a name="p57465850193633"></a>listener_members(self, listener, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56352080192945"><a name="p56352080192945"></a><a name="p56352080192945"></a>GET /v1.0/{project_id}/elbaas/listeners/{listener_id}/members</p>
<p id="p179200331417"><a name="p179200331417"></a><a name="p179200331417"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_hd_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5837080718515"><td class="cellrowborder" rowspan="4" valign="top" width="25.4%" headers="mcps1.1.4.1.1 "><p id="p686197818545"><a name="p686197818545"></a><a name="p686197818545"></a>Certificate Operations</p>
</td>
<td class="cellrowborder" valign="top" width="42.3%" headers="mcps1.1.4.1.2 "><p id="p7353157193656"><a name="p7353157193656"></a><a name="p7353157193656"></a>create_certificate(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="32.300000000000004%" headers="mcps1.1.4.1.3 "><p id="p59232235192953"><a name="p59232235192953"></a><a name="p59232235192953"></a>POST /v1.0/{project_id}/elbaas/certificate</p>
<p id="p914183610117"><a name="p914183610117"></a><a name="p914183610117"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_zs_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row50024167192450"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p954153193720"><a name="p954153193720"></a><a name="p954153193720"></a>certificates(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3561527319303"><a name="p3561527319303"></a><a name="p3561527319303"></a>GET /v1.0/{project_id}/elbaas/certificate</p>
<p id="p122598388119"><a name="p122598388119"></a><a name="p122598388119"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_zs_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row45785296192443"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p45890432193731"><a name="p45890432193731"></a><a name="p45890432193731"></a>update_certificate(self, certificate, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1945658319309"><a name="p1945658319309"></a><a name="p1945658319309"></a>PUT /v1.0/{project_id}/elbaas/certificate/{certificate_id}</p>
<p id="p1255241211"><a name="p1255241211"></a><a name="p1255241211"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_zs_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row50832686193016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p39411762193742"><a name="p39411762193742"></a><a name="p39411762193742"></a>delete_certificate(self, certificate, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46277853193025"><a name="p46277853193025"></a><a name="p46277853193025"></a>DELETE /v1.0/{project_id}/elbaas/certificate/{certificate_id}</p>
<p id="p205381432017"><a name="p205381432017"></a><a name="p205381432017"></a><a href="https://support.huaweicloud.com/api-elb/elb_jd_zs_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

