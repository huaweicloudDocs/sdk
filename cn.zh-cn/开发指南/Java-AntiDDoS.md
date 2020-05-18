# AntiDDoS<a name="sdk_11_0016"></a>

基于Antiddos v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table138844"></a>
<table><thead align="left"><tr id="row35094160"><th class="cellrowborder" valign="top" width="28.799999999999997%" id="mcps1.1.4.1.1"><p id="p33735697152039"><a name="p33735697152039"></a><a name="p33735697152039"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.49%" id="mcps1.1.4.1.2"><p id="p2273746"><a name="p2273746"></a><a name="p2273746"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.709999999999994%" id="mcps1.1.4.1.3"><p id="p49955752"><a name="p49955752"></a><a name="p49955752"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row19884118"><td class="cellrowborder" rowspan="9" valign="top" width="28.799999999999997%" headers="mcps1.1.4.1.1 "><p id="p48236959152039"><a name="p48236959152039"></a><a name="p48236959152039"></a>AntiDDoSService</p>
</td>
<td class="cellrowborder" valign="top" width="35.49%" headers="mcps1.1.4.1.2 "><p id="p1872881752419"><a name="p1872881752419"></a><a name="p1872881752419"></a>AntiDDoSConfig listConfigs()</p>
</td>
<td class="cellrowborder" valign="top" width="35.709999999999994%" headers="mcps1.1.4.1.3 "><p id="p18018956175536"><a name="p18018956175536"></a><a name="p18018956175536"></a>GET /v1/{project_id}/antiddos/query_config_list</p>
<p id="p1436135114710"><a name="p1436135114710"></a><a name="p1436135114710"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0017.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row66441544"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p319294312412"><a name="p319294312412"></a><a name="p319294312412"></a>AntiDDoS get(String floatingIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p66796549175536"><a name="p66796549175536"></a><a name="p66796549175536"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}</p>
<p id="p1174517146487"><a name="p1174517146487"></a><a name="p1174517146487"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62271039"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p40757867175536"><a name="p40757867175536"></a><a name="p40757867175536"></a>Task update(AntiDDoS entity, String floatingIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13052970175536"><a name="p13052970175536"></a><a name="p13052970175536"></a>PUT /v1/{project_id}/antiddos/{floating_ip_id}</p>
<p id="p11628179487"><a name="p11628179487"></a><a name="p11628179487"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0021.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row40084941"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p195725589248"><a name="p195725589248"></a><a name="p195725589248"></a>Task getTask(String taskId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19575195175536"><a name="p19575195175536"></a><a name="p19575195175536"></a>GET /v1/{project_id}/query_task_status</p>
<p id="p83591198484"><a name="p83591198484"></a><a name="p83591198484"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0022.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46070087"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18611580258"><a name="p18611580258"></a><a name="p18611580258"></a>AntiDDoSStatus listStatus()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12665956175536"><a name="p12665956175536"></a><a name="p12665956175536"></a>GET /v1/{project_id}/antiddos</p>
<p id="p56472216486"><a name="p56472216486"></a><a name="p56472216486"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0023.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row588929"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p39568229175536"><a name="p39568229175536"></a><a name="p39568229175536"></a>AntiDDoSStatusDetail getStatus(String floatingIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p50909979175536"><a name="p50909979175536"></a><a name="p50909979175536"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}/status</p>
<p id="p57628254489"><a name="p57628254489"></a><a name="p57628254489"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0024.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13286310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2172991175536"><a name="p2172991175536"></a><a name="p2172991175536"></a>List&lt;? extends AntiDDoSDailyData&gt; dailyReport(String floatingIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p41794587175536"><a name="p41794587175536"></a><a name="p41794587175536"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}/daily</p>
<p id="p04285287487"><a name="p04285287487"></a><a name="p04285287487"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0025.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row40742509"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p697633202713"><a name="p697633202713"></a><a name="p697633202713"></a>List&lt;? extends AntiDDoSLog&gt; listLogs(String floatingIpId, AntiDDoSLogListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p121034175536"><a name="p121034175536"></a><a name="p121034175536"></a>GET /v1/{project_id}/antiddos/{floating_ip_id}/logs</p>
<p id="p147782305480"><a name="p147782305480"></a><a name="p147782305480"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0026.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18774354"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17675443192711"><a name="p17675443192711"></a><a name="p17675443192711"></a>AntiDDoSWeeklyData weeklyReport(Date periodStartDate)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p33450710175536"><a name="p33450710175536"></a><a name="p33450710175536"></a>GET /v1/{project_id}/antiddos/weekly</p>
<p id="p18828163214489"><a name="p18828163214489"></a><a name="p18828163214489"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0027.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row35520730"><td class="cellrowborder" valign="top" width="28.799999999999997%" headers="mcps1.1.4.1.1 "><p id="p066311581591"><a name="p066311581591"></a><a name="p066311581591"></a>AntiDDoSWarnService</p>
</td>
<td class="cellrowborder" valign="top" width="35.49%" headers="mcps1.1.4.1.2 "><p id="p18929448192716"><a name="p18929448192716"></a><a name="p18929448192716"></a>AntiDDoSWarn query()</p>
</td>
<td class="cellrowborder" valign="top" width="35.709999999999994%" headers="mcps1.1.4.1.3 "><p id="p15809395175536"><a name="p15809395175536"></a><a name="p15809395175536"></a>GET /v2/{project_id}/ warnalert/alertconfig/query</p>
<p id="p117861735124812"><a name="p117861735124812"></a><a name="p117861735124812"></a><a href="https://support.huaweicloud.com/api-antiddos/antiddos_02_0029.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

