# RDS<a name="sdk_11_0028"></a>

基于RDS v3 API的SDK接口如下，调用方式请参考示例代码。

<a name="table8484916201010"></a>
<table><thead align="left"><tr id="row157021316171019"><th class="cellrowborder" valign="top" width="25.722572257225725%" id="mcps1.1.4.1.1"><p id="p157026162107"><a name="p157026162107"></a><a name="p157026162107"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.43394339433943%" id="mcps1.1.4.1.2"><p id="p370211618107"><a name="p370211618107"></a><a name="p370211618107"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.84348434843484%" id="mcps1.1.4.1.3"><p id="p1670231681013"><a name="p1670231681013"></a><a name="p1670231681013"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row970281614107"><td class="cellrowborder" rowspan="11" valign="top" width="25.722572257225725%" headers="mcps1.1.4.1.1 "><p id="p16397124734818"><a name="p16397124734818"></a><a name="p16397124734818"></a>InstanceManageService</p>
</td>
<td class="cellrowborder" valign="top" width="39.43394339433943%" headers="mcps1.1.4.1.2 "><p id="p15157154134616"><a name="p15157154134616"></a><a name="p15157154134616"></a>CreateInstanceResponse create(CreateInstanceRequest createRequest)</p>
</td>
<td class="cellrowborder" valign="top" width="34.84348434843484%" headers="mcps1.1.4.1.3 "><p id="p131581149463"><a name="p131581149463"></a><a name="p131581149463"></a>POST /v3/{project_id}/instances</p>
<p id="p856681014714"><a name="p856681014714"></a><a name="p856681014714"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11702121671016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1158184184619"><a name="p1158184184619"></a><a name="p1158184184619"></a>ListInstanceResponse list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p612619476710"><a name="p612619476710"></a><a name="p612619476710"></a>GET</p>
<p id="p81586474610"><a name="p81586474610"></a><a name="p81586474610"></a>/v3/{project_id}/instances</p>
<p id="p133391815778"><a name="p133391815778"></a><a name="p133391815778"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row370341612101"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p161585464613"><a name="p161585464613"></a><a name="p161585464613"></a>ListInstanceResponse list(Map&lt;String, String&gt; queryParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1242710521878"><a name="p1242710521878"></a><a name="p1242710521878"></a>GET</p>
<p id="p10158144134613"><a name="p10158144134613"></a><a name="p10158144134613"></a>/v3/{project_id}/instances</p>
<p id="p1226213200710"><a name="p1226213200710"></a><a name="p1226213200710"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19703716191017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41583494615"><a name="p41583494615"></a><a name="p41583494615"></a>ActionResponse delete(String instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p161587494613"><a name="p161587494613"></a><a name="p161587494613"></a>DELETE /v3/{project_id}/instances/{instanceId}</p>
<p id="p88711252714"><a name="p88711252714"></a><a name="p88711252714"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1070320164101"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1315810414611"><a name="p1315810414611"></a><a name="p1315810414611"></a>InstanceCommonResponse restart(RestartInstanceRequest request, String instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p355035515711"><a name="p355035515711"></a><a name="p355035515711"></a>PUT</p>
<p id="p1715854124619"><a name="p1715854124619"></a><a name="p1715854124619"></a>/v3/{project_id}/instances/{instanceId}/action</p>
<p id="p07745291178"><a name="p07745291178"></a><a name="p07745291178"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row797185710453"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5594470614"><a name="p5594470614"></a><a name="p5594470614"></a>InstanceCommonResponse</p>
<p id="p132756458612"><a name="p132756458612"></a><a name="p132756458612"></a>singleToHa(SingleToHaRdsRequest request, String instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p141515578711"><a name="p141515578711"></a><a name="p141515578711"></a>GET</p>
<p id="p1415817411468"><a name="p1415817411468"></a><a name="p1415817411468"></a>/v3/{project_id}/instances/{instanceId}/action</p>
<p id="p1580819341179"><a name="p1580819341179"></a><a name="p1580819341179"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1755210544455"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7414721196"><a name="p7414721196"></a><a name="p7414721196"></a>InstanceCommonResponse resizeFlavor(ResizeFlavorRequest request, String instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p153880983"><a name="p153880983"></a><a name="p153880983"></a>POST</p>
<p id="p1158184184613"><a name="p1158184184613"></a><a name="p1158184184613"></a>/v3/{project_id}/instances/{instanceId}/action</p>
<p id="p13505183913719"><a name="p13505183913719"></a><a name="p13505183913719"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0101.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15551051174514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p146469351107"><a name="p146469351107"></a><a name="p146469351107"></a>InstanceCommonResponse enlargeVolume(EnlargeVolumeRequest request, String instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8157821989"><a name="p8157821989"></a><a name="p8157821989"></a>POST</p>
<p id="p71585484612"><a name="p71585484612"></a><a name="p71585484612"></a>/v3/{project_id}/instances/{instanceId}/action</p>
<p id="p1220411451272"><a name="p1220411451272"></a><a name="p1220411451272"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0102.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10507184820457"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p515817434615"><a name="p515817434615"></a><a name="p515817434615"></a>ErrorLogResponse listErrorLog(Map&lt;String, String&gt; queryParams, String instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p359612211440"><a name="p359612211440"></a><a name="p359612211440"></a>GET</p>
<p id="p515920413463"><a name="p515920413463"></a><a name="p515920413463"></a>/v3/{project_id}/instances/{instanceId} /errorlog</p>
<p id="p193082500712"><a name="p193082500712"></a><a name="p193082500712"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1025318820156"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p625468141515"><a name="p625468141515"></a><a name="p625468141515"></a>SlowLogListResponse listSlowLog(Map&lt;String, String&gt; queryParams, String instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p51046196419"><a name="p51046196419"></a><a name="p51046196419"></a>GET</p>
<p id="p17254118141519"><a name="p17254118141519"></a><a name="p17254118141519"></a>/v3/{project_id}/instances/{instanceId}/slowlog</p>
<p id="p1719745610254"><a name="p1719745610254"></a><a name="p1719745610254"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row884391861515"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12843161821518"><a name="p12843161821518"></a><a name="p12843161821518"></a>FlavorList listFlavors(Map&lt;String, String&gt; filteringParams, String engineName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p168884158420"><a name="p168884158420"></a><a name="p168884158420"></a>GET</p>
<p id="p1064204419196"><a name="p1064204419196"></a><a name="p1064204419196"></a>/v3/{project_id}/flavors/{engineName}</p>
<p id="p477115862511"><a name="p477115862511"></a><a name="p477115862511"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row95867571544"><td class="cellrowborder" rowspan="3" valign="top" width="25.722572257225725%" headers="mcps1.1.4.1.1 "><p id="p323851555"><a name="p323851555"></a><a name="p323851555"></a>BackupsAndRestoreService</p>
</td>
<td class="cellrowborder" valign="top" width="39.43394339433943%" headers="mcps1.1.4.1.2 "><p id="p12586175755420"><a name="p12586175755420"></a><a name="p12586175755420"></a>ManualBackupResponse create(ManualBackupRequest request)</p>
</td>
<td class="cellrowborder" valign="top" width="34.84348434843484%" headers="mcps1.1.4.1.3 "><p id="p15586757165417"><a name="p15586757165417"></a><a name="p15586757165417"></a>POST</p>
<p id="p1095013212018"><a name="p1095013212018"></a><a name="p1095013212018"></a>/v3/{project_id}/backups</p>
<p id="p2870631922"><a name="p2870631922"></a><a name="p2870631922"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1476413015520"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p976411005517"><a name="p976411005517"></a><a name="p976411005517"></a>BackupsResponse list(String instanceId, Map&lt;String, String&gt; filterParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p177551350439"><a name="p177551350439"></a><a name="p177551350439"></a>GET</p>
<p id="p157551250834"><a name="p157551250834"></a><a name="p157551250834"></a>/v3/{project_id}/backups</p>
<p id="p1175595014311"><a name="p1175595014311"></a><a name="p1175595014311"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9779353195413"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19780353125418"><a name="p19780353125418"></a><a name="p19780353125418"></a>ActionResponse delete(String backupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p208641151131"><a name="p208641151131"></a><a name="p208641151131"></a>DELETE</p>
<p id="p188644511938"><a name="p188644511938"></a><a name="p188644511938"></a>/v3/{project_id}/backups/{backupId}</p>
<p id="p18641451232"><a name="p18641451232"></a><a name="p18641451232"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

