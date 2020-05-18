# AntiDDoS<a name="sdk_12_0016"></a>

基于AntiDDoS v1 API的SDK接口如下，调用方式举例：conn.anti\_ddos.query\_config\_list\(\)

<a name="table138844"></a>
<table><thead align="left"><tr id="row35094160"><th class="cellrowborder" valign="top" width="27.312731273127312%" id="mcps1.1.4.1.1"><p id="p67010553152228"><a name="p67010553152228"></a><a name="p67010553152228"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.713571357135706%" id="mcps1.1.4.1.2"><p id="p2273746"><a name="p2273746"></a><a name="p2273746"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.97369736973697%" id="mcps1.1.4.1.3"><p id="p49955752"><a name="p49955752"></a><a name="p49955752"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row19884118"><td class="cellrowborder" valign="top" width="27.312731273127312%" headers="mcps1.1.4.1.1 "><p id="p59145746152228"><a name="p59145746152228"></a><a name="p59145746152228"></a>QueryConfigList Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.713571357135706%" headers="mcps1.1.4.1.2 "><p id="p5666365175647"><a name="p5666365175647"></a><a name="p5666365175647"></a>query_config_list()</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p56322424175647"><a name="p56322424175647"></a><a name="p56322424175647"></a>GET /v1/{project_id}/antiddos/query_config_list</p>
<p id="p42381418105518"><a name="p42381418105518"></a><a name="p42381418105518"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0017.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row66441544"><td class="cellrowborder" rowspan="7" valign="top" width="27.312731273127312%" headers="mcps1.1.4.1.1 "><p id="p103271332101812"><a name="p103271332101812"></a><a name="p103271332101812"></a>EIP Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.713571357135706%" headers="mcps1.1.4.1.2 "><p id="p32472947175647"><a name="p32472947175647"></a><a name="p32472947175647"></a>get_floating_ip(floating_ip)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p13063063175647"><a name="p13063063175647"></a><a name="p13063063175647"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}</p>
<p id="p330764911562"><a name="p330764911562"></a><a name="p330764911562"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62271039"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60623138175647"><a name="p60623138175647"></a><a name="p60623138175647"></a>update_floating_ip(floating_ip, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11527154175647"><a name="p11527154175647"></a><a name="p11527154175647"></a>PUT /v1/{project_id}/antiddos/{floating_ip_id}</p>
<p id="p1872820314575"><a name="p1872820314575"></a><a name="p1872820314575"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0021.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row40084941"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14687449175647"><a name="p14687449175647"></a><a name="p14687449175647"></a>query_task_status(task_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p36841436175647"><a name="p36841436175647"></a><a name="p36841436175647"></a>GET /v1/{project_id}/query_task_status</p>
<p id="p416463719570"><a name="p416463719570"></a><a name="p416463719570"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0022.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46070087"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13861404175647"><a name="p13861404175647"></a><a name="p13861404175647"></a>floating_ips(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38634566175647"><a name="p38634566175647"></a><a name="p38634566175647"></a>GET /v1/{project_id}/antiddos</p>
<p id="p153632488589"><a name="p153632488589"></a><a name="p153632488589"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0023.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row588929"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p45985100175647"><a name="p45985100175647"></a><a name="p45985100175647"></a>get_eip_status(floating_ip_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33805629175647"><a name="p33805629175647"></a><a name="p33805629175647"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}/status</p>
<p id="p12511191310596"><a name="p12511191310596"></a><a name="p12511191310596"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0024.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13286310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15350830175647"><a name="p15350830175647"></a><a name="p15350830175647"></a>list_eip_daily(floating_ip_id, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p35457703175647"><a name="p35457703175647"></a><a name="p35457703175647"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}/daily</p>
<p id="p598153915582"><a name="p598153915582"></a><a name="p598153915582"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0025.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row40742509"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11753190175647"><a name="p11753190175647"></a><a name="p11753190175647"></a>list_eip_log(floating_ip_id, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12484305175647"><a name="p12484305175647"></a><a name="p12484305175647"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}/logs</p>
<p id="p87467117016"><a name="p87467117016"></a><a name="p87467117016"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0026.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18774354"><td class="cellrowborder" valign="top" width="27.312731273127312%" headers="mcps1.1.4.1.1 "><p id="p16454360152228"><a name="p16454360152228"></a><a name="p16454360152228"></a>EIPWeekly Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.713571357135706%" headers="mcps1.1.4.1.2 "><p id="p41362105175647"><a name="p41362105175647"></a><a name="p41362105175647"></a>get_eip_weekly(period_start_date)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p61996176175647"><a name="p61996176175647"></a><a name="p61996176175647"></a>GET /v1/{project_id}/antiddos/weekly</p>
<p id="p3815624403"><a name="p3815624403"></a><a name="p3815624403"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0027.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row35520730"><td class="cellrowborder" valign="top" width="27.312731273127312%" headers="mcps1.1.4.1.1 "><p id="p57734794152228"><a name="p57734794152228"></a><a name="p57734794152228"></a>AlertConfig Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.713571357135706%" headers="mcps1.1.4.1.2 "><p id="p30947380175647"><a name="p30947380175647"></a><a name="p30947380175647"></a>get_alert_config()</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p23709826175647"><a name="p23709826175647"></a><a name="p23709826175647"></a>GET /v1/{project_id}/warnalert/alertconfig/query</p>
<p id="p9693251614"><a name="p9693251614"></a><a name="p9693251614"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0029.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

