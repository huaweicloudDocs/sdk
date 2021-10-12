# VBS<a name="sdk_11_0011"></a>

基于VBS v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table65847680"></a>
<table><thead align="left"><tr id="row38664423"><th class="cellrowborder" valign="top" width="28.689999999999998%" id="mcps1.1.4.1.1"><p id="p44810590"><a name="p44810590"></a><a name="p44810590"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.96%" id="mcps1.1.4.1.2"><p id="p5779136"><a name="p5779136"></a><a name="p5779136"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.35%" id="mcps1.1.4.1.3"><p id="p65456887"><a name="p65456887"></a><a name="p65456887"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row407659"><td class="cellrowborder" rowspan="8" valign="top" width="28.689999999999998%" headers="mcps1.1.4.1.1 "><p id="p1524012110577"><a name="p1524012110577"></a><a name="p1524012110577"></a>AsyncVolumeBackupService</p>
</td>
<td class="cellrowborder" valign="top" width="35.96%" headers="mcps1.1.4.1.2 "><p id="p17686124716526"><a name="p17686124716526"></a><a name="p17686124716526"></a>AsyncVolumeBackupJob create(AsyncVolumeBackupCreate cvbc)</p>
</td>
<td class="cellrowborder" valign="top" width="35.35%" headers="mcps1.1.4.1.3 "><p id="p53319751181248"><a name="p53319751181248"></a><a name="p53319751181248"></a>POST /v2/{tenant_id}/cloudbackups</p>
</td>
</tr>
<tr id="row41825741"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1819205555213"><a name="p1819205555213"></a><a name="p1819205555213"></a>VolumeBackup create(VolumeBackupCreate vbc)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14066452181248"><a name="p14066452181248"></a><a name="p14066452181248"></a>Post /v2/{project_id}/backups</p>
</td>
</tr>
<tr id="row27781335"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p193061537532"><a name="p193061537532"></a><a name="p193061537532"></a>AsyncVolumeBackupJob restore(String volumeBackupId, String volumeId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53896352181248"><a name="p53896352181248"></a><a name="p53896352181248"></a>POST /v2/{tenant_id}/cloudbackups/{backup_id}/restore</p>
</td>
</tr>
<tr id="row60341581174028"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p154320243543"><a name="p154320243543"></a><a name="p154320243543"></a>List&lt;? extends VolumeBackup&gt; list(boolean detail, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p31755374181248"><a name="p31755374181248"></a><a name="p31755374181248"></a>GET /v2/{tenant_id}/backups</p>
</td>
</tr>
<tr id="row3579130717415"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p63911232105413"><a name="p63911232105413"></a><a name="p63911232105413"></a>List&lt;? extends VolumeBackup&gt; list(boolean detail, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p64218761181248"><a name="p64218761181248"></a><a name="p64218761181248"></a>GET /v2/{tenant_id}/backups/detail</p>
</td>
</tr>
<tr id="row3043936917418"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1491584019544"><a name="p1491584019544"></a><a name="p1491584019544"></a>VolumeBackup get(String backupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p40599109181248"><a name="p40599109181248"></a><a name="p40599109181248"></a>GET /v2/{tenant_id}/backups/{backup_id}</p>
</td>
</tr>
<tr id="row16105474174112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4945448165411"><a name="p4945448165411"></a><a name="p4945448165411"></a>ActionResponse delete(String backupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1741563181248"><a name="p1741563181248"></a><a name="p1741563181248"></a>DELETE /v2/{tenant_id}/backups/{backup_id}</p>
</td>
</tr>
<tr id="row34707136174115"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1316551541"><a name="p1316551541"></a><a name="p1316551541"></a>AsyncVolumeBackupJob get(String jobId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p61640400181248"><a name="p61640400181248"></a><a name="p61640400181248"></a>GET /v1/{tenant_id}/jobs/{job_id}</p>
</td>
</tr>
<tr id="row51034272"><td class="cellrowborder" rowspan="10" valign="top" width="28.689999999999998%" headers="mcps1.1.4.1.1 "><p id="p181802256577"><a name="p181802256577"></a><a name="p181802256577"></a>BlockVolumeBackupPolicyService</p>
</td>
<td class="cellrowborder" valign="top" width="35.96%" headers="mcps1.1.4.1.2 "><p id="p1197212665511"><a name="p1197212665511"></a><a name="p1197212665511"></a>VolumeBackupPolicy create(VolumeBackupPolicy policy)</p>
</td>
<td class="cellrowborder" valign="top" width="35.35%" headers="mcps1.1.4.1.3 "><p id="p17659298181351"><a name="p17659298181351"></a><a name="p17659298181351"></a>POST /v2/{tenant_id}/backuppolicy</p>
</td>
</tr>
<tr id="row5122214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p48142257181339"><a name="p48142257181339"></a><a name="p48142257181339"></a>List&lt;? extends VolumeBackupPolicy&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55835538181351"><a name="p55835538181351"></a><a name="p55835538181351"></a>GET /v2/{tenant_id}/backuppolicy</p>
</td>
</tr>
<tr id="row1986696"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p332422516556"><a name="p332422516556"></a><a name="p332422516556"></a>VolumeBackupPolicy update(VolumeBackupPolicy updated)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p36135881181351"><a name="p36135881181351"></a><a name="p36135881181351"></a>PUT /v2/{tenant_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
<tr id="row3918391418131"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p156821933145515"><a name="p156821933145515"></a><a name="p156821933145515"></a>ActionResponse delete(String backupPolicyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p36382858181351"><a name="p36382858181351"></a><a name="p36382858181351"></a>DELETE /v2/{tenant_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
<tr id="row2963296618134"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p56198331181339"><a name="p56198331181339"></a><a name="p56198331181339"></a>VolumeBackupPolicyResourceActionResult linkResources(String backupPolicyId, List&lt;String&gt; resourceIds)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15102624181351"><a name="p15102624181351"></a><a name="p15102624181351"></a>POST /v2/{tenant_id}/backuppolicyresources</p>
</td>
</tr>
<tr id="row928682118137"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p157741452145515"><a name="p157741452145515"></a><a name="p157741452145515"></a>VolumeBackupPolicyResourceActionResult unlinkResources(String backupPolicyId, List&lt;String&gt; resourceIds)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3959839181351"><a name="p3959839181351"></a><a name="p3959839181351"></a>POST /v2/{tenant_id}/backuppolicyresources/{policy_id}/deleted_resources</p>
</td>
</tr>
<tr id="row4080558918139"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1641137568"><a name="p1641137568"></a><a name="p1641137568"></a>ActionResponse execute(String backupPolicyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1041696181351"><a name="p1041696181351"></a><a name="p1041696181351"></a>POST /v2/{tenant_id}/backuppolicy/{policy_id}/action</p>
</td>
</tr>
<tr id="row58618560181312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60454883181339"><a name="p60454883181339"></a><a name="p60454883181339"></a>List&lt;? extends VolumeBackupPolicyBackupTask&gt; tasks(String policyId, BakcupTaskListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p21199496181351"><a name="p21199496181351"></a><a name="p21199496181351"></a>GET /v2/{tenant_id}/backuppolicy/{policy_id}/backuptasks</p>
</td>
</tr>
<tr id="row28367869181318"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1639914152569"><a name="p1639914152569"></a><a name="p1639914152569"></a>VolumeBackupPolicy enable(String backupPolicyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19394241181351"><a name="p19394241181351"></a><a name="p19394241181351"></a>PUT /v2/{tenant_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
<tr id="row38459673181320"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p36487879181339"><a name="p36487879181339"></a><a name="p36487879181339"></a>VolumeBackupPolicy disable(String backupPolicyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p45540478181351"><a name="p45540478181351"></a><a name="p45540478181351"></a>PUT /v2/{tenant_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
</tbody>
</table>

