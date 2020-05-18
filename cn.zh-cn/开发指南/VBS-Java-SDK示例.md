# VBS Java SDK示例<a name="sdk_01_0022"></a>

## 创建云硬盘备份<a name="section1253044183628"></a>

下面代码为创建云硬盘备份的过程，用户可以根据需求进行相应的参数配置，创建完成后，新创建的备份会在VBS的备份列表显示。

```
public static void createBackup() {
    AsyncVolumeBackupCreate vbc = Builders.asyncVolumeBackupCreate()
            .name(backupName)
            .volumeId(volume.getId())
            .build();
    AsyncVolumeBackupJob job = osclient.blockStorage().asyncBackups().create(vbc);
    Assert.assertNotNull(job.getId());
    backupJobId = job.getId();
}
```

**表 1**  请求参数说明

<a name="table3329396232853"></a>
<table><thead align="left"><tr id="row2287857532853"><th class="cellrowborder" valign="top" width="15.6%" id="mcps1.2.5.1.1"><p id="p4122527132853"><a name="p4122527132853"></a><a name="p4122527132853"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.07%" id="mcps1.2.5.1.2"><p id="p5091263132853"><a name="p5091263132853"></a><a name="p5091263132853"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.28%" id="mcps1.2.5.1.3"><p id="p3028245632853"><a name="p3028245632853"></a><a name="p3028245632853"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.05%" id="mcps1.2.5.1.4"><p id="p3695987332853"><a name="p3695987332853"></a><a name="p3695987332853"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4095977132853"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p2940718232853"><a name="p2940718232853"></a><a name="p2940718232853"></a>backup</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p3317152132853"><a name="p3317152132853"></a><a name="p3317152132853"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.2.5.1.3 "><p id="p253865232853"><a name="p253865232853"></a><a name="p253865232853"></a>dict</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p430426432853"><a name="p430426432853"></a><a name="p430426432853"></a>待创建的备份。</p>
</td>
</tr>
<tr id="row3873838032853"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p5080104332853"><a name="p5080104332853"></a><a name="p5080104332853"></a>volume_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p2124383932853"><a name="p2124383932853"></a><a name="p2124383932853"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.2.5.1.3 "><p id="p4302943232853"><a name="p4302943232853"></a><a name="p4302943232853"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p6283197332853"><a name="p6283197332853"></a><a name="p6283197332853"></a>需要进行备份的磁盘ID。</p>
</td>
</tr>
<tr id="row2861685132853"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p3626359432853"><a name="p3626359432853"></a><a name="p3626359432853"></a>snapshot_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p5166999332853"><a name="p5166999332853"></a><a name="p5166999332853"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.2.5.1.3 "><p id="p2451992932853"><a name="p2451992932853"></a><a name="p2451992932853"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p3995725032853"><a name="p3995725032853"></a><a name="p3995725032853"></a>需要进行备份的磁盘对应的快照ID。</p>
</td>
</tr>
<tr id="row2407093132853"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p358835532853"><a name="p358835532853"></a><a name="p358835532853"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p2222131132853"><a name="p2222131132853"></a><a name="p2222131132853"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.2.5.1.3 "><p id="p5509579232853"><a name="p5509579232853"></a><a name="p5509579232853"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p3357420632853"><a name="p3357420632853"></a><a name="p3357420632853"></a>备份名称，最大支持64个字符(不区分中英文)，只能是中文、英文、数字、下划线（_）和中划线（-）。</p>
</td>
</tr>
<tr id="row3373240332853"><td class="cellrowborder" valign="top" width="15.6%" headers="mcps1.2.5.1.1 "><p id="p4797013532853"><a name="p4797013532853"></a><a name="p4797013532853"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p6037569032853"><a name="p6037569032853"></a><a name="p6037569032853"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.28%" headers="mcps1.2.5.1.3 "><p id="p5859275932853"><a name="p5859275932853"></a><a name="p5859275932853"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p4839302832853"><a name="p4839302832853"></a><a name="p4839302832853"></a>备份描述，最大支持64个字符(不区分中英文)，且不能包含“&lt;”和“&gt;”。</p>
</td>
</tr>
</tbody>
</table>

## 查询备份详情列表<a name="section1955604333538"></a>

下面代码为查询备份列表的过程，返回每个备份的详细信息，用户可以根据需求进行相应的参数配置。

```
public static void queryNativeBackupsDetail(){
    // 无查询条件
    List<? extends VolumeBackup> list = osclient.blockStorage().backups().list(true);
    Assert.assertNotEquals(list.size(), 0);

    // 条件查询
    HashMap<String, String> filter = new HashMap<>();
    filter.put("name", backupName);
    List<? extends VolumeBackup> list2 = osclient.blockStorage().backups().list(true, filter);
    for (VolumeBackup backup: list2) {
        Assert.assertEquals(backup.getName(), backupName);
    }
}
```

**表 2**  请求参数说明

<a name="table2997175432924"></a>
<table><thead align="left"><tr id="row4301668532924"><th class="cellrowborder" valign="top" width="16.53%" id="mcps1.2.5.1.1"><p id="p6179946532924"><a name="p6179946532924"></a><a name="p6179946532924"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.83%" id="mcps1.2.5.1.2"><p id="p3970076532924"><a name="p3970076532924"></a><a name="p3970076532924"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.59%" id="mcps1.2.5.1.3"><p id="p6164542632924"><a name="p6164542632924"></a><a name="p6164542632924"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.05%" id="mcps1.2.5.1.4"><p id="p2722363232924"><a name="p2722363232924"></a><a name="p2722363232924"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1794532832924"><td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.1 "><p id="p5426807933054"><a name="p5426807933054"></a><a name="p5426807933054"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="p3363829233054"><a name="p3363829233054"></a><a name="p3363829233054"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.59%" headers="mcps1.2.5.1.3 "><p id="p4034711733054"><a name="p4034711733054"></a><a name="p4034711733054"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p4689104333054"><a name="p4689104333054"></a><a name="p4689104333054"></a>指定查询的备份名称。用于过滤名称为指定字符串的备份。</p>
</td>
</tr>
<tr id="row3530653732924"><td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.1 "><p id="p2515866333054"><a name="p2515866333054"></a><a name="p2515866333054"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="p2458582733054"><a name="p2458582733054"></a><a name="p2458582733054"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.59%" headers="mcps1.2.5.1.3 "><p id="p4529496733054"><a name="p4529496733054"></a><a name="p4529496733054"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p4501374033054"><a name="p4501374033054"></a><a name="p4501374033054"></a>指定查询的备份状态。用于过滤特定状态的备份。可选的值目前只支持：“available”，“error”，“restoring”，“creating”，“deleting”，“error_restoring”。</p>
</td>
</tr>
<tr id="row3163626732924"><td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.1 "><p id="p6589138733054"><a name="p6589138733054"></a><a name="p6589138733054"></a>offset</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="p3560213633054"><a name="p3560213633054"></a><a name="p3560213633054"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.59%" headers="mcps1.2.5.1.3 "><p id="p6520078633054"><a name="p6520078633054"></a><a name="p6520078633054"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p4677230433054"><a name="p4677230433054"></a><a name="p4677230433054"></a>指定查询信息列表的偏移量。</p>
</td>
</tr>
<tr id="row1862338233141"><td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.1 "><p id="p4449525733154"><a name="p4449525733154"></a><a name="p4449525733154"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="p4734605033154"><a name="p4734605033154"></a><a name="p4734605033154"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.59%" headers="mcps1.2.5.1.3 "><p id="p982484033154"><a name="p982484033154"></a><a name="p982484033154"></a>int</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p5761454633154"><a name="p5761454633154"></a><a name="p5761454633154"></a>指定返回结果个数限制。</p>
</td>
</tr>
<tr id="row4682385633145"><td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.1 "><p id="p5796424033154"><a name="p5796424033154"></a><a name="p5796424033154"></a>volume_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="p6459186033154"><a name="p6459186033154"></a><a name="p6459186033154"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.59%" headers="mcps1.2.5.1.3 "><p id="p6455820133154"><a name="p6455820133154"></a><a name="p6455820133154"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p6183181533154"><a name="p6183181533154"></a><a name="p6183181533154"></a>指定查询备份的磁盘ID。用于过滤指定磁盘ID对应的备份。</p>
</td>
</tr>
</tbody>
</table>

## 从备份恢复磁盘<a name="section5821080034116"></a>

下面代码为选择一个备份恢复到磁盘的过程，用户可以根据需求进行相应的参数配置。

```
public static void restoreBackup() {
    AsyncVolumeBackupJob job = osclient.blockStorage()
            .asyncBackups()
            .restore(backupId, volume.getId());
    Assert.assertNotNull(job.getId());
}
```

**表 3**  请求参数说明

<a name="table244191134116"></a>
<table><thead align="left"><tr id="row2698448534116"><th class="cellrowborder" valign="top" width="14.67%" id="mcps1.2.5.1.1"><p id="p3825970934116"><a name="p3825970934116"></a><a name="p3825970934116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.25%" id="mcps1.2.5.1.2"><p id="p1202870934116"><a name="p1202870934116"></a><a name="p1202870934116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.03%" id="mcps1.2.5.1.3"><p id="p3480134934116"><a name="p3480134934116"></a><a name="p3480134934116"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.05%" id="mcps1.2.5.1.4"><p id="p33703034116"><a name="p33703034116"></a><a name="p33703034116"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2729947134116"><td class="cellrowborder" valign="top" width="14.67%" headers="mcps1.2.5.1.1 "><p id="p836370034246"><a name="p836370034246"></a><a name="p836370034246"></a>restore</p>
</td>
<td class="cellrowborder" valign="top" width="15.25%" headers="mcps1.2.5.1.2 "><p id="p637113234246"><a name="p637113234246"></a><a name="p637113234246"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.03%" headers="mcps1.2.5.1.3 "><p id="p4629966834246"><a name="p4629966834246"></a><a name="p4629966834246"></a>dict</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p5928560434246"><a name="p5928560434246"></a><a name="p5928560434246"></a>标记从备份恢复磁盘操作。</p>
</td>
</tr>
<tr id="row1192230234116"><td class="cellrowborder" valign="top" width="14.67%" headers="mcps1.2.5.1.1 "><p id="p109734534246"><a name="p109734534246"></a><a name="p109734534246"></a>backup_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.25%" headers="mcps1.2.5.1.2 "><p id="p2177613434246"><a name="p2177613434246"></a><a name="p2177613434246"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.03%" headers="mcps1.2.5.1.3 "><p id="p1903641534246"><a name="p1903641534246"></a><a name="p1903641534246"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p6555464534246"><a name="p6555464534246"></a><a name="p6555464534246"></a>需要恢复的备份ID</p>
</td>
</tr>
<tr id="row3815242734116"><td class="cellrowborder" valign="top" width="14.67%" headers="mcps1.2.5.1.1 "><p id="p782512934246"><a name="p782512934246"></a><a name="p782512934246"></a>volume_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.25%" headers="mcps1.2.5.1.2 "><p id="p2985571734246"><a name="p2985571734246"></a><a name="p2985571734246"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.03%" headers="mcps1.2.5.1.3 "><p id="p239400934246"><a name="p239400934246"></a><a name="p239400934246"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p5969707034246"><a name="p5969707034246"></a><a name="p5969707034246"></a>将要被恢复的磁盘ID。</p>
</td>
</tr>
</tbody>
</table>

## 删除备份<a name="section450686303436"></a>

下面代码为删除一个备份的过程，用户可以根据需求进行相应的参数配置。

```
public static void deleteNativeBackup() 
{
    ActionResponse delete = osclient.blockStorage().backups().delete(backupId);
    Assert.assertEquals(delete.isSuccess(), true);
}
```

**表 4**  请求参数说明

<a name="table44875573436"></a>
<table><thead align="left"><tr id="row186880613436"><th class="cellrowborder" valign="top" width="15.72%" id="mcps1.2.5.1.1"><p id="p373380073436"><a name="p373380073436"></a><a name="p373380073436"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.899999999999999%" id="mcps1.2.5.1.2"><p id="p44797543436"><a name="p44797543436"></a><a name="p44797543436"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.33%" id="mcps1.2.5.1.3"><p id="p273157733436"><a name="p273157733436"></a><a name="p273157733436"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.05%" id="mcps1.2.5.1.4"><p id="p650939763436"><a name="p650939763436"></a><a name="p650939763436"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row381207083436"><td class="cellrowborder" valign="top" width="15.72%" headers="mcps1.2.5.1.1 "><p id="p6042468934419"><a name="p6042468934419"></a><a name="p6042468934419"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.899999999999999%" headers="mcps1.2.5.1.2 "><p id="p6256165934419"><a name="p6256165934419"></a><a name="p6256165934419"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.3 "><p id="p3432960934419"><a name="p3432960934419"></a><a name="p3432960934419"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p572917693436"><a name="p572917693436"></a><a name="p572917693436"></a>租户ID。</p>
</td>
</tr>
<tr id="row458638733436"><td class="cellrowborder" valign="top" width="15.72%" headers="mcps1.2.5.1.1 "><p id="p6178794134419"><a name="p6178794134419"></a><a name="p6178794134419"></a>backup_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.899999999999999%" headers="mcps1.2.5.1.2 "><p id="p3876734234419"><a name="p3876734234419"></a><a name="p3876734234419"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.33%" headers="mcps1.2.5.1.3 "><p id="p5314696734419"><a name="p5314696734419"></a><a name="p5314696734419"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p158100833436"><a name="p158100833436"></a><a name="p158100833436"></a>需要恢复的备份ID。</p>
</td>
</tr>
</tbody>
</table>

## 创建备份策略<a name="section6079600434820"></a>

下面代码为备份策略的创建过程，用户可以根据需求进行相应的参数配置。

```
public static void createPolicy() 
{
    // 先创建 scheduled policy
    VBSVolumeBackupScheduledPolicy scheduledPolicy = VBSVolumeBackupScheduledPolicy.builder()
            .frequency(10)
            .maxBackupAmount(10)
            .retainFirstBackupOfCurrentMonth(true)
            .startTime("01:00")
            .status(VolumeBackupPolicy.VolumeBackupPolicyStatus.OFF)
            .build();
    Assert.assertNotNull(scheduledPolicy);

    // 创建 backup policy 对象
    VolumeBackupPolicy create = VBSVolumeBackupPolicy.builder()
            .name(policyName)
            .scheduledPolicy(scheduledPolicy)
            .build();
    VolumeBackupPolicy policy = osclient.blockStorage().policies().create(create);
    Assert.assertNotNull(policy.getId());

```

**表 5**  请求参数说明

<a name="table1107126234820"></a>
<table><thead align="left"><tr id="row4943469434820"><th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.5.1.1"><p id="p4478727734820"><a name="p4478727734820"></a><a name="p4478727734820"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.44%" id="mcps1.2.5.1.2"><p id="p389081234820"><a name="p389081234820"></a><a name="p389081234820"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p4672038034820"><a name="p4672038034820"></a><a name="p4672038034820"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.05%" id="mcps1.2.5.1.4"><p id="p2625445334820"><a name="p2625445334820"></a><a name="p2625445334820"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4623591834820"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p114411453501"><a name="p114411453501"></a><a name="p114411453501"></a>backup_policy_name</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p543175433501"><a name="p543175433501"></a><a name="p543175433501"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p376448663501"><a name="p376448663501"></a><a name="p376448663501"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p293352813501"><a name="p293352813501"></a><a name="p293352813501"></a>备份策略名称</p>
<p id="p626909403501"><a name="p626909403501"></a><a name="p626909403501"></a>只能由数字、字母、汉字、下划线、中划线组成，同时不能以default开头，长度1到64位。</p>
</td>
</tr>
<tr id="row3254810734820"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p5589573501"><a name="p5589573501"></a><a name="p5589573501"></a>scheduled_policy</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p452755293501"><a name="p452755293501"></a><a name="p452755293501"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p434392583501"><a name="p434392583501"></a><a name="p434392583501"></a>dict</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p289190483501"><a name="p289190483501"></a><a name="p289190483501"></a>调度策略详情。</p>
</td>
</tr>
<tr id="row5052150534928"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p98031533501"><a name="p98031533501"></a><a name="p98031533501"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p558578923501"><a name="p558578923501"></a><a name="p558578923501"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p281954413501"><a name="p281954413501"></a><a name="p281954413501"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p21293743501"><a name="p21293743501"></a><a name="p21293743501"></a>备份开始时间，需要转化成本地时间对应的UTC时间（目前只支持整点）。</p>
<p id="p191643683501"><a name="p191643683501"></a><a name="p191643683501"></a>格式为HH:mm</p>
</td>
</tr>
<tr id="row5442279134935"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p121808573501"><a name="p121808573501"></a><a name="p121808573501"></a>frequency</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p471253673501"><a name="p471253673501"></a><a name="p471253673501"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p590584223501"><a name="p590584223501"></a><a name="p590584223501"></a>integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p190029103501"><a name="p190029103501"></a><a name="p190029103501"></a>备份间隔（1-14天），该字段和week_frequency字段二选一，如果同时设置，默认以该字段为准。</p>
</td>
</tr>
<tr id="row1302346734935"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p286956233501"><a name="p286956233501"></a><a name="p286956233501"></a>week_frequency</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p426441553501"><a name="p426441553501"></a><a name="p426441553501"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p316245313501"><a name="p316245313501"></a><a name="p316245313501"></a>list&lt;dict&gt;</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p114502323501"><a name="p114502323501"></a><a name="p114502323501"></a>按指定周进行备份，取值为以下值的一个或者多个：</p>
<p id="p359432263501"><a name="p359432263501"></a><a name="p359432263501"></a>SUN，MON，TUE，WED，THU，FRI，SAT</p>
</td>
</tr>
<tr id="row5485946034941"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p301553993501"><a name="p301553993501"></a><a name="p301553993501"></a>rentention_num</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p266682253501"><a name="p266682253501"></a><a name="p266682253501"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p126425993501"><a name="p126425993501"></a><a name="p126425993501"></a>integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p174176353501"><a name="p174176353501"></a><a name="p174176353501"></a>备份保留个数（最小值为2），该字段和rentention_day字段二先一，如果同时设置，默认以该字段为准。</p>
</td>
</tr>
<tr id="row3309449034941"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p138806883501"><a name="p138806883501"></a><a name="p138806883501"></a>rentention_day</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p505939663501"><a name="p505939663501"></a><a name="p505939663501"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p44705563501"><a name="p44705563501"></a><a name="p44705563501"></a>integer</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p265707223501"><a name="p265707223501"></a><a name="p265707223501"></a>备份保留天数。</p>
</td>
</tr>
<tr id="row1271241634941"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p427038603501"><a name="p427038603501"></a><a name="p427038603501"></a>remain_first_backup_of_curMonth</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p364606393501"><a name="p364606393501"></a><a name="p364606393501"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p5217583501"><a name="p5217583501"></a><a name="p5217583501"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p422624263501"><a name="p422624263501"></a><a name="p422624263501"></a>是否保留当月的第一个备份。</p>
<a name="ul448175143501"></a><a name="ul448175143501"></a><ul id="ul448175143501"><li>Y</li><li>N</li></ul>
</td>
</tr>
<tr id="row656270634948"><td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.5.1.1 "><p id="p584422473501"><a name="p584422473501"></a><a name="p584422473501"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="14.44%" headers="mcps1.2.5.1.2 "><p id="p362016053501"><a name="p362016053501"></a><a name="p362016053501"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p466489033501"><a name="p466489033501"></a><a name="p466489033501"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p204648223501"><a name="p204648223501"></a><a name="p204648223501"></a>策略状态：启用或停用。</p>
<a name="ul499656733501"></a><a name="ul499656733501"></a><ul id="ul499656733501"><li>ON</li><li>OFF</li></ul>
</td>
</tr>
</tbody>
</table>

## 删除备份策略<a name="section1557609435021"></a>

下面代码为备份策略的删除过程，用户可以根据需求进行相应的参数配置。

```
public static void deletePolicy() {
    osclient.blockStorage().policies().delete(policyId);
    List<? extends VolumeBackupPolicy> policies = osclient.blockStorage().policies().list();
    boolean isSuccess = true;
    for (VolumeBackupPolicy policy:
            policies) {
        if (policy.getId().equals(policyId)) {
            isSuccess = false;
            break;
        }
    }
    Assert.assertEquals(isSuccess, true);
}
```

**表 6**  请求参数说明

<a name="table1047633535021"></a>
<table><thead align="left"><tr id="row1348421735021"><th class="cellrowborder" valign="top" width="16.3%" id="mcps1.2.5.1.1"><p id="p1847980735021"><a name="p1847980735021"></a><a name="p1847980735021"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.340000000000002%" id="mcps1.2.5.1.2"><p id="p2046940535021"><a name="p2046940535021"></a><a name="p2046940535021"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.310000000000002%" id="mcps1.2.5.1.3"><p id="p4740914835021"><a name="p4740914835021"></a><a name="p4740914835021"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.05%" id="mcps1.2.5.1.4"><p id="p1493581235021"><a name="p1493581235021"></a><a name="p1493581235021"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row184124435021"><td class="cellrowborder" valign="top" width="16.3%" headers="mcps1.2.5.1.1 "><p id="p4474311435116"><a name="p4474311435116"></a><a name="p4474311435116"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.340000000000002%" headers="mcps1.2.5.1.2 "><p id="p31362335116"><a name="p31362335116"></a><a name="p31362335116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.310000000000002%" headers="mcps1.2.5.1.3 "><p id="p2540352135116"><a name="p2540352135116"></a><a name="p2540352135116"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p6489075235021"><a name="p6489075235021"></a><a name="p6489075235021"></a>租户ID</p>
</td>
</tr>
<tr id="row4714586335021"><td class="cellrowborder" valign="top" width="16.3%" headers="mcps1.2.5.1.1 "><p id="p6422948335116"><a name="p6422948335116"></a><a name="p6422948335116"></a>policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.340000000000002%" headers="mcps1.2.5.1.2 "><p id="p3520565935116"><a name="p3520565935116"></a><a name="p3520565935116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.310000000000002%" headers="mcps1.2.5.1.3 "><p id="p3308614835116"><a name="p3308614835116"></a><a name="p3308614835116"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="53.05%" headers="mcps1.2.5.1.4 "><p id="p4009666535021"><a name="p4009666535021"></a><a name="p4009666535021"></a>策略ID</p>
</td>
</tr>
</tbody>
</table>

## 查询备份策略<a name="section1499991735125"></a>

下面代码为查询备份策略的过程，用户可以根据需求进行相应的参数配置。

```
public static void queryPolicy() {
    List<? extends VolumeBackupPolicy> policies = osclient.blockStorage().policies().list();
    boolean isSuccess = false;
    for (VolumeBackupPolicy policy:
         policies) {
        if (policy.getName().equals(policyName)) {
            isSuccess = true;
            policyId = policy.getId();
            break;
        }
    }
    Assert.assertEquals(isSuccess, true);
}

```

