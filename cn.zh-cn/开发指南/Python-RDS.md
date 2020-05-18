# RDS<a name="sdk_12_0019"></a>

基于RDS v3 API的SDK接口如下，调用方式举例：**conn.rds\_v3.create\_instance\(\)**

<a name="table4567131392218"></a>
<table><thead align="left"><tr id="row4567151312215"><th class="cellrowborder" valign="top" width="26.25%" id="mcps1.1.4.1.1"><p id="p13567191372219"><a name="p13567191372219"></a><a name="p13567191372219"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.66%" id="mcps1.1.4.1.2"><p id="p16567161315224"><a name="p16567161315224"></a><a name="p16567161315224"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="37.09%" id="mcps1.1.4.1.3"><p id="p1567151313226"><a name="p1567151313226"></a><a name="p1567151313226"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row956781332213"><td class="cellrowborder" rowspan="7" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p195671913132219"><a name="p195671913132219"></a><a name="p195671913132219"></a>Instance Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.66%" headers="mcps1.1.4.1.2 "><p id="p856710133228"><a name="p856710133228"></a><a name="p856710133228"></a>create_instance(self, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="37.09%" headers="mcps1.1.4.1.3 "><p id="p5567191372218"><a name="p5567191372218"></a><a name="p5567191372218"></a>POST /v3/{project_id}/instances</p>
<p id="p118061537175715"><a name="p118061537175715"></a><a name="p118061537175715"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1956731362210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17568191382219"><a name="p17568191382219"></a><a name="p17568191382219"></a>instances(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14568181382218"><a name="p14568181382218"></a><a name="p14568181382218"></a>GET /v3/{project_id}/instances?id={id}&amp;name={name}&amp;type={type}&amp;datastore_type={datastore_type}&amp;vpc_id={vpc_id}&amp;subnet_id={subnet_id}&amp;offset={offset}&amp;limit={limit}</p>
<p id="p42553192168"><a name="p42553192168"></a><a name="p42553192168"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10568413132220"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p95681313162219"><a name="p95681313162219"></a><a name="p95681313162219"></a>delete_instance(self, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8568113152218"><a name="p8568113152218"></a><a name="p8568113152218"></a>DELETE /v3/{project_id}/instances/{instance_id}</p>
<p id="p14424104112179"><a name="p14424104112179"></a><a name="p14424104112179"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2311341283"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p63112416818"><a name="p63112416818"></a><a name="p63112416818"></a>resize_instance(self, instance, flavorRef)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1831119411788"><a name="p1831119411788"></a><a name="p1831119411788"></a>POST  /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p18798333162310"><a name="p18798333162310"></a><a name="p18798333162310"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0101.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row569824913816"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1269918493812"><a name="p1269918493812"></a><a name="p1269918493812"></a>resize_instance_volume(instance, size)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1469974910813"><a name="p1469974910813"></a><a name="p1469974910813"></a>POST  /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p35181414152518"><a name="p35181414152518"></a><a name="p35181414152518"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0102.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13794454181"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1979445412812"><a name="p1979445412812"></a><a name="p1979445412812"></a>restart_instance(instance)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15614751171215"><a name="p15614751171215"></a><a name="p15614751171215"></a>POST  /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p1249115456258"><a name="p1249115456258"></a><a name="p1249115456258"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row117943547814"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p167944541687"><a name="p167944541687"></a><a name="p167944541687"></a>single_to_ha(instance,**single_to_ha_param)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5794155414817"><a name="p5794155414817"></a><a name="p5794155414817"></a>POST  /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p12362132132619"><a name="p12362132132619"></a><a name="p12362132132619"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row85686135225"><td class="cellrowborder" rowspan="6" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p756861322219"><a name="p756861322219"></a><a name="p756861322219"></a>Backup Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.66%" headers="mcps1.1.4.1.2 "><p id="p95681313152218"><a name="p95681313152218"></a><a name="p95681313152218"></a>create_backup(self, **kwarg)</p>
</td>
<td class="cellrowborder" valign="top" width="37.09%" headers="mcps1.1.4.1.3 "><p id="p1772260163015"><a name="p1772260163015"></a><a name="p1772260163015"></a>POST /v3/{project_id}/backups</p>
<p id="p5621191519302"><a name="p5621191519302"></a><a name="p5621191519302"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row105681713102212"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16568111362215"><a name="p16568111362215"></a><a name="p16568111362215"></a>backups(self, **kwarg)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1296782293017"><a name="p1296782293017"></a><a name="p1296782293017"></a>GET /v3/{project_id}/backups?instance_id={instance_id}&amp;backup_id={backup_id}&amp;backup_type={backup_type}&amp;offset={offset}&amp;limit={limit}&amp;begin_time={begin _time}&amp;end_time={end_time}</p>
<p id="p18812922153213"><a name="p18812922153213"></a><a name="p18812922153213"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row106803865912"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p126826805919"><a name="p126826805919"></a><a name="p126826805919"></a>restore_time(self, **kwarg)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4294112818013"><a name="p4294112818013"></a><a name="p4294112818013"></a>GET v3/{project_id}/instances/{instance_id}/restore-time</p>
<p id="p1771665220323"><a name="p1771665220323"></a><a name="p1771665220323"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row856814138224"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p95693139223"><a name="p95693139223"></a><a name="p95693139223"></a>delete_backup(self, id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p856951352215"><a name="p856951352215"></a><a name="p856951352215"></a>DELETE /v3/{project_id}/backups/{backup_id}</p>
<p id="p356253883313"><a name="p356253883313"></a><a name="p356253883313"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1178853211137"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5789173291310"><a name="p5789173291310"></a><a name="p5789173291310"></a>backup_files(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15789153221317"><a name="p15789153221317"></a><a name="p15789153221317"></a>GET  /v3/{project_id}/backup-files?backup_id={backup_id}</p>
<p id="p7124152043410"><a name="p7124152043410"></a><a name="p7124152043410"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6951650141415"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1596115020146"><a name="p1596115020146"></a><a name="p1596115020146"></a>recovery_instance(**recovery_point)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p596185016146"><a name="p596185016146"></a><a name="p596185016146"></a>POST  /v3/{project_id}/instances</p>
<p id="p13710810466"><a name="p13710810466"></a><a name="p13710810466"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1956912136226"><td class="cellrowborder" rowspan="2" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p55692133221"><a name="p55692133221"></a><a name="p55692133221"></a>Backup Policy Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.66%" headers="mcps1.1.4.1.2 "><p id="p209291727104211"><a name="p209291727104211"></a><a name="p209291727104211"></a>create_backup_policy(self, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="37.09%" headers="mcps1.1.4.1.3 "><p id="p656911318229"><a name="p656911318229"></a><a name="p656911318229"></a>PUT /v3/{project_id}/instances/{instance_id}/backups/policy</p>
<p id="p3643133019556"><a name="p3643133019556"></a><a name="p3643133019556"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12569171312218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1586810411425"><a name="p1586810411425"></a><a name="p1586810411425"></a>get_backup_policy(self, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18569813172213"><a name="p18569813172213"></a><a name="p18569813172213"></a>GET /v3/{project_id}/instances/{instance_id}/backups/policy</p>
<p id="p1761522118016"><a name="p1761522118016"></a><a name="p1761522118016"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18569181310221"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p9569191317221"><a name="p9569191317221"></a><a name="p9569191317221"></a>Flavor Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.66%" headers="mcps1.1.4.1.2 "><p id="p161969918435"><a name="p161969918435"></a><a name="p161969918435"></a>flavors(self, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="37.09%" headers="mcps1.1.4.1.3 "><p id="p7569713112213"><a name="p7569713112213"></a><a name="p7569713112213"></a>GET /v3/{project_id}/flavors/{database_name}?version_name={version_name}</p>
<p id="p11232717116"><a name="p11232717116"></a><a name="p11232717116"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row156961312224"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p11569201322214"><a name="p11569201322214"></a><a name="p11569201322214"></a>Datastore Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.66%" headers="mcps1.1.4.1.2 "><p id="p125701613132217"><a name="p125701613132217"></a><a name="p125701613132217"></a>datastore_versions(self, dbname)</p>
</td>
<td class="cellrowborder" valign="top" width="37.09%" headers="mcps1.1.4.1.3 "><p id="p15570161362218"><a name="p15570161362218"></a><a name="p15570161362218"></a>GET /v3/{project_id}/datastores/{database_name}</p>
<p id="p194606441615"><a name="p194606441615"></a><a name="p194606441615"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10718237195220"><td class="cellrowborder" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p1371933713527"><a name="p1371933713527"></a><a name="p1371933713527"></a>Configuration Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.66%" headers="mcps1.1.4.1.2 "><p id="p8719103710521"><a name="p8719103710521"></a><a name="p8719103710521"></a>configurations(self, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="37.09%" headers="mcps1.1.4.1.3 "><p id="p67199377520"><a name="p67199377520"></a><a name="p67199377520"></a>GET /v3/{project_id}/configurations</p>
<p id="p19236165854"><a name="p19236165854"></a><a name="p19236165854"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0301.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row927224515519"><td class="cellrowborder" rowspan="2" valign="top" width="26.25%" headers="mcps1.1.4.1.1 "><p id="p17243124011169"><a name="p17243124011169"></a><a name="p17243124011169"></a>Log Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.66%" headers="mcps1.1.4.1.2 "><p id="p122847561164"><a name="p122847561164"></a><a name="p122847561164"></a>list_instance_errorlog(**query)</p>
</td>
<td class="cellrowborder" valign="top" width="37.09%" headers="mcps1.1.4.1.3 "><p id="p8274194514515"><a name="p8274194514515"></a><a name="p8274194514515"></a>GET instances/{instance_id}/errorlog?start_date={start_date}&amp;end_date={end_date}</p>
<p id="p411102620817"><a name="p411102620817"></a><a name="p411102620817"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row188393123175"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1683911121174"><a name="p1683911121174"></a><a name="p1683911121174"></a>list_instance_slowlog(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1771865813176"><a name="p1771865813176"></a><a name="p1771865813176"></a>GET  /v3/{project_id}/instances/{instance_id}/slowlog?start_date={start_date}&amp;end_date={end_date}</p>
<p id="p613492941220"><a name="p613492941220"></a><a name="p613492941220"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

