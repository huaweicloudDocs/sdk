# Java-IAM<a name="ZH-CN_TOPIC_0070867953"></a>

基于IAM API的SDK接口如下，调用方式请参考示例代码。

<a name="table14641430131717"></a>
<table><thead align="left"><tr id="row196671630191710"><th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.1.4.1.1"><p id="p8667230101713"><a name="p8667230101713"></a><a name="p8667230101713"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.39393939393939%" id="mcps1.1.4.1.2"><p id="p136671830141714"><a name="p136671830141714"></a><a name="p136671830141714"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="43.43434343434344%" id="mcps1.1.4.1.3"><p id="p15667193051713"><a name="p15667193051713"></a><a name="p15667193051713"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row156671430131715"><td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p1466733019178"><a name="p1466733019178"></a><a name="p1466733019178"></a>SecuritytokenService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p466723071713"><a name="p466723071713"></a><a name="p466723071713"></a>Securitytoken create(Auth auth)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p266763012176"><a name="p266763012176"></a><a name="p266763012176"></a>POST /v3.0/OS-CREDENTIAL/securitytokens</p>
<p id="p06671730171715"><a name="p06671730171715"></a><a name="p06671730171715"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0097949518.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56678306177"><td class="cellrowborder" rowspan="2" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p136674302177"><a name="p136674302177"></a><a name="p136674302177"></a>RegionService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p466743018172"><a name="p466743018172"></a><a name="p466743018172"></a>List&lt;? extends Region&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p266743014174"><a name="p266743014174"></a><a name="p266743014174"></a>GET /v3/regions</p>
<p id="p13667230161714"><a name="p13667230161714"></a><a name="p13667230161714"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148043.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1566773015171"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p266814306176"><a name="p266814306176"></a><a name="p266814306176"></a>Region get(String regionId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12668153081718"><a name="p12668153081718"></a><a name="p12668153081718"></a>GET /v3/regions/{region_id}</p>
<p id="p166686301174"><a name="p166686301174"></a><a name="p166686301174"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148044.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3808518365"><td class="cellrowborder" rowspan="6" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p196684305179"><a name="p196684305179"></a><a name="p196684305179"></a>ProjectService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p68214519367"><a name="p68214519367"></a><a name="p68214519367"></a>List&lt;? extends Project&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p1246113315367"><a name="p1246113315367"></a><a name="p1246113315367"></a>GET /v3/projects</p>
<p id="p1246163113365"><a name="p1246163113365"></a><a name="p1246163113365"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row197443190227"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18745101922216"><a name="p18745101922216"></a><a name="p18745101922216"></a>List&lt;? extends Project&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1672475162319"><a name="p1672475162319"></a><a name="p1672475162319"></a>GET /v3/projects</p>
<p id="p11276262411"><a name="p11276262411"></a><a name="p11276262411"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17668330141712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5668730181716"><a name="p5668730181716"></a><a name="p5668730181716"></a>Project getByName(String projectName, String domainId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12351114423819"><a name="p12351114423819"></a><a name="p12351114423819"></a>GET /v3/projects?name={projectName}&amp;&amp;domain_id={domainId}</p>
<p id="p4668193041715"><a name="p4668193041715"></a><a name="p4668193041715"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845625.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11668193019176"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1666833001713"><a name="p1666833001713"></a><a name="p1666833001713"></a>Project create(String domainId, String name, String description, boolean enabled)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p156681530181716"><a name="p156681530181716"></a><a name="p156681530181716"></a>POST /v3/projects</p>
<p id="p06684302172"><a name="p06684302172"></a><a name="p06684302172"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0066154565.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row176682309170"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6668113014171"><a name="p6668113014171"></a><a name="p6668113014171"></a>Project update(Project project)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15668153020177"><a name="p15668153020177"></a><a name="p15668153020177"></a>PATCH /v3/projects/{project_id}</p>
<p id="p76682030201716"><a name="p76682030201716"></a><a name="p76682030201716"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0066154566.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10668153014177"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26689304170"><a name="p26689304170"></a><a name="p26689304170"></a>Project get(String projectId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9668630171715"><a name="p9668630171715"></a><a name="p9668630171715"></a>GET /v3/projects/{project_id}</p>
<p id="p1668730121715"><a name="p1668730121715"></a><a name="p1668730121715"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0066154567.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56681430151713"><td class="cellrowborder" rowspan="12" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p5668173061717"><a name="p5668173061717"></a><a name="p5668173061717"></a>UserService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p96681530121710"><a name="p96681530121710"></a><a name="p96681530121710"></a>List&lt;? extends Project&gt; listUserProjects(String userId)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p1566853019172"><a name="p1566853019172"></a><a name="p1566853019172"></a>GET /v3/users/{user_id}/projects</p>
<p id="p14669103011178"><a name="p14669103011178"></a><a name="p14669103011178"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845622.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1766943081719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3669143015171"><a name="p3669143015171"></a><a name="p3669143015171"></a>List&lt;? extends User&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17669230181719"><a name="p17669230181719"></a><a name="p17669230181719"></a>GET /v3/users</p>
<p id="p186693305176"><a name="p186693305176"></a><a name="p186693305176"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845638.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13529111813265"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20839141916266"><a name="p20839141916266"></a><a name="p20839141916266"></a>List&lt;? extends User&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3839171942616"><a name="p3839171942616"></a><a name="p3839171942616"></a>GET /v3/users</p>
<p id="p13839819192612"><a name="p13839819192612"></a><a name="p13839819192612"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845638.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10669630181711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p866910306171"><a name="p866910306171"></a><a name="p866910306171"></a>User get(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7669173016173"><a name="p7669173016173"></a><a name="p7669173016173"></a>GET /v3/users/{user_id}</p>
<p id="p266993019179"><a name="p266993019179"></a><a name="p266993019179"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845652.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17847161719399"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18222272394"><a name="p18222272394"></a><a name="p18222272394"></a>List&lt;? extends User&gt; getByName(String userName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1422172783911"><a name="p1422172783911"></a><a name="p1422172783911"></a>GET /v3/users?name={user_name}</p>
<p id="p622132717392"><a name="p622132717392"></a><a name="p622132717392"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845638.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row186981415203911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0226273394"><a name="p0226273394"></a><a name="p0226273394"></a>User getByName(String userName, String domainId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1122727183918"><a name="p1122727183918"></a><a name="p1122727183918"></a>GET /v3/users?name={user_name}&amp;&amp;domain_id={domain_id}</p>
<p id="p82242733913"><a name="p82242733913"></a><a name="p82242733913"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845638.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16695305178"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5669030141717"><a name="p5669030141717"></a><a name="p5669030141717"></a>List&lt;? extends Group&gt; listUserGroups(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p76696309173"><a name="p76696309173"></a><a name="p76696309173"></a>GET /v3/users/{user_id}/groups</p>
<p id="p6669103051710"><a name="p6669103051710"></a><a name="p6669103051710"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845554.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1566914308173"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16693302171"><a name="p16693302171"></a><a name="p16693302171"></a>User create(String domainId, String name, String password, String email, boolean enabled)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p76691330191714"><a name="p76691330191714"></a><a name="p76691330191714"></a>POST /v3/users</p>
<p id="p7669330161717"><a name="p7669330161717"></a><a name="p7669330161717"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845637.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7251830184014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14723163418405"><a name="p14723163418405"></a><a name="p14723163418405"></a>User create(User user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p37231334124012"><a name="p37231334124012"></a><a name="p37231334124012"></a>POST /v3/users</p>
<p id="p207231334134017"><a name="p207231334134017"></a><a name="p207231334134017"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845637.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row766933015177"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6669143019174"><a name="p6669143019174"></a><a name="p6669143019174"></a>ActionResponse changePassword(String userId,String originalPassword,String password)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6669230151710"><a name="p6669230151710"></a><a name="p6669230151710"></a>POST /v3/users/{user_id}/password</p>
<p id="p10669173001711"><a name="p10669173001711"></a><a name="p10669173001711"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845653.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row566943061717"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1366916309176"><a name="p1366916309176"></a><a name="p1366916309176"></a>User update(User user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p186691030191717"><a name="p186691030191717"></a><a name="p186691030191717"></a>PATCH /v3/users/{user_id}</p>
<p id="p17669143019175"><a name="p17669143019175"></a><a name="p17669143019175"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845611.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1766913091712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0669183013176"><a name="p0669183013176"></a><a name="p0669183013176"></a>ActionResponse delete(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8669123021715"><a name="p8669123021715"></a><a name="p8669123021715"></a>DELETE /v3/users/{user_id}</p>
<p id="p1766920309179"><a name="p1766920309179"></a><a name="p1766920309179"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845630.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2669103091715"><td class="cellrowborder" rowspan="3" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p15669930111714"><a name="p15669930111714"></a><a name="p15669930111714"></a>TokenService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p566923010176"><a name="p566923010176"></a><a name="p566923010176"></a>List&lt;? extends Project&gt; getProjectScopes(String tokenId)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p36699303179"><a name="p36699303179"></a><a name="p36699303179"></a>GET /v3/auth/projects</p>
<p id="p1466933013171"><a name="p1466933013171"></a><a name="p1466933013171"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845558.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11669330111719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4670193018177"><a name="p4670193018177"></a><a name="p4670193018177"></a>List&lt;? extends Domain&gt; getDomainScopes(String tokenId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p267073061715"><a name="p267073061715"></a><a name="p267073061715"></a>GET /v3/auth/domains</p>
<p id="p1867073031714"><a name="p1867073031714"></a><a name="p1867073031714"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845574.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4670203041713"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4670113071711"><a name="p4670113071711"></a><a name="p4670113071711"></a>Token get(String tokenId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1667018301174"><a name="p1667018301174"></a><a name="p1667018301174"></a>GET /v3/auth/tokens</p>
<p id="p7670143051719"><a name="p7670143051719"></a><a name="p7670143051719"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845585.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3670133011719"><td class="cellrowborder" rowspan="2" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p13670193011719"><a name="p13670193011719"></a><a name="p13670193011719"></a>DomainService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p8670103016170"><a name="p8670103016170"></a><a name="p8670103016170"></a>PasswordConfig getDomainPasswordConfig(String domainId)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p1670193081714"><a name="p1670193081714"></a><a name="p1670193081714"></a>GET /v3/domains/{domain_id}/config/security_compliance</p>
<p id="p20670163011715"><a name="p20670163011715"></a><a name="p20670163011715"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4670230131711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16670330101716"><a name="p16670330101716"></a><a name="p16670330101716"></a>PasswordConfig getDomainPasswordConfigByOption(String domainId, String option)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18670103081717"><a name="p18670103081717"></a><a name="p18670103081717"></a>GET /v3/domains/{domain_id}/config/security_compliance/{option}</p>
<p id="p19670133021719"><a name="p19670133021719"></a><a name="p19670133021719"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0113.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1670103011179"><td class="cellrowborder" rowspan="12" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p16701930141710"><a name="p16701930141710"></a><a name="p16701930141710"></a>GroupService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p11670163015174"><a name="p11670163015174"></a><a name="p11670163015174"></a>List&lt;? extends User&gt; listGroupUsers(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p8670203011174"><a name="p8670203011174"></a><a name="p8670203011174"></a>GET /v3/groups/{group_id}/users</p>
<p id="p167016302174"><a name="p167016302174"></a><a name="p167016302174"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845561.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16670133017177"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10670130101711"><a name="p10670130101711"></a><a name="p10670130101711"></a>ActionResponse removeUserFromGroup(String groupId, String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p067083021711"><a name="p067083021711"></a><a name="p067083021711"></a>DELETE /v3/groups/{group_id}/users/{user_id}</p>
<p id="p1367013014175"><a name="p1367013014175"></a><a name="p1367013014175"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845601.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8890146113214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p147811481324"><a name="p147811481324"></a><a name="p147811481324"></a>List&lt;? extends Group&gt; getByName(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p114791148183219"><a name="p114791148183219"></a><a name="p114791148183219"></a>GET /v3/groups</p>
<p id="p4479248133218"><a name="p4479248133218"></a><a name="p4479248133218"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845602.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18670930121711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p458311332413"><a name="p458311332413"></a><a name="p458311332413"></a>List&lt;? extends Group&gt; getByName(String groupName, String domainId )</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1225112412416"><a name="p1225112412416"></a><a name="p1225112412416"></a>GET /v3/groups?name={groupName}&amp;&amp;domain_id={domainId}</p>
<p id="p96705301179"><a name="p96705301179"></a><a name="p96705301179"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845602.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10670730151718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p86701030111717"><a name="p86701030111717"></a><a name="p86701030111717"></a>Group get(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1367019300175"><a name="p1367019300175"></a><a name="p1367019300175"></a>GET /v3/groups/{group_id}</p>
<p id="p567023071716"><a name="p567023071716"></a><a name="p567023071716"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845618.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12670330101712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p186715309176"><a name="p186715309176"></a><a name="p186715309176"></a>Group create(String domainId, String name, String description)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8671133031718"><a name="p8671133031718"></a><a name="p8671133031718"></a>POST /v3/groups</p>
<p id="p867113017176"><a name="p867113017176"></a><a name="p867113017176"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845650.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row146715307174"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p267153051720"><a name="p267153051720"></a><a name="p267153051720"></a>ActionResponse addUserToGroup(String groupId, String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p167133016172"><a name="p167133016172"></a><a name="p167133016172"></a>PUT /v3/groups/{group_id}/users/{user_id}</p>
<p id="p1467118306174"><a name="p1467118306174"></a><a name="p1467118306174"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845654.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17671030171710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p167133081720"><a name="p167133081720"></a><a name="p167133081720"></a>Group update(Group group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p106711930101712"><a name="p106711930101712"></a><a name="p106711930101712"></a>PATCH /v3/groups/{group_id}</p>
<p id="p156711230121715"><a name="p156711230121715"></a><a name="p156711230121715"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845600.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6671143015171"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p196718306176"><a name="p196718306176"></a><a name="p196718306176"></a>ActionResponse delete(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p86711430101718"><a name="p86711430101718"></a><a name="p86711430101718"></a>DELETE /v3/groups/{group_id}</p>
<p id="p16671163019172"><a name="p16671163019172"></a><a name="p16671163019172"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845566.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1067163091715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p867113302170"><a name="p867113302170"></a><a name="p867113302170"></a>ActionResponse checkGroupUser(String groupId, String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1967115303175"><a name="p1967115303175"></a><a name="p1967115303175"></a>HEAD /v3/groups/{group_id}/users/{user_id}</p>
<p id="p667103010179"><a name="p667103010179"></a><a name="p667103010179"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845599.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row126711430161710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5671163014170"><a name="p5671163014170"></a><a name="p5671163014170"></a>List&lt;? extends Role&gt; listDomainGroupRoles(String groupId, String domainId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6671163019171"><a name="p6671163019171"></a><a name="p6671163019171"></a>GET /v3/domains/{domain_id}/groups/{group_id}/roles</p>
<p id="p1867173017174"><a name="p1867173017174"></a><a name="p1867173017174"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845571.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row367113091713"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1367113015172"><a name="p1367113015172"></a><a name="p1367113015172"></a>List&lt;? extends Role&gt; listProjectGroupRoles(String groupId, String projectId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1367123018173"><a name="p1367123018173"></a><a name="p1367123018173"></a>GET /v3/projects/{project_id}/groups/{group_id}/roles</p>
<p id="p1367123041711"><a name="p1367123041711"></a><a name="p1367123041711"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845640.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row166711430201719"><td class="cellrowborder" rowspan="8" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p86721130171711"><a name="p86721130171711"></a><a name="p86721130171711"></a>RoleService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p86720308172"><a name="p86720308172"></a><a name="p86720308172"></a>List&lt;? extends Role&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p116721030161718"><a name="p116721030161718"></a><a name="p116721030161718"></a>GET /v3/roles</p>
<p id="p1467220301172"><a name="p1467220301172"></a><a name="p1467220301172"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845591.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8672193091720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p967273051713"><a name="p967273051713"></a><a name="p967273051713"></a>Role get(String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1067263081714"><a name="p1067263081714"></a><a name="p1067263081714"></a>GET /v3/roles/{role_id}</p>
<p id="p767283015177"><a name="p767283015177"></a><a name="p767283015177"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845603.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row126721330131717"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p767210308179"><a name="p767210308179"></a><a name="p767210308179"></a>ActionResponse grantDomainGroupRole(String domainId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7672163015176"><a name="p7672163015176"></a><a name="p7672163015176"></a>PUT /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p067233061715"><a name="p067233061715"></a><a name="p067233061715"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845623.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row146721330151716"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p96721830161710"><a name="p96721830161710"></a><a name="p96721830161710"></a>ActionResponse grantProjectGroupRole(String projectId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1267213020177"><a name="p1267213020177"></a><a name="p1267213020177"></a>PUT /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p76724302177"><a name="p76724302177"></a><a name="p76724302177"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845597.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row367214306176"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12672163001710"><a name="p12672163001710"></a><a name="p12672163001710"></a>ActionResponse revokeProjectGroupRole(String projectId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p66721301175"><a name="p66721301175"></a><a name="p66721301175"></a>DELETE /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p6672153001717"><a name="p6672153001717"></a><a name="p6672153001717"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845572.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row96721308178"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7672153051719"><a name="p7672153051719"></a><a name="p7672153051719"></a>ActionResponse revokeDomainGroupRole(String domainId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19672183020171"><a name="p19672183020171"></a><a name="p19672183020171"></a>DELETE /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p467273015177"><a name="p467273015177"></a><a name="p467273015177"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845560.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row667218309178"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7672153091712"><a name="p7672153091712"></a><a name="p7672153091712"></a>ActionResponse checkDomainGroupRole(String domainId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46721630151718"><a name="p46721630151718"></a><a name="p46721630151718"></a>HEAD /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p86726309178"><a name="p86726309178"></a><a name="p86726309178"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845632.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row156721530131712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66721030151711"><a name="p66721030151711"></a><a name="p66721030151711"></a>ActionResponse checkProjectGroupRole(String projectId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3672193015177"><a name="p3672193015177"></a><a name="p3672193015177"></a>HEAD /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p11673193013176"><a name="p11673193013176"></a><a name="p11673193013176"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845620.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20673123016178"><td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p86731930171720"><a name="p86731930171720"></a><a name="p86731930171720"></a>VersionService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p667312301176"><a name="p667312301176"></a><a name="p667312301176"></a>Version get()</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p96731530201719"><a name="p96731530201719"></a><a name="p96731530201719"></a>GET /v3</p>
<p id="p1167314301176"><a name="p1167314301176"></a><a name="p1167314301176"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845613.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46731730141718"><td class="cellrowborder" rowspan="6" valign="top" width="17.17171717171717%" headers="mcps1.1.4.1.1 "><p id="p1867312309178"><a name="p1867312309178"></a><a name="p1867312309178"></a>ServiceEndpointService</p>
</td>
<td class="cellrowborder" valign="top" width="39.39393939393939%" headers="mcps1.1.4.1.2 "><p id="p26739308176"><a name="p26739308176"></a><a name="p26739308176"></a>List&lt;? extends Service&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="43.43434343434344%" headers="mcps1.1.4.1.3 "><p id="p19673173015177"><a name="p19673173015177"></a><a name="p19673173015177"></a>GET /v3/services</p>
<p id="p12673030181719"><a name="p12673030181719"></a><a name="p12673030181719"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845587.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1839717567334"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11427175723318"><a name="p11427175723318"></a><a name="p11427175723318"></a>List&lt;? extends Service&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8427757143320"><a name="p8427757143320"></a><a name="p8427757143320"></a>GET /v3/services</p>
<p id="p1742795716337"><a name="p1742795716337"></a><a name="p1742795716337"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845587.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20673143071719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1167316301171"><a name="p1167316301171"></a><a name="p1167316301171"></a>Service get(String serviceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p167323011175"><a name="p167323011175"></a><a name="p167323011175"></a>GET /v3/services/{service_id}</p>
<p id="p186733305172"><a name="p186733305172"></a><a name="p186733305172"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148045.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row136731030201710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1667315307175"><a name="p1667315307175"></a><a name="p1667315307175"></a>List&lt;? extends Endpoint&gt; listEndpoints()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p166731830101711"><a name="p166731830101711"></a><a name="p166731830101711"></a>GET /v3/endpoints</p>
<p id="p11673133013171"><a name="p11673133013171"></a><a name="p11673133013171"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845562.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1373094473417"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1817174533416"><a name="p1817174533416"></a><a name="p1817174533416"></a>List&lt;? extends Endpoint&gt; listEndpoints(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1281719454341"><a name="p1281719454341"></a><a name="p1281719454341"></a>GET /v3/endpoints</p>
<p id="p168171745163414"><a name="p168171745163414"></a><a name="p168171745163414"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0057845562.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18673530161713"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12673330111714"><a name="p12673330111714"></a><a name="p12673330111714"></a>Endpoint getEndpoint(String endpointId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15673030171710"><a name="p15673030171710"></a><a name="p15673030171710"></a>GET /v3/endpoints/{endpoint_id}</p>
<p id="p116731130171710"><a name="p116731130171710"></a><a name="p116731130171710"></a><a href="https://support.huaweicloud.com/api-iam/zh-cn_topic_0067148046.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

