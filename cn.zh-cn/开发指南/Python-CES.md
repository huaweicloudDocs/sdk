# Python-CES<a name="ZH-CN_TOPIC_0072142411"></a>

基于CES v1.0 API的SDK接口如下，调用方式举例：conn.cloud\_eye.metrics\(\)

<a name="table19848473182148"></a>
<table><thead align="left"><tr id="row54179233182148"><th class="cellrowborder" valign="top" width="16.35%" id="mcps1.1.4.1.1"><p id="p26441759182148"><a name="p26441759182148"></a><a name="p26441759182148"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="49.38%" id="mcps1.1.4.1.2"><p id="p61407774182148"><a name="p61407774182148"></a><a name="p61407774182148"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.27%" id="mcps1.1.4.1.3"><p id="p7973830182148"><a name="p7973830182148"></a><a name="p7973830182148"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row41900478182148"><td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.1.4.1.1 "><p id="p38495534182148"><a name="p38495534182148"></a><a name="p38495534182148"></a>Metric Operations</p>
</td>
<td class="cellrowborder" valign="top" width="49.38%" headers="mcps1.1.4.1.2 "><p id="p29700906193852"><a name="p29700906193852"></a><a name="p29700906193852"></a>metrics(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.27%" headers="mcps1.1.4.1.3 "><p id="p49515129182148"><a name="p49515129182148"></a><a name="p49515129182148"></a>GET /V1.0/{project_id}/metrics</p>
</td>
</tr>
<tr id="row42982981182148"><td class="cellrowborder" rowspan="4" valign="top" width="16.35%" headers="mcps1.1.4.1.1 "><p id="p59069416182148"><a name="p59069416182148"></a><a name="p59069416182148"></a>Alarm Operations</p>
</td>
<td class="cellrowborder" valign="top" width="49.38%" headers="mcps1.1.4.1.2 "><p id="p44822543182148"><a name="p44822543182148"></a><a name="p44822543182148"></a>alarms(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.27%" headers="mcps1.1.4.1.3 "><p id="p6747403182148"><a name="p6747403182148"></a><a name="p6747403182148"></a>GET /V1.0/{project_id}/alarms</p>
</td>
</tr>
<tr id="row60726627182148"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19909784182148"><a name="p19909784182148"></a><a name="p19909784182148"></a>get_alarm(self, alarm)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2079830182148"><a name="p2079830182148"></a><a name="p2079830182148"></a>GET /V1.0/{project_id}/alarms/{alarm_id}</p>
</td>
</tr>
<tr id="row18718471182148"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1505904419394"><a name="p1505904419394"></a><a name="p1505904419394"></a>enable_alarm(self, alarm)</p>
<p id="p1182308819394"><a name="p1182308819394"></a><a name="p1182308819394"></a>disable_alarm(self, alarm)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p24037329182148"><a name="p24037329182148"></a><a name="p24037329182148"></a>PUT /V1.0/{project_id}/alarms/{alarm_id}/action</p>
</td>
</tr>
<tr id="row15009372182148"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7799623182148"><a name="p7799623182148"></a><a name="p7799623182148"></a>delete_alarm(self, alarm, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p27789702182148"><a name="p27789702182148"></a><a name="p27789702182148"></a>DELETE /V1.0/{project_id}/alarms/{alarm_id}</p>
</td>
</tr>
<tr id="row48780729182148"><td class="cellrowborder" rowspan="2" valign="top" width="16.35%" headers="mcps1.1.4.1.1 "><p id="p58924946182148"><a name="p58924946182148"></a><a name="p58924946182148"></a>Metric Data Operations</p>
</td>
<td class="cellrowborder" valign="top" width="49.38%" headers="mcps1.1.4.1.2 "><p id="p6612686182148"><a name="p6612686182148"></a><a name="p6612686182148"></a>metric_aggregations(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.27%" headers="mcps1.1.4.1.3 "><p id="p65865583182148"><a name="p65865583182148"></a><a name="p65865583182148"></a>GET /V1.0/{project_id}/metric-data</p>
</td>
</tr>
<tr id="row55919343182148"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33172954182148"><a name="p33172954182148"></a><a name="p33172954182148"></a>add_metric_data(self, data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2654766182148"><a name="p2654766182148"></a><a name="p2654766182148"></a>POST /V1.0/{project_id}/metric-data</p>
</td>
</tr>
<tr id="row23892894182148"><td class="cellrowborder" valign="top" width="16.35%" headers="mcps1.1.4.1.1 "><p id="p56276257182148"><a name="p56276257182148"></a><a name="p56276257182148"></a>Quota Operations</p>
</td>
<td class="cellrowborder" valign="top" width="49.38%" headers="mcps1.1.4.1.2 "><p id="p5848210193914"><a name="p5848210193914"></a><a name="p5848210193914"></a>quotas(self)</p>
</td>
<td class="cellrowborder" valign="top" width="34.27%" headers="mcps1.1.4.1.3 "><p id="p48918886182148"><a name="p48918886182148"></a><a name="p48918886182148"></a>GET /V1.0/{project_id}/quotas</p>
</td>
</tr>
</tbody>
</table>

