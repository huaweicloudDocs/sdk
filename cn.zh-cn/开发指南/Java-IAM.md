# IAM<a name="sdk_11_0001"></a>

基于IAM API的SDK接口如下，调用方式请参考示例代码。

<a name="table14641430131717"></a>
<table><thead align="left"><tr id="row196671630191710"><th class="cellrowborder" valign="top" width="28.372837283728376%" id="mcps1.1.4.1.1"><p id="p8667230101713"><a name="p8667230101713"></a><a name="p8667230101713"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.98359835983598%" id="mcps1.1.4.1.2"><p id="p136671830141714"><a name="p136671830141714"></a><a name="p136671830141714"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.64356435643564%" id="mcps1.1.4.1.3"><p id="p15667193051713"><a name="p15667193051713"></a><a name="p15667193051713"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row7767143910913"><td class="cellrowborder" rowspan="5" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p19767103915914"><a name="p19767103915914"></a><a name="p19767103915914"></a>TokenService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p3239529101"><a name="p3239529101"></a><a name="p3239529101"></a>Token create(String nocatalog, Auth auth)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p82397217108"><a name="p82397217108"></a><a name="p82397217108"></a>POST /v3/auth/tokens</p>
<p id="p323911217109"><a name="p323911217109"></a><a name="p323911217109"></a>获取用户token（使用密码）<a href="https://support.huaweicloud.com/api-iam/iam_30_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p42391626108"><a name="p42391626108"></a><a name="p42391626108"></a>获取用户token（使用密码+虚拟MFA）<a href="https://support.huaweicloud.com/api-iam/iam_03_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p92409217102"><a name="p92409217102"></a><a name="p92409217102"></a>获取委托Token<a href="https://support.huaweicloud.com/api-iam/iam_30_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1122864518919"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1724017281012"><a name="p1724017281012"></a><a name="p1724017281012"></a>Token get(String tokenId)</p>
<p id="p324052201019"><a name="p324052201019"></a><a name="p324052201019"></a>Token getWithoutCatalog(String tokenId, String nocatalog</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p524013281017"><a name="p524013281017"></a><a name="p524013281017"></a>GET /v3/auth/tokens</p>
<p id="p024020210109"><a name="p024020210109"></a><a name="p024020210109"></a><a href="https://support.huaweicloud.com/api-iam/iam_30_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row194390421091"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1224092111010"><a name="p1224092111010"></a><a name="p1224092111010"></a>List&lt;? extends Project&gt; getProjectScopes(String tokenId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p92407214106"><a name="p92407214106"></a><a name="p92407214106"></a>GET /v3/auth/projects</p>
<p id="p72405219103"><a name="p72405219103"></a><a name="p72405219103"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1211920372099"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p92401325101"><a name="p92401325101"></a><a name="p92401325101"></a>List&lt;? extends Domain&gt; getDomainScopes(String tokenId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p82401725101"><a name="p82401725101"></a><a name="p82401725101"></a>GET /v3/auth/domains</p>
<p id="p924011251018"><a name="p924011251018"></a><a name="p924011251018"></a><a href="https://support.huaweicloud.com/api-iam/iam_07_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row131811928798"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18240122111017"><a name="p18240122111017"></a><a name="p18240122111017"></a>List&lt;? extends Service&gt; getServiceCatalog()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32408219109"><a name="p32408219109"></a><a name="p32408219109"></a>GET /v3/auth/catalog</p>
<p id="p524062171013"><a name="p524062171013"></a><a name="p524062171013"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row156671430131715"><td class="cellrowborder" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p1466733019178"><a name="p1466733019178"></a><a name="p1466733019178"></a>SecuritytokenService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p466723071713"><a name="p466723071713"></a><a name="p466723071713"></a>Securitytoken create(Auth auth)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p266763012176"><a name="p266763012176"></a><a name="p266763012176"></a>POST /v3.0/OS-CREDENTIAL/securitytokens</p>
<p id="p06671730171715"><a name="p06671730171715"></a><a name="p06671730171715"></a><a href="https://support.huaweicloud.com/api-iam/iam_04_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9973458121413"><td class="cellrowborder" rowspan="5" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p9973115816143"><a name="p9973115816143"></a><a name="p9973115816143"></a>CredentialService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p1842812237154"><a name="p1842812237154"></a><a name="p1842812237154"></a>PermanentCredentialResp createPermanentAccessKey(CreatePermanentCredentialReq createPermanentCredentialReq)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p12428152317157"><a name="p12428152317157"></a><a name="p12428152317157"></a>POST /v3.0/OS-CREDENTIAL/credentials</p>
<p id="p9428523131515"><a name="p9428523131515"></a><a name="p9428523131515"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7222173191515"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8428223171519"><a name="p8428223171519"></a><a name="p8428223171519"></a>Credentials listPermanentAccessKeys(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9428423191519"><a name="p9428423191519"></a><a name="p9428423191519"></a>GET /v3.0/OS-CREDENTIAL/credentials</p>
<p id="p3428152331510"><a name="p3428152331510"></a><a name="p3428152331510"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row45236851519"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p94281123121513"><a name="p94281123121513"></a><a name="p94281123121513"></a>PermanentCredentialResp queryPermanentAccessKey(String accessKey)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p184281323101510"><a name="p184281323101510"></a><a name="p184281323101510"></a>GET /v3.0/OS-CREDENTIAL/credentials/{access_key}</p>
<p id="p114280233150"><a name="p114280233150"></a><a name="p114280233150"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1196821141511"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11428162315159"><a name="p11428162315159"></a><a name="p11428162315159"></a>UpdateCredentialResp updatePermanentAccessKey(String accessKey, UpdateCredentialReq updateCredentialReq)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10428223121517"><a name="p10428223121517"></a><a name="p10428223121517"></a>PUT /v3.0/OS-CREDENTIAL/credentials/{access_key}</p>
<p id="p3428192371510"><a name="p3428192371510"></a><a name="p3428192371510"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row78967513156"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1942862311154"><a name="p1942862311154"></a><a name="p1942862311154"></a>ActionResponse deletePermanentAccessKey(String accessKey)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p04282234154"><a name="p04282234154"></a><a name="p04282234154"></a>DELETE /v3.0/OS-CREDENTIAL/credentials/{access_key}</p>
<p id="p3428223181511"><a name="p3428223181511"></a><a name="p3428223181511"></a><a href="https://support.huaweicloud.com/api-iam/iam_03_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56678306177"><td class="cellrowborder" rowspan="2" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p136674302177"><a name="p136674302177"></a><a name="p136674302177"></a>RegionService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p466743018172"><a name="p466743018172"></a><a name="p466743018172"></a>List&lt;? extends Region&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p266743014174"><a name="p266743014174"></a><a name="p266743014174"></a>GET /v3/regions</p>
<p id="p13667230161714"><a name="p13667230161714"></a><a name="p13667230161714"></a><a href="https://support.huaweicloud.com/api-iam/iam_05_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1566773015171"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p266814306176"><a name="p266814306176"></a><a name="p266814306176"></a>Region get(String regionId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12668153081718"><a name="p12668153081718"></a><a name="p12668153081718"></a>GET /v3/regions/{region_id}</p>
<p id="p166686301174"><a name="p166686301174"></a><a name="p166686301174"></a><a href="https://support.huaweicloud.com/api-iam/iam_05_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3808518365"><td class="cellrowborder" rowspan="4" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p196684305179"><a name="p196684305179"></a><a name="p196684305179"></a>ProjectService(identity)</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p68214519367"><a name="p68214519367"></a><a name="p68214519367"></a>List&lt;? extends Project&gt; listByObject(Map&lt;String, Object&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p1246113315367"><a name="p1246113315367"></a><a name="p1246113315367"></a>GET /v3/projects</p>
<p id="p1246163113365"><a name="p1246163113365"></a><a name="p1246163113365"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16520123619203"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2052123616205"><a name="p2052123616205"></a><a name="p2052123616205"></a>Project create(Project project)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17152354211"><a name="p17152354211"></a><a name="p17152354211"></a>POST /v3/projects</p>
<p id="p41533516212"><a name="p41533516212"></a><a name="p41533516212"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17318123916206"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1831993911206"><a name="p1831993911206"></a><a name="p1831993911206"></a>Project update(Project project)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p177021517192118"><a name="p177021517192118"></a><a name="p177021517192118"></a>PATCH /v3/projects/{project_id}</p>
<p id="p2070291742118"><a name="p2070291742118"></a><a name="p2070291742118"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17190154218205"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41901542142017"><a name="p41901542142017"></a><a name="p41901542142017"></a>Project get(String projectId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8552742217"><a name="p8552742217"></a><a name="p8552742217"></a>GET /v3/projects/{project_id}</p>
<p id="p1855318432114"><a name="p1855318432114"></a><a name="p1855318432114"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row197443190227"><td class="cellrowborder" rowspan="2" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p1054441272212"><a name="p1054441272212"></a><a name="p1054441272212"></a>ProjectService(iam)</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p148451891237"><a name="p148451891237"></a><a name="p148451891237"></a>ActionResponse updateStatus(String projectId, UpdateProjectReq project)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p48450913237"><a name="p48450913237"></a><a name="p48450913237"></a>PUT /v3-ext/projects/{project_id}</p>
<p id="p484517919235"><a name="p484517919235"></a><a name="p484517919235"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17668330141712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p857319155257"><a name="p857319155257"></a><a name="p857319155257"></a>QueryProjectResp query(String projectId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p457316154259"><a name="p457316154259"></a><a name="p457316154259"></a>GET /v3-ext/projects/{project_id}</p>
<p id="p1957391512258"><a name="p1957391512258"></a><a name="p1957391512258"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11668193019176"><td class="cellrowborder" rowspan="2" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p12544151210228"><a name="p12544151210228"></a><a name="p12544151210228"></a>DomainService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p14981104716252"><a name="p14981104716252"></a><a name="p14981104716252"></a>PasswordConfig getDomainPasswordConfig(String domainId)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p129811147122513"><a name="p129811147122513"></a><a name="p129811147122513"></a>GET /v3/domains/{domain_id}/config/security_compliance</p>
<p id="p89811347102518"><a name="p89811347102518"></a><a name="p89811347102518"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row176682309170"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p298134719256"><a name="p298134719256"></a><a name="p298134719256"></a>PasswordConfig getDomainPasswordConfigByOption(String domainId, String option)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p199814478253"><a name="p199814478253"></a><a name="p199814478253"></a>GET /v3/domains/{domain_id}/config/security_compliance/{option}</p>
<p id="p198113479252"><a name="p198113479252"></a><a name="p198113479252"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0113.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row56681430151713"><td class="cellrowborder" rowspan="8" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p5668173061717"><a name="p5668173061717"></a><a name="p5668173061717"></a>UserService(identity)</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p1660891619282"><a name="p1660891619282"></a><a name="p1660891619282"></a>List&lt;? extends User&gt; list()</p>
<p id="p1608181620288"><a name="p1608181620288"></a><a name="p1608181620288"></a>List&lt;? extends User&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p1760810168287"><a name="p1760810168287"></a><a name="p1760810168287"></a>GET /v3/users</p>
<p id="p16608191617283"><a name="p16608191617283"></a><a name="p16608191617283"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1766943081719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p76081165288"><a name="p76081165288"></a><a name="p76081165288"></a>User get(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p560821611288"><a name="p560821611288"></a><a name="p560821611288"></a>GET /v3/users/{user_id}</p>
<p id="p11608201642816"><a name="p11608201642816"></a><a name="p11608201642816"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13529111813265"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1960821616284"><a name="p1960821616284"></a><a name="p1960821616284"></a>List&lt;? extends Group&gt; listUserGroups(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16085168289"><a name="p16085168289"></a><a name="p16085168289"></a>GET /v3/users/{user_id}/groups</p>
<p id="p260812165281"><a name="p260812165281"></a><a name="p260812165281"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10669630181711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p560831615283"><a name="p560831615283"></a><a name="p560831615283"></a>User create(User user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4608516202817"><a name="p4608516202817"></a><a name="p4608516202817"></a>POST /v3/users</p>
<p id="p8608101612281"><a name="p8608101612281"></a><a name="p8608101612281"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17847161719399"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16080163281"><a name="p16080163281"></a><a name="p16080163281"></a>ActionResponse changePassword(String userId,String originalPassword,String password)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1860831692815"><a name="p1860831692815"></a><a name="p1860831692815"></a>POST /v3/users/{user_id}/password</p>
<p id="p96081716102815"><a name="p96081716102815"></a><a name="p96081716102815"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row186981415203911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1660812162283"><a name="p1660812162283"></a><a name="p1660812162283"></a>User update(User user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6608141672810"><a name="p6608141672810"></a><a name="p6608141672810"></a>PATCH /v3/users/{user_id}</p>
<p id="p3608111622811"><a name="p3608111622811"></a><a name="p3608111622811"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16695305178"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1360819163284"><a name="p1360819163284"></a><a name="p1360819163284"></a>ActionResponse delete(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6609191622820"><a name="p6609191622820"></a><a name="p6609191622820"></a>DELETE /v3/users/{user_id}</p>
<p id="p16609181618283"><a name="p16609181618283"></a><a name="p16609181618283"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1566914308173"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1260931622819"><a name="p1260931622819"></a><a name="p1260931622819"></a>List&lt;? extends Project&gt; listUserProjects(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1609516202811"><a name="p1609516202811"></a><a name="p1609516202811"></a>GET /v3/users/{user_id}/projects</p>
<p id="p15609216182810"><a name="p15609216182810"></a><a name="p15609216182810"></a><a href="https://support.huaweicloud.com/api-iam/iam_06_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1919732119303"><td class="cellrowborder" rowspan="4" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p8197921163016"><a name="p8197921163016"></a><a name="p8197921163016"></a>UserService(iam)</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p1573214579302"><a name="p1573214579302"></a><a name="p1573214579302"></a>CreateUserResp create(CreateUserReq user)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p13732175719304"><a name="p13732175719304"></a><a name="p13732175719304"></a>POST /v3.0/OS-USER/users</p>
<p id="p773285711307"><a name="p773285711307"></a><a name="p773285711307"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0015.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10818152313308"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p373217575309"><a name="p373217575309"></a><a name="p373217575309"></a>QueryUserResp query(String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p073295723019"><a name="p073295723019"></a><a name="p073295723019"></a>GET /v3.0/OS-USER/users/{user_id}</p>
<p id="p7732157133016"><a name="p7732157133016"></a><a name="p7732157133016"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1256202603010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20732155723015"><a name="p20732155723015"></a><a name="p20732155723015"></a>ActionResponse update(String userId, UpdateUserReq user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10732105783010"><a name="p10732105783010"></a><a name="p10732105783010"></a>PUT /v3.0/OS-USER/users/{user_id}/info</p>
<p id="p073245753016"><a name="p073245753016"></a><a name="p073245753016"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1766913091712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p07326572305"><a name="p07326572305"></a><a name="p07326572305"></a>UpdateUserByAdminResp updateByAdmin(String userId, UpdateUserByAdminReq user)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2732155753012"><a name="p2732155753012"></a><a name="p2732155753012"></a>PUT /v3.0/OS-USER/users/{user_id}</p>
<p id="p2732857143019"><a name="p2732857143019"></a><a name="p2732857143019"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row22391638143112"><td class="cellrowborder" rowspan="11" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p3240938123119"><a name="p3240938123119"></a><a name="p3240938123119"></a>GroupService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p173981223113312"><a name="p173981223113312"></a><a name="p173981223113312"></a>List&lt;? extends Group&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p3399923193319"><a name="p3399923193319"></a><a name="p3399923193319"></a>GET /v3/groups</p>
<p id="p139922320338"><a name="p139922320338"></a><a name="p139922320338"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18667165611326"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p139920235332"><a name="p139920235332"></a><a name="p139920235332"></a>Group get(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1639982320337"><a name="p1639982320337"></a><a name="p1639982320337"></a>GET /v3/groups/{group_id}</p>
<p id="p12399323103320"><a name="p12399323103320"></a><a name="p12399323103320"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row22001328339"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33998232331"><a name="p33998232331"></a><a name="p33998232331"></a>Group create(Group group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8399132323319"><a name="p8399132323319"></a><a name="p8399132323319"></a>POST /v3/groups</p>
<p id="p1739972320333"><a name="p1739972320333"></a><a name="p1739972320333"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row136438019332"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p133998237335"><a name="p133998237335"></a><a name="p133998237335"></a>Group update(Group group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4399152373320"><a name="p4399152373320"></a><a name="p4399152373320"></a>PATCH /v3/groups/{group_id}</p>
<p id="p193996236339"><a name="p193996236339"></a><a name="p193996236339"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10501185815325"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14399122303314"><a name="p14399122303314"></a><a name="p14399122303314"></a>ActionResponse delete(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5399192320339"><a name="p5399192320339"></a><a name="p5399192320339"></a>DELETE /v3/groups/{group_id}</p>
<p id="p19399623113317"><a name="p19399623113317"></a><a name="p19399623113317"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5203154993219"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p83991523113318"><a name="p83991523113318"></a><a name="p83991523113318"></a>ActionResponse checkGroupUser(String groupId, String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p93991123173317"><a name="p93991123173317"></a><a name="p93991123173317"></a>HEAD /v3/groups/{group_id}/users/{user_id}</p>
<p id="p1239972333314"><a name="p1239972333314"></a><a name="p1239972333314"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1745985463215"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p43992023203314"><a name="p43992023203314"></a><a name="p43992023203314"></a>ActionResponse addUserToGroup(String groupId, String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53990232335"><a name="p53990232335"></a><a name="p53990232335"></a>PUT /v3/groups/{group_id}/users/{user_id}</p>
<p id="p0399182312336"><a name="p0399182312336"></a><a name="p0399182312336"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14561652133210"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p133990236339"><a name="p133990236339"></a><a name="p133990236339"></a>ActionResponse removeUserFromGroup(String groupId, String userId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12399122313337"><a name="p12399122313337"></a><a name="p12399122313337"></a>DELETE /v3/groups/{group_id}/users/{user_id}</p>
<p id="p639922313313"><a name="p639922313313"></a><a name="p639922313313"></a><a href="https://support.huaweicloud.com/api-iam/iam_09_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3899124410317"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p93991823173310"><a name="p93991823173310"></a><a name="p93991823173310"></a>List&lt;? extends User&gt; listGroupUsers(String groupId, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p139916236339"><a name="p139916236339"></a><a name="p139916236339"></a>GET /v3/groups/{group_id}/users</p>
<p id="p1399223203312"><a name="p1399223203312"></a><a name="p1399223203312"></a><a href="https://support.huaweicloud.com/api-iam/iam_08_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14531114643216"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p153991123123319"><a name="p153991123123319"></a><a name="p153991123123319"></a>List&lt;? extends Role&gt; listDomainGroupRoles(String groupId, String domainId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2400112383315"><a name="p2400112383315"></a><a name="p2400112383315"></a>GET /v3/domains/{domain_id}/groups/{group_id}/roles</p>
<p id="p1540018239331"><a name="p1540018239331"></a><a name="p1540018239331"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2561144233117"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13400162303314"><a name="p13400162303314"></a><a name="p13400162303314"></a>List&lt;? extends Role&gt; listProjectGroupRoles(String groupId, String projectId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1240052383314"><a name="p1240052383314"></a><a name="p1240052383314"></a>GET /v3/projects/{project_id}/groups/{group_id}/roles</p>
<p id="p1440012312333"><a name="p1440012312333"></a><a name="p1440012312333"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6525131815300"><td class="cellrowborder" rowspan="9" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p15482424173414"><a name="p15482424173414"></a><a name="p15482424173414"></a>RoleService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p19629145112348"><a name="p19629145112348"></a><a name="p19629145112348"></a>List&lt;? extends Role&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p1762995123414"><a name="p1762995123414"></a><a name="p1762995123414"></a>GET /v3/roles</p>
<p id="p6629135115345"><a name="p6629135115345"></a><a name="p6629135115345"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2669103091715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p196291851153418"><a name="p196291851153418"></a><a name="p196291851153418"></a>Role get(String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p196303510341"><a name="p196303510341"></a><a name="p196303510341"></a>GET /v3/roles/{role_id}</p>
<p id="p19630185143419"><a name="p19630185143419"></a><a name="p19630185143419"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11669330111719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1563016518349"><a name="p1563016518349"></a><a name="p1563016518349"></a>ActionResponse grantDomainGroupRole(String domainId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17630151173413"><a name="p17630151173413"></a><a name="p17630151173413"></a>PUT /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p063014512346"><a name="p063014512346"></a><a name="p063014512346"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4670203041713"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p146301451123417"><a name="p146301451123417"></a><a name="p146301451123417"></a>ActionResponse grantProjectGroupRole(String projectId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7630551163414"><a name="p7630551163414"></a><a name="p7630551163414"></a>PUT /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p663035114348"><a name="p663035114348"></a><a name="p663035114348"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3670133011719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p963016514346"><a name="p963016514346"></a><a name="p963016514346"></a>ActionResponse checkDomainGroupRole(String domainId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p86301851153414"><a name="p86301851153414"></a><a name="p86301851153414"></a>HEAD /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p56301351133418"><a name="p56301351133418"></a><a name="p56301351133418"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4670230131711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5630125118348"><a name="p5630125118348"></a><a name="p5630125118348"></a>ActionResponse checkProjectGroupRole(String projectId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18630251133416"><a name="p18630251133416"></a><a name="p18630251133416"></a>HEAD /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p76300515344"><a name="p76300515344"></a><a name="p76300515344"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1670103011179"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p166300517340"><a name="p166300517340"></a><a name="p166300517340"></a>ActionResponse revokeDomainGroupRole(String domainId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p563065133417"><a name="p563065133417"></a><a name="p563065133417"></a>DELETE /v3/domains/{domain_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p16301551193418"><a name="p16301551193418"></a><a name="p16301551193418"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16670133017177"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1963065119348"><a name="p1963065119348"></a><a name="p1963065119348"></a>ActionResponse revokeProjectGroupRole(String projectId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p663065123415"><a name="p663065123415"></a><a name="p663065123415"></a>DELETE /v3/projects/{project_id}/groups/{group_id}/roles/{role_id}</p>
<p id="p176302510343"><a name="p176302510343"></a><a name="p176302510343"></a><a href="https://support.huaweicloud.com/api-iam/iam_10_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8890146113214"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2063095119342"><a name="p2063095119342"></a><a name="p2063095119342"></a>ActionResponse grantGroupAllProjectsRole(String domainId, String groupId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p146301551143412"><a name="p146301551143412"></a><a name="p146301551143412"></a>PUT /v3/OS-INHERIT/domains/{domain_id}/groups/{group_id}/roles/{role_id}/inherited_to_projects</p>
<p id="p1263035110342"><a name="p1263035110342"></a><a name="p1263035110342"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0519.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18670930121711"><td class="cellrowborder" rowspan="5" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p6708927356"><a name="p6708927356"></a><a name="p6708927356"></a>CustomRoleService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p137551273617"><a name="p137551273617"></a><a name="p137551273617"></a>List&lt;CreateRoleResp&gt; list().getRoles()</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p183757121368"><a name="p183757121368"></a><a name="p183757121368"></a>GET /v3.0/OS-ROLE/roles</p>
<p id="p183754126367"><a name="p183754126367"></a><a name="p183754126367"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10670730151718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1537541211365"><a name="p1537541211365"></a><a name="p1537541211365"></a>QueryRoleResp get(String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p137591233615"><a name="p137591233615"></a><a name="p137591233615"></a>GET /v3.0/OS-ROLE/roles/{role_id}</p>
<p id="p123753124361"><a name="p123753124361"></a><a name="p123753124361"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0012.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row12670330101712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p837517121363"><a name="p837517121363"></a><a name="p837517121363"></a>CreateRoleResp create(CreateRoleReq roleReq)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1337531213619"><a name="p1337531213619"></a><a name="p1337531213619"></a>POST /v3.0/OS-ROLE/roles</p>
<p id="p137591253614"><a name="p137591253614"></a><a name="p137591253614"></a>创建云服务自定义策略的<a href="https://support.huaweicloud.com/api-iam/iam_02_0013.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p637591211360"><a name="p637591211360"></a><a name="p637591211360"></a>创建委托自定义策略的<a href="https://support.huaweicloud.com/api-iam/iam_02_0016.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row146715307174"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p173751912143619"><a name="p173751912143619"></a><a name="p173751912143619"></a>UpdateRoleResp update(String roleId, UpdateRoleReq updateRoleReq)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p73753122362"><a name="p73753122362"></a><a name="p73753122362"></a>PATCH /v3.0/OS-ROLE/roles/{role_id}</p>
<p id="p5375141220362"><a name="p5375141220362"></a><a name="p5375141220362"></a>修改云服务自定义策略<a href="https://support.huaweicloud.com/api-iam/iam_02_0014.html" target="_blank" rel="noopener noreferrer">链接</a></p>
<p id="p17375212153613"><a name="p17375212153613"></a><a name="p17375212153613"></a>修改委托自定义策略<a href="https://support.huaweicloud.com/api-iam/iam_02_0017.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17671030171710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2375712123612"><a name="p2375712123612"></a><a name="p2375712123612"></a>ActionResponse delete(String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p183766128364"><a name="p183766128364"></a><a name="p183766128364"></a>DELETE /v3.0/OS-ROLE/roles/{role_id}</p>
<p id="p537618127369"><a name="p537618127369"></a><a name="p537618127369"></a><a href="https://support.huaweicloud.com/api-iam/iam_02_0015.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6671143015171"><td class="cellrowborder" rowspan="13" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p970812214350"><a name="p970812214350"></a><a name="p970812214350"></a>AgencyService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p4549111373811"><a name="p4549111373811"></a><a name="p4549111373811"></a>ListAgenciesResp listAgencies(String domainId, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p1354981319384"><a name="p1354981319384"></a><a name="p1354981319384"></a>GET /v3.0/OS-AGENCY/agencies</p>
<p id="p9549151313820"><a name="p9549151313820"></a><a name="p9549151313820"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1067163091715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p35491413113811"><a name="p35491413113811"></a><a name="p35491413113811"></a>AgencyResp get(String agencyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p05491134389"><a name="p05491134389"></a><a name="p05491134389"></a>GET /v3.0/OS-AGENCY/agencies/{agency_id}</p>
<p id="p654971316385"><a name="p654971316385"></a><a name="p654971316385"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row126711430161710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1854911136388"><a name="p1854911136388"></a><a name="p1854911136388"></a>AgencyResp create(CreateAgencyReq createAgencyReq)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p65490134388"><a name="p65490134388"></a><a name="p65490134388"></a>POST /v3.0/OS-AGENCY/agencies</p>
<p id="p18549201323811"><a name="p18549201323811"></a><a name="p18549201323811"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row367113091713"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18549913133820"><a name="p18549913133820"></a><a name="p18549913133820"></a>AgencyResp update(String agencyId, UpdateAgencyReq updateAgencyReq)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1254916134384"><a name="p1254916134384"></a><a name="p1254916134384"></a>PUT /v3.0/OS-AGENCY/agencies/{agency_id}</p>
<p id="p05491613183815"><a name="p05491613183815"></a><a name="p05491613183815"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row166711430201719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p45508135386"><a name="p45508135386"></a><a name="p45508135386"></a>ActionResponse delete(String agencyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p25501813203819"><a name="p25501813203819"></a><a name="p25501813203819"></a>DELETE /v3.0/OS-AGENCY/agencies/{agency_id}</p>
<p id="p205504132384"><a name="p205504132384"></a><a name="p205504132384"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8672193091720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15550151373818"><a name="p15550151373818"></a><a name="p15550151373818"></a>ListPermissionsResp listPermissionsOnDomain(String domainId, String agencyID)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p755031303811"><a name="p755031303811"></a><a name="p755031303811"></a>GET /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles</p>
<p id="p105507134385"><a name="p105507134385"></a><a name="p105507134385"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row126721330131717"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p555081316383"><a name="p555081316383"></a><a name="p555081316383"></a>ListPermissionsResp listPermissionsOnProject(String projectId, String agencyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14550613153817"><a name="p14550613153817"></a><a name="p14550613153817"></a>GET /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles</p>
<p id="p35509133381"><a name="p35509133381"></a><a name="p35509133381"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row146721330151716"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19550151363810"><a name="p19550151363810"></a><a name="p19550151363810"></a>ActionResponse addPermissionOnDomain(String domainId, String agencyId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p055015133386"><a name="p055015133386"></a><a name="p055015133386"></a>PUT /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p1455051310382"><a name="p1455051310382"></a><a name="p1455051310382"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row367214306176"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p855021323816"><a name="p855021323816"></a><a name="p855021323816"></a>ActionResponse addPermissionOnProject(String projectId, String agencyId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1055071315386"><a name="p1055071315386"></a><a name="p1055071315386"></a>PUT /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p555051383819"><a name="p555051383819"></a><a name="p555051383819"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row96721308178"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1255091393817"><a name="p1255091393817"></a><a name="p1255091393817"></a>ActionResponse checkPermissionOnDomain(String domainId, String agencyId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4550191316385"><a name="p4550191316385"></a><a name="p4550191316385"></a>HEAD /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p18550181333819"><a name="p18550181333819"></a><a name="p18550181333819"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row667218309178"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1455011373818"><a name="p1455011373818"></a><a name="p1455011373818"></a>ActionResponse checkPermissionOnProject(String projectId, String agencyId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p755019131385"><a name="p755019131385"></a><a name="p755019131385"></a>HEAD /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p115501513123820"><a name="p115501513123820"></a><a name="p115501513123820"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0011.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row156721530131712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p35507131383"><a name="p35507131383"></a><a name="p35507131383"></a>ActionResponse deletePermissionOnDomain(String domainId, String agencyId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16550213173814"><a name="p16550213173814"></a><a name="p16550213173814"></a>DELETE /v3.0/OS-AGENCY/domains/{domain_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p175501132389"><a name="p175501132389"></a><a name="p175501132389"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0012.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20673123016178"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p185501013183818"><a name="p185501013183818"></a><a name="p185501013183818"></a>ActionResponse deletePermissionOnProject(String projectId, String agencyId, String roleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p85507134383"><a name="p85507134383"></a><a name="p85507134383"></a>DELETE /v3.0/OS-AGENCY/projects/{project_id}/agencies/{agency_id}/roles/{role_id}</p>
<p id="p19550613163810"><a name="p19550613163810"></a><a name="p19550613163810"></a><a href="https://support.huaweicloud.com/api-iam/iam_12_0013.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46731730141718"><td class="cellrowborder" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p9800205415382"><a name="p9800205415382"></a><a name="p9800205415382"></a>VersionService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p19801354143819"><a name="p19801354143819"></a><a name="p19801354143819"></a>Version get()</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p28011754183812"><a name="p28011754183812"></a><a name="p28011754183812"></a>GET /v3</p>
<p id="p1801554183813"><a name="p1801554183813"></a><a name="p1801554183813"></a><a href="https://support.huaweicloud.com/api-iam/iam_15_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1839717567334"><td class="cellrowborder" rowspan="4" valign="top" width="28.372837283728376%" headers="mcps1.1.4.1.1 "><p id="p820412503370"><a name="p820412503370"></a><a name="p820412503370"></a>ServiceEndpointService</p>
</td>
<td class="cellrowborder" valign="top" width="35.98359835983598%" headers="mcps1.1.4.1.2 "><p id="p85551845399"><a name="p85551845399"></a><a name="p85551845399"></a>List&lt;? extends Service&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="35.64356435643564%" headers="mcps1.1.4.1.3 "><p id="p05551846390"><a name="p05551846390"></a><a name="p05551846390"></a>GET /v3/services</p>
<p id="p135551142396"><a name="p135551142396"></a><a name="p135551142396"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20673143071719"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p165554413393"><a name="p165554413393"></a><a name="p165554413393"></a>Service get(String serviceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p05555419394"><a name="p05555419394"></a><a name="p05555419394"></a>GET /v3/services/{service_id}</p>
<p id="p2055518420399"><a name="p2055518420399"></a><a name="p2055518420399"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row136731030201710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10555247391"><a name="p10555247391"></a><a name="p10555247391"></a>List&lt;? extends Endpoint&gt; listEndpoints(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17555046399"><a name="p17555046399"></a><a name="p17555046399"></a>GET /v3/endpoints</p>
<p id="p1355516415396"><a name="p1355516415396"></a><a name="p1355516415396"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1373094473417"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p655564173917"><a name="p655564173917"></a><a name="p655564173917"></a>Endpoint getEndpoint(String endpointId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15555124173912"><a name="p15555124173912"></a><a name="p15555124173912"></a>GET /v3/endpoints/{endpoint_id}</p>
<p id="p13555846396"><a name="p13555846396"></a><a name="p13555846396"></a><a href="https://support.huaweicloud.com/api-iam/iam_16_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

