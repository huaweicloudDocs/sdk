# EVS<a name="sdk_11_0005"></a>

基于EVS v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table221254613615"></a>
<table><thead align="left"><tr id="row621374663619"><th class="cellrowborder" valign="top" width="29.972997299729975%" id="mcps1.1.4.1.1"><p id="p18207582364"><a name="p18207582364"></a><a name="p18207582364"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.923592359235926%" id="mcps1.1.4.1.2"><p id="p28281583366"><a name="p28281583366"></a><a name="p28281583366"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.103410341034106%" id="mcps1.1.4.1.3"><p id="p582015820368"><a name="p582015820368"></a><a name="p582015820368"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1021334623612"><td class="cellrowborder" rowspan="4" valign="top" width="29.972997299729975%" headers="mcps1.1.4.1.1 "><p id="p3722154417374"><a name="p3722154417374"></a><a name="p3722154417374"></a>VolumeService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p54951775108"><a name="p54951775108"></a><a name="p54951775108"></a>String create(CloudVolumes volume)</p>
</td>
<td class="cellrowborder" valign="top" width="34.103410341034106%" headers="mcps1.1.4.1.3 "><p id="p74956781017"><a name="p74956781017"></a><a name="p74956781017"></a>POST /v2/{project_id}/cloudvolumes</p>
<p id="p176491642193219"><a name="p176491642193219"></a><a name="p176491642193219"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2013.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row121374619365"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8495167121010"><a name="p8495167121010"></a><a name="p8495167121010"></a>String extend(Extend extend,String volumeId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1449587191016"><a name="p1449587191016"></a><a name="p1449587191016"></a>POST /v2/{project_id}/cloudvolumes/{volume_id}/action</p>
<p id="p182071610183316"><a name="p182071610183316"></a><a name="p182071610183316"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2014.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1621318466362"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5495578106"><a name="p5495578106"></a><a name="p5495578106"></a>CloudVolumeResponse list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p134952717102"><a name="p134952717102"></a><a name="p134952717102"></a>GET /v2/{project_id}/cloudvolumes/detail</p>
<p id="p1439111273318"><a name="p1439111273318"></a><a name="p1439111273318"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7213154612360"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1249514712102"><a name="p1249514712102"></a><a name="p1249514712102"></a>CloudVolumesResponse list(Map&lt;String,Object&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1449612716105"><a name="p1449612716105"></a><a name="p1449612716105"></a>GET /v2/{project_id}/cloudvolumes/detail</p>
<p id="p5687213183312"><a name="p5687213183312"></a><a name="p5687213183312"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14213174617367"><td class="cellrowborder" rowspan="4" valign="top" width="29.972997299729975%" headers="mcps1.1.4.1.1 "><p id="p353135643718"><a name="p353135643718"></a><a name="p353135643718"></a>VolumeSnapshotService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p10496772106"><a name="p10496772106"></a><a name="p10496772106"></a>CloudVolumeSnapshotsResponse list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.103410341034106%" headers="mcps1.1.4.1.3 "><p id="p44961672104"><a name="p44961672104"></a><a name="p44961672104"></a>GET /v2/{project_id}/cloudsnapshots/detail</p>
<p id="p208958152337"><a name="p208958152337"></a><a name="p208958152337"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2021.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row62141646163618"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p24961273102"><a name="p24961273102"></a><a name="p24961273102"></a>CloudVolumeSnapshotsResponse list(Map&lt;String,Object&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p94961576107"><a name="p94961576107"></a><a name="p94961576107"></a>GET /v2/{project_id}/cloudsnapshots/detail</p>
<p id="p648571914331"><a name="p648571914331"></a><a name="p648571914331"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2021.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row162142469369"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15496147181017"><a name="p15496147181017"></a><a name="p15496147181017"></a>RollbackResponse rollback(String snapshotId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8496774103"><a name="p8496774103"></a><a name="p8496774103"></a>POST /v2/{project_id}/cloudsnapshots/{snapshot_id}/rollback</p>
<p id="p208531022163310"><a name="p208531022163310"></a><a name="p208531022163310"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row921484663616"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1249618791015"><a name="p1249618791015"></a><a name="p1249618791015"></a>RollbackResponse rollback(String snapshotId, Rollback rollback)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p749612731012"><a name="p749612731012"></a><a name="p749612731012"></a>POST /v2/{project_id}/cloudsnapshots/{snapshot_id}/rollback</p>
<p id="p9271134104217"><a name="p9271134104217"></a><a name="p9271134104217"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row721444693610"><td class="cellrowborder" valign="top" width="29.972997299729975%" headers="mcps1.1.4.1.1 "><p id="p31412623817"><a name="p31412623817"></a><a name="p31412623817"></a>JobService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p19166318165918"><a name="p19166318165918"></a><a name="p19166318165918"></a>Job get(String job_id)</p>
</td>
<td class="cellrowborder" valign="top" width="34.103410341034106%" headers="mcps1.1.4.1.3 "><p id="p1144271418591"><a name="p1144271418591"></a><a name="p1144271418591"></a>GET /v1/{project_id}/jobs/{job_id}</p>
<p id="p14985173173312"><a name="p14985173173312"></a><a name="p14985173173312"></a><a href="https://support.huaweicloud.com/api-evs/evs_04_2020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于EVS v2.1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table3454091516227"></a>
<table><thead align="left"><tr id="row4281391716227"><th class="cellrowborder" valign="top" width="29.54%" id="mcps1.1.4.1.1"><p id="p4405103216325"><a name="p4405103216325"></a><a name="p4405103216325"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.77%" id="mcps1.1.4.1.2"><p id="p4210422016325"><a name="p4210422016325"></a><a name="p4210422016325"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.69%" id="mcps1.1.4.1.3"><p id="p6127191116325"><a name="p6127191116325"></a><a name="p6127191116325"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row4801534316227"><td class="cellrowborder" rowspan="2" valign="top" width="29.54%" headers="mcps1.1.4.1.1 "><p id="p4272130516254"><a name="p4272130516254"></a><a name="p4272130516254"></a>VolumeService</p>
</td>
<td class="cellrowborder" valign="top" width="36.77%" headers="mcps1.1.4.1.2 "><p id="p1090630103219"><a name="p1090630103219"></a><a name="p1090630103219"></a>AsyncRespEntity create(Volumes volume)</p>
</td>
<td class="cellrowborder" valign="top" width="33.69%" headers="mcps1.1.4.1.3 "><p id="p3168119316247"><a name="p3168119316247"></a><a name="p3168119316247"></a>POST /v2.1/{project_id}/cloudvolumes</p>
<p id="p118721613123511"><a name="p118721613123511"></a><a name="p118721613123511"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6116147716227"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3861436193213"><a name="p3861436193213"></a><a name="p3861436193213"></a>AsyncRespEntity extend(Extend extend,String volumeId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4939391716247"><a name="p4939391716247"></a><a name="p4939391716247"></a>POST /v2.1/{project_id}/cloudvolumes/{volume_id}/action</p>
<p id="p15206018113518"><a name="p15206018113518"></a><a name="p15206018113518"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Cinder v2 API的SDK接口如下，调用方式请参考示例代码。

<a name="table14253264"></a>
<table><thead align="left"><tr id="row57177053"><th class="cellrowborder" valign="top" width="29.122912291229124%" id="mcps1.1.4.1.1"><p id="p829755"><a name="p829755"></a><a name="p829755"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.51375137513751%" id="mcps1.1.4.1.2"><p id="p101341"><a name="p101341"></a><a name="p101341"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.36333633363336%" id="mcps1.1.4.1.3"><p id="p8208684"><a name="p8208684"></a><a name="p8208684"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row60923663"><td class="cellrowborder" rowspan="12" valign="top" width="29.122912291229124%" headers="mcps1.1.4.1.1 "><p id="p35869679"><a name="p35869679"></a><a name="p35869679"></a>BlockVolumeService</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p19762867"><a name="p19762867"></a><a name="p19762867"></a>Volume create(Volume volume)</p>
</td>
<td class="cellrowborder" valign="top" width="33.36333633363336%" headers="mcps1.1.4.1.3 "><p id="p57288388"><a name="p57288388"></a><a name="p57288388"></a>POST /v2/{project_id}/volumes</p>
<p id="p243813464332"><a name="p243813464332"></a><a name="p243813464332"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2065.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row224964215591"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p131751331404"><a name="p131751331404"></a><a name="p131751331404"></a>Volume create(Volume volume, Map&lt;String, Object&gt; schedulerHints)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p51751732011"><a name="p51751732011"></a><a name="p51751732011"></a>POST /v2/{project_id}/volumes</p>
<p id="p65181848143315"><a name="p65181848143315"></a><a name="p65181848143315"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2065.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row131464018595"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p21751232012"><a name="p21751232012"></a><a name="p21751232012"></a>Volume update(String volumeId, CinderVolumeUpdate volume)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p01752037016"><a name="p01752037016"></a><a name="p01752037016"></a>PUT /v2/{project_id}/volumes/{volume_id}</p>
<p id="p4369051123314"><a name="p4369051123314"></a><a name="p4369051123314"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2067.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row45833444"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p21521490"><a name="p21521490"></a><a name="p21521490"></a>ActionResponse delete(String volumeId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p65519169"><a name="p65519169"></a><a name="p65519169"></a>DELETE /v2/{project_id}/volumes/{volume_id}</p>
<p id="p4899165363316"><a name="p4899165363316"></a><a name="p4899165363316"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2066.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52801617"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p49072547"><a name="p49072547"></a><a name="p49072547"></a>ActionResponse extend(String volumeId, Integer newSize)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15453386"><a name="p15453386"></a><a name="p15453386"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p6921156123310"><a name="p6921156123310"></a><a name="p6921156123310"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2083.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4862753"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58338722"><a name="p58338722"></a><a name="p58338722"></a>Volume get(String volumeId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p27816043"><a name="p27816043"></a><a name="p27816043"></a>GET /v2/{project_id}/volumes/{volume_id}</p>
<p id="p186587591333"><a name="p186587591333"></a><a name="p186587591333"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2070.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row49017803"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11019092"><a name="p11019092"></a><a name="p11019092"></a>List&lt;? extends Volume&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p20131258"><a name="p20131258"></a><a name="p20131258"></a>GET /v2/{project_id}/volumes/detail</p>
<p id="p1779661143410"><a name="p1779661143410"></a><a name="p1779661143410"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46963595"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p45954822"><a name="p45954822"></a><a name="p45954822"></a>List&lt;? extends Volume&gt; list(Map&lt;String,String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul39972034153010"></a><a name="ul39972034153010"></a><ul id="ul39972034153010"><li>GET /v2/{project_id}/volumes/detail?limit={limit_nmuber}</li><li>GET /v2/{project_id}/volumes/detail?marker={volume_id}</li></ul>
<p id="p398510352443"><a name="p398510352443"></a><a name="p398510352443"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56573654"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19063291"><a name="p19063291"></a><a name="p19063291"></a>ActionResponse update(String volumeId, String name, String description)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p622761"><a name="p622761"></a><a name="p622761"></a>PUT /v2/{project_id}/volumes/{volume_id}</p>
<p id="p0332142083417"><a name="p0332142083417"></a><a name="p0332142083417"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2067.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row117111733909"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p24208491602"><a name="p24208491602"></a><a name="p24208491602"></a>VolumeUploadImage uploadToImage(String volumeId, UploadImageData data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34206496017"><a name="p34206496017"></a><a name="p34206496017"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p896113224347"><a name="p896113224347"></a><a name="p896113224347"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2086.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row177747371708"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19421349502"><a name="p19421349502"></a><a name="p19421349502"></a>ActionResponse readOnlyModeUpdate(String volumeId, boolean readonly)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13421749107"><a name="p13421749107"></a><a name="p13421749107"></a>POST /v2/{project_id}/volumes/{volume_id}/action</p>
<p id="p23697259345"><a name="p23697259345"></a><a name="p23697259345"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2085.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row495113612126"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1117511462188"><a name="p1117511462188"></a><a name="p1117511462188"></a>List&lt;? extends VolumeType&gt; listVolumeTypes()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2706191212199"><a name="p2706191212199"></a><a name="p2706191212199"></a>GET /v2/{project_id}/types</p>
<p id="p34528275347"><a name="p34528275347"></a><a name="p34528275347"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2071.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5604850"><td class="cellrowborder" rowspan="6" valign="top" width="29.122912291229124%" headers="mcps1.1.4.1.1 "><p id="p51339711"><a name="p51339711"></a><a name="p51339711"></a>BlockVolumeSnapshotService</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p64875945"><a name="p64875945"></a><a name="p64875945"></a>ActionResponse delete(String snapshotId)</p>
</td>
<td class="cellrowborder" valign="top" width="33.36333633363336%" headers="mcps1.1.4.1.3 "><p id="p20460183"><a name="p20460183"></a><a name="p20460183"></a>DELETE /v2/{project_id}/snapshots/{snapshot_id}</p>
<p id="p4787630123419"><a name="p4787630123419"></a><a name="p4787630123419"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2094.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row470622103818"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p205641517113811"><a name="p205641517113811"></a><a name="p205641517113811"></a>VolumeSnapshot create(VolumeSnapshot snapshot)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p656411716389"><a name="p656411716389"></a><a name="p656411716389"></a>POST /v2/{project_id}/snapshots</p>
<p id="p9894143283418"><a name="p9894143283418"></a><a name="p9894143283418"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2093.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row525357380"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1072092283819"><a name="p1072092283819"></a><a name="p1072092283819"></a>ActionResponse update(String snapshotId, String name, String description)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p272110228385"><a name="p272110228385"></a><a name="p272110228385"></a>PUT /v2/{project_id}/snapshots/{snapshot_id}</p>
<p id="p13195193533413"><a name="p13195193533413"></a><a name="p13195193533413"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2095.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row49923923"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17305987"><a name="p17305987"></a><a name="p17305987"></a>VolumeSnapshot get(String snapshotId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p59607724"><a name="p59607724"></a><a name="p59607724"></a>GET /v2/{project_id}/snapshots/{snapshot_id}</p>
<p id="p130812385343"><a name="p130812385343"></a><a name="p130812385343"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2098.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row66707469"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p34595869"><a name="p34595869"></a><a name="p34595869"></a>List&lt;? extends VolumeSnapshot&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p50801977"><a name="p50801977"></a><a name="p50801977"></a>GET /v2/{project_id}/snapshots</p>
<p id="p78222040163419"><a name="p78222040163419"></a><a name="p78222040163419"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2096.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row54564616"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p57657762"><a name="p57657762"></a><a name="p57657762"></a>List&lt;? extends VolumeSnapshot&gt; list(Map&lt;String,String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p39767165"><a name="p39767165"></a><a name="p39767165"></a>GET /v2/{project_id}/snapshots?volume_id={volume_id}</p>
<p id="p18310743183418"><a name="p18310743183418"></a><a name="p18310743183418"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2096.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row22360170"><td class="cellrowborder" valign="top" width="29.122912291229124%" headers="mcps1.1.4.1.1 "><p id="p66343369"><a name="p66343369"></a><a name="p66343369"></a>CinderZoneService</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p5103804"><a name="p5103804"></a><a name="p5103804"></a>List&lt;? extends AvailabilityZone&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="33.36333633363336%" headers="mcps1.1.4.1.3 "><p id="p10754988"><a name="p10754988"></a><a name="p10754988"></a>GET /v2/{project_id}/os-availability-zone</p>
<p id="p1449074610349"><a name="p1449074610349"></a><a name="p1449074610349"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2081.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row182341432618"><td class="cellrowborder" rowspan="7" valign="top" width="29.122912291229124%" headers="mcps1.1.4.1.1 "><p id="p84911558419"><a name="p84911558419"></a><a name="p84911558419"></a>BlockVolumeTransferService</p>
</td>
<td class="cellrowborder" valign="top" width="37.51375137513751%" headers="mcps1.1.4.1.2 "><p id="p03861612728"><a name="p03861612728"></a><a name="p03861612728"></a>List&lt;? extends VolumeTransfer&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="33.36333633363336%" headers="mcps1.1.4.1.3 "><p id="p63861412523"><a name="p63861412523"></a><a name="p63861412523"></a>GET /v2/{project_id}/os-volume-transfer/detail</p>
<p id="p1300749103411"><a name="p1300749103411"></a><a name="p1300749103411"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2111.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1098093511120"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12386121216219"><a name="p12386121216219"></a><a name="p12386121216219"></a>List&lt;? extends VolumeTransfer&gt; list(boolean detailed)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><a name="ul11646152105016"></a><a name="ul11646152105016"></a><ul id="ul11646152105016"><li>GET /v2/{project_id}/os-volume-transfer<p id="p196417992811"><a name="p196417992811"></a><a name="p196417992811"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2110.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li><li>GET /v2/{project_id}/os-volume-transfer/detail<p id="p1950141795018"><a name="p1950141795018"></a><a name="p1950141795018"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2111.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</li></ul>
</td>
</tr>
<tr id="row039401018"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p113861912128"><a name="p113861912128"></a><a name="p113861912128"></a>VolumeTransfer get(String transferId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7386612329"><a name="p7386612329"></a><a name="p7386612329"></a>GET /v2/{project_id}/os-volume-transfer/{transfer_id}</p>
<p id="p183968566349"><a name="p183968566349"></a><a name="p183968566349"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2109.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1440044320113"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1738611123211"><a name="p1738611123211"></a><a name="p1738611123211"></a>VolumeTransfer create(String volumeId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p153864122217"><a name="p153864122217"></a><a name="p153864122217"></a>POST /v2/{project_id}/os-volume-transfer</p>
<p id="p856265911347"><a name="p856265911347"></a><a name="p856265911347"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2106.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row78101647312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p53863129219"><a name="p53863129219"></a><a name="p53863129219"></a>VolumeTransfer create(String volumeId, String name)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p638691219211"><a name="p638691219211"></a><a name="p638691219211"></a>POST /v2/{project_id}/os-volume-transfer</p>
<p id="p86775273511"><a name="p86775273511"></a><a name="p86775273511"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2106.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row795312501119"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p103879121321"><a name="p103879121321"></a><a name="p103879121321"></a>VolumeTransfer accept(String transferId, String authKey)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23876121328"><a name="p23876121328"></a><a name="p23876121328"></a>POST /v2/{project_id}/os-volume-transfer/{transfer_id}/accept</p>
<p id="p16528195153515"><a name="p16528195153515"></a><a name="p16528195153515"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2107.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row153114551512"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1438791210211"><a name="p1438791210211"></a><a name="p1438791210211"></a>ActionResponse delete(String transferId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1938716128216"><a name="p1938716128216"></a><a name="p1938716128216"></a>DELETE /v2/{project_id}/os-volume-transfer/{transfer_id}</p>
<p id="p18310881357"><a name="p18310881357"></a><a name="p18310881357"></a><a href="https://support.huaweicloud.com/zh-cn/api-evs/evs_04_2108.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

