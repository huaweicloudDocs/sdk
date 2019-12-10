# Python-IAM<a name="ZH-CN_TOPIC_0070868140"></a>

基于IAM API的SDK接口如下，调用方式请参考示例代码。

<a name="table074810952016"></a>
<table><thead align="left"><tr id="row1796218918207"><th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.1.4.1.1"><p id="p99624915209"><a name="p99624915209"></a><a name="p99624915209"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.39393939393939%" id="mcps1.1.4.1.2"><p id="p149623911203"><a name="p149623911203"></a><a name="p149623911203"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="43.43434343434344%" id="mcps1.1.4.1.3"><p id="p119625916202"><a name="p119625916202"></a><a name="p119625916202"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1696239182011"><td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p169628912020"><a name="p169628912020"></a><a name="p169628912020"></a>Securitytoken Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p69629912015"><a name="p69629912015"></a><a name="p69629912015"></a>create_securitytoken(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p796217918205"><a name="p796217918205"></a><a name="p796217918205"></a>POST /v3.0/OS-CREDENTIAL/securitytokens</p>
<p id="p2962139152017"><a name="p2962139152017"></a><a name="p2962139152017"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0097949518.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1496219152014"><td class="cellrowborder" rowspan="2" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p696213913209"><a name="p696213913209"></a><a name="p696213913209"></a>Region Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p13962893203"><a name="p13962893203"></a><a name="p13962893203"></a>regions(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p39621999207"><a name="p39621999207"></a><a name="p39621999207"></a>GET /v3/regions</p>
<p id="p89621895209"><a name="p89621895209"></a><a name="p89621895209"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148043.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row896212982012"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1396216915208"><a name="p1396216915208"></a><a name="p1396216915208"></a>get_region(self, region)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p49623982016"><a name="p49623982016"></a><a name="p49623982016"></a>GET /v3/regions/{region_id}</p>
<p id="p2962192200"><a name="p2962192200"></a><a name="p2962192200"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148044.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row139626952016"><td class="cellrowborder" rowspan="6" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p696218982014"><a name="p696218982014"></a><a name="p696218982014"></a>Project Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p296316914201"><a name="p296316914201"></a><a name="p296316914201"></a>projects(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p183511525154219"><a name="p183511525154219"></a><a name="p183511525154219"></a>GET /v3/projects</p>
<p id="p1796319922011"><a name="p1796319922011"></a><a name="p1796319922011"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39637962012"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p99631972019"><a name="p99631972019"></a><a name="p99631972019"></a>list_user_projects(self, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p129636972020"><a name="p129636972020"></a><a name="p129636972020"></a>GET /v3/users/{user_id}/projects</p>
<p id="p2963139152020"><a name="p2963139152020"></a><a name="p2963139152020"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845622.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row596311919204"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2963199182013"><a name="p2963199182013"></a><a name="p2963199182013"></a>get_project_scopes(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p159632918203"><a name="p159632918203"></a><a name="p159632918203"></a>GET /v3/auth/projects</p>
<p id="p199631490207"><a name="p199631490207"></a><a name="p199631490207"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845558.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row296313922015"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p159637962014"><a name="p159637962014"></a><a name="p159637962014"></a>create_project(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p169637920206"><a name="p169637920206"></a><a name="p169637920206"></a>POST /v3/projects</p>
<p id="p1596316913209"><a name="p1596316913209"></a><a name="p1596316913209"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0066154565.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12963198209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1996319172019"><a name="p1996319172019"></a><a name="p1996319172019"></a>update_project(self, project, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1796379102010"><a name="p1796379102010"></a><a name="p1796379102010"></a>PATCH /v3/projects/{project_id}</p>
<p id="p496369152012"><a name="p496369152012"></a><a name="p496369152012"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0066154566.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2963209112015"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p696314914208"><a name="p696314914208"></a><a name="p696314914208"></a>get_project(self, project)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p296314952010"><a name="p296314952010"></a><a name="p296314952010"></a>GET /v3/projects/{project_id}</p>
<p id="p149639982013"><a name="p149639982013"></a><a name="p149639982013"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0066154567.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row89631992013"><td class="cellrowborder" rowspan="9" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p29641392206"><a name="p29641392206"></a><a name="p29641392206"></a>User Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p59641912202"><a name="p59641912202"></a><a name="p59641912202"></a>list_group_users(self, group_id)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p12964796209"><a name="p12964796209"></a><a name="p12964796209"></a>GET /v3/groups/{group_id}/users</p>
<p id="p1496410922017"><a name="p1496410922017"></a><a name="p1496410922017"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845561.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row89648910206"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p79641982010"><a name="p79641982010"></a><a name="p79641982010"></a>remove_user_from_group(self, group_id, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1696489142017"><a name="p1696489142017"></a><a name="p1696489142017"></a>DELETE /v3/groups/{group_id}/users/{user_id}</p>
<p id="p096420962015"><a name="p096420962015"></a><a name="p096420962015"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845601.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row59642942014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p39641893203"><a name="p39641893203"></a><a name="p39641893203"></a>users(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p199641293209"><a name="p199641293209"></a><a name="p199641293209"></a>GET /v3/users</p>
<p id="p296418916203"><a name="p296418916203"></a><a name="p296418916203"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845638.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0964189142020"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19964496207"><a name="p19964496207"></a><a name="p19964496207"></a>get_user(self, user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8964593201"><a name="p8964593201"></a><a name="p8964593201"></a>GET /v3/users/{user_id}</p>
<p id="p09645918201"><a name="p09645918201"></a><a name="p09645918201"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845652.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1196414916209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p169641395207"><a name="p169641395207"></a><a name="p169641395207"></a>list_user_groups(self, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1196439112018"><a name="p1196439112018"></a><a name="p1196439112018"></a>GET /v3/users/{user_id}/groups</p>
<p id="p39647915201"><a name="p39647915201"></a><a name="p39647915201"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845554.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row396420910206"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9964199102014"><a name="p9964199102014"></a><a name="p9964199102014"></a>create_user(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7964894209"><a name="p7964894209"></a><a name="p7964894209"></a>POST /v3/users</p>
<p id="p1964119182010"><a name="p1964119182010"></a><a name="p1964119182010"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845637.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row199641094204"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p169643942014"><a name="p169643942014"></a><a name="p169643942014"></a>change_password(self, user_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p79641195200"><a name="p79641195200"></a><a name="p79641195200"></a>POST /v3/users/{user_id}/password</p>
<p id="p159641913207"><a name="p159641913207"></a><a name="p159641913207"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845653.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row796489112011"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p59642910207"><a name="p59642910207"></a><a name="p59642910207"></a>update_user(self, user, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2096409112015"><a name="p2096409112015"></a><a name="p2096409112015"></a>PATCH /v3/users/{user_id}</p>
<p id="p119648912012"><a name="p119648912012"></a><a name="p119648912012"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845611.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8964293205"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p149643972014"><a name="p149643972014"></a><a name="p149643972014"></a>delete_user(self, user, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5965194203"><a name="p5965194203"></a><a name="p5965194203"></a>DELETE /v3/users/{user_id}</p>
<p id="p16965119122020"><a name="p16965119122020"></a><a name="p16965119122020"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845630.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row196512972017"><td class="cellrowborder" rowspan="3" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p9965169172011"><a name="p9965169172011"></a><a name="p9965169172011"></a>Domain Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p189658992013"><a name="p189658992013"></a><a name="p189658992013"></a>get_domain_scopes(self)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p11965139192015"><a name="p11965139192015"></a><a name="p11965139192015"></a>GET /v3/auth/domains</p>
<p id="p13965892207"><a name="p13965892207"></a><a name="p13965892207"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845574.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row179653919202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p119658915202"><a name="p119658915202"></a><a name="p119658915202"></a>get_password_config(self, domain_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p99651893203"><a name="p99651893203"></a><a name="p99651893203"></a>GET /v3/domains/{domain_id}/config/security_compliance</p>
<p id="p09659952017"><a name="p09659952017"></a><a name="p09659952017"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5965179182020"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1296569132019"><a name="p1296569132019"></a><a name="p1296569132019"></a>get_password_config_by_option(self, domain_id, option)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p99651995204"><a name="p99651995204"></a><a name="p99651995204"></a>GET /v3/domains/{domain_id}/config/security_compliance/{option}</p>
<p id="p896520922013"><a name="p896520922013"></a><a name="p896520922013"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0113.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2965598206"><td class="cellrowborder" rowspan="7" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p1965697203"><a name="p1965697203"></a><a name="p1965697203"></a>Group Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p199651395201"><a name="p199651395201"></a><a name="p199651395201"></a>groups(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p195601214320"><a name="p195601214320"></a><a name="p195601214320"></a>GET /v3/groups</p>
<p id="p696520982010"><a name="p696520982010"></a><a name="p696520982010"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845602.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1596519912016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p139657918208"><a name="p139657918208"></a><a name="p139657918208"></a>get_group(self, group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11965159172010"><a name="p11965159172010"></a><a name="p11965159172010"></a>GET /v3/groups/{group_id}</p>
<p id="p10965199192011"><a name="p10965199192011"></a><a name="p10965199192011"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845618.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row296549162018"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1296518942018"><a name="p1296518942018"></a><a name="p1296518942018"></a>create_group(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p99655922019"><a name="p99655922019"></a><a name="p99655922019"></a>POST /v3/groups</p>
<p id="p29651090200"><a name="p29651090200"></a><a name="p29651090200"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845650.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row169659918202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p096516972014"><a name="p096516972014"></a><a name="p096516972014"></a>add_user_to_group(self, group_id, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10965149122020"><a name="p10965149122020"></a><a name="p10965149122020"></a>PUT /v3/groups/{group_id}/users/{user_id}</p>
<p id="p4965194205"><a name="p4965194205"></a><a name="p4965194205"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845654.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1896511932013"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p29651091207"><a name="p29651091207"></a><a name="p29651091207"></a>update_group(self, group, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1796512911208"><a name="p1796512911208"></a><a name="p1796512911208"></a>PATCH /v3/groups/{group_id}</p>
<p id="p69665919206"><a name="p69665919206"></a><a name="p69665919206"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845600.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1966593201"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p096639182013"><a name="p096639182013"></a><a name="p096639182013"></a>delete_group(self, group, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19668917207"><a name="p19668917207"></a><a name="p19668917207"></a>DELETE /v3/groups/{group_id}</p>
<p id="p496669102012"><a name="p496669102012"></a><a name="p496669102012"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845566.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1966192207"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p09663922014"><a name="p09663922014"></a><a name="p09663922014"></a>check_group_user(self, group_id, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11966597207"><a name="p11966597207"></a><a name="p11966597207"></a>HEAD /v3/groups/{group_id}/users/{user_id}</p>
<p id="p79669932017"><a name="p79669932017"></a><a name="p79669932017"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845599.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row696629132017"><td class="cellrowborder" rowspan="10" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p15966119162013"><a name="p15966119162013"></a><a name="p15966119162013"></a>Role Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p139661916206"><a name="p139661916206"></a><a name="p139661916206"></a>list_domain_user_group_role(self, domain_id, group_id)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p0966791208"><a name="p0966791208"></a><a name="p0966791208"></a>GET /v3/domains/{domain_id}/groups/{group_id}/roles</p>
<p id="p89667917205"><a name="p89667917205"></a><a name="p89667917205"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845571.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7966119172014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1996689142013"><a name="p1996689142013"></a><a name="p1996689142013"></a>list_project_user_group_role(self, project_id, group_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p196613919201"><a name="p196613919201"></a><a name="p196613919201"></a>GET /v3/projects/{project_id}/groups/{group_id}/roles</p>
<p id="p4966898205"><a name="p4966898205"></a><a name="p4966898205"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845640.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39666962010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p89661796206"><a name="p89661796206"></a><a name="p89661796206"></a>roles(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3966193204"><a name="p3966193204"></a><a name="p3966193204"></a>GET /v3/roles</p>
<p id="p169667911201"><a name="p169667911201"></a><a name="p169667911201"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845591.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6966197206"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p696615982019"><a name="p696615982019"></a><a name="p696615982019"></a>get_role(self, role)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12966894208"><a name="p12966894208"></a><a name="p12966894208"></a>GET /v3/roles/{role_id}</p>
<p id="p296610922013"><a name="p296610922013"></a><a name="p296610922013"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845603.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row199661696204"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3967894204"><a name="p3967894204"></a><a name="p3967894204"></a>grant_domain_group_role(self, domain_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p896713915205"><a name="p896713915205"></a><a name="p896713915205"></a>PUT /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p1696779162017"><a name="p1696779162017"></a><a name="p1696779162017"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845623.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row129673952010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p109671698204"><a name="p109671698204"></a><a name="p109671698204"></a>grant_project_group_role(self, project_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p119671991206"><a name="p119671991206"></a><a name="p119671991206"></a>PUT /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p1996712912011"><a name="p1996712912011"></a><a name="p1996712912011"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845597.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19671091202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1996718962019"><a name="p1996718962019"></a><a name="p1996718962019"></a>delete_project_group_role(self, project_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p119670952014"><a name="p119670952014"></a><a name="p119670952014"></a>DELETE /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p79677922017"><a name="p79677922017"></a><a name="p79677922017"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845572.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row596710919209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p209674912015"><a name="p209674912015"></a><a name="p209674912015"></a>delete_domain_group_role(self, domain_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p296713920204"><a name="p296713920204"></a><a name="p296713920204"></a>DELETE /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p19675912011"><a name="p19675912011"></a><a name="p19675912011"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845560.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39670912209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19967109142016"><a name="p19967109142016"></a><a name="p19967109142016"></a>check_domain_group_role(self, domain_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p196713932017"><a name="p196713932017"></a><a name="p196713932017"></a>HEAD /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p89675972018"><a name="p89675972018"></a><a name="p89675972018"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845632.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row159671913209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0967179172017"><a name="p0967179172017"></a><a name="p0967179172017"></a>check_project_group_role(self, project_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1696711982019"><a name="p1696711982019"></a><a name="p1696711982019"></a>HEAD /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p19967097209"><a name="p19967097209"></a><a name="p19967097209"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845620.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row996729122011"><td class="cellrowborder" rowspan="2" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p596719916202"><a name="p596719916202"></a><a name="p596719916202"></a>Service Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p129677962016"><a name="p129677962016"></a><a name="p129677962016"></a>services(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p17301141804317"><a name="p17301141804317"></a><a name="p17301141804317"></a>GET /v3/services</p>
<p id="p8968292207"><a name="p8968292207"></a><a name="p8968292207"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845587.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row159681694207"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p596889182014"><a name="p596889182014"></a><a name="p596889182014"></a>get_service(self, service)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1896839122017"><a name="p1896839122017"></a><a name="p1896839122017"></a>GET /v3/services/{service_id}</p>
<p id="p196814932014"><a name="p196814932014"></a><a name="p196814932014"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148045.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row196879152018"><td class="cellrowborder" rowspan="2" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p396889132012"><a name="p396889132012"></a><a name="p396889132012"></a>Endpoint Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p996818918208"><a name="p996818918208"></a><a name="p996818918208"></a>endpoints(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p179687910205"><a name="p179687910205"></a><a name="p179687910205"></a>GET /v3/endpoints</p>
<p id="p2096817916206"><a name="p2096817916206"></a><a name="p2096817916206"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845562.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row396818912202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p109687918207"><a name="p109687918207"></a><a name="p109687918207"></a>get_endpoint(self, endpoint)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p199685992012"><a name="p199685992012"></a><a name="p199685992012"></a>GET /v3/endpoints/{endpoint_id}</p>
<p id="p1696815917202"><a name="p1696815917202"></a><a name="p1696815917202"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148046.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

