# IAM<a name="sdk_12_0001"></a>

基于IAM API的SDK接口如下，调用方式请参考示例代码。

<a name="table074810952016"></a>
<table><thead align="left"><tr id="row1796218918207"><th class="cellrowborder" valign="top" width="26.142614261426147%" id="mcps1.1.4.1.1"><p id="p99624915209"><a name="p99624915209"></a><a name="p99624915209"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.64396439643964%" id="mcps1.1.4.1.2"><p id="p149623911203"><a name="p149623911203"></a><a name="p149623911203"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.21342134213422%" id="mcps1.1.4.1.3"><p id="p119625916202"><a name="p119625916202"></a><a name="p119625916202"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row158331013174615"><td class="cellrowborder" rowspan="2" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p14819153134616"><a name="p14819153134616"></a><a name="p14819153134616"></a>AuthToken Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p1368402217469"><a name="p1368402217469"></a><a name="p1368402217469"></a>create_authtoken(self, attr, nocatalog=None)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p126841822104613"><a name="p126841822104613"></a><a name="p126841822104613"></a>POST /v3/auth/tokens</p>
<a name="ul10475141517523"></a><a name="ul10475141517523"></a><ul id="ul10475141517523"><li>获取用户token（使用密码）<a href="https://support.huaweicloud.com/api-iam/iam_30_0001.html" target="_blank" rel="noopener noreferrer">链接</a></li><li>获取用户token（使用密码+虚拟MFA）<a href="https://support.huaweicloud.com/api-iam/iam_03_0006.html" target="_blank" rel="noopener noreferrer">链接</a></li><li>获取委托Token<a href="https://support.huaweicloud.com/api-iam/iam_30_0003.html" target="_blank" rel="noopener noreferrer">链接</a></li></ul>
</td>
</tr>
<tr id="row1372514157461"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8684192264619"><a name="p8684192264619"></a><a name="p8684192264619"></a>validate_authtoken(self, x_subject_token, nocatalog=None):</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p79151614354"><a name="p79151614354"></a><a name="p79151614354"></a>GET /v3/auth/tokens</p>
<p id="p1591518149514"><a name="p1591518149514"></a><a name="p1591518149514"></a><a href="https://support.huaweicloud.com/api-iam/iam_30_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1696239182011"><td class="cellrowborder" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p5501184451114"><a name="p5501184451114"></a><a name="p5501184451114"></a>Securitytoken Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p0501164411118"><a name="p0501164411118"></a><a name="p0501164411118"></a>create_securitytoken(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p4501044151120"><a name="p4501044151120"></a><a name="p4501044151120"></a>POST /v3.0/OS-CREDENTIAL/securitytokens</p>
<a name="ul17348195012112"></a><a name="ul17348195012112"></a><ul id="ul17348195012112"><li>通过委托方式的<a href="https://support.huaweicloud.com/api-iam/iam_04_0101.html" target="_blank" rel="noopener noreferrer">链接</a></li><li>通过token方式的<a href="https://support.huaweicloud.com/api-iam/iam_04_0002.html" target="_blank" rel="noopener noreferrer">链接</a></li></ul>
</td>
</tr>
<tr id="row105164741419"><td class="cellrowborder" rowspan="5" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p11133533146"><a name="p11133533146"></a><a name="p11133533146"></a>Credential Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p1961678101518"><a name="p1961678101518"></a><a name="p1961678101518"></a>create_credential(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p661620813151"><a name="p661620813151"></a><a name="p661620813151"></a>POST /v3.0/OS-CREDENTIAL/credentials</p>
<p id="p1161648151511"><a name="p1161648151511"></a><a name="p1161648151511"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7858444131420"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4616383156"><a name="p4616383156"></a><a name="p4616383156"></a>credentials(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8616208151512"><a name="p8616208151512"></a><a name="p8616208151512"></a>GET /v3.0/OS-CREDENTIAL/credentials</p>
<p id="p146168810155"><a name="p146168810155"></a><a name="p146168810155"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1862511428143"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6616138181510"><a name="p6616138181510"></a><a name="p6616138181510"></a>get_credential(self, access_key)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16163811158"><a name="p16163811158"></a><a name="p16163811158"></a>GET /v3.0/OS-CREDENTIAL/credentials/{access_key}</p>
<p id="p16616158151513"><a name="p16616158151513"></a><a name="p16616158151513"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row24151540161410"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1261616831515"><a name="p1261616831515"></a><a name="p1261616831515"></a>update_credential(self, access_key, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8616178141512"><a name="p8616178141512"></a><a name="p8616178141512"></a>PUT /v3.0/OS-CREDENTIAL/credentials/{access_key}</p>
<p id="p1561688181517"><a name="p1561688181517"></a><a name="p1561688181517"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5366103817142"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15616168181513"><a name="p15616168181513"></a><a name="p15616168181513"></a>delete_credential(self, access_key)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4617158121516"><a name="p4617158121516"></a><a name="p4617158121516"></a>DELETE /v3.0/OS-CREDENTIAL/credentials/{access_key}</p>
<p id="p1261748201510"><a name="p1261748201510"></a><a name="p1261748201510"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1496219152014"><td class="cellrowborder" rowspan="2" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p696213913209"><a name="p696213913209"></a><a name="p696213913209"></a>Region Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p13962893203"><a name="p13962893203"></a><a name="p13962893203"></a>regions(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p39621999207"><a name="p39621999207"></a><a name="p39621999207"></a>GET /v3/regions</p>
<p id="p89621895209"><a name="p89621895209"></a><a name="p89621895209"></a><a href="https://support.huaweicloud.com/api-iam/iam_05_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row896212982012"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1396216915208"><a name="p1396216915208"></a><a name="p1396216915208"></a>get_region(self, region)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p49623982016"><a name="p49623982016"></a><a name="p49623982016"></a>GET /v3/regions/{region_id}</p>
<p id="p2962192200"><a name="p2962192200"></a><a name="p2962192200"></a><a href="https://support.huaweicloud.com/api-iam/iam_05_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row139626952016"><td class="cellrowborder" rowspan="6" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p696218982014"><a name="p696218982014"></a><a name="p696218982014"></a>Project Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p296316914201"><a name="p296316914201"></a><a name="p296316914201"></a>projects(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p183511525154219"><a name="p183511525154219"></a><a name="p183511525154219"></a>GET /v3/projects</p>
<p id="p1796319922011"><a name="p1796319922011"></a><a name="p1796319922011"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39637962012"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p99631972019"><a name="p99631972019"></a><a name="p99631972019"></a>list_user_projects(self, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p129636972020"><a name="p129636972020"></a><a name="p129636972020"></a>GET /v3/users/{user_id}/projects</p>
<p id="p2963139152020"><a name="p2963139152020"></a><a name="p2963139152020"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row596311919204"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2963199182013"><a name="p2963199182013"></a><a name="p2963199182013"></a>get_project_scopes(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p159632918203"><a name="p159632918203"></a><a name="p159632918203"></a>GET /v3/auth/projects</p>
<p id="p199631490207"><a name="p199631490207"></a><a name="p199631490207"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row296313922015"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p159637962014"><a name="p159637962014"></a><a name="p159637962014"></a>create_project(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p169637920206"><a name="p169637920206"></a><a name="p169637920206"></a>POST /v3/projects</p>
<p id="p1596316913209"><a name="p1596316913209"></a><a name="p1596316913209"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12963198209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1996319172019"><a name="p1996319172019"></a><a name="p1996319172019"></a>update_project(self, project, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1796379102010"><a name="p1796379102010"></a><a name="p1796379102010"></a>PATCH /v3/projects/{project_id}</p>
<p id="p496369152012"><a name="p496369152012"></a><a name="p496369152012"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2963209112015"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p696314914208"><a name="p696314914208"></a><a name="p696314914208"></a>get_project(self, project)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p296314952010"><a name="p296314952010"></a><a name="p296314952010"></a>GET /v3/projects/{project_id}</p>
<p id="p149639982013"><a name="p149639982013"></a><a name="p149639982013"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12620103318183"><td class="cellrowborder" rowspan="2" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p1126920229195"><a name="p1126920229195"></a><a name="p1126920229195"></a>Project Operations (iam)</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p1991916119197"><a name="p1991916119197"></a><a name="p1991916119197"></a>update_project_status(self, project_id, attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p17919141111194"><a name="p17919141111194"></a><a name="p17919141111194"></a>PUT /v3-ext/projects/{project_id}</p>
<p id="p691913116197"><a name="p691913116197"></a><a name="p691913116197"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1168563115180"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p891931112193"><a name="p891931112193"></a><a name="p891931112193"></a>get_project_details_and_status(self, project_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18919171121914"><a name="p18919171121914"></a><a name="p18919171121914"></a>GET /v3-ext/projects/{project_id}</p>
<p id="p19197111195"><a name="p19197111195"></a><a name="p19197111195"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7749132917189"><td class="cellrowborder" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p196674244214"><a name="p196674244214"></a><a name="p196674244214"></a>Domain Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p3919711141913"><a name="p3919711141913"></a><a name="p3919711141913"></a>get_domain_scopes(self)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p391941110199"><a name="p391941110199"></a><a name="p391941110199"></a>GET /v3/auth/domains</p>
<p id="p79191411101916"><a name="p79191411101916"></a><a name="p79191411101916"></a><a href="https://support.huaweicloud.com/api-iam/iam_07_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row659672715187"><td class="cellrowborder" rowspan="2" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p3744243182120"><a name="p3744243182120"></a><a name="p3744243182120"></a>PasswordConfig Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p09196112192"><a name="p09196112192"></a><a name="p09196112192"></a>get_password_config(self, domain_id)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p15919611181918"><a name="p15919611181918"></a><a name="p15919611181918"></a>GET /v3/domains/{domain_id}/config/security_compliance</p>
<p id="p20919711101910"><a name="p20919711101910"></a><a name="p20919711101910"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3225172518186"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11919911121918"><a name="p11919911121918"></a><a name="p11919911121918"></a>get_password_config_by_option(self, domain_id, option)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7919181181913"><a name="p7919181181913"></a><a name="p7919181181913"></a>GET /v3/domains/{domain_id}/config/security_compliance/{option}</p>
<p id="p15919411101912"><a name="p15919411101912"></a><a name="p15919411101912"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0113.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12946827229"><td class="cellrowborder" rowspan="8" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p1389752992519"><a name="p1389752992519"></a><a name="p1389752992519"></a>User Operations (identity)</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p872017395324"><a name="p872017395324"></a><a name="p872017395324"></a>users(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p8720439153215"><a name="p8720439153215"></a><a name="p8720439153215"></a>GET /v3/users</p>
<p id="p37201439113218"><a name="p37201439113218"></a><a name="p37201439113218"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row618117502218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p97201396321"><a name="p97201396321"></a><a name="p97201396321"></a>get_user(self, user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p87200397325"><a name="p87200397325"></a><a name="p87200397325"></a>GET /v3/users/{user_id}</p>
<p id="p2720183911325"><a name="p2720183911325"></a><a name="p2720183911325"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row89631992013"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17207392320"><a name="p17207392320"></a><a name="p17207392320"></a>list_group_users(self, group_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12720113933215"><a name="p12720113933215"></a><a name="p12720113933215"></a>GET /v3/groups/{group_id}/users</p>
<p id="p17205391325"><a name="p17205391325"></a><a name="p17205391325"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row89648910206"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13720193963216"><a name="p13720193963216"></a><a name="p13720193963216"></a>create_user(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17720133911325"><a name="p17720133911325"></a><a name="p17720133911325"></a>POST /v3/users</p>
<p id="p1872020390329"><a name="p1872020390329"></a><a name="p1872020390329"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row59642942014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p872013393328"><a name="p872013393328"></a><a name="p872013393328"></a>change_password(self, user_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1972012394329"><a name="p1972012394329"></a><a name="p1972012394329"></a>POST /v3/users/{user_id}/password</p>
<p id="p772053953214"><a name="p772053953214"></a><a name="p772053953214"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0964189142020"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1720163914329"><a name="p1720163914329"></a><a name="p1720163914329"></a>update_user(self, user, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p172043963216"><a name="p172043963216"></a><a name="p172043963216"></a>PATCH /v3/users/{user_id}</p>
<p id="p37202398326"><a name="p37202398326"></a><a name="p37202398326"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1196414916209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6720173912324"><a name="p6720173912324"></a><a name="p6720173912324"></a>delete_user(self, user, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p77201439143217"><a name="p77201439143217"></a><a name="p77201439143217"></a>DELETE /v3/users/{user_id}</p>
<p id="p7720133973210"><a name="p7720133973210"></a><a name="p7720133973210"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row396420910206"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2072143983214"><a name="p2072143983214"></a><a name="p2072143983214"></a>remove_user_from_group(self, group_id, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5721839173219"><a name="p5721839173219"></a><a name="p5721839173219"></a>DELETE /v3/groups/{group_id}/users/{user_id}</p>
<p id="p16721133973213"><a name="p16721133973213"></a><a name="p16721133973213"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row682681173511"><td class="cellrowborder" rowspan="4" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p3831162511354"><a name="p3831162511354"></a><a name="p3831162511354"></a>User Operations (iam)</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p1930918223350"><a name="p1930918223350"></a><a name="p1930918223350"></a>query_user_details(self, user_id)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p53097221352"><a name="p53097221352"></a><a name="p53097221352"></a>GET /v3.0/OS-USER/users/{user_id}</p>
<p id="p1830972214357"><a name="p1830972214357"></a><a name="p1830972214357"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row199641094204"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11309152253514"><a name="p11309152253514"></a><a name="p11309152253514"></a>create_user(self, **user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p530932210351"><a name="p530932210351"></a><a name="p530932210351"></a>POST /v3.0/OS-USER/users</p>
<p id="p9309182213351"><a name="p9309182213351"></a><a name="p9309182213351"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0015.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row796489112011"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1309522193516"><a name="p1309522193516"></a><a name="p1309522193516"></a>update_user_information(self, user_id, **user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17309202211350"><a name="p17309202211350"></a><a name="p17309202211350"></a>PUT /v3.0/OS-USER/users/{user_id}/info</p>
<p id="p53091122163510"><a name="p53091122163510"></a><a name="p53091122163510"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8964293205"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p930932203512"><a name="p930932203512"></a><a name="p930932203512"></a>update_user_information_by_admin(self, user_id, **user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53091122203510"><a name="p53091122203510"></a><a name="p53091122203510"></a>PUT /v3.0/OS-USER/users/{user_id}</p>
<p id="p230910227355"><a name="p230910227355"></a><a name="p230910227355"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2965598206"><td class="cellrowborder" rowspan="8" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p1965697203"><a name="p1965697203"></a><a name="p1965697203"></a>Group Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p153637234388"><a name="p153637234388"></a><a name="p153637234388"></a>groups(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p17363112333819"><a name="p17363112333819"></a><a name="p17363112333819"></a>GET /v3/groups</p>
<p id="p10363122314389"><a name="p10363122314389"></a><a name="p10363122314389"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1596519912016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4363122320383"><a name="p4363122320383"></a><a name="p4363122320383"></a>get_group(self, group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13363172311384"><a name="p13363172311384"></a><a name="p13363172311384"></a>GET /v3/groups/{group_id}</p>
<p id="p9363823163815"><a name="p9363823163815"></a><a name="p9363823163815"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row296549162018"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p133632237389"><a name="p133632237389"></a><a name="p133632237389"></a>create_group(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3363162323814"><a name="p3363162323814"></a><a name="p3363162323814"></a>POST /v3/groups</p>
<p id="p173635232386"><a name="p173635232386"></a><a name="p173635232386"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row169659918202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p123631223183810"><a name="p123631223183810"></a><a name="p123631223183810"></a>update_group(self, group, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7363142353815"><a name="p7363142353815"></a><a name="p7363142353815"></a>PATCH /v3/groups/{group_id}</p>
<p id="p8364152343812"><a name="p8364152343812"></a><a name="p8364152343812"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1896511932013"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1336462311383"><a name="p1336462311383"></a><a name="p1336462311383"></a>delete_group(self, group, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19364132319380"><a name="p19364132319380"></a><a name="p19364132319380"></a>DELETE /v3/groups/{group_id}</p>
<p id="p16364122393819"><a name="p16364122393819"></a><a name="p16364122393819"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1966593201"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15364102363812"><a name="p15364102363812"></a><a name="p15364102363812"></a>check_group_user(self, group_id, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14364202320385"><a name="p14364202320385"></a><a name="p14364202320385"></a>HEAD /v3/groups/{group_id}/users/{user_id}</p>
<p id="p936418232387"><a name="p936418232387"></a><a name="p936418232387"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row85121916203819"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14364123193816"><a name="p14364123193816"></a><a name="p14364123193816"></a>add_user_to_group(self, group_id, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p63641523133814"><a name="p63641523133814"></a><a name="p63641523133814"></a>PUT /v3/groups/{group_id}/users/{user_id}</p>
<p id="p936432303812"><a name="p936432303812"></a><a name="p936432303812"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1966192207"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5364523103815"><a name="p5364523103815"></a><a name="p5364523103815"></a>list_user_groups(self, user_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p436462363810"><a name="p436462363810"></a><a name="p436462363810"></a>GET /v3/users/{user_id}/groups</p>
<p id="p83645234388"><a name="p83645234388"></a><a name="p83645234388"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row696629132017"><td class="cellrowborder" rowspan="11" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p15966119162013"><a name="p15966119162013"></a><a name="p15966119162013"></a>Role Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p5968050164719"><a name="p5968050164719"></a><a name="p5968050164719"></a>roles(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p1896875044714"><a name="p1896875044714"></a><a name="p1896875044714"></a>GET /v3/roles</p>
<p id="p2096815019472"><a name="p2096815019472"></a><a name="p2096815019472"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7966119172014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p496855054713"><a name="p496855054713"></a><a name="p496855054713"></a>get_role(self, role)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p129688503475"><a name="p129688503475"></a><a name="p129688503475"></a>GET /v3/roles/{role_id}</p>
<p id="p18968125015474"><a name="p18968125015474"></a><a name="p18968125015474"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39666962010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13968195014472"><a name="p13968195014472"></a><a name="p13968195014472"></a>list_domain_user_group_role(self, domain_id, group_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15968125054710"><a name="p15968125054710"></a><a name="p15968125054710"></a>GET /v3/domains/{domain_id}/groups/{group_id}/roles</p>
<p id="p99681750164710"><a name="p99681750164710"></a><a name="p99681750164710"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6966197206"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12968175074716"><a name="p12968175074716"></a><a name="p12968175074716"></a>list_project_user_group_role(self, project_id, group_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p696825074720"><a name="p696825074720"></a><a name="p696825074720"></a>GET /v3/projects/{project_id}/groups/{group_id}/roles</p>
<p id="p159688500473"><a name="p159688500473"></a><a name="p159688500473"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row199661696204"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1996812500475"><a name="p1996812500475"></a><a name="p1996812500475"></a>grant_domain_group_role(self, domain_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9968135024719"><a name="p9968135024719"></a><a name="p9968135024719"></a>PUT /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p79681450134715"><a name="p79681450134715"></a><a name="p79681450134715"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row129673952010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p496810508479"><a name="p496810508479"></a><a name="p496810508479"></a>grant_project_group_role(self, project_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13968950124718"><a name="p13968950124718"></a><a name="p13968950124718"></a>PUT /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p18968185044715"><a name="p18968185044715"></a><a name="p18968185044715"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19671091202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p996920505479"><a name="p996920505479"></a><a name="p996920505479"></a>check_domain_group_role(self, domain_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p296955014475"><a name="p296955014475"></a><a name="p296955014475"></a>HEAD /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p2096975015476"><a name="p2096975015476"></a><a name="p2096975015476"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row596710919209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4969195084719"><a name="p4969195084719"></a><a name="p4969195084719"></a>check_project_group_role(self, project_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p199691350124717"><a name="p199691350124717"></a><a name="p199691350124717"></a>HEAD /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p996965013471"><a name="p996965013471"></a><a name="p996965013471"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39670912209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p39691950184712"><a name="p39691950184712"></a><a name="p39691950184712"></a>delete_domain_group_role(self, domain_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2096945094710"><a name="p2096945094710"></a><a name="p2096945094710"></a>DELETE /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p096945094719"><a name="p096945094719"></a><a name="p096945094719"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7928183610478"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5969185013479"><a name="p5969185013479"></a><a name="p5969185013479"></a>delete_project_group_role(self, project_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19969165064711"><a name="p19969165064711"></a><a name="p19969165064711"></a>DELETE /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p1396975018471"><a name="p1396975018471"></a><a name="p1396975018471"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row159671913209"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p179693505475"><a name="p179693505475"></a><a name="p179693505475"></a>grant_all_projects_group_role(self, domain_id, group_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5969155034710"><a name="p5969155034710"></a><a name="p5969155034710"></a>PUT /v3/OS-INHERIT/domains/{domain_id}/groups/{group_id}/roles/{role_id}/inherited_to_projects</p>
<p id="p10969165034719"><a name="p10969165034719"></a><a name="p10969165034719"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0519.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1217615513523"><td class="cellrowborder" rowspan="5" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p1971932675319"><a name="p1971932675319"></a><a name="p1971932675319"></a>Customrole Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p1933812163526"><a name="p1933812163526"></a><a name="p1933812163526"></a>custom_roles(self)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p1633841645214"><a name="p1633841645214"></a><a name="p1633841645214"></a>GET /v3.0/OS-ROLE/roles</p>
<p id="p4338161645218"><a name="p4338161645218"></a><a name="p4338161645218"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12514103205218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9339111615212"><a name="p9339111615212"></a><a name="p9339111615212"></a>get_custom_role(self, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17339131615527"><a name="p17339131615527"></a><a name="p17339131615527"></a>GET /v3.0/OS-ROLE/roles/{role_id}</p>
<p id="p15339116135213"><a name="p15339116135213"></a><a name="p15339116135213"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0012.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1888341195210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p123391516175215"><a name="p123391516175215"></a><a name="p123391516175215"></a>create_custom_role(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23397169526"><a name="p23397169526"></a><a name="p23397169526"></a>POST /v3.0/OS-ROLE/roles</p>
<a name="ul15299722195213"></a><a name="ul15299722195213"></a><ul id="ul15299722195213"><li>创建云服务自定义策略的<a href="https://support.huaweicloud.com/api-iam/iam_02_0013.html" target="_blank" rel="noopener noreferrer">链接</a></li><li>创建委托自定义策略的<a href="https://support.huaweicloud.com/api-iam/iam_02_0016.html" target="_blank" rel="noopener noreferrer">链接</a></li></ul>
</td>
</tr>
<tr id="row2594013525"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1339131612529"><a name="p1339131612529"></a><a name="p1339131612529"></a>update_custom_role(self, role_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p133971610528"><a name="p133971610528"></a><a name="p133971610528"></a>PATCH /v3.0/OS-ROLE/roles/{role_id}</p>
<a name="ul18873448135211"></a><a name="ul18873448135211"></a><ul id="ul18873448135211"><li>修改云服务自定义策略<a href="https://support.huaweicloud.com/api-iam/iam_02_0014.html" target="_blank" rel="noopener noreferrer">链接</a></li><li>修改委托自定义策略<a href="https://support.huaweicloud.com/api-iam/iam_02_0017.html" target="_blank" rel="noopener noreferrer">链接</a></li></ul>
</td>
</tr>
<tr id="row15231958125114"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p433911617520"><a name="p433911617520"></a><a name="p433911617520"></a>delete_custom_role(self, role_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23391416135213"><a name="p23391416135213"></a><a name="p23391416135213"></a>DELETE /v3.0/OS-ROLE/roles/{role_id}</p>
<p id="p1633911655213"><a name="p1633911655213"></a><a name="p1633911655213"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0015.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row164145810319"><td class="cellrowborder" rowspan="13" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p32656261947"><a name="p32656261947"></a><a name="p32656261947"></a>Agency Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p4759180416"><a name="p4759180416"></a><a name="p4759180416"></a>agencies(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p175919810413"><a name="p175919810413"></a><a name="p175919810413"></a>GET /v3.0/OS-AGENCY/agencies</p>
<p id="p17593811416"><a name="p17593811416"></a><a name="p17593811416"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7641658837"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p157597815411"><a name="p157597815411"></a><a name="p157597815411"></a>get_agency(self, agency_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p575958749"><a name="p575958749"></a><a name="p575958749"></a>GET /v3.0/OS-AGENCY/agencies/{agency_id}</p>
<p id="p07592816415"><a name="p07592816415"></a><a name="p07592816415"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row765458133"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19759789417"><a name="p19759789417"></a><a name="p19759789417"></a>create_agency(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p137593817413"><a name="p137593817413"></a><a name="p137593817413"></a>POST /v3.0/OS-AGENCY/agencies</p>
<p id="p37592810414"><a name="p37592810414"></a><a name="p37592810414"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3651458530"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13760581945"><a name="p13760581945"></a><a name="p13760581945"></a>update_agency(self, agency_id, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2760198846"><a name="p2760198846"></a><a name="p2760198846"></a>PUT /v3.0/OS-AGENCY/agencies/{agency_id}</p>
<p id="p11760181417"><a name="p11760181417"></a><a name="p11760181417"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1365145819319"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p37609812414"><a name="p37609812414"></a><a name="p37609812414"></a>delete_agency(self, agency_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2760481243"><a name="p2760481243"></a><a name="p2760481243"></a>DELETE /v3.0/OS-AGENCY/agencies/{agency_id}</p>
<p id="p18760785416"><a name="p18760785416"></a><a name="p18760785416"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15467205119319"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1976048947"><a name="p1976048947"></a><a name="p1976048947"></a>list_domain_agency_role(self, domain_id, agency_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18760681846"><a name="p18760681846"></a><a name="p18760681846"></a>GET /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles</p>
<p id="p14760481741"><a name="p14760481741"></a><a name="p14760481741"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7467251536"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13760128748"><a name="p13760128748"></a><a name="p13760128748"></a>list_project_agency_role(self, project_id, agency_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p47601581941"><a name="p47601581941"></a><a name="p47601581941"></a>GET /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles</p>
<p id="p167601881840"><a name="p167601881840"></a><a name="p167601881840"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2046717512314"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2760178145"><a name="p2760178145"></a><a name="p2760178145"></a>grant_domain_agency_role(self, domain_id, agency_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10760281043"><a name="p10760281043"></a><a name="p10760281043"></a>PUT /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p15760884413"><a name="p15760884413"></a><a name="p15760884413"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row146819511631"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20760188417"><a name="p20760188417"></a><a name="p20760188417"></a>grant_project_agency_role(self, project_id, agency_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p87601989420"><a name="p87601989420"></a><a name="p87601989420"></a>PUT /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p5760178047"><a name="p5760178047"></a><a name="p5760178047"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14953471536"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1476016819412"><a name="p1476016819412"></a><a name="p1476016819412"></a>check_domain_agency_role(self, domain_id, agency_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14760785414"><a name="p14760785414"></a><a name="p14760785414"></a>HEAD /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p4760138845"><a name="p4760138845"></a><a name="p4760138845"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row109617477312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p67608818417"><a name="p67608818417"></a><a name="p67608818417"></a>check_project_agency_role(self, project_id, agency_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p476019819417"><a name="p476019819417"></a><a name="p476019819417"></a>HEAD /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p167602817415"><a name="p167602817415"></a><a name="p167602817415"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row187699401937"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p117601785410"><a name="p117601785410"></a><a name="p117601785410"></a>delete_domain_agency_role(self, domain_id, agency_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13760789417"><a name="p13760789417"></a><a name="p13760789417"></a>DELETE /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p157601983418"><a name="p157601983418"></a><a name="p157601983418"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0012.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1215619381039"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13760148047"><a name="p13760148047"></a><a name="p13760148047"></a>delete_project_agency_role(self, project_id, agency_id, role_id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8760118349"><a name="p8760118349"></a><a name="p8760118349"></a>DELETE /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p147601381046"><a name="p147601381046"></a><a name="p147601381046"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0013.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4384141938"><td class="cellrowborder" rowspan="2" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p34092810317"><a name="p34092810317"></a><a name="p34092810317"></a>Version Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p233918146320"><a name="p233918146320"></a><a name="p233918146320"></a>get_version_of_keystone(self)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p183390146320"><a name="p183390146320"></a><a name="p183390146320"></a>GET /</p>
<p id="p1533951419314"><a name="p1533951419314"></a><a name="p1533951419314"></a><a href="https://support.huaweicloud.com/api-iam/iam_15_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1075520591218"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p123391914935"><a name="p123391914935"></a><a name="p123391914935"></a>get_version3_of_keystone(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10339181418315"><a name="p10339181418315"></a><a name="p10339181418315"></a>GET /v3</p>
<p id="p9339114338"><a name="p9339114338"></a><a name="p9339114338"></a><a href="https://support.huaweicloud.com/api-iam/iam_15_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row996729122011"><td class="cellrowborder" rowspan="3" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p596719916202"><a name="p596719916202"></a><a name="p596719916202"></a>Service Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p129677962016"><a name="p129677962016"></a><a name="p129677962016"></a>services(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p17301141804317"><a name="p17301141804317"></a><a name="p17301141804317"></a>GET /v3/services</p>
<p id="p8968292207"><a name="p8968292207"></a><a name="p8968292207"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row159681694207"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p596889182014"><a name="p596889182014"></a><a name="p596889182014"></a>get_service(self, service)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1896839122017"><a name="p1896839122017"></a><a name="p1896839122017"></a>GET /v3/services/{service_id}</p>
<p id="p196814932014"><a name="p196814932014"></a><a name="p196814932014"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42559324211"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p43471847122"><a name="p43471847122"></a><a name="p43471847122"></a>get_service_catalog(self)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p103473473213"><a name="p103473473213"></a><a name="p103473473213"></a>GET /v3/auth/catalog</p>
<p id="p18347347523"><a name="p18347347523"></a><a name="p18347347523"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row196879152018"><td class="cellrowborder" rowspan="2" valign="top" width="26.142614261426147%" headers="mcps1.1.4.1.1 "><p id="p396889132012"><a name="p396889132012"></a><a name="p396889132012"></a>Endpoint Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.64396439643964%" headers="mcps1.1.4.1.2 "><p id="p996818918208"><a name="p996818918208"></a><a name="p996818918208"></a>endpoints(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="34.21342134213422%" headers="mcps1.1.4.1.3 "><p id="p179687910205"><a name="p179687910205"></a><a name="p179687910205"></a>GET /v3/endpoints</p>
<p id="p2096817916206"><a name="p2096817916206"></a><a name="p2096817916206"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row396818912202"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p109687918207"><a name="p109687918207"></a><a name="p109687918207"></a>get_endpoint(self, endpoint)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p199685992012"><a name="p199685992012"></a><a name="p199685992012"></a>GET /v3/endpoints/{endpoint_id}</p>
<p id="p1696815917202"><a name="p1696815917202"></a><a name="p1696815917202"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

