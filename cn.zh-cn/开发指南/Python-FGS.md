# Python-FGS<a name="ZH-CN_TOPIC_0187492664"></a>

基于函数工作流FGS v2.0 Python API的SDK接口如下，调用方式举例：conn.fgs.get\_function\_list\(\)。

<a name="table131110432351"></a>
<table><tbody><tr id="row174391343143517"><td class="cellrowborder" valign="top" width="10.94109410941094%"><p id="p1043916437357"><a name="p1043916437357"></a><a name="p1043916437357"></a>Interface</p>
</td>
<td class="cellrowborder" valign="top" width="39.563956395639565%"><p id="p19439243123519"><a name="p19439243123519"></a><a name="p19439243123519"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="49.494949494949495%"><p id="p124391643113516"><a name="p124391643113516"></a><a name="p124391643113516"></a>API</p>
</td>
</tr>
<tr id="row84391943123513"><td class="cellrowborder" rowspan="16" valign="top" width="10.94109410941094%"><p id="p94392431354"><a name="p94392431354"></a><a name="p94392431354"></a>Functions</p>
</td>
<td class="cellrowborder" valign="top" width="39.563956395639565%"><p id="p186615332482"><a name="p186615332482"></a><a name="p186615332482"></a>functions(**function)</p>
</td>
<td class="cellrowborder" valign="top" width="49.494949494949495%"><p id="p94396437356"><a name="p94396437356"></a><a name="p94396437356"></a>GET /v2/{project_id}/fgs/functions?marker={marker}&amp;maxitems={maxitems}</p>
</td>
</tr>
<tr id="row16439443193513"><td class="cellrowborder" valign="top"><p id="p123370398489"><a name="p123370398489"></a><a name="p123370398489"></a>get_function_metadata(function_urn)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p1944024363519"><a name="p1944024363519"></a><a name="p1944024363519"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row1944074312356"><td class="cellrowborder" valign="top"><p id="p036394410482"><a name="p036394410482"></a><a name="p036394410482"></a>get_function_code(function_urn)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p1844018436352"><a name="p1844018436352"></a><a name="p1844018436352"></a>GET</p>
<p id="p1244084318353"><a name="p1244084318353"></a><a name="p1244084318353"></a>/v2/{project_id}/fgs/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row1844018436359"><td class="cellrowborder" valign="top"><p id="p13360115312480"><a name="p13360115312480"></a><a name="p13360115312480"></a>create_function(**attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p174401843113514"><a name="p174401843113514"></a><a name="p174401843113514"></a>POST</p>
<p id="p6440154310351"><a name="p6440154310351"></a><a name="p6440154310351"></a>/v2/{project_id}/fgs/functions</p>
</td>
</tr>
<tr id="row1644064311358"><td class="cellrowborder" valign="top"><p id="p175827595483"><a name="p175827595483"></a><a name="p175827595483"></a>delete_function(function_urn)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p184401143183513"><a name="p184401143183513"></a><a name="p184401143183513"></a>DELETE /v2/{project_id}/fgs/functions/{function_urn}</p>
</td>
</tr>
<tr id="row13440204383516"><td class="cellrowborder" valign="top"><p id="p1199116764916"><a name="p1199116764916"></a><a name="p1199116764916"></a>update_function_code(function_urn, **attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p1444014316357"><a name="p1444014316357"></a><a name="p1444014316357"></a>PUT /v2/{project_id}/fgs/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row1440114313510"><td class="cellrowborder" valign="top"><p id="p1387591210495"><a name="p1387591210495"></a><a name="p1387591210495"></a>update_function_metadata(function_urn, **attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p1244113439352"><a name="p1244113439352"></a><a name="p1244113439352"></a>PUT</p>
<p id="p16441843133513"><a name="p16441843133513"></a><a name="p16441843133513"></a>/v2/{project_id}/fgs/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row14441943183511"><td class="cellrowborder" valign="top"><p id="p88959174497"><a name="p88959174497"></a><a name="p88959174497"></a>publish_function_version(function_urn,**attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p19441144314359"><a name="p19441144314359"></a><a name="p19441144314359"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/versions</p>
</td>
</tr>
<tr id="row24419434357"><td class="cellrowborder" valign="top"><p id="p17322725134914"><a name="p17322725134914"></a><a name="p17322725134914"></a>get_function_version(function_urn,**attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p64411943103514"><a name="p64411943103514"></a><a name="p64411943103514"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/versions?marker={marker}&amp;maxitems={maxitems}</p>
</td>
</tr>
<tr id="row1441194310350"><td class="cellrowborder" valign="top"><p id="p77772029174914"><a name="p77772029174914"></a><a name="p77772029174914"></a>create_function_aliase(function_urn,**attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p164411743143515"><a name="p164411743143515"></a><a name="p164411743143515"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row11441443153514"><td class="cellrowborder" valign="top"><p id="p1754973454914"><a name="p1754973454914"></a><a name="p1754973454914"></a>update_function_aliase(function_urn,alias_name, **attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p15441124313352"><a name="p15441124313352"></a><a name="p15441124313352"></a>PUT /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row8441154319355"><td class="cellrowborder" valign="top"><p id="p1756820458490"><a name="p1756820458490"></a><a name="p1756820458490"></a>delete_function_aliase(function_urn,alias_name)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p6441194314358"><a name="p6441194314358"></a><a name="p6441194314358"></a>DELETE /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row6442194373512"><td class="cellrowborder" valign="top"><p id="p1048274916497"><a name="p1048274916497"></a><a name="p1048274916497"></a>get_function_aliase(function_urn,alias_name)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p154421743193518"><a name="p154421743193518"></a><a name="p154421743193518"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row134421343203513"><td class="cellrowborder" valign="top"><p id="p183774530496"><a name="p183774530496"></a><a name="p183774530496"></a>function_aliases(function_urn,**function)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p044274363516"><a name="p044274363516"></a><a name="p044274363516"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row5442134383512"><td class="cellrowborder" valign="top"><p id="p18794135984912"><a name="p18794135984912"></a><a name="p18794135984912"></a>execute_function_synchronously(function_urn,**attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p0442943103520"><a name="p0442943103520"></a><a name="p0442943103520"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/invocations</p>
</td>
</tr>
<tr id="row1544284383511"><td class="cellrowborder" valign="top"><p id="p1895515519500"><a name="p1895515519500"></a><a name="p1895515519500"></a>execute_function_asynchronously(function_urn,**attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p1844294353513"><a name="p1844294353513"></a><a name="p1844294353513"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/invocations-async</p>
</td>
</tr>
<tr id="row2044217434352"><td class="cellrowborder" rowspan="5" valign="top" width="10.94109410941094%"><p id="p44421543193510"><a name="p44421543193510"></a><a name="p44421543193510"></a>triggers</p>
</td>
<td class="cellrowborder" valign="top" width="39.563956395639565%"><p id="p19699111025020"><a name="p19699111025020"></a><a name="p19699111025020"></a>triggers(function_urn,**attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="49.494949494949495%"><p id="p194421543113510"><a name="p194421543113510"></a><a name="p194421543113510"></a>GET</p>
<p id="p1144210436353"><a name="p1144210436353"></a><a name="p1144210436353"></a>/v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row144423433355"><td class="cellrowborder" valign="top"><p id="p713251710502"><a name="p713251710502"></a><a name="p713251710502"></a>get_trigger(function_urn,trigger_type_code,trigger_id)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p17442144319359"><a name="p17442144319359"></a><a name="p17442144319359"></a>GET /v2/{project_id}/fgs/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
<tr id="row544264317356"><td class="cellrowborder" valign="top"><p id="p188839227501"><a name="p188839227501"></a><a name="p188839227501"></a>delete_all_triggers(function_urn)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p144422435359"><a name="p144422435359"></a><a name="p144422435359"></a>DELETE</p>
<p id="p1044213432351"><a name="p1044213432351"></a><a name="p1044213432351"></a>/v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row34421443183520"><td class="cellrowborder" valign="top"><p id="p31401828125018"><a name="p31401828125018"></a><a name="p31401828125018"></a>create_trigger(function_urn,**attrs)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p544317434352"><a name="p544317434352"></a><a name="p544317434352"></a>POST</p>
<p id="p244318435350"><a name="p244318435350"></a><a name="p244318435350"></a>/v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row84431543183511"><td class="cellrowborder" valign="top"><p id="p139814341505"><a name="p139814341505"></a><a name="p139814341505"></a>delete_trigger(function_urn,trigger_type_code,trigger_id)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p144431243103517"><a name="p144431243103517"></a><a name="p144431243103517"></a>DELETE /v2/{project_id}/fgs/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
</tbody>
</table>

