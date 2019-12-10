# Java-FGS<a name="ZH-CN_TOPIC_0187492663"></a>

基于FGS v1.0 JAVA API的SDK接口如下，调用方式请参考示例代码。

<a name="table750161062210"></a>
<table><thead align="left"><tr id="row1184521022216"><th class="cellrowborder" valign="top" width="17.98%" id="mcps1.1.4.1.1"><p id="p38463102221"><a name="p38463102221"></a><a name="p38463102221"></a><strong id="b9846151072211"><a name="b9846151072211"></a><a name="b9846151072211"></a>Resource</strong></p>
</th>
<th class="cellrowborder" valign="top" width="39.32%" id="mcps1.1.4.1.2"><p id="p8846131002220"><a name="p8846131002220"></a><a name="p8846131002220"></a><strong id="b28461310162211"><a name="b28461310162211"></a><a name="b28461310162211"></a>Method</strong></p>
</th>
<th class="cellrowborder" valign="top" width="42.699999999999996%" id="mcps1.1.4.1.3"><p id="p208461010102211"><a name="p208461010102211"></a><a name="p208461010102211"></a><strong id="b9846510152213"><a name="b9846510152213"></a><a name="b9846510152213"></a>API</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row188469103221"><td class="cellrowborder" rowspan="9" valign="top" width="17.98%" headers="mcps1.1.4.1.1 "><p id="p1846111019224"><a name="p1846111019224"></a><a name="p1846111019224"></a>Functions</p>
</td>
<td class="cellrowborder" valign="top" width="39.32%" headers="mcps1.1.4.1.2 "><p id="p98461610102218"><a name="p98461610102218"></a><a name="p98461610102218"></a>FunctionMetadata.Functions listFunction(int marker, int maxItems)</p>
</td>
<td class="cellrowborder" valign="top" width="42.699999999999996%" headers="mcps1.1.4.1.3 "><p id="p2847121013225"><a name="p2847121013225"></a><a name="p2847121013225"></a>GET /v1.0/{project_id}/fss/functions?marker={marker}&amp;maxitems={maxitems}</p>
</td>
</tr>
<tr id="row384713101224"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20847171015226"><a name="p20847171015226"></a><a name="p20847171015226"></a>FunctionMetadata getFunctionMetadata(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p584713104220"><a name="p584713104220"></a><a name="p584713104220"></a>GET /v1.0/{project_id}/fss/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row784751016227"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18847131092214"><a name="p18847131092214"></a><a name="p18847131092214"></a>FunctionMetadata getFunctionCode(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14847191072219"><a name="p14847191072219"></a><a name="p14847191072219"></a>GET /v1.0/{project_id}/fss/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row14847101022219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6847310172219"><a name="p6847310172219"></a><a name="p6847310172219"></a>FunctionMetadata createFunction(FunctionMetadata functionMetadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1484711101222"><a name="p1484711101222"></a><a name="p1484711101222"></a>POST /v1.0/{project_id}/fss/functions</p>
</td>
</tr>
<tr id="row884821052218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11848010132212"><a name="p11848010132212"></a><a name="p11848010132212"></a>ActionResponse deleteFunction(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1084818105229"><a name="p1084818105229"></a><a name="p1084818105229"></a>DELETE /v1.0/{project_id}/fss/functions/{function_urn}</p>
</td>
</tr>
<tr id="row10848131092214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18481710132213"><a name="p18481710132213"></a><a name="p18481710132213"></a>FunctionMetadata updateFunctionCode(String function_urn, FunctionMetadata functionMetadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7848121013223"><a name="p7848121013223"></a><a name="p7848121013223"></a>PUT    /v1.0/{project_id}/fss/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row68480101224"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14848310152220"><a name="p14848310152220"></a><a name="p14848310152220"></a>FunctionMetadata updateFunctionConfig(String function_urn, FunctionMetadata functionMetadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10848410152213"><a name="p10848410152213"></a><a name="p10848410152213"></a>PUT /v1.0/{project_id}/fss/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row084991072216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p158492010112210"><a name="p158492010112210"></a><a name="p158492010112210"></a>String invokeFunction(String function_urn, Map&lt;?, ?&gt; data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16849111010221"><a name="p16849111010221"></a><a name="p16849111010221"></a>POST    /v1.0/{project_id}/fss/functions/{function_urn}/invocations</p>
</td>
</tr>
<tr id="row58491210192220"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1784911104223"><a name="p1784911104223"></a><a name="p1784911104223"></a>String asyncInvokeFunction(String function_urn, Map&lt;?, ?&gt; data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p188491710202218"><a name="p188491710202218"></a><a name="p188491710202218"></a>POST    /v1.0/{project_id}/fss/functions/{function_urn}/invocations-async</p>
</td>
</tr>
<tr id="row10849171020222"><td class="cellrowborder" rowspan="7" valign="top" width="17.98%" headers="mcps1.1.4.1.1 "><p id="p1084981016221"><a name="p1084981016221"></a><a name="p1084981016221"></a>Versions</p>
</td>
<td class="cellrowborder" valign="top" width="39.32%" headers="mcps1.1.4.1.2 "><p id="p108491108223"><a name="p108491108223"></a><a name="p108491108223"></a>FunctionMetadata PublishVersion(String function_urn, FunctionMetadata fmd);</p>
</td>
<td class="cellrowborder" valign="top" width="42.699999999999996%" headers="mcps1.1.4.1.3 "><p id="p1185018108226"><a name="p1185018108226"></a><a name="p1185018108226"></a>POST /v1.0/{project_id}/fss/functions/{function_urn}/versions</p>
</td>
</tr>
<tr id="row2085051017223"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p198501610172210"><a name="p198501610172210"></a><a name="p198501610172210"></a>FunctionMetadata.FunctionVersions listFunctionVersions(String function_urn, int marker, int maxItems)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1485051062214"><a name="p1485051062214"></a><a name="p1485051062214"></a>GET /v1.0/{project_id}/fss/functions/{function_urn}/versions?marker={marker}&amp;maxitems={maxitems}</p>
</td>
</tr>
<tr id="row485081016229"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9850141042211"><a name="p9850141042211"></a><a name="p9850141042211"></a>FunctionVersionAlias createVersionAlias(String function_urn, FunctionVersionAlias functionVersionAlias)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1385081082211"><a name="p1385081082211"></a><a name="p1385081082211"></a>POST /v1.0/{project_id}/fss/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row118508105221"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1385021013227"><a name="p1385021013227"></a><a name="p1385021013227"></a>FunctionVersionAlias  updateVersionAlias (String function_urn, FunctionVersionAlias functionVersionAlias)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p385041010227"><a name="p385041010227"></a><a name="p385041010227"></a>PUT /v1.0/{project_id}/fss/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row1285111107229"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p985111072215"><a name="p985111072215"></a><a name="p985111072215"></a>void DeleteVersionAlias(String function_urn, String alias_name);</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5851111082215"><a name="p5851111082215"></a><a name="p5851111082215"></a>DELETE    /v1.0/{project_id}/fss/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row16851410202210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p48516106229"><a name="p48516106229"></a><a name="p48516106229"></a>FunctionVersionAlias GetVersionAlias(String function_urn, String alias_name);</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p585181019223"><a name="p585181019223"></a><a name="p585181019223"></a>GET /v1.0/{project_id}/fss/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row188511106226"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14851910182217"><a name="p14851910182217"></a><a name="p14851910182217"></a>List&lt;FunctionVersionAlias&gt; ListVersionAlias(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7851210192217"><a name="p7851210192217"></a><a name="p7851210192217"></a>GET /v1.0/{project_id}/fss/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row2085151015228"><td class="cellrowborder" rowspan="5" valign="top" width="17.98%" headers="mcps1.1.4.1.1 "><p id="p1285201082213"><a name="p1285201082213"></a><a name="p1285201082213"></a>Triggers</p>
</td>
<td class="cellrowborder" valign="top" width="39.32%" headers="mcps1.1.4.1.2 "><p id="p20852610142212"><a name="p20852610142212"></a><a name="p20852610142212"></a>FunctionTrigger[] listTriggersForFunction(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" width="42.699999999999996%" headers="mcps1.1.4.1.3 "><p id="p1852510142215"><a name="p1852510142215"></a><a name="p1852510142215"></a>GET /v1.0/{project_id}/fss/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row985261092218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p158521710152213"><a name="p158521710152213"></a><a name="p158521710152213"></a>FunctionTriggers CreateTriggerInstance(String function_urn, FunctionTriggers functionTriggers)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10852201082212"><a name="p10852201082212"></a><a name="p10852201082212"></a>POST /v1.0/{project_id}/fss/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row68528100221"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p685211102226"><a name="p685211102226"></a><a name="p685211102226"></a>void DeleteTrigger(String function_urn, String trigger_type_code, String trigger_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p285211092210"><a name="p285211092210"></a><a name="p285211092210"></a>DELETE /v1.0/{project_id}/fss/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
<tr id="row28521310172213"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p98532106227"><a name="p98532106227"></a><a name="p98532106227"></a>FunctionTriggers&lt;?&gt; GetTriggerInstance(String function_urn, String trigger_type_code, String trigger_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p285381012211"><a name="p285381012211"></a><a name="p285381012211"></a>GET /v1.0/{project_id}/fss/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
<tr id="row98538103229"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58538101225"><a name="p58538101225"></a><a name="p58538101225"></a>void DeleteAllTriggersForFunction(String function_urn);</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1985321012227"><a name="p1985321012227"></a><a name="p1985321012227"></a>DELETE /v1.0/{project_id}/fss/triggers/{function_urn}</p>
</td>
</tr>
</tbody>
</table>

基于FGS v2.0 JAVA API的SDK接口如下，调用方式请参考示例代码。

<a name="table1960332932317"></a>
<table><thead align="left"><tr id="row69444297234"><th class="cellrowborder" valign="top" width="17.98%" id="mcps1.1.4.1.1"><p id="p1394417297236"><a name="p1394417297236"></a><a name="p1394417297236"></a><strong id="b20944129112314"><a name="b20944129112314"></a><a name="b20944129112314"></a>Resource</strong></p>
</th>
<th class="cellrowborder" valign="top" width="39.32%" id="mcps1.1.4.1.2"><p id="p194522942313"><a name="p194522942313"></a><a name="p194522942313"></a><strong id="b394511299231"><a name="b394511299231"></a><a name="b394511299231"></a>Method</strong></p>
</th>
<th class="cellrowborder" valign="top" width="42.699999999999996%" id="mcps1.1.4.1.3"><p id="p12945192916234"><a name="p12945192916234"></a><a name="p12945192916234"></a><strong id="b1794582912316"><a name="b1794582912316"></a><a name="b1794582912316"></a>API</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row7945129132315"><td class="cellrowborder" rowspan="13" valign="top" width="17.98%" headers="mcps1.1.4.1.1 "><p id="p394514292231"><a name="p394514292231"></a><a name="p394514292231"></a>Functions</p>
</td>
<td class="cellrowborder" valign="top" width="39.32%" headers="mcps1.1.4.1.2 "><p id="p12945192962316"><a name="p12945192962316"></a><a name="p12945192962316"></a>FunctionMetadata.Functions listFunction(int marker, int maxItems)</p>
</td>
<td class="cellrowborder" valign="top" width="42.699999999999996%" headers="mcps1.1.4.1.3 "><p id="p19945529192318"><a name="p19945529192318"></a><a name="p19945529192318"></a>GET /v2/{project_id}/fgs/functions?marker={marker}&amp;maxitems={maxitems}</p>
</td>
</tr>
<tr id="row17945202918231"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1094532982312"><a name="p1094532982312"></a><a name="p1094532982312"></a>FunctionMetadata.Functions listFunction()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18945162992318"><a name="p18945162992318"></a><a name="p18945162992318"></a>GET /v2/{project_id}/fgs/functions</p>
</td>
</tr>
<tr id="row0945192910232"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p394514298236"><a name="p394514298236"></a><a name="p394514298236"></a>FunctionMetadata getFunctionMetadata(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p59459296238"><a name="p59459296238"></a><a name="p59459296238"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row139450299231"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8945172992317"><a name="p8945172992317"></a><a name="p8945172992317"></a>FunctionMetadata getFunctionCode(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p494582911239"><a name="p494582911239"></a><a name="p494582911239"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row2094582919239"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14946182913233"><a name="p14946182913233"></a><a name="p14946182913233"></a>FunctionMetadata createFunction(FunctionMetadata functionMetadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11946429162310"><a name="p11946429162310"></a><a name="p11946429162310"></a>POST /v2/{project_id}/fgs/functions</p>
</td>
</tr>
<tr id="row594622912318"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1594617298239"><a name="p1594617298239"></a><a name="p1594617298239"></a>ActionResponse deleteFunction(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7946192918238"><a name="p7946192918238"></a><a name="p7946192918238"></a>DELETE /v2/{project_id}/fgs/functions/{function_urn}</p>
</td>
</tr>
<tr id="row12946829172319"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p794615291237"><a name="p794615291237"></a><a name="p794615291237"></a>FunctionMetadata updateFunctionCode(String function_urn, FunctionMetadata functionMetadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p199464294232"><a name="p199464294232"></a><a name="p199464294232"></a>PUT    /v2/{project_id}/fgs/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row1494619299232"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p294617294238"><a name="p294617294238"></a><a name="p294617294238"></a>FunctionMetadata updateFunctionConfig(String function_urn, FunctionMetadata functionMetadata)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p159465295237"><a name="p159465295237"></a><a name="p159465295237"></a>PUT /v2/{project_id}/fgs/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row11946162912238"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9947142982311"><a name="p9947142982311"></a><a name="p9947142982311"></a>FunctionMetadata createFunctionVersion(String function_urn, FunctionMetadata fmd);</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1994718298236"><a name="p1994718298236"></a><a name="p1994718298236"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/versions</p>
</td>
</tr>
<tr id="row12947729192312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p394792917232"><a name="p394792917232"></a><a name="p394792917232"></a>FunctionMetadata.FunctionVersions listFunctionVersion(String function_urn, int marker, int maxItems)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p139471929122319"><a name="p139471929122319"></a><a name="p139471929122319"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/versions?marker={marker}&amp;maxitems={maxitems}</p>
</td>
</tr>
<tr id="row1794792920238"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1494752918232"><a name="p1494752918232"></a><a name="p1494752918232"></a>FunctionMetadata.FunctionVersions listFunctionVersion(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p169471293235"><a name="p169471293235"></a><a name="p169471293235"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/versions</p>
</td>
</tr>
<tr id="row79471329172310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11947929172314"><a name="p11947929172314"></a><a name="p11947929172314"></a>FuncInvocations invokeFunction(String function_urn, Map&lt;?, ?&gt; data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1894712915234"><a name="p1894712915234"></a><a name="p1894712915234"></a>POST    /v2/{project_id}/fgs/functions/{function_urn}/invocations</p>
</td>
</tr>
<tr id="row1394792917232"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p169471429122312"><a name="p169471429122312"></a><a name="p169471429122312"></a>FuncInvocations asyncInvokeFunction(String function_urn, Map&lt;?, ?&gt; data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10947112912312"><a name="p10947112912312"></a><a name="p10947112912312"></a>POST  /v2/{project_id}/fgs/functions/{function_urn}/invocations-async</p>
</td>
</tr>
<tr id="row19947162902310"><td class="cellrowborder" rowspan="5" valign="top" width="17.98%" headers="mcps1.1.4.1.1 "><p id="p3947329112319"><a name="p3947329112319"></a><a name="p3947329112319"></a>Versions</p>
</td>
<td class="cellrowborder" valign="top" width="39.32%" headers="mcps1.1.4.1.2 "><p id="p19480293232"><a name="p19480293232"></a><a name="p19480293232"></a>FunctionVersionAlias createVersionAlias(String function_urn, FunctionVersionAlias functionVersionAlias)</p>
</td>
<td class="cellrowborder" valign="top" width="42.699999999999996%" headers="mcps1.1.4.1.3 "><p id="p10948229112316"><a name="p10948229112316"></a><a name="p10948229112316"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row209481529162312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1594811295237"><a name="p1594811295237"></a><a name="p1594811295237"></a>FunctionVersionAlias  updateVersionAlias (String function_urn, FunctionVersionAlias functionVersionAlias)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12948629162311"><a name="p12948629162311"></a><a name="p12948629162311"></a>PUT /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row10948112914230"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1094872942316"><a name="p1094872942316"></a><a name="p1094872942316"></a>ActionResponse deleteVersionAlias(String function_urn, String alias_name);</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p794852917237"><a name="p794852917237"></a><a name="p794852917237"></a>DELETE  /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row894842912320"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5948142962314"><a name="p5948142962314"></a><a name="p5948142962314"></a>FunctionVersionAlias getVersionAlias(String function_urn, String alias_name);</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p094882932318"><a name="p094882932318"></a><a name="p094882932318"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row1694811298238"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p09486295236"><a name="p09486295236"></a><a name="p09486295236"></a>List&lt;FunctionVersionAlias&gt; listVersionAlias(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5948152918236"><a name="p5948152918236"></a><a name="p5948152918236"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row1994816290235"><td class="cellrowborder" rowspan="5" valign="top" width="17.98%" headers="mcps1.1.4.1.1 "><p id="p119482293233"><a name="p119482293233"></a><a name="p119482293233"></a>Triggers</p>
</td>
<td class="cellrowborder" valign="top" width="39.32%" headers="mcps1.1.4.1.2 "><p id="p294919298238"><a name="p294919298238"></a><a name="p294919298238"></a>FunctionTrigger[] listTriggersForFunction(String function_urn)</p>
</td>
<td class="cellrowborder" valign="top" width="42.699999999999996%" headers="mcps1.1.4.1.3 "><p id="p1494917292232"><a name="p1494917292232"></a><a name="p1494917292232"></a>GET /v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row149491429112317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1894915292231"><a name="p1894915292231"></a><a name="p1894915292231"></a>FunctionTriggers createTriggerInstance(String function_urn, FunctionTriggers functionTriggers)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6949162952316"><a name="p6949162952316"></a><a name="p6949162952316"></a>POST /v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row6949529122313"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1094982914238"><a name="p1094982914238"></a><a name="p1094982914238"></a>ActionResponse deleteTrigger(String function_urn, String trigger_type_code, String trigger_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p994919297236"><a name="p994919297236"></a><a name="p994919297236"></a>DELETE /v2/{project_id}/fgs/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
<tr id="row99491329102311"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19949102932310"><a name="p19949102932310"></a><a name="p19949102932310"></a>FunctionTriggers&lt;?&gt; getTriggerInstance(String function_urn, String trigger_type_code, String trigger_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1994912296232"><a name="p1994912296232"></a><a name="p1994912296232"></a>GET /v2/{project_id}/fgs/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
<tr id="row1894972932313"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13949729172317"><a name="p13949729172317"></a><a name="p13949729172317"></a>ActionResponse deleteAllTriggersForFunction(String function_urn);</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19501292234"><a name="p19501292234"></a><a name="p19501292234"></a>DELETE /v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
</tbody>
</table>

