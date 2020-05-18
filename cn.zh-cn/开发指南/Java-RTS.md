# RTS<a name="sdk_11_0006"></a>

基于Heat v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table142838307145"></a>
<table><thead align="left"><tr id="row454613309141"><th class="cellrowborder" valign="top" width="28.48284828482848%" id="mcps1.1.4.1.1"><p id="p454623013149"><a name="p454623013149"></a><a name="p454623013149"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.263826382638264%" id="mcps1.1.4.1.2"><p id="p1254683012141"><a name="p1254683012141"></a><a name="p1254683012141"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.25332533253326%" id="mcps1.1.4.1.3"><p id="p18546730151411"><a name="p18546730151411"></a><a name="p18546730151411"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row654616309144"><td class="cellrowborder" rowspan="3" valign="top" width="28.48284828482848%" headers="mcps1.1.4.1.1 "><p id="p105463305144"><a name="p105463305144"></a><a name="p105463305144"></a>EventsService</p>
</td>
<td class="cellrowborder" valign="top" width="38.263826382638264%" headers="mcps1.1.4.1.2 "><p id="p5546153081418"><a name="p5546153081418"></a><a name="p5546153081418"></a>List&lt;? extends Event&gt; list(String stackName, String stackId)</p>
</td>
<td class="cellrowborder" valign="top" width="33.25332533253326%" headers="mcps1.1.4.1.3 "><p id="p654610300148"><a name="p654610300148"></a><a name="p654610300148"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/events</p>
</td>
</tr>
<tr id="row15461930191410"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16546430121410"><a name="p16546430121410"></a><a name="p16546430121410"></a>List&lt;? extends Event&gt; list(String stackName, String stackId, String resourceName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3546630141417"><a name="p3546630141417"></a><a name="p3546630141417"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/resources/{resource_name}/events</p>
</td>
</tr>
<tr id="row1254613018147"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10546193016148"><a name="p10546193016148"></a><a name="p10546193016148"></a>Event show(String stackName, String stackId, String resourceName, String eventId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p454633061418"><a name="p454633061418"></a><a name="p454633061418"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/resources/{resource_name}/events/{event_id}</p>
</td>
</tr>
<tr id="row13546163011419"><td class="cellrowborder" rowspan="3" valign="top" width="28.48284828482848%" headers="mcps1.1.4.1.1 "><p id="p14546143021416"><a name="p14546143021416"></a><a name="p14546143021416"></a>ResourcesService</p>
</td>
<td class="cellrowborder" valign="top" width="38.263826382638264%" headers="mcps1.1.4.1.2 "><p id="p175461530111413"><a name="p175461530111413"></a><a name="p175461530111413"></a>List&lt;? extends Resource&gt; list(String stackNameOrId)</p>
</td>
<td class="cellrowborder" valign="top" width="33.25332533253326%" headers="mcps1.1.4.1.3 "><p id="p1554615309146"><a name="p1554615309146"></a><a name="p1554615309146"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/resources</p>
</td>
</tr>
<tr id="row1554619308142"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17546730131418"><a name="p17546730131418"></a><a name="p17546730131418"></a>List&lt;? extends Resource&gt; list(String stackName, String stackId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p85482309143"><a name="p85482309143"></a><a name="p85482309143"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/resources</p>
</td>
</tr>
<tr id="row18548183011419"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p165481130111413"><a name="p165481130111413"></a><a name="p165481130111413"></a>Resource show(String stackName, String stackId, String resourceName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12548173021419"><a name="p12548173021419"></a><a name="p12548173021419"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/resources/{resource_name}</p>
</td>
</tr>
<tr id="row35488300147"><td class="cellrowborder" rowspan="3" valign="top" width="28.48284828482848%" headers="mcps1.1.4.1.1 "><p id="p6548153031418"><a name="p6548153031418"></a><a name="p6548153031418"></a>SoftwareConfigService</p>
</td>
<td class="cellrowborder" valign="top" width="38.263826382638264%" headers="mcps1.1.4.1.2 "><p id="p125486307144"><a name="p125486307144"></a><a name="p125486307144"></a>SoftwareConfig create(SoftwareConfig sc)</p>
</td>
<td class="cellrowborder" valign="top" width="33.25332533253326%" headers="mcps1.1.4.1.3 "><p id="p15482030171414"><a name="p15482030171414"></a><a name="p15482030171414"></a>POST /V1/{project_id}/software_configs</p>
</td>
</tr>
<tr id="row554853010147"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2548630131416"><a name="p2548630131416"></a><a name="p2548630131416"></a>ActionResponse delete(String configId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p854823011410"><a name="p854823011410"></a><a name="p854823011410"></a>DELETE /V1/{project_id}/software_configs/{software_config_id}</p>
</td>
</tr>
<tr id="row19548430111411"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p175481930171410"><a name="p175481930171410"></a><a name="p175481930171410"></a>SoftwareConfig show(String configId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11548330201412"><a name="p11548330201412"></a><a name="p11548330201412"></a>GET /V1/{project_id}/software_configs/{software_config_id}</p>
</td>
</tr>
<tr id="row155484307144"><td class="cellrowborder" rowspan="7" valign="top" width="28.48284828482848%" headers="mcps1.1.4.1.1 "><p id="p5548030121419"><a name="p5548030121419"></a><a name="p5548030121419"></a>StackService</p>
</td>
<td class="cellrowborder" valign="top" width="38.263826382638264%" headers="mcps1.1.4.1.2 "><p id="p16548130101413"><a name="p16548130101413"></a><a name="p16548130101413"></a>Stack create(StackCreate newStack)</p>
</td>
<td class="cellrowborder" valign="top" width="33.25332533253326%" headers="mcps1.1.4.1.3 "><p id="p1554815304143"><a name="p1554815304143"></a><a name="p1554815304143"></a>POST /V1/{project_id}/stacks</p>
</td>
</tr>
<tr id="row15548153071418"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6548143018144"><a name="p6548143018144"></a><a name="p6548143018144"></a>Stack create(String name, String template, Map&lt;String,String&gt; parameters, boolean disableRollback, Long timeOutMins)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p135481630111414"><a name="p135481630111414"></a><a name="p135481630111414"></a>POST /V1/{project_id}/stacks</p>
</td>
</tr>
<tr id="row145489306144"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1554816302144"><a name="p1554816302144"></a><a name="p1554816302144"></a>ActionResponse delete(String stackName, String stackId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4549230141412"><a name="p4549230141412"></a><a name="p4549230141412"></a>DELETE /V1/{project_id}/stacks/{stack_name}/{stack_id}</p>
</td>
</tr>
<tr id="row254983015145"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p55491530181419"><a name="p55491530181419"></a><a name="p55491530181419"></a>Stack getDetails(String stackName, String stackId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1549230201412"><a name="p1549230201412"></a><a name="p1549230201412"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}</p>
</td>
</tr>
<tr id="row185491630171416"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p125491830121410"><a name="p125491830121410"></a><a name="p125491830121410"></a>Stack getStackByName(String name)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1754911301147"><a name="p1754911301147"></a><a name="p1754911301147"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}</p>
</td>
</tr>
<tr id="row19549730101412"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18549430181415"><a name="p18549430181415"></a><a name="p18549430181415"></a>List&lt;? extends Stack&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1054963013141"><a name="p1054963013141"></a><a name="p1054963013141"></a>GET /V1/{project_id}/stacks</p>
</td>
</tr>
<tr id="row1549113016149"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1754913017142"><a name="p1754913017142"></a><a name="p1754913017142"></a>ActionResponse update(String stackName, String stackId, StackUpdate stackUpdate)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p105491630151413"><a name="p105491630151413"></a><a name="p105491630151413"></a>PUT /V1/{project_id}/stacks/{stack_name}/{stack_id}</p>
</td>
</tr>
<tr id="row19549193019149"><td class="cellrowborder" rowspan="6" valign="top" width="28.48284828482848%" headers="mcps1.1.4.1.1 "><p id="p10549630191420"><a name="p10549630191420"></a><a name="p10549630191420"></a>TemplateService</p>
</td>
<td class="cellrowborder" valign="top" width="38.263826382638264%" headers="mcps1.1.4.1.2 "><p id="p8549130111412"><a name="p8549130111412"></a><a name="p8549130111412"></a>Map&lt;String,Object&gt; getTemplateAsMap(String stackNameOrId)</p>
</td>
<td class="cellrowborder" valign="top" width="33.25332533253326%" headers="mcps1.1.4.1.3 "><p id="p0549930161411"><a name="p0549930161411"></a><a name="p0549930161411"></a>GET /V1/{project_id}/stacks/{stack_name}/template</p>
</td>
</tr>
<tr id="row8549230141413"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3549103013142"><a name="p3549103013142"></a><a name="p3549103013142"></a>Map&lt;String,Object&gt; getTemplateAsMap(String stackName, String stackId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8549330171414"><a name="p8549330171414"></a><a name="p8549330171414"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/template</p>
</td>
</tr>
<tr id="row11549330111411"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11549143061410"><a name="p11549143061410"></a><a name="p11549143061410"></a>String getTemplateAsString(String stackName, String stackId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p454914308145"><a name="p454914308145"></a><a name="p454914308145"></a>GET /V1/{project_id}/stacks/{stack_name}/{stack_id}/template</p>
</td>
</tr>
<tr id="row14549123021415"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11549130121416"><a name="p11549130121416"></a><a name="p11549130121416"></a>TemplateResponse validateTemplate(String template)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p75491530131410"><a name="p75491530131410"></a><a name="p75491530131410"></a>POST /V1/{project_id}/validate</p>
</td>
</tr>
<tr id="row654943071418"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4549203051418"><a name="p4549203051418"></a><a name="p4549203051418"></a>TemplateResponse validateTemplate(Template template)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14549830191413"><a name="p14549830191413"></a><a name="p14549830191413"></a>POST /V1/{project_id}/validate</p>
</td>
</tr>
<tr id="row05491630101416"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p054983031413"><a name="p054983031413"></a><a name="p054983031413"></a>TemplateResponse validateTemplateByURL(String templateURL)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6549183011144"><a name="p6549183011144"></a><a name="p6549183011144"></a>POST /V1/{project_id}/validate</p>
</td>
</tr>
</tbody>
</table>

