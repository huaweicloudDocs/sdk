# Python-VBS<a name="ZH-CN_TOPIC_0072142414"></a>

基于VBS v2 API的SDK接口如下，调用方式举例：conn.volume\_backup.create\_backup\(\)

<a name="table65847680"></a>
<table><thead align="left"><tr id="row38664423"><th class="cellrowborder" valign="top" width="26.777322267773222%" id="mcps1.1.4.1.1"><p id="p44810590"><a name="p44810590"></a><a name="p44810590"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="34.916508349165085%" id="mcps1.1.4.1.2"><p id="p5779136"><a name="p5779136"></a><a name="p5779136"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="38.30616938306169%" id="mcps1.1.4.1.3"><p id="p65456887"><a name="p65456887"></a><a name="p65456887"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row407659"><td class="cellrowborder" rowspan="7" valign="top" width="26.777322267773222%" headers="mcps1.1.4.1.1 "><p id="p33020419"><a name="p33020419"></a><a name="p33020419"></a>VolumeBackup Operations</p>
</td>
<td class="cellrowborder" valign="top" width="34.916508349165085%" headers="mcps1.1.4.1.2 "><p id="p47787559181531"><a name="p47787559181531"></a><a name="p47787559181531"></a>create_backup(**backup)</p>
</td>
<td class="cellrowborder" valign="top" width="38.30616938306169%" headers="mcps1.1.4.1.3 "><p id="p59972191181539"><a name="p59972191181539"></a><a name="p59972191181539"></a>POST /v2/{project_id}/cloudbackups</p>
</td>
</tr>
<tr id="row41825741"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7630392181531"><a name="p7630392181531"></a><a name="p7630392181531"></a>create_native_backup(**backup)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p31857357181539"><a name="p31857357181539"></a><a name="p31857357181539"></a>Post /v2/{project_id}/backups</p>
</td>
</tr>
<tr id="row27781335"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p59629342181531"><a name="p59629342181531"></a><a name="p59629342181531"></a>restore_backup(volume_backup_id, volume_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4346561181539"><a name="p4346561181539"></a><a name="p4346561181539"></a>POST/v2/{project_id}/cloudbackups/{backup_id}/restore</p>
</td>
</tr>
<tr id="row3579130717415"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p938430181531"><a name="p938430181531"></a><a name="p938430181531"></a>backups(self, details=False, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53634862181539"><a name="p53634862181539"></a><a name="p53634862181539"></a>GET /v2/{project_id}/backups</p>
</td>
</tr>
<tr id="row3043936917418"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1433654612614"><a name="p1433654612614"></a><a name="p1433654612614"></a>get_backup(self, backup)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p42456086181539"><a name="p42456086181539"></a><a name="p42456086181539"></a>GET /v2/{project_id}/backups/{backup_id}</p>
</td>
</tr>
<tr id="row16105474174112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p34658687181531"><a name="p34658687181531"></a><a name="p34658687181531"></a>delete_backup(self, backup, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13300960181539"><a name="p13300960181539"></a><a name="p13300960181539"></a>DELETE /v2/{project_id}/backups/{backup_id}</p>
</td>
</tr>
<tr id="row34707136174115"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p192517352713"><a name="p192517352713"></a><a name="p192517352713"></a>get_job(self, job)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32724120181539"><a name="p32724120181539"></a><a name="p32724120181539"></a>GET /v1/{project_id}/jobs/{job_id}</p>
</td>
</tr>
<tr id="row51034272"><td class="cellrowborder" rowspan="10" valign="top" width="26.777322267773222%" headers="mcps1.1.4.1.1 "><p id="p28225828181320"><a name="p28225828181320"></a><a name="p28225828181320"></a>VolumeBackupPolicy Operations</p>
</td>
<td class="cellrowborder" valign="top" width="34.916508349165085%" headers="mcps1.1.4.1.2 "><p id="p56301706181551"><a name="p56301706181551"></a><a name="p56301706181551"></a>create_backup_policy(volume_backup_name, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="38.30616938306169%" headers="mcps1.1.4.1.3 "><p id="p3030129418161"><a name="p3030129418161"></a><a name="p3030129418161"></a>POST /v2/{project_id}/backuppolicy</p>
</td>
</tr>
<tr id="row5122214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p40428352181551"><a name="p40428352181551"></a><a name="p40428352181551"></a>backup_policies()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1082760618161"><a name="p1082760618161"></a><a name="p1082760618161"></a>GET /v2/{project_id}/backuppolicy</p>
</td>
</tr>
<tr id="row1986696"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11477564181551"><a name="p11477564181551"></a><a name="p11477564181551"></a>update_backup_policy(policy, **updated)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4158825618161"><a name="p4158825618161"></a><a name="p4158825618161"></a>PUT /v2/{project_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
<tr id="row3918391418131"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p45645032181551"><a name="p45645032181551"></a><a name="p45645032181551"></a>delete_backup_policy(policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5174165618161"><a name="p5174165618161"></a><a name="p5174165618161"></a>DELETE /v2/{project_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
<tr id="row2963296618134"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p56341241181551"><a name="p56341241181551"></a><a name="p56341241181551"></a>link_resources_to_policy(policy, volumes)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p448583918161"><a name="p448583918161"></a><a name="p448583918161"></a>POST /v2/{project_id}/backuppolicyresources</p>
</td>
</tr>
<tr id="row928682118137"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2140457181551"><a name="p2140457181551"></a><a name="p2140457181551"></a>unlink_resources_of_policy(policy, volumes)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4895165018161"><a name="p4895165018161"></a><a name="p4895165018161"></a>POST /v2/{project_id}/backuppolicyresources/{policy_id}/deleted_resources</p>
</td>
</tr>
<tr id="row4080558918139"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16889851181551"><a name="p16889851181551"></a><a name="p16889851181551"></a>execute_policy(policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5094622618161"><a name="p5094622618161"></a><a name="p5094622618161"></a>POST /v2/{project_id}/backuppolicy/{policy_id}/action</p>
</td>
</tr>
<tr id="row58618560181312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p31779963181551"><a name="p31779963181551"></a><a name="p31779963181551"></a>tasks(backup_policy_id, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2859761218161"><a name="p2859761218161"></a><a name="p2859761218161"></a>GET /v2/{project_id}/backuppolicy/{policy_id}/backuptasks</p>
</td>
</tr>
<tr id="row28367869181318"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15035130181551"><a name="p15035130181551"></a><a name="p15035130181551"></a>enable_policy(policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4391181018161"><a name="p4391181018161"></a><a name="p4391181018161"></a>PUT /v2/{project_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
<tr id="row38459673181320"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p21865429181551"><a name="p21865429181551"></a><a name="p21865429181551"></a>disable_policy(policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p78180718161"><a name="p78180718161"></a><a name="p78180718161"></a>PUT /v2/{project_id}/backuppolicy/{policy_id}</p>
</td>
</tr>
</tbody>
</table>

