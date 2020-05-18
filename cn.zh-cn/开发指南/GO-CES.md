# CES<a name="sdk_13_0012"></a>

<a name="table88286590166"></a>
<table><thead align="left"><tr id="row582865915163"><th class="cellrowborder" valign="top" width="26.142614261426147%" id="mcps1.1.4.1.1"><p id="p14828105991617"><a name="p14828105991617"></a><a name="p14828105991617"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.883688368836886%" id="mcps1.1.4.1.2"><p id="p1782875941610"><a name="p1782875941610"></a><a name="p1782875941610"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.97369736973697%" id="mcps1.1.4.1.3"><p id="p58281959111614"><a name="p58281959111614"></a><a name="p58281959111614"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row11151923102211"><td class="cellrowborder" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p1699824771819"><a name="p1699824771819"></a><a name="p1699824771819"></a>MetricService</p>
</td>
<td class="cellrowborder" valign="top" width="36.883688368836886%" headers="mcps1.1.4.1.2 "><p id="p359214451910"><a name="p359214451910"></a><a name="p359214451910"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder) pagination.Pager</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p165929451918"><a name="p165929451918"></a><a name="p165929451918"></a>GET /V1.0/{project_id}/metrics</p>
<p id="p2029139131910"><a name="p2029139131910"></a><a name="p2029139131910"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0023.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8829185951616"><td class="cellrowborder" rowspan="5" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p11444132692812"><a name="p11444132692812"></a><a name="p11444132692812"></a>AlarmService</p>
</td>
<td class="cellrowborder" valign="top" width="36.883688368836886%" headers="mcps1.1.4.1.2 "><p id="p10850135715277"><a name="p10850135715277"></a><a name="p10850135715277"></a>List(client *gophercloud.ServiceClient, opts ListOpts) pagination.Pager</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p8850135722718"><a name="p8850135722718"></a><a name="p8850135722718"></a>GET /V1.0/{project_id}/alarms</p>
<p id="p18230103012919"><a name="p18230103012919"></a><a name="p18230103012919"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0027.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row88291359181611"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p785025752713"><a name="p785025752713"></a><a name="p785025752713"></a>Get(client *gophercloud.ServiceClient, alarmId string) (r GetResult)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16850105742714"><a name="p16850105742714"></a><a name="p16850105742714"></a>GET /V1.0/{project_id}/alarms/{alarm_id}</p>
<p id="p0992113942910"><a name="p0992113942910"></a><a name="p0992113942910"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0028.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18385153271915"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7850757112710"><a name="p7850757112710"></a><a name="p7850757112710"></a>Update(client *gophercloud.ServiceClient, alarmId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8850115722710"><a name="p8850115722710"></a><a name="p8850115722710"></a>PUT /V1.0/{project_id}/alarms/{alarm_id}/action</p>
<p id="p18478155172917"><a name="p18478155172917"></a><a name="p18478155172917"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0029.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8260103516192"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11851165713275"><a name="p11851165713275"></a><a name="p11851165713275"></a>Update(client *gophercloud.ServiceClient, alarmId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p985125752718"><a name="p985125752718"></a><a name="p985125752718"></a>PUT /V1.0/{project_id}/alarms/{alarm_id}/action</p>
<p id="p10807165862915"><a name="p10807165862915"></a><a name="p10807165862915"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0029.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row415714292194"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9851457192714"><a name="p9851457192714"></a><a name="p9851457192714"></a>Delete(client *gophercloud.ServiceClient, alarmId string) (r DeleteResult)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1585135711279"><a name="p1585135711279"></a><a name="p1585135711279"></a>DELETE /V1.0/{project_id}/alarms/{alarm_id}</p>
<p id="p715572113011"><a name="p715572113011"></a><a name="p715572113011"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0030.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17109926171913"><td class="cellrowborder" rowspan="2" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p925051732812"><a name="p925051732812"></a><a name="p925051732812"></a>MetricDataService</p>
</td>
<td class="cellrowborder" valign="top" width="36.883688368836886%" headers="mcps1.1.4.1.2 "><p id="p349344412287"><a name="p349344412287"></a><a name="p349344412287"></a>Get(client *gophercloud.ServiceClient, opts GetOpts)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p44931944132811"><a name="p44931944132811"></a><a name="p44931944132811"></a>GET /V1.0/{project_id}/metric-data</p>
<p id="p672719593010"><a name="p672719593010"></a><a name="p672719593010"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0033.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row382912593166"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p94931644182817"><a name="p94931644182817"></a><a name="p94931644182817"></a>AddMetricData(client *gophercloud.ServiceClient, opts AddMetricDataOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p114934440281"><a name="p114934440281"></a><a name="p114934440281"></a>POST /V1.0/{project_id}/metric-data</p>
<p id="p1539317943014"><a name="p1539317943014"></a><a name="p1539317943014"></a><a href="https://support.huaweicloud.com/api-ces/zh-cn_topic_0032831274.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row195415438615"><td class="cellrowborder" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p3909412162914"><a name="p3909412162914"></a><a name="p3909412162914"></a>QuotaService</p>
</td>
<td class="cellrowborder" valign="top" width="36.883688368836886%" headers="mcps1.1.4.1.2 "><p id="p1690910125299"><a name="p1690910125299"></a><a name="p1690910125299"></a>Get(client *gophercloud.ServiceClient) (r GetResult)</p>
</td>
<td class="cellrowborder" valign="top" width="36.97369736973697%" headers="mcps1.1.4.1.3 "><p id="p13910512182915"><a name="p13910512182915"></a><a name="p13910512182915"></a>GET /V1.0/{project_id}/quotas</p>
<p id="p15479111253019"><a name="p15479111253019"></a><a name="p15479111253019"></a><a href="https://support.huaweicloud.com/api-ces/ces_03_0037.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

