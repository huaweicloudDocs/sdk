# RDS<a name="sdk_13_0010"></a>

基于RDS v3 Go SDK的SDK接口如下，调用方式参考示例代码。

<a name="table88286590166"></a>
<table><thead align="left"><tr id="row582865915163"><th class="cellrowborder" valign="top" width="26.25262526252625%" id="mcps1.1.4.1.1"><p id="p14828105991617"><a name="p14828105991617"></a><a name="p14828105991617"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.51375137513751%" id="mcps1.1.4.1.2"><p id="p1782875941610"><a name="p1782875941610"></a><a name="p1782875941610"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.23362336233624%" id="mcps1.1.4.1.3"><p id="p58281959111614"><a name="p58281959111614"></a><a name="p58281959111614"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row11151923102211"><td class="cellrowborder" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p191151238224"><a name="p191151238224"></a><a name="p191151238224"></a>Datastores</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p11161723132212"><a name="p11161723132212"></a><a name="p11161723132212"></a>func listURL(sc *gophercloud.ServiceClient, databasename string)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p811642342211"><a name="p811642342211"></a><a name="p811642342211"></a>GET /v3/{project_id}/datastores/{database_name}</p>
<p id="p1699013172311"><a name="p1699013172311"></a><a name="p1699013172311"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8829185951616"><td class="cellrowborder" rowspan="9" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p1082995919160"><a name="p1082995919160"></a><a name="p1082995919160"></a>Instances</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p882915596165"><a name="p882915596165"></a><a name="p882915596165"></a>func createURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p7829959111613"><a name="p7829959111613"></a><a name="p7829959111613"></a>POST /v3/{project_id}/instances</p>
<p id="p118061537175715"><a name="p118061537175715"></a><a name="p118061537175715"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row88291359181611"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18829185991613"><a name="p18829185991613"></a><a name="p18829185991613"></a>func resizeURL(sc *gophercloud.ServiceClient, instancesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p182925913163"><a name="p182925913163"></a><a name="p182925913163"></a>POST /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p11580958287"><a name="p11580958287"></a><a name="p11580958287"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0101.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18385153271915"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1638510322192"><a name="p1638510322192"></a><a name="p1638510322192"></a>func enlargeURL(sc *gophercloud.ServiceClient, instancesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17385123219198"><a name="p17385123219198"></a><a name="p17385123219198"></a>POST /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p315010251896"><a name="p315010251896"></a><a name="p315010251896"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0102.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8260103516192"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1726133581913"><a name="p1726133581913"></a><a name="p1726133581913"></a>func singletohaURL(sc *gophercloud.ServiceClient, instancesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32611235141918"><a name="p32611235141918"></a><a name="p32611235141918"></a>POST /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p89321053171020"><a name="p89321053171020"></a><a name="p89321053171020"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row415714292194"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p131581129111915"><a name="p131581129111915"></a><a name="p131581129111915"></a>func restartURL(sc *gophercloud.ServiceClient, instancesId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11158029161918"><a name="p11158029161918"></a><a name="p11158029161918"></a>POST /v3/{project_id}/instances/{instance_id}/action</p>
<p id="p14348217171216"><a name="p14348217171216"></a><a name="p14348217171216"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17109926171913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5110826151918"><a name="p5110826151918"></a><a name="p5110826151918"></a>func deleteURL(sc *gophercloud.ServiceClient, serverID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1110122641910"><a name="p1110122641910"></a><a name="p1110122641910"></a>DELETE /v3/{project_id}/instances/{instance_id}</p>
<p id="p8242145412123"><a name="p8242145412123"></a><a name="p8242145412123"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row382912593166"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1682915914169"><a name="p1682915914169"></a><a name="p1682915914169"></a>func listURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7829155911165"><a name="p7829155911165"></a><a name="p7829155911165"></a>GET /v3/{project_id}/instances</p>
<p id="p8992127141515"><a name="p8992127141515"></a><a name="p8992127141515"></a><a href="https://support.huaweicloud.com/api-rds/rds_01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row195415438615"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14954124317617"><a name="p14954124317617"></a><a name="p14954124317617"></a>func listerrorlogURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16954104319615"><a name="p16954104319615"></a><a name="p16954104319615"></a>GET /v3/{project_id}/instances/{instance_id}/errorlog</p>
<p id="p499513915710"><a name="p499513915710"></a><a name="p499513915710"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1498011461966"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p119805466610"><a name="p119805466610"></a><a name="p119805466610"></a>func listslowlogURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3353838198"><a name="p3353838198"></a><a name="p3353838198"></a>GET /v3/{project_id}/instances/{instance_id}/slowlog</p>
<p id="p698019460618"><a name="p698019460618"></a><a name="p698019460618"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row296118314616"><td class="cellrowborder" rowspan="2" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p175204411761"><a name="p175204411761"></a><a name="p175204411761"></a>Configurations</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p1696117318610"><a name="p1696117318610"></a><a name="p1696117318610"></a>func listURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p169715261107"><a name="p169715261107"></a><a name="p169715261107"></a>GET /v3/{project_id}/configurations</p>
<p id="p187131055151213"><a name="p187131055151213"></a><a name="p187131055151213"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0301.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row147913379615"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6480737465"><a name="p6480737465"></a><a name="p6480737465"></a>func createURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6840643157"><a name="p6840643157"></a><a name="p6840643157"></a>POST /v3/{project_id}/configurations</p>
<p id="p1165673312168"><a name="p1165673312168"></a><a name="p1165673312168"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0302.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16791910195511"><td class="cellrowborder" rowspan="9" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p16680121015555"><a name="p16680121015555"></a><a name="p16680121015555"></a>Backups</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p1268081011555"><a name="p1268081011555"></a><a name="p1268081011555"></a>func updatepolicyURL(sc *gophercloud.ServiceClient, instanceId string)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p10680111035513"><a name="p10680111035513"></a><a name="p10680111035513"></a>PUT /v3/{project_id}/instances/{instance_id}/backups/policy</p>
<p id="p119961419122911"><a name="p119961419122911"></a><a name="p119961419122911"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15051415155513"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1850581519557"><a name="p1850581519557"></a><a name="p1850581519557"></a>func getpolicyURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8505415195514"><a name="p8505415195514"></a><a name="p8505415195514"></a>GET /v3/{project_id}/instances/{instance_id}/backups/policy</p>
<p id="p188761538143316"><a name="p188761538143316"></a><a name="p188761538143316"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9986187555"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p899161818553"><a name="p899161818553"></a><a name="p899161818553"></a>func createURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p699161875511"><a name="p699161875511"></a><a name="p699161875511"></a>POST /v3/{project_id}/backups</p>
<p id="p164911717155115"><a name="p164911717155115"></a><a name="p164911717155115"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5168172145512"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p81688217551"><a name="p81688217551"></a><a name="p81688217551"></a>func listURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12169102118551"><a name="p12169102118551"></a><a name="p12169102118551"></a>GET /v3/{project_id}/backups</p>
<p id="p4962012165718"><a name="p4962012165718"></a><a name="p4962012165718"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11316184712554"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11317124755512"><a name="p11317124755512"></a><a name="p11317124755512"></a>func listfilesURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1931784795516"><a name="p1931784795516"></a><a name="p1931784795516"></a>GET /v3/{project_id}/backup-files</p>
<p id="p2096763616432"><a name="p2096763616432"></a><a name="p2096763616432"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16380175016556"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13380195005510"><a name="p13380195005510"></a><a name="p13380195005510"></a>func deleteURL(sc *gophercloud.ServiceClient, backupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15380450195516"><a name="p15380450195516"></a><a name="p15380450195516"></a>DELETE /v3/{project_id}/backups/{backup_id}</p>
<p id="p1156110520610"><a name="p1156110520610"></a><a name="p1156110520610"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11859195395515"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p185917537554"><a name="p185917537554"></a><a name="p185917537554"></a>func getrestoretimeURL(sc *gophercloud.ServiceClient, instanceId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1187418167916"><a name="p1187418167916"></a><a name="p1187418167916"></a>GET /v3/{project_id}/instances/{instance_id}/restore-time</p>
<p id="p178529279914"><a name="p178529279914"></a><a name="p178529279914"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row47661656115519"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p207661056115511"><a name="p207661056115511"></a><a name="p207661056115511"></a>func restoreURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p044941044913"><a name="p044941044913"></a><a name="p044941044913"></a>POST /v3/{project_id}/instances</p>
<p id="p8405153013509"><a name="p8405153013509"></a><a name="p8405153013509"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19533619135617"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p853411917565"><a name="p853411917565"></a><a name="p853411917565"></a>func recoveryURL(sc *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1979418565710"><a name="p1979418565710"></a><a name="p1979418565710"></a>GET /v3/{project_id}/instances/recovery</p>
<p id="p1753461935616"><a name="p1753461935616"></a><a name="p1753461935616"></a><a href="https://support.huaweicloud.com/api-rds/rds_09_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row132338311265"><td class="cellrowborder" rowspan="5" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p14234143162618"><a name="p14234143162618"></a><a name="p14234143162618"></a>Database</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p323417392616"><a name="p323417392616"></a><a name="p323417392616"></a>func createURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p12234123152617"><a name="p12234123152617"></a><a name="p12234123152617"></a>POST /v3/{project_id}/instances/{instance_id}/database</p>
<p id="p57464382261"><a name="p57464382261"></a><a name="p57464382261"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1374791919285"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p57474193287"><a name="p57474193287"></a><a name="p57474193287"></a>func listURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11747419142819"><a name="p11747419142819"></a><a name="p11747419142819"></a>GET /v3/{project_id}/instances/{instance_id}/database/detail</p>
<p id="p114714852917"><a name="p114714852917"></a><a name="p114714852917"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0035.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13285151613113"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1628515163318"><a name="p1628515163318"></a><a name="p1628515163318"></a>func deleteURL(sc *gophercloud.ServiceClient, instanceID string,dbName string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p179621502588"><a name="p179621502588"></a><a name="p179621502588"></a>DELETE</p>
<p id="p132851116193120"><a name="p132851116193120"></a><a name="p132851116193120"></a>/v3/{project_id}/instances/{instance_id}/database/{db_name}</p>
<p id="p15468184933415"><a name="p15468184933415"></a><a name="p15468184933415"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11332194583314"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1433318455331"><a name="p1433318455331"></a><a name="p1433318455331"></a>func createURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8333114543310"><a name="p8333114543310"></a><a name="p8333114543310"></a>POST /v3/{project_id}/instances/{instance_id}/db_privilege</p>
<p id="p17748163113715"><a name="p17748163113715"></a><a name="p17748163113715"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0013.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1133813525431"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1233965211434"><a name="p1233965211434"></a><a name="p1233965211434"></a>func deleteURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3339165264318"><a name="p3339165264318"></a><a name="p3339165264318"></a>DELETE /v3/{project_id}/instances/{instance_id}/db_privilege</p>
<p id="p14977947154515"><a name="p14977947154515"></a><a name="p14977947154515"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0014.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13115202213483"><td class="cellrowborder" rowspan="3" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p18116122210482"><a name="p18116122210482"></a><a name="p18116122210482"></a>DbUser</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p201161221485"><a name="p201161221485"></a><a name="p201161221485"></a>func createURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p54581299498"><a name="p54581299498"></a><a name="p54581299498"></a>POST /v3/{project_id}/instances/{instance_id}/db_user</p>
<p id="p1811622234814"><a name="p1811622234814"></a><a name="p1811622234814"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1266142412487"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p186611249486"><a name="p186611249486"></a><a name="p186611249486"></a>func listURL(sc *gophercloud.ServiceClient, instanceID string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p794921517558"><a name="p794921517558"></a><a name="p794921517558"></a>GET /v3/{project_id}/instances/{instance_id}/db_user/detail</p>
<p id="p135491544185315"><a name="p135491544185315"></a><a name="p135491544185315"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0032.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row174591215718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p846212155718"><a name="p846212155718"></a><a name="p846212155718"></a>func deleteURL(sc *gophercloud.ServiceClient, instanceID string, dbuser string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2046151219577"><a name="p2046151219577"></a><a name="p2046151219577"></a>DELETE v3/{project_id}/instances/{instance_id}/db_user/{user_name}</p>
<p id="p144357112585"><a name="p144357112585"></a><a name="p144357112585"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0012.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17960127155813"><td class="cellrowborder" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p13960182785814"><a name="p13960182785814"></a><a name="p13960182785814"></a>Flavors</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p1696052765816"><a name="p1696052765816"></a><a name="p1696052765816"></a>func listURL(sc *gophercloud.ServiceClient, databasename string)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p1650201110115"><a name="p1650201110115"></a><a name="p1650201110115"></a>GET /v3/{project_id}/flavors/{database_name}</p>
<p id="p1096112713585"><a name="p1096112713585"></a><a name="p1096112713585"></a><a href="https://support.huaweicloud.com/api-rds/rds_06_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19831111718315"><td class="cellrowborder" valign="top" width="26.25262526252625%" headers="mcps1.1.4.1.1 "><p id="p16832101718313"><a name="p16832101718313"></a><a name="p16832101718313"></a>StorageType</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p128328174318"><a name="p128328174318"></a><a name="p128328174318"></a>func listURL(sc *gophercloud.ServiceClient, databasename string)</p>
</td>
<td class="cellrowborder" valign="top" width="36.23362336233624%" headers="mcps1.1.4.1.3 "><p id="p16832161713316"><a name="p16832161713316"></a><a name="p16832161713316"></a>GET/v3/{project_id}/storage-type/{database_name}</p>
<p id="p171635581139"><a name="p171635581139"></a><a name="p171635581139"></a><a href="https://support.huaweicloud.com/api-rds/rds_04_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

