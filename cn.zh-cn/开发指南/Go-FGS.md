# Go-FGS<a name="ZH-CN_TOPIC_0187492665"></a>

基于函数工作流FGD v2 Go SDK的SDK接口如下，调用方式请参考示例代码。

<a name="table99661756144018"></a>
<table><thead align="left"><tr id="row620285718402"><th class="cellrowborder" valign="top" width="19.101910191019105%" id="mcps1.1.4.1.1"><p id="p162021573403"><a name="p162021573403"></a><a name="p162021573403"></a><strong id="b2202125754018"><a name="b2202125754018"></a><a name="b2202125754018"></a>Resource</strong></p>
</th>
<th class="cellrowborder" valign="top" width="37.07370737073707%" id="mcps1.1.4.1.2"><p id="p12202657184011"><a name="p12202657184011"></a><a name="p12202657184011"></a><strong id="b1920214578406"><a name="b1920214578406"></a><a name="b1920214578406"></a>Method</strong></p>
</th>
<th class="cellrowborder" valign="top" width="43.824382438243816%" id="mcps1.1.4.1.3"><p id="p10203155717409"><a name="p10203155717409"></a><a name="p10203155717409"></a><strong id="b1920385717403"><a name="b1920385717403"></a><a name="b1920385717403"></a>API</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row1520395712409"><td class="cellrowborder" rowspan="16" valign="top" width="19.101910191019105%" headers="mcps1.1.4.1.1 "><p id="p1820375714400"><a name="p1820375714400"></a><a name="p1820375714400"></a>Functions</p>
</td>
<td class="cellrowborder" valign="top" width="37.07370737073707%" headers="mcps1.1.4.1.2 "><p id="p1920318571404"><a name="p1920318571404"></a><a name="p1920318571404"></a>Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="43.824382438243816%" headers="mcps1.1.4.1.3 "><p id="p152038572407"><a name="p152038572407"></a><a name="p152038572407"></a>POST /v2/{project_id}/fgs/functions</p>
</td>
</tr>
<tr id="row132031257144013"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8203457124013"><a name="p8203457124013"></a><a name="p8203457124013"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15203157174017"><a name="p15203157174017"></a><a name="p15203157174017"></a>GET /v2/{project_id}/fgs/functions?{marker}=marker&amp;{maxitems}=maxitems</p>
</td>
</tr>
<tr id="row020319575406"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p320355716404"><a name="p320355716404"></a><a name="p320355716404"></a>GetMetadata(c *gophercloud.ServiceClient, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p162031957114012"><a name="p162031957114012"></a><a name="p162031957114012"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row620312579404"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6203175720403"><a name="p6203175720403"></a><a name="p6203175720403"></a>GetCode(c *gophercloud.ServiceClient, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5203115784011"><a name="p5203115784011"></a><a name="p5203115784011"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row6203105754011"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6203115713404"><a name="p6203115713404"></a><a name="p6203115713404"></a>Delete(c *gophercloud.ServiceClient, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13204357134016"><a name="p13204357134016"></a><a name="p13204357134016"></a>DELETE /v2/{project_id}/fgs/functions/{function_urn}</p>
</td>
</tr>
<tr id="row5204145720402"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1420414576409"><a name="p1420414576409"></a><a name="p1420414576409"></a>UpdateCode(c *gophercloud.ServiceClient, functionUrn string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6204155794013"><a name="p6204155794013"></a><a name="p6204155794013"></a>PUT  /v2/{project_id}/fgs/functions/{function_urn}/code</p>
</td>
</tr>
<tr id="row220425784018"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1220405774019"><a name="p1220405774019"></a><a name="p1220405774019"></a>UpdateMetadata(c *gophercloud.ServiceClient, functionUrn string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5204857144019"><a name="p5204857144019"></a><a name="p5204857144019"></a>PUT /v2/{project_id}/fgs/functions/{function_urn}/config</p>
</td>
</tr>
<tr id="row182047573404"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20204105714013"><a name="p20204105714013"></a><a name="p20204105714013"></a>CreateVersion(c *gophercloud.ServiceClient, opts CreateOptsBuilder, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p920445764012"><a name="p920445764012"></a><a name="p920445764012"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/versions</p>
</td>
</tr>
<tr id="row2204195754019"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1920495715403"><a name="p1920495715403"></a><a name="p1920495715403"></a>ListVersion(c *gophercloud.ServiceClient, opts ListOptsBuilder, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5204857154016"><a name="p5204857154016"></a><a name="p5204857154016"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/versions?marker={marker}&amp;maxitems={maxitems}</p>
</td>
</tr>
<tr id="row16204135715402"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p02057572401"><a name="p02057572401"></a><a name="p02057572401"></a>CreateAlias(c *gophercloud.ServiceClient, opts CreateOptsBuilder, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p182055571403"><a name="p182055571403"></a><a name="p182055571403"></a>POST /v2/{project_id}/fgs/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row5205165717404"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p112051157124014"><a name="p112051157124014"></a><a name="p112051157124014"></a>UpdateAlias(c *gophercloud.ServiceClient, functionUrn, aliasName string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1205157144010"><a name="p1205157144010"></a><a name="p1205157144010"></a>PUT /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row14205657184011"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9205165720402"><a name="p9205165720402"></a><a name="p9205165720402"></a>DeleteAlias(c *gophercloud.ServiceClient, functionUrn, aliasName string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4205105713401"><a name="p4205105713401"></a><a name="p4205105713401"></a>DELETE  /v1.0/{project_id}/fss/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row7205135724018"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1820645774011"><a name="p1820645774011"></a><a name="p1820645774011"></a>GetAlias(c *gophercloud.ServiceClient, functionUrn, aliasName string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3206195734016"><a name="p3206195734016"></a><a name="p3206195734016"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/aliases/{alias_name}</p>
</td>
</tr>
<tr id="row15206175714014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p52062579405"><a name="p52062579405"></a><a name="p52062579405"></a>ListAlias(c *gophercloud.ServiceClient, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p102061257174016"><a name="p102061257174016"></a><a name="p102061257174016"></a>GET /v2/{project_id}/fgs/functions/{function_urn}/aliases</p>
</td>
</tr>
<tr id="row10206657104015"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1320618575402"><a name="p1320618575402"></a><a name="p1320618575402"></a>Invoke(c *gophercloud.ServiceClient, m map[string]interface{}, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p112061457174018"><a name="p112061457174018"></a><a name="p112061457174018"></a>POST  /v2/{project_id}/fgs/functions/{function_urn}/invocations</p>
</td>
</tr>
<tr id="row320645717405"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14206257124014"><a name="p14206257124014"></a><a name="p14206257124014"></a>AsyncInvoke(c *gophercloud.ServiceClient, m map[string]interface{}, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1620614574408"><a name="p1620614574408"></a><a name="p1620614574408"></a>POST  /v2/{project_id}/fgs/functions/{function_urn}/invocations-async</p>
</td>
</tr>
<tr id="row22062057204018"><td class="cellrowborder" rowspan="5" valign="top" width="19.101910191019105%" headers="mcps1.1.4.1.1 "><p id="p102061157154018"><a name="p102061157154018"></a><a name="p102061157154018"></a>Triggers</p>
</td>
<td class="cellrowborder" valign="top" width="37.07370737073707%" headers="mcps1.1.4.1.2 "><p id="p102071957184015"><a name="p102071957184015"></a><a name="p102071957184015"></a>List(c *gophercloud.ServiceClient, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" width="43.824382438243816%" headers="mcps1.1.4.1.3 "><p id="p220735716404"><a name="p220735716404"></a><a name="p220735716404"></a>GET /v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row182075571407"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3207105734013"><a name="p3207105734013"></a><a name="p3207105734013"></a>Create(c *gophercloud.ServiceClient, opts CreateOptsBuilder, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p22071957134013"><a name="p22071957134013"></a><a name="p22071957134013"></a>POST /v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
<tr id="row20207357184011"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12073570406"><a name="p12073570406"></a><a name="p12073570406"></a>Delete(c *gophercloud.ServiceClient, functionUrn, triggerTypeCode, triggerId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11207175774012"><a name="p11207175774012"></a><a name="p11207175774012"></a>DELETE /v2/{project_id}/fgs/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
<tr id="row16207757114016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p172072057114019"><a name="p172072057114019"></a><a name="p172072057114019"></a>Get(c *gophercloud.ServiceClient, functionUrn, triggerTypeCode, triggerId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1820718574408"><a name="p1820718574408"></a><a name="p1820718574408"></a>GET /v2/{project_id}/fgs/triggers/{function_urn}/{trigger_type_code}/{trigger_id}</p>
</td>
</tr>
<tr id="row1320725784018"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p62071057184010"><a name="p62071057184010"></a><a name="p62071057184010"></a>DeleteAll(c *gophercloud.ServiceClient, functionUrn string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2207125710407"><a name="p2207125710407"></a><a name="p2207125710407"></a>DELETE /v2/{project_id}/fgs/triggers/{function_urn}</p>
</td>
</tr>
</tbody>
</table>

