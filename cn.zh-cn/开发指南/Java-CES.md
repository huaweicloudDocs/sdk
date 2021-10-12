# CES<a name="sdk_11_0008"></a>

基于CES V1.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table15713293295"></a>
<table><thead align="left"><tr id="row3717292295"><th class="cellrowborder" valign="top" width="28.060000000000002%" id="mcps1.1.4.1.1"><p id="p07929162911"><a name="p07929162911"></a><a name="p07929162911"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.61%" id="mcps1.1.4.1.2"><p id="p13742915291"><a name="p13742915291"></a><a name="p13742915291"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.33%" id="mcps1.1.4.1.3"><p id="p107102912297"><a name="p107102912297"></a><a name="p107102912297"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row074295299"><td class="cellrowborder" valign="top" width="28.060000000000002%" headers="mcps1.1.4.1.1 "><p id="p6534172323017"><a name="p6534172323017"></a><a name="p6534172323017"></a><span>MetricService</span></p>
</td>
<td class="cellrowborder" valign="top" width="38.61%" headers="mcps1.1.4.1.2 "><p id="p453413238305"><a name="p453413238305"></a><a name="p453413238305"></a><span>List</span><span>&lt;</span><span>? extends Metric</span><span>&gt;</span><span> getList(MetricFilterOptions options);</span></p>
</td>
<td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.3 "><p id="p753442316301"><a name="p753442316301"></a><a name="p753442316301"></a><span>GET /V1.0/{project_id}/metrics</span></p>
</td>
</tr>
<tr id="row15474153952914"><td class="cellrowborder" rowspan="5" valign="top" width="28.060000000000002%" headers="mcps1.1.4.1.1 "><p id="p674118342302"><a name="p674118342302"></a><a name="p674118342302"></a><span>AlarmService</span></p>
</td>
<td class="cellrowborder" valign="top" width="38.61%" headers="mcps1.1.4.1.2 "><p id="p197412349301"><a name="p197412349301"></a><a name="p197412349301"></a><span>List</span><span>&lt;</span><span>? extends Alarm</span><span>&gt;</span><span> list(AlarmFilterOptions options);</span></p>
</td>
<td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.3 "><p id="p5741163423015"><a name="p5741163423015"></a><a name="p5741163423015"></a><span>GET /V1.0/{project_id}/alarms</span></p>
</td>
</tr>
<tr id="row419411548291"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15741133453014"><a name="p15741133453014"></a><a name="p15741133453014"></a><span>List</span><span>&lt;</span><span>? extends Alarm</span><span>&gt;</span><span> get(String alarmId);</span></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p27411634133012"><a name="p27411634133012"></a><a name="p27411634133012"></a><span>GET /V1.0/{project_id}/alarms/{alarm_id}</span></p>
</td>
</tr>
<tr id="row15422154311294"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p137411734143015"><a name="p137411734143015"></a><a name="p137411734143015"></a><span>ActionResponse startAlarm(String alarmId)</span></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9741203473010"><a name="p9741203473010"></a><a name="p9741203473010"></a><span>PUT /V1.0/{project_id}/alarms/{alarm_id}/action</span></p>
</td>
</tr>
<tr id="row156951958182918"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p146306563313"><a name="p146306563313"></a><a name="p146306563313"></a>ActionResponse stopAlarm(String alarmId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8630115612310"><a name="p8630115612310"></a><a name="p8630115612310"></a>PUT /V1.0/{project_id}/alarms/{alarm_id}/action</p>
</td>
</tr>
<tr id="row16139694306"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p167411342304"><a name="p167411342304"></a><a name="p167411342304"></a><span>ActionResponse deleteAlarm(String alarmId);</span></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p07411343307"><a name="p07411343307"></a><a name="p07411343307"></a><span>DELETE /V1.0/{project_id}/alarms/{alarm_id}</span></p>
</td>
</tr>
<tr id="row1813812912304"><td class="cellrowborder" rowspan="2" valign="top" width="28.060000000000002%" headers="mcps1.1.4.1.1 "><p id="p4102109143015"><a name="p4102109143015"></a><a name="p4102109143015"></a><span>MetricDataService</span></p>
</td>
<td class="cellrowborder" valign="top" width="38.61%" headers="mcps1.1.4.1.2 "><p id="p558512715326"><a name="p558512715326"></a><a name="p558512715326"></a><span>MetricAggregation get(String namespace, String metric_name, Date from, Date to, Period period, Filter filter, String[] dimValues);</span></p>
</td>
<td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.3 "><p id="p158511719329"><a name="p158511719329"></a><a name="p158511719329"></a><span>GET /V1.0/{project_id}/metric-data</span></p>
</td>
</tr>
<tr id="row91382923015"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1958512713323"><a name="p1958512713323"></a><a name="p1958512713323"></a><span>ActionResponse add(List</span><span>&lt;</span><span>? extends MetricData</span><span>&gt;</span><span> metrics);</span></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p758567163216"><a name="p758567163216"></a><a name="p758567163216"></a><span>POST /V1.0/{project_id}/metric-data</span></p>
</td>
</tr>
<tr id="row111378913010"><td class="cellrowborder" valign="top" width="28.060000000000002%" headers="mcps1.1.4.1.1 "><p id="p131028973020"><a name="p131028973020"></a><a name="p131028973020"></a><span>QuotaService</span></p>
</td>
<td class="cellrowborder" valign="top" width="38.61%" headers="mcps1.1.4.1.2 "><p id="p9585137193220"><a name="p9585137193220"></a><a name="p9585137193220"></a><span>CloudEyeQuota get();</span></p>
</td>
<td class="cellrowborder" valign="top" width="33.33%" headers="mcps1.1.4.1.3 "><p id="p1958611713320"><a name="p1958611713320"></a><a name="p1958611713320"></a><span>GET /V1.0/{project_id}/quotas</span></p>
</td>
</tr>
</tbody>
</table>

