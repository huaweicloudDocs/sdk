# Go-AS<a name="ZH-CN_TOPIC_0168402939"></a>

基于AS v1 Go SDK的SDK接口如下，调用方式请参考示例代码。

<a name="table13788732172917"></a>
<table><thead align="left"><tr id="row04401185303"><th class="cellrowborder" valign="top" width="13.020000000000001%" id="mcps1.1.4.1.1"><p id="p3763296319273"><a name="p3763296319273"></a><a name="p3763296319273"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="45.989999999999995%" id="mcps1.1.4.1.2"><p id="p950753419273"><a name="p950753419273"></a><a name="p950753419273"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="40.99%" id="mcps1.1.4.1.3"><p id="p2230708619273"><a name="p2230708619273"></a><a name="p2230708619273"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row37533162911"><td class="cellrowborder" rowspan="5" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p1922184514118"><a name="p1922184514118"></a><a name="p1922184514118"></a>Configures</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p1246142525"><a name="p1246142525"></a><a name="p1246142525"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p12461725214"><a name="p12461725214"></a><a name="p12461725214"></a>POST /autoscaling-api/v1/{project_id}/scaling_configuration</p>
<p id="p135211520216"><a name="p135211520216"></a><a name="p135211520216"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063055.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row187143372920"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9465214214"><a name="p9465214214"></a><a name="p9465214214"></a>Delete(client *gophercloud.ServiceClient, scalingConfigurationId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10466213215"><a name="p10466213215"></a><a name="p10466213215"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_configuration/{scaling_configuration_id}</p>
<p id="p145815274216"><a name="p145815274216"></a><a name="p145815274216"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063060.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17203372917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4461125215"><a name="p4461125215"></a><a name="p4461125215"></a>DeleteWithBatch(client *gophercloud.ServiceClient, opts DeleteWithBatchOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p846192424"><a name="p846192424"></a><a name="p846192424"></a>POST /autoscaling-api/v1/{project_id}/scaling_configurations</p>
<p id="p1554012301626"><a name="p1554012301626"></a><a name="p1554012301626"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063049.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5793372913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4469213214"><a name="p4469213214"></a><a name="p4469213214"></a>Get(client *gophercloud.ServiceClient, scalingConfigurationId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17471221323"><a name="p17471221323"></a><a name="p17471221323"></a>GET /autoscaling-api/v1/{project_id}/scaling_configuration/{scaling_configuration_id}</p>
<p id="p1414553315210"><a name="p1414553315210"></a><a name="p1414553315210"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063052.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19763382910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p134710217214"><a name="p134710217214"></a><a name="p134710217214"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5471821326"><a name="p5471821326"></a><a name="p5471821326"></a>GET /autoscaling-api/v1/{project_id}/scaling_configuration</p>
<p id="p62377361128"><a name="p62377361128"></a><a name="p62377361128"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063056.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row67193352915"><td class="cellrowborder" rowspan="6" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p223810441323"><a name="p223810441323"></a><a name="p223810441323"></a>Groups</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p26471718832"><a name="p26471718832"></a><a name="p26471718832"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p56471718030"><a name="p56471718030"></a><a name="p56471718030"></a>POST /autoscaling-api/v1/{project_id}/scaling_group</p>
<p id="p5472434417"><a name="p5472434417"></a><a name="p5472434417"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063023.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1271233102916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p964715181033"><a name="p964715181033"></a><a name="p964715181033"></a>Delete(client *gophercloud.ServiceClient, scalingGroupId string, opts DeleteOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1364716181033"><a name="p1364716181033"></a><a name="p1364716181033"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p5351461444"><a name="p5351461444"></a><a name="p5351461444"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063041.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row207173313297"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6647818132"><a name="p6647818132"></a><a name="p6647818132"></a>Enable(client *gophercloud.ServiceClient, scalingGroupId string, opts EnableOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p864841819314"><a name="p864841819314"></a><a name="p864841819314"></a>POST /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}/action</p>
<p id="p324511920413"><a name="p324511920413"></a><a name="p324511920413"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063017.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1571433112910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1664816182031"><a name="p1664816182031"></a><a name="p1664816182031"></a>Get(client *gophercloud.ServiceClient,  scalingGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1064818182318"><a name="p1064818182318"></a><a name="p1064818182318"></a>GET /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p1637181210414"><a name="p1637181210414"></a><a name="p1637181210414"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063073.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row971339290"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1364815189311"><a name="p1364815189311"></a><a name="p1364815189311"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p76481518933"><a name="p76481518933"></a><a name="p76481518933"></a>GET /autoscaling-api/v1/{project_id}/scaling_group</p>
<p id="p777619141943"><a name="p777619141943"></a><a name="p777619141943"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063030.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row167816581023"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19648141814318"><a name="p19648141814318"></a><a name="p19648141814318"></a>Update(client *gophercloud.ServiceClient, scalingGroupId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56484180314"><a name="p56484180314"></a><a name="p56484180314"></a>PUT /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p1944519191243"><a name="p1944519191243"></a><a name="p1944519191243"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063036.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9723314299"><td class="cellrowborder" rowspan="3" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p179951844416"><a name="p179951844416"></a><a name="p179951844416"></a>Instances</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p4151845345"><a name="p4151845345"></a><a name="p4151845345"></a>Action(client *gophercloud.ServiceClient, scalingGroupId string, opts ActionOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p715134515412"><a name="p715134515412"></a><a name="p715134515412"></a>POST /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/action</p>
<p id="p195316431525"><a name="p195316431525"></a><a name="p195316431525"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063053.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row873333297"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3158455417"><a name="p3158455417"></a><a name="p3158455417"></a>Delete(client *gophercloud.ServiceClient, instanceId string, opts DeleteOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3151745041"><a name="p3151745041"></a><a name="p3151745041"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_group_instance/{instance_id}</p>
<p id="p86811049324"><a name="p86811049324"></a><a name="p86811049324"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063059.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row87533162913"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41511451745"><a name="p41511451745"></a><a name="p41511451745"></a>List(client *gophercloud.ServiceClient, scalingGroupId string, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1154458411"><a name="p1154458411"></a><a name="p1154458411"></a>GET /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/list</p>
<p id="p1664712523215"><a name="p1664712523215"></a><a name="p1664712523215"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063045.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row271133192910"><td class="cellrowborder" rowspan="7" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p484914472315"><a name="p484914472315"></a><a name="p484914472315"></a>LifecycleHooks</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p4452840552"><a name="p4452840552"></a><a name="p4452840552"></a>CallBack(client *gophercloud.ServiceClient,  scalingGroupId string, opts CallBackOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p1545212401054"><a name="p1545212401054"></a><a name="p1545212401054"></a>PUT /autoscaling-api/v1/{project_id}/scaling_instance_hook/{scaling_group_id}/callback</p>
<p id="p172281156622"><a name="p172281156622"></a><a name="p172281156622"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063028.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row37163312910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p64522401951"><a name="p64522401951"></a><a name="p64522401951"></a>Create(client *gophercloud.ServiceClient,scalingGroupId string, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14525408511"><a name="p14525408511"></a><a name="p14525408511"></a>POST /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}</p>
<p id="p1872719591925"><a name="p1872719591925"></a><a name="p1872719591925"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063074.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row07433112920"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p184521640857"><a name="p184521640857"></a><a name="p184521640857"></a>Delete(client *gophercloud.ServiceClient,scalingGroupId string,lifecycleHookName string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p164521040657"><a name="p164521040657"></a><a name="p164521040657"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p10886121317310"><a name="p10886121317310"></a><a name="p10886121317310"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063026.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19743382910"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p945212406516"><a name="p945212406516"></a><a name="p945212406516"></a>Get(client *gophercloud.ServiceClient, scalingGroupId string, lifecycleHookName string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p545314014511"><a name="p545314014511"></a><a name="p545314014511"></a>GET /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p163466161832"><a name="p163466161832"></a><a name="p163466161832"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063031.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1838214191156"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p114533402058"><a name="p114533402058"></a><a name="p114533402058"></a>List(client *gophercloud.ServiceClient, scalingGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14538401259"><a name="p14538401259"></a><a name="p14538401259"></a>GET /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/list</p>
<p id="p12738191819318"><a name="p12738191819318"></a><a name="p12738191819318"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10723392917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p124531840557"><a name="p124531840557"></a><a name="p124531840557"></a>ListWithSuspension(client *gophercloud.ServiceClient, scalingGroupId string, opts ListWithSuspensionOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p124531740459"><a name="p124531740459"></a><a name="p124531740459"></a>GET /autoscaling-api/v1/{project_id}/scaling_instance_hook/{scaling_group_id}/list</p>
<p id="p3681421936"><a name="p3681421936"></a><a name="p3681421936"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row147579151355"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174539401955"><a name="p174539401955"></a><a name="p174539401955"></a>Update(client *gophercloud.ServiceClient, scalingGroupId string, lifecycleHookName string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1445374016512"><a name="p1445374016512"></a><a name="p1445374016512"></a>PUT /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p1220052415320"><a name="p1220052415320"></a><a name="p1220052415320"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063040.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row178345506512"><td class="cellrowborder" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p117263591656"><a name="p117263591656"></a><a name="p117263591656"></a>Logs</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p07267594512"><a name="p07267594512"></a><a name="p07267594512"></a>List(client *gophercloud.ServiceClient, scalingGroupId string, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p272610591855"><a name="p272610591855"></a><a name="p272610591855"></a>GET /autoscaling-api/v1/{project_id}/scaling_activity_log/{scaling_group_id}</p>
<p id="p483483012316"><a name="p483483012316"></a><a name="p483483012316"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063071.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1371533102913"><td class="cellrowborder" rowspan="3" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p1919316401966"><a name="p1919316401966"></a><a name="p1919316401966"></a>Notifications</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p1619364016613"><a name="p1619364016613"></a><a name="p1619364016613"></a>Delete(client *gophercloud.ServiceClient, scalingGroupId string, topicUrn string)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p171944401161"><a name="p171944401161"></a><a name="p171944401161"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}/{topic_urn}</p>
<p id="p9682433434"><a name="p9682433434"></a><a name="p9682433434"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063035.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row571233152919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p61941340261"><a name="p61941340261"></a><a name="p61941340261"></a>ConfigNotification(client *gophercloud.ServiceClient, scalingGroupId string, opts ConfigNotificationOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p119416408617"><a name="p119416408617"></a><a name="p119416408617"></a>PUT /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}</p>
<p id="p78260360314"><a name="p78260360314"></a><a name="p78260360314"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063033.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16843320291"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4194640462"><a name="p4194640462"></a><a name="p4194640462"></a>List(client *gophercloud.ServiceClient, scalingGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p819414019615"><a name="p819414019615"></a><a name="p819414019615"></a>GET /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}</p>
<p id="p195719391317"><a name="p195719391317"></a><a name="p195719391317"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063054.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row540655345510"><td class="cellrowborder" rowspan="6" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p48689290713"><a name="p48689290713"></a><a name="p48689290713"></a>Policies</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p188688291174"><a name="p188688291174"></a><a name="p188688291174"></a>Action(client *gophercloud.ServiceClient, scalingPolicyId string, opts ActionOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p986952910713"><a name="p986952910713"></a><a name="p986952910713"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}/action</p>
<p id="p1334114433312"><a name="p1334114433312"></a><a name="p1334114433312"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063075.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row577113365610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1586919291774"><a name="p1586919291774"></a><a name="p1586919291774"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5869429374"><a name="p5869429374"></a><a name="p5869429374"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy</p>
<p id="p61058461132"><a name="p61058461132"></a><a name="p61058461132"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063062.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row191776195610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58697291778"><a name="p58697291778"></a><a name="p58697291778"></a>Delete(client *gophercloud.ServiceClient, scalingPolicyId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p186917293718"><a name="p186917293718"></a><a name="p186917293718"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p027534814314"><a name="p027534814314"></a><a name="p027534814314"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063065.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0889658165517"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15869529170"><a name="p15869529170"></a><a name="p15869529170"></a>Get(client *gophercloud.ServiceClient, scalingPolicyId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19869929271"><a name="p19869929271"></a><a name="p19869929271"></a>GET /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p171546511836"><a name="p171546511836"></a><a name="p171546511836"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063043.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1264825613559"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p786912918716"><a name="p786912918716"></a><a name="p786912918716"></a>List(client *gophercloud.ServiceClient, scalingGroupId string, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15869929076"><a name="p15869929076"></a><a name="p15869929076"></a>GET /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_group_id}/list</p>
<p id="p18847154738"><a name="p18847154738"></a><a name="p18847154738"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0134002033.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19893392915"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p08696294719"><a name="p08696294719"></a><a name="p08696294719"></a>Update(client *gophercloud.ServiceClient, scalingPolicyId string，opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1486972913713"><a name="p1486972913713"></a><a name="p1486972913713"></a>PUT /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p1372858333"><a name="p1372858333"></a><a name="p1372858333"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063080.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row24596362713"><td class="cellrowborder" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p73791342173"><a name="p73791342173"></a><a name="p73791342173"></a>PolicyLogs</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p1437954211711"><a name="p1437954211711"></a><a name="p1437954211711"></a>List(client *gophercloud.ServiceClient, scalingPolicyId string, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p18379642575"><a name="p18379642575"></a><a name="p18379642575"></a>GET /autoscaling-api/v1/{project_id}/scaling_policy_execute_log/{scaling_policy_id}</p>
<p id="p109610161848"><a name="p109610161848"></a><a name="p109610161848"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0102994869.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11911333290"><td class="cellrowborder" rowspan="2" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p1481414489"><a name="p1481414489"></a><a name="p1481414489"></a>Quotas</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p10815041481"><a name="p10815041481"></a><a name="p10815041481"></a>List(client *gophercloud.ServiceClient)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p17815144817"><a name="p17815144817"></a><a name="p17815144817"></a>GET /autoscaling-api/v1/{project_id}/quotas</p>
<p id="p1884411912414"><a name="p1884411912414"></a><a name="p1884411912414"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063063.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row891533172916"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19815542818"><a name="p19815542818"></a><a name="p19815542818"></a>ListWithInstances(client *gophercloud.ServiceClient, scalingGroupId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p881517417814"><a name="p881517417814"></a><a name="p881517417814"></a>GET /autoscaling-api/v1/{project_id}/quotas/{scaling_group_id}</p>
<p id="p1916952213416"><a name="p1916952213416"></a><a name="p1916952213416"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row993332295"><td class="cellrowborder" rowspan="4" valign="top" width="13.020000000000001%" headers="mcps1.1.4.1.1 "><p id="p1181564986"><a name="p1181564986"></a><a name="p1181564986"></a>Tags</p>
</td>
<td class="cellrowborder" valign="top" width="45.989999999999995%" headers="mcps1.1.4.1.2 "><p id="p0815204682"><a name="p0815204682"></a><a name="p0815204682"></a>ListResourceTags(client *gophercloud.ServiceClient, resourceType string, resourceId string)</p>
</td>
<td class="cellrowborder" valign="top" width="40.99%" headers="mcps1.1.4.1.3 "><p id="p148152041487"><a name="p148152041487"></a><a name="p148152041487"></a>GET /autoscaling-api/v1/{project_id}/{resource_type}/{resource_id}/tags</p>
<p id="p10863251644"><a name="p10863251644"></a><a name="p10863251644"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0066763618.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row29113313293"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2081510410816"><a name="p2081510410816"></a><a name="p2081510410816"></a>ListTenantTags(client *gophercloud.ServiceClient, resourceType string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p581513414812"><a name="p581513414812"></a><a name="p581513414812"></a>GET /autoscaling-api/v1/{project_id}/{resource_type}/tags</p>
<p id="p223316291440"><a name="p223316291440"></a><a name="p223316291440"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0066763617.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14919332295"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p138151410812"><a name="p138151410812"></a><a name="p138151410812"></a>ListInstanceTags(client *gophercloud.ServiceClient, resourceType string, opts InstanceOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p281515413812"><a name="p281515413812"></a><a name="p281515413812"></a>POST /autoscaling-api/v1/{project_id}/{resource_type}/resource_instances/action</p>
<p id="p41251321841"><a name="p41251321841"></a><a name="p41251321841"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0127174043.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1311143318299"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p681594181"><a name="p681594181"></a><a name="p681594181"></a>Update(client *gophercloud.ServiceClient, resourceType string, resourceId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p188162410820"><a name="p188162410820"></a><a name="p188162410820"></a>POST /autoscaling-api/v1/{project_id}/{resource_type}/{resource_id}/tags/action</p>
<p id="p10670337349"><a name="p10670337349"></a><a name="p10670337349"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0066763619.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于AS v2.0 Go SDK的SDK接口如下，调用方式请参考示例代码。

<a name="table394172911130"></a>
<table><thead align="left"><tr id="row1961329191318"><th class="cellrowborder" valign="top" width="19.01190119011901%" id="mcps1.1.4.1.1"><p id="p14777752101313"><a name="p14777752101313"></a><a name="p14777752101313"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="47.65476547654765%" id="mcps1.1.4.1.2"><p id="p1077715218131"><a name="p1077715218131"></a><a name="p1077715218131"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="p777785231311"><a name="p777785231311"></a><a name="p777785231311"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1796152961313"><td class="cellrowborder" rowspan="5" valign="top" width="19.01190119011901%" headers="mcps1.1.4.1.1 "><p id="p1273104631518"><a name="p1273104631518"></a><a name="p1273104631518"></a>Policies</p>
</td>
<td class="cellrowborder" valign="top" width="47.65476547654765%" headers="mcps1.1.4.1.2 "><p id="p95541305154"><a name="p95541305154"></a><a name="p95541305154"></a>Create(client *gophercloud.ServiceClient, opts CreateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p75548018159"><a name="p75548018159"></a><a name="p75548018159"></a>POST /autoscaling-api/v2/{project_id}/scaling_policy</p>
<p id="p755411021518"><a name="p755411021518"></a><a name="p755411021518"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0103010240.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row129652910137"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14554160141512"><a name="p14554160141512"></a><a name="p14554160141512"></a>Get(client *gophercloud.ServiceClient, scalingPolicyId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p175541507154"><a name="p175541507154"></a><a name="p175541507154"></a>GET /autoscaling-api/v2/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p755416031511"><a name="p755416031511"></a><a name="p755416031511"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0103010243.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6969290132"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p135541604152"><a name="p135541604152"></a><a name="p135541604152"></a>GetPolicyListByResourceID(client *gophercloud.ServiceClient, scalingResourceId string, opts ResourceListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p05541003157"><a name="p05541003157"></a><a name="p05541003157"></a>GET /autoscaling-api/v2/{project_id}/scaling_policy/{scaling_resource_id}/list</p>
<p id="p4554110111510"><a name="p4554110111510"></a><a name="p4554110111510"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0103010242.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1996142981313"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p175541041510"><a name="p175541041510"></a><a name="p175541041510"></a>Update(client *gophercloud.ServiceClient, scalingPolicyId string, opts UpdateOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8554170191512"><a name="p8554170191512"></a><a name="p8554170191512"></a>PUT /autoscaling-api/v2/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p1455418019159"><a name="p1455418019159"></a><a name="p1455418019159"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0103010241.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2965292138"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p255417051516"><a name="p255417051516"></a><a name="p255417051516"></a>List(client *gophercloud.ServiceClient, opts ListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p20555130181517"><a name="p20555130181517"></a><a name="p20555130181517"></a>GET /autoscaling-api/v2/{project_id}/scaling_policy</p>
<p id="p355530131518"><a name="p355530131518"></a><a name="p355530131518"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0131969082.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

