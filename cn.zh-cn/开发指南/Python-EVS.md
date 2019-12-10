# Python-EVS<a name="ZH-CN_TOPIC_0070868144"></a>

基于EVS v2 API的SDK接口如下，调用方式举例：conn.evs.create\_volume\(\)

<a name="table12806135412310"></a>
<table><thead align="left"><tr id="row1580812547235"><th class="cellrowborder" valign="top" width="16.23%" id="mcps1.1.4.1.1"><p id="p78081154152312"><a name="p78081154152312"></a><a name="p78081154152312"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.65%" id="mcps1.1.4.1.2"><p id="p580915547237"><a name="p580915547237"></a><a name="p580915547237"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="45.12%" id="mcps1.1.4.1.3"><p id="p14811854102310"><a name="p14811854102310"></a><a name="p14811854102310"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row381285472315"><td class="cellrowborder" rowspan="5" valign="top" width="16.23%" headers="mcps1.1.4.1.1 "><p id="p178121954192317"><a name="p178121954192317"></a><a name="p178121954192317"></a>Volume Operations</p>
</td>
<td class="cellrowborder" valign="top" width="38.65%" headers="mcps1.1.4.1.2 "><p id="p29268714259"><a name="p29268714259"></a><a name="p29268714259"></a>create_volume(**data)</p>
</td>
<td class="cellrowborder" valign="top" width="45.12%" headers="mcps1.1.4.1.3 "><p id="p20926187192516"><a name="p20926187192516"></a><a name="p20926187192516"></a>POST /v2/{project_id}/cloudvolumes</p>
<p id="p6113039105413"><a name="p6113039105413"></a><a name="p6113039105413"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235144.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1581616548235"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p39264710253"><a name="p39264710253"></a><a name="p39264710253"></a>update_volume(volume_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p192612717257"><a name="p192612717257"></a><a name="p192612717257"></a>PUT /v2/{project_id}/cloudvolumes/{volume_id}</p>
<p id="p17545144205418"><a name="p17545144205418"></a><a name="p17545144205418"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235147.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3178172332418"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1292687142518"><a name="p1292687142518"></a><a name="p1292687142518"></a>get_volume(volume_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p492647172512"><a name="p492647172512"></a><a name="p492647172512"></a>GET /v2/{project_id}/cloudvolumes/{volume_id}</p>
<p id="p1550119453541"><a name="p1550119453541"></a><a name="p1550119453541"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0127949639.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1058962220453"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9923048194518"><a name="p9923048194518"></a><a name="p9923048194518"></a>resize_volume(self, volume_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2092314874517"><a name="p2092314874517"></a><a name="p2092314874517"></a>POST /v2/{project_id}/cloudvolumes/{volume_id}/action</p>
<p id="p343704811546"><a name="p343704811546"></a><a name="p343704811546"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235145.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row194248318458"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15924348104518"><a name="p15924348104518"></a><a name="p15924348104518"></a>volumes(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13924124813459"><a name="p13924124813459"></a><a name="p13924124813459"></a>GET /v2/{project_id}/cloudvolumes/detail</p>
<p id="p7128165535413"><a name="p7128165535413"></a><a name="p7128165535413"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0127947068.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6485182711"><td class="cellrowborder" valign="top" width="16.23%" headers="mcps1.1.4.1.1 "><p id="p142389317467"><a name="p142389317467"></a><a name="p142389317467"></a>Job Operations</p>
</td>
<td class="cellrowborder" valign="top" width="38.65%" headers="mcps1.1.4.1.2 "><p id="p1923818312467"><a name="p1923818312467"></a><a name="p1923818312467"></a>get_job(self, job_id)</p>
</td>
<td class="cellrowborder" valign="top" width="45.12%" headers="mcps1.1.4.1.3 "><p id="p923873154619"><a name="p923873154619"></a><a name="p923873154619"></a>GET /v1/{project_id}/jobs/{job_id}</p>
<p id="p10902132515415"><a name="p10902132515415"></a><a name="p10902132515415"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235138.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于EVS v2.1 API的SDK接口如下，调用方式举例：conn.evs.create\_volume\_ext\(\)

<a name="table16433625154316"></a>
<table><thead align="left"><tr id="row7346778154316"><th class="cellrowborder" valign="top" width="16.23%" id="mcps1.1.4.1.1"><p id="p24290209154334"><a name="p24290209154334"></a><a name="p24290209154334"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="47.24%" id="mcps1.1.4.1.2"><p id="p34408676154334"><a name="p34408676154334"></a><a name="p34408676154334"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.53%" id="mcps1.1.4.1.3"><p id="p62164999154334"><a name="p62164999154334"></a><a name="p62164999154334"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row47891631154316"><td class="cellrowborder" rowspan="2" valign="top" width="16.23%" headers="mcps1.1.4.1.1 "><p id="p16907912154425"><a name="p16907912154425"></a><a name="p16907912154425"></a>Volume Operations</p>
</td>
<td class="cellrowborder" valign="top" width="47.24%" headers="mcps1.1.4.1.2 "><p id="p2335206315446"><a name="p2335206315446"></a><a name="p2335206315446"></a>create_volume_ext(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.53%" headers="mcps1.1.4.1.3 "><p id="p3193521515446"><a name="p3193521515446"></a><a name="p3193521515446"></a>POST /v2.1/{project_id}/cloudvolumes</p>
<p id="p720913225514"><a name="p720913225514"></a><a name="p720913225514"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0094124248.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6441243154316"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2243663115446"><a name="p2243663115446"></a><a name="p2243663115446"></a>resize_volume_ext(self, volume_id, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2508138015446"><a name="p2508138015446"></a><a name="p2508138015446"></a>POST /v2.1/{project_id}/cloudvolumes/{volume_id}/action</p>
<p id="p20902154135512"><a name="p20902154135512"></a><a name="p20902154135512"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0094124249.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Cinder v2 API的SDK接口如下，调用方式举例：conn.block\_store.create\_volume\(\)

<a name="table526619"></a>
<table><thead align="left"><tr id="row45283762"><th class="cellrowborder" valign="top" width="16.41%" id="mcps1.1.4.1.1"><p id="p44106115"><a name="p44106115"></a><a name="p44106115"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="44.940000000000005%" id="mcps1.1.4.1.2"><p id="p15825564"><a name="p15825564"></a><a name="p15825564"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="38.65%" id="mcps1.1.4.1.3"><p id="p6802342"><a name="p6802342"></a><a name="p6802342"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row14118857"><td class="cellrowborder" rowspan="4" valign="top" width="16.41%" headers="mcps1.1.4.1.1 "><p id="p2776748"><a name="p2776748"></a><a name="p2776748"></a>Snapshot Operations</p>
</td>
<td class="cellrowborder" valign="top" width="44.940000000000005%" headers="mcps1.1.4.1.2 "><p id="p23590007"><a name="p23590007"></a><a name="p23590007"></a>get_snapshot(self, snapshot)</p>
</td>
<td class="cellrowborder" valign="top" width="38.65%" headers="mcps1.1.4.1.3 "><p id="p31742419"><a name="p31742419"></a><a name="p31742419"></a>GET /v2/{project_id}/snapshots/{snapshot_id}</p>
<p id="p15908197195516"><a name="p15908197195516"></a><a name="p15908197195516"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0051408628.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17246319"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54774566"><a name="p54774566"></a><a name="p54774566"></a>snapshots(self, details=True, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7554882"><a name="p7554882"></a><a name="p7554882"></a>GET /v2/{project_id}/snapshots/detail</p>
<p id="p65051610195517"><a name="p65051610195517"></a><a name="p65051610195517"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0051408627.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row885082"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4582792"><a name="p4582792"></a><a name="p4582792"></a>create_snapshot(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p35661838"><a name="p35661838"></a><a name="p35661838"></a>POST /v2/{project_id}/snapshots</p>
<p id="p19834161217554"><a name="p19834161217554"></a><a name="p19834161217554"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0051408624.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52521090"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26349888"><a name="p26349888"></a><a name="p26349888"></a>delete_snapshot(self, snapshot, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53966187"><a name="p53966187"></a><a name="p53966187"></a>DELETE /v2/{project_id}/snapshots/{snapshot_id}</p>
<p id="p99131214165512"><a name="p99131214165512"></a><a name="p99131214165512"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0051408625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15933636"><td class="cellrowborder" rowspan="2" valign="top" width="16.41%" headers="mcps1.1.4.1.1 "><p id="p15556157"><a name="p15556157"></a><a name="p15556157"></a>Type Operations</p>
</td>
<td class="cellrowborder" valign="top" width="44.940000000000005%" headers="mcps1.1.4.1.2 "><p id="p52089174"><a name="p52089174"></a><a name="p52089174"></a>get_type(self, type)</p>
</td>
<td class="cellrowborder" valign="top" width="38.65%" headers="mcps1.1.4.1.3 "><p id="p58473527"><a name="p58473527"></a><a name="p58473527"></a>GET /v2/{project_id}/types/{volume_type_id}</p>
<p id="p17348123564"><a name="p17348123564"></a><a name="p17348123564"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235132.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56499698"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13072851"><a name="p13072851"></a><a name="p13072851"></a>types(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52268049"><a name="p52268049"></a><a name="p52268049"></a>GET /v2/{project_id}/types</p>
<p id="p174681256566"><a name="p174681256566"></a><a name="p174681256566"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235131.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row650398"><td class="cellrowborder" rowspan="4" valign="top" width="16.41%" headers="mcps1.1.4.1.1 "><p id="p52682290"><a name="p52682290"></a><a name="p52682290"></a>Volume Operations</p>
</td>
<td class="cellrowborder" valign="top" width="44.940000000000005%" headers="mcps1.1.4.1.2 "><p id="p39407061"><a name="p39407061"></a><a name="p39407061"></a>get_volume(self, volume)</p>
</td>
<td class="cellrowborder" valign="top" width="38.65%" headers="mcps1.1.4.1.3 "><p id="p37855410"><a name="p37855410"></a><a name="p37855410"></a>GET /v2/{project_id}/volumes/{volume_id}</p>
<p id="p37707108560"><a name="p37707108560"></a><a name="p37707108560"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0020235170.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5154373"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14851049"><a name="p14851049"></a><a name="p14851049"></a>volumes(self, details=True, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p62084314"><a name="p62084314"></a><a name="p62084314"></a>GET /v2/{project_id}/volumes/detail</p>
<p id="p1689321355618"><a name="p1689321355618"></a><a name="p1689321355618"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0058762431.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21887914"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p28090616"><a name="p28090616"></a><a name="p28090616"></a>create_volume(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p60747463"><a name="p60747463"></a><a name="p60747463"></a>POST /v2/{project_id}/volumes</p>
<p id="p99957161565"><a name="p99957161565"></a><a name="p99957161565"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0058762427.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9856263"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p752064018201"><a name="p752064018201"></a><a name="p752064018201"></a>delete_volume(self, volume, ignore_missing=True, cascade=False)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p41105728"><a name="p41105728"></a><a name="p41105728"></a>DELETE /v2/{project_id}/volumes/{volume_id}</p>
<p id="p1728461985611"><a name="p1728461985611"></a><a name="p1728461985611"></a><a href="https://support.huaweicloud.com/api-evs/zh-cn_topic_0058762428.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

