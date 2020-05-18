# VPC<a name="sdk_11_0003"></a>

基于VPC v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table13932119153012"></a>
<table><thead align="left"><tr id="row10933159173015"><th class="cellrowborder" valign="top" width="29.762976297629763%" id="mcps1.1.4.1.1"><p id="p1313216289303"><a name="p1313216289303"></a><a name="p1313216289303"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.923592359235926%" id="mcps1.1.4.1.2"><p id="p1113412813015"><a name="p1113412813015"></a><a name="p1113412813015"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.31343134313431%" id="mcps1.1.4.1.3"><p id="p2013511285302"><a name="p2013511285302"></a><a name="p2013511285302"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1353414516315"><td class="cellrowborder" rowspan="6" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p3212181916324"><a name="p3212181916324"></a><a name="p3212181916324"></a>VpcService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p17361810193210"><a name="p17361810193210"></a><a name="p17361810193210"></a>Vpc create(VpcCreate creation)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p7361810163217"><a name="p7361810163217"></a><a name="p7361810163217"></a>POST /v1/{project_id}/vpcs</p>
<p id="p129159532208"><a name="p129159532208"></a><a name="p129159532208"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17021347153118"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p936310183218"><a name="p936310183218"></a><a name="p936310183218"></a>Vpc get(String vpcId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p736201063217"><a name="p736201063217"></a><a name="p736201063217"></a>GET /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p141113298219"><a name="p141113298219"></a><a name="p141113298219"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1648758133116"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1936171033219"><a name="p1936171033219"></a><a name="p1936171033219"></a>List&lt;? extends Vpc&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p736121010324"><a name="p736121010324"></a><a name="p736121010324"></a>GET /v1/{project_id}/vpcs</p>
<p id="p47641148132114"><a name="p47641148132114"></a><a name="p47641148132114"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2053941123217"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p336710143210"><a name="p336710143210"></a><a name="p336710143210"></a>List&lt;? extends Vpc&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1536111018325"><a name="p1536111018325"></a><a name="p1536111018325"></a>GET /v1/{project_id}/vpcs</p>
<p id="p4166810152214"><a name="p4166810152214"></a><a name="p4166810152214"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14754115516318"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8364109324"><a name="p8364109324"></a><a name="p8364109324"></a>Vpc update(String vpcId, VpcUpdate vpcUpdate)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11361110153211"><a name="p11361110153211"></a><a name="p11361110153211"></a>PUT /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p20749141818221"><a name="p20749141818221"></a><a name="p20749141818221"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1726615473212"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15361410153214"><a name="p15361410153214"></a><a name="p15361410153214"></a>ActionResponse delete(String vpcId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p436101063210"><a name="p436101063210"></a><a name="p436101063210"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}</p>
<p id="p12110133682214"><a name="p12110133682214"></a><a name="p12110133682214"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_api01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1447443401314"><td class="cellrowborder" rowspan="6" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p793315918303"><a name="p793315918303"></a><a name="p793315918303"></a>PublicIpService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p83138761412"><a name="p83138761412"></a><a name="p83138761412"></a>VirtualPublicIpsResp apply(VirtualPublicIps virtualPublicIps)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p19313177111417"><a name="p19313177111417"></a><a name="p19313177111417"></a>POST /v1/{project_id}/publicips</p>
<p id="p6321032193916"><a name="p6321032193916"></a><a name="p6321032193916"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row09336963010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13957119101213"><a name="p13957119101213"></a><a name="p13957119101213"></a>VirtualPublicIp get(String publicipId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8605142153014"><a name="p8605142153014"></a><a name="p8605142153014"></a>GET /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p144317140236"><a name="p144317140236"></a><a name="p144317140236"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10611183717136"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p85204592138"><a name="p85204592138"></a><a name="p85204592138"></a>List&lt;? extends PublicIp&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p135201959161312"><a name="p135201959161312"></a><a name="p135201959161312"></a>GET /v1/{project_id}/publicips</p>
<p id="p27535285231"><a name="p27535285231"></a><a name="p27535285231"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5481174016139"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18520459111314"><a name="p18520459111314"></a><a name="p18520459111314"></a>List&lt;? extends PublicIp&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19520195914137"><a name="p19520195914137"></a><a name="p19520195914137"></a>GET /v1/{project_id}/publicips</p>
<p id="p0788133632317"><a name="p0788133632317"></a><a name="p0788133632317"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1582694816131"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1552075913136"><a name="p1552075913136"></a><a name="p1552075913136"></a>PublicIp update(String publicIpId, PublicIpUpdate publicIpUpdate)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p052025901318"><a name="p052025901318"></a><a name="p052025901318"></a>PUT /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p7761164611232"><a name="p7761164611232"></a><a name="p7761164611232"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1069823104911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p142012711498"><a name="p142012711498"></a><a name="p142012711498"></a>ActionResponse delete(String publicIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p74207272496"><a name="p74207272496"></a><a name="p74207272496"></a>DELETE /v1/{project_id}/publicips/{publicip_id}</p>
<p id="p17532854172312"><a name="p17532854172312"></a><a name="p17532854172312"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3755201101711"><td class="cellrowborder" rowspan="5" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p1876893711173"><a name="p1876893711173"></a><a name="p1876893711173"></a>PrivateIpService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p57681937101718"><a name="p57681937101718"></a><a name="p57681937101718"></a>List&lt;? extends PrivateIp&gt; apply(PrivateIps privateIps)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p17768143715173"><a name="p17768143715173"></a><a name="p17768143715173"></a>POST /v1/{project_id}/privateips</p>
<p id="p38484513246"><a name="p38484513246"></a><a name="p38484513246"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row59951319121714"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p576883716179"><a name="p576883716179"></a><a name="p576883716179"></a>PrivateIp get(String privateIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p376893711171"><a name="p376893711171"></a><a name="p376893711171"></a>GET /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p65511113192414"><a name="p65511113192414"></a><a name="p65511113192414"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1198161771720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15768163791720"><a name="p15768163791720"></a><a name="p15768163791720"></a>List&lt;? extends PrivateIp&gt; list(String subnetId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13768153716171"><a name="p13768153716171"></a><a name="p13768153716171"></a>GET /v1/{project_id}/subnets/{subnet_id}/privateips</p>
<p id="p84821621132410"><a name="p84821621132410"></a><a name="p84821621132410"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4516314131718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7768153712177"><a name="p7768153712177"></a><a name="p7768153712177"></a>List&lt;? extends PrivateIp&gt; list(String subnetId, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19768123719179"><a name="p19768123719179"></a><a name="p19768123719179"></a>GET /v1/{project_id}/subnets/{subnet_id}/privateips</p>
<p id="p14806142802413"><a name="p14806142802413"></a><a name="p14806142802413"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row37644551711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p97681376176"><a name="p97681376176"></a><a name="p97681376176"></a>ActionResponse delete(String privateIpId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14768437191719"><a name="p14768437191719"></a><a name="p14768437191719"></a>DELETE /v1/{project_id}/privateips/{privateip_id}</p>
<p id="p14515103710242"><a name="p14515103710242"></a><a name="p14515103710242"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_privateip_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row16443245183"><td class="cellrowborder" rowspan="10" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p1132618461918"><a name="p1132618461918"></a><a name="p1132618461918"></a>SecurityGroupService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p9326124181910"><a name="p9326124181910"></a><a name="p9326124181910"></a>SecurityGroup create(SecurityGroupCreate securityGroup)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p632618412199"><a name="p632618412199"></a><a name="p632618412199"></a>POST /v1/{project_id}/security-groups</p>
<p id="p1345664617246"><a name="p1345664617246"></a><a name="p1345664617246"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46391234171817"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p43269419198"><a name="p43269419198"></a><a name="p43269419198"></a>SecurityGroup get(String securityGroupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p43265471919"><a name="p43265471919"></a><a name="p43265471919"></a>GET /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p1834165219245"><a name="p1834165219245"></a><a name="p1834165219245"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row105723851819"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p133261549195"><a name="p133261549195"></a><a name="p133261549195"></a>List&lt;? extends SecurityGroup&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23265451914"><a name="p23265451914"></a><a name="p23265451914"></a>GET /v1/{project_id}/security-groups</p>
<p id="p2904112252"><a name="p2904112252"></a><a name="p2904112252"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1073484031812"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p432610441912"><a name="p432610441912"></a><a name="p432610441912"></a>List&lt;? extends SecurityGroup&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p163271845194"><a name="p163271845194"></a><a name="p163271845194"></a>GET /v1/{project_id}/security-groups</p>
<p id="p185951683254"><a name="p185951683254"></a><a name="p185951683254"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1281714501816"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p83271348194"><a name="p83271348194"></a><a name="p83271348194"></a>ActionResponse delete(String securityGroupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p173276418196"><a name="p173276418196"></a><a name="p173276418196"></a>DELETE /v1/{project_id}/security-groups/{security_group_id}</p>
<p id="p7583151582510"><a name="p7583151582510"></a><a name="p7583151582510"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15153164321813"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p83271647198"><a name="p83271647198"></a><a name="p83271647198"></a>SecurityGroupRule createSecurityGroupRule(SecurityGroupRule securityGroupRule)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p43278431919"><a name="p43278431919"></a><a name="p43278431919"></a>POST /v1/{project_id}/security-group-rules</p>
<p id="p83021322172512"><a name="p83021322172512"></a><a name="p83021322172512"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row289013316185"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p53272417199"><a name="p53272417199"></a><a name="p53272417199"></a>SecurityGroupRule getSecurityGroupRule(String securityGroupRuleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23279491916"><a name="p23279491916"></a><a name="p23279491916"></a>GET /v1/{project_id}/security-group-rules/{rules_security_groups_id}</p>
<p id="p1484332882511"><a name="p1484332882511"></a><a name="p1484332882511"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row65681329101813"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13279420198"><a name="p13279420198"></a><a name="p13279420198"></a>List&lt;? extends SecurityGroupRule&gt; listSecurityGroupRules()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p203275431913"><a name="p203275431913"></a><a name="p203275431913"></a>GET /v1/{project_id}/security-group-rules</p>
<p id="p44493712251"><a name="p44493712251"></a><a name="p44493712251"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21381527111812"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8327144181913"><a name="p8327144181913"></a><a name="p8327144181913"></a>List&lt;? extends SecurityGroupRule&gt; listSecurityGroupRules(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p63279431912"><a name="p63279431912"></a><a name="p63279431912"></a>GET /v1/{project_id}/security-group-rules</p>
<p id="p894434542520"><a name="p894434542520"></a><a name="p894434542520"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14896415141814"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16327144141915"><a name="p16327144141915"></a><a name="p16327144141915"></a>ActionResponse deleteSecurityGroupRule(String securityGroupRuleId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p123271410199"><a name="p123271410199"></a><a name="p123271410199"></a>DELETE /v1/{project_id}/security-group-rules/{rules_security_groups_id}</p>
<p id="p586317524255"><a name="p586317524255"></a><a name="p586317524255"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg01_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19933199173015"><td class="cellrowborder" rowspan="4" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p1981919199312"><a name="p1981919199312"></a><a name="p1981919199312"></a>BandWidthService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p18857427131216"><a name="p18857427131216"></a><a name="p18857427131216"></a>VirtualBandWidths get(String bandwidthId)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p16052042153013"><a name="p16052042153013"></a><a name="p16052042153013"></a>GET /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p68171309268"><a name="p68171309268"></a><a name="p68171309268"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row393319943016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p116052042163018"><a name="p116052042163018"></a><a name="p116052042163018"></a>List&lt;VirtualBandWidths&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17605114219300"><a name="p17605114219300"></a><a name="p17605114219300"></a>GET /v1/{project_id}/bandwidths</p>
<p id="p375298162614"><a name="p375298162614"></a><a name="p375298162614"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19335915301"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p631754712121"><a name="p631754712121"></a><a name="p631754712121"></a>List&lt;VirtualBandWidths&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17605184216302"><a name="p17605184216302"></a><a name="p17605184216302"></a>GET /v1/{project_id}/bandwidths</p>
<p id="p1544021514269"><a name="p1544021514269"></a><a name="p1544021514269"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1262132341514"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14350113711153"><a name="p14350113711153"></a><a name="p14350113711153"></a>VirtualBandWidths update(VirtualBandWidthUpdate bandWidtUpdate, String bandwidthId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9350137201512"><a name="p9350137201512"></a><a name="p9350137201512"></a>PUT /v1/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p152242231267"><a name="p152242231267"></a><a name="p152242231267"></a><a href="https://support.huaweicloud.com/api-eip/eip_apiBandwidth_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row14947255151511"><td class="cellrowborder" rowspan="2" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p899018264167"><a name="p899018264167"></a><a name="p899018264167"></a>QuotaService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p399142613167"><a name="p399142613167"></a><a name="p399142613167"></a>Quotas list()</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p099192620165"><a name="p099192620165"></a><a name="p099192620165"></a>GET /v1/{project_id}/quotas</p>
<p id="p2370204332614"><a name="p2370204332614"></a><a name="p2370204332614"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_quota_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row175101659141513"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5991726111612"><a name="p5991726111612"></a><a name="p5991726111612"></a>Quotas list(String type)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p399111260169"><a name="p399111260169"></a><a name="p399111260169"></a>GET /v1/{project_id}/quotas</p>
<p id="p1423335072614"><a name="p1423335072614"></a><a name="p1423335072614"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_quota_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row10882131972610"><td class="cellrowborder" rowspan="6" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p1072264442615"><a name="p1072264442615"></a><a name="p1072264442615"></a>SubnetService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p134921459182610"><a name="p134921459182610"></a><a name="p134921459182610"></a>Subnet create(SubnetCreate creation)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p1749255920264"><a name="p1749255920264"></a><a name="p1749255920264"></a>POST /v1/{project_id}/subnets</p>
<p id="p922718563261"><a name="p922718563261"></a><a name="p922718563261"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1924332715268"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11492459112619"><a name="p11492459112619"></a><a name="p11492459112619"></a>Subnet get(String subnetId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1349217595269"><a name="p1349217595269"></a><a name="p1349217595269"></a>GET /v1/{project_id}/subnets/{subnet_id}</p>
<p id="p3938346277"><a name="p3938346277"></a><a name="p3938346277"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row116531040133710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p28624916129"><a name="p28624916129"></a><a name="p28624916129"></a>List&lt;? extends Subnet&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1586124915122"><a name="p1586124915122"></a><a name="p1586124915122"></a>GET /v1/{project_id}/subnets</p>
<p id="p1156011119279"><a name="p1156011119279"></a><a name="p1156011119279"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1839713301260"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1849285902615"><a name="p1849285902615"></a><a name="p1849285902615"></a>List&lt;? extends Subnet&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44921059132611"><a name="p44921059132611"></a><a name="p44921059132611"></a>GET /v1/{project_id}/subnets</p>
<p id="p1243282172716"><a name="p1243282172716"></a><a name="p1243282172716"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18275153412263"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3492135914267"><a name="p3492135914267"></a><a name="p3492135914267"></a>SubnetUpdateResp update(String vpcId, String subnetId, SubnetUpdate subnetUpdate)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10492125918267"><a name="p10492125918267"></a><a name="p10492125918267"></a>PUT /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p1414430162719"><a name="p1414430162719"></a><a name="p1414430162719"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6781537172617"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1949285912267"><a name="p1949285912267"></a><a name="p1949285912267"></a>ActionResponse delete(String vpcId,String subnetId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p154921459132613"><a name="p154921459132613"></a><a name="p154921459132613"></a>DELETE /v1/{project_id}/vpcs/{vpc_id}/subnets/{subnet_id}</p>
<p id="p153591383276"><a name="p153591383276"></a><a name="p153591383276"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6183539131918"><td class="cellrowborder" rowspan="6" valign="top" width="29.762976297629763%" headers="mcps1.1.4.1.1 "><p id="p4680111711209"><a name="p4680111711209"></a><a name="p4680111711209"></a>PortService</p>
</td>
<td class="cellrowborder" valign="top" width="35.923592359235926%" headers="mcps1.1.4.1.2 "><p id="p868011762019"><a name="p868011762019"></a><a name="p868011762019"></a>Port create(PortCreate port)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p09351534110"><a name="p09351534110"></a><a name="p09351534110"></a>POST /v1/{project_id}/ports</p>
<p id="p314889182820"><a name="p314889182820"></a><a name="p314889182820"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row0133942141911"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p768015172208"><a name="p768015172208"></a><a name="p768015172208"></a>Port get(String portId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1860221824120"><a name="p1860221824120"></a><a name="p1860221824120"></a>GET /v1/{project_id}/ports/{port_id}</p>
<p id="p12893111520286"><a name="p12893111520286"></a><a name="p12893111520286"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row285115315193"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14680417152019"><a name="p14680417152019"></a><a name="p14680417152019"></a>List&lt;? extends Port&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p66801717172016"><a name="p66801717172016"></a><a name="p66801717172016"></a>GET /v1/{project_id}/ports</p>
<p id="p045132217286"><a name="p045132217286"></a><a name="p045132217286"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row123482059201917"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1368071732017"><a name="p1368071732017"></a><a name="p1368071732017"></a>List&lt;? extends Port&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16680017172016"><a name="p16680017172016"></a><a name="p16680017172016"></a>GET /v1/{project_id}/ports</p>
<p id="p363762862813"><a name="p363762862813"></a><a name="p363762862813"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21579215203"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20680617102010"><a name="p20680617102010"></a><a name="p20680617102010"></a>Port update(String portId, PortUpdate portUpdate)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p159069275416"><a name="p159069275416"></a><a name="p159069275416"></a>PUT /v1/{project_id}/ports/{port_id}</p>
<p id="p5902143411286"><a name="p5902143411286"></a><a name="p5902143411286"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row751613565195"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12680617202012"><a name="p12680617202012"></a><a name="p12680617202012"></a>ActionResponse delete(String portId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p147301330144116"><a name="p147301330144116"></a><a name="p147301330144116"></a>DELETE /v1/{project_id}/ports/{port_id}</p>
<p id="p11589134192820"><a name="p11589134192820"></a><a name="p11589134192820"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于VPC v2.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table120500281647"></a>
<table><thead align="left"><tr id="row222582271647"><th class="cellrowborder" valign="top" width="29.652965296529647%" id="mcps1.1.4.1.1"><p id="p35465461650"><a name="p35465461650"></a><a name="p35465461650"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.03360336033604%" id="mcps1.1.4.1.2"><p id="p233839291650"><a name="p233839291650"></a><a name="p233839291650"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.31343134313431%" id="mcps1.1.4.1.3"><p id="p16716361650"><a name="p16716361650"></a><a name="p16716361650"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row565746271647"><td class="cellrowborder" valign="top" width="29.652965296529647%" headers="mcps1.1.4.1.1 "><p id="p4509826216441"><a name="p4509826216441"></a><a name="p4509826216441"></a>PublicIpService</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p1786345641211"><a name="p1786345641211"></a><a name="p1786345641211"></a>AsyncPublicipRespEntity apply(VirtualPublicIps virtualPublicIps)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p542342516441"><a name="p542342516441"></a><a name="p542342516441"></a>POST /v2.0/{project_id}/publicips</p>
<p id="p17781359182818"><a name="p17781359182818"></a><a name="p17781359182818"></a><a href="https://support.huaweicloud.com/api-eip/eip_api_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row602723261647"><td class="cellrowborder" valign="top" width="29.652965296529647%" headers="mcps1.1.4.1.1 "><p id="p3619627016441"><a name="p3619627016441"></a><a name="p3619627016441"></a>BandWidthService</p>
</td>
<td class="cellrowborder" valign="top" width="36.03360336033604%" headers="mcps1.1.4.1.2 "><p id="p181358319134"><a name="p181358319134"></a><a name="p181358319134"></a>AsyncBandWidthRespEntity update(VirtualBandWidths bandWidth, String bandwidthId)</p>
</td>
<td class="cellrowborder" valign="top" width="34.31343134313431%" headers="mcps1.1.4.1.3 "><p id="p3880679616441"><a name="p3880679616441"></a><a name="p3880679616441"></a>PUT /v2.0/{project_id}/bandwidths/{bandwidth_id}</p>
<p id="p018005622914"><a name="p018005622914"></a><a name="p018005622914"></a><a href="https://support.huaweicloud.com/api-eip/eip_apisharedbandwidth_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

基于Neutron v2.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table41033878"></a>
<table><thead align="left"><tr id="row59951903"><th class="cellrowborder" valign="top" width="29.222922292229224%" id="mcps1.1.4.1.1"><p id="p24265995"><a name="p24265995"></a><a name="p24265995"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.773677367736774%" id="mcps1.1.4.1.2"><p id="p19388612"><a name="p19388612"></a><a name="p19388612"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.003400340034005%" id="mcps1.1.4.1.3"><p id="p26973745"><a name="p26973745"></a><a name="p26973745"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row37389755"><td class="cellrowborder" rowspan="7" valign="top" width="29.222922292229224%" headers="mcps1.1.4.1.1 "><p id="p8671305"><a name="p8671305"></a><a name="p8671305"></a>NetFloatingIPService</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.1.4.1.2 "><p id="p31287108"><a name="p31287108"></a><a name="p31287108"></a>NetFloatingIP associateToPort(String id, String portId)</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.4.1.3 "><p id="p51227795"><a name="p51227795"></a><a name="p51227795"></a>PUT /v2.0/floatingips/{floatingip_id}</p>
<p id="p529812501326"><a name="p529812501326"></a><a name="p529812501326"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row58396974"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32534423"><a name="p32534423"></a><a name="p32534423"></a>NetFloatingIP create(NetFloatingIP floatingIp)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18042568"><a name="p18042568"></a><a name="p18042568"></a>POST /v2.0/floatingips</p>
<p id="p18169576328"><a name="p18169576328"></a><a name="p18169576328"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row28165387"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66803900"><a name="p66803900"></a><a name="p66803900"></a>ActionResponse delete(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p42406858"><a name="p42406858"></a><a name="p42406858"></a>DELETE /v2.0/floatingips/{floatingip_id}</p>
<p id="p5624118143412"><a name="p5624118143412"></a><a name="p5624118143412"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0010.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46117407"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p44522499"><a name="p44522499"></a><a name="p44522499"></a>NetFloatingIP disassociateFromPort(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p49552630"><a name="p49552630"></a><a name="p49552630"></a>PUT /v2.0/floatingips/{floatingip_id}</p>
<p id="p9127191612349"><a name="p9127191612349"></a><a name="p9127191612349"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port01_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row43320494"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19299134"><a name="p19299134"></a><a name="p19299134"></a>NetFloatingIP get(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19726002"><a name="p19726002"></a><a name="p19726002"></a>GET /v2.0/floatingips/{floatingip_id}</p>
<p id="p10969722143414"><a name="p10969722143414"></a><a name="p10969722143414"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row43316293"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18958859"><a name="p18958859"></a><a name="p18958859"></a>List&lt;? extends NetFloatingIP&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p59272617"><a name="p59272617"></a><a name="p59272617"></a>GET /v2.0/floatingips</p>
<p id="p13523290344"><a name="p13523290344"></a><a name="p13523290344"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row63691513"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p58738960"><a name="p58738960"></a><a name="p58738960"></a>List&lt;? extends NetFloatingIP&gt; list(Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p60235282"><a name="p60235282"></a><a name="p60235282"></a>GET /v2.0/floatingips</p>
<p id="p2951635133416"><a name="p2951635133416"></a><a name="p2951635133416"></a><a href="https://support.huaweicloud.com/api-eip/eip_openstackapi_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5246632"><td class="cellrowborder" rowspan="6" valign="top" width="29.222922292229224%" headers="mcps1.1.4.1.1 "><p id="p22324024"><a name="p22324024"></a><a name="p22324024"></a>NetworkService</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.1.4.1.2 "><p id="p63415529"><a name="p63415529"></a><a name="p63415529"></a>Network create(Network network)</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.4.1.3 "><p id="p36384226"><a name="p36384226"></a><a name="p36384226"></a>POST /v2.0/networks</p>
<p id="p88121744123418"><a name="p88121744123418"></a><a name="p88121744123418"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row59022586"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16100147"><a name="p16100147"></a><a name="p16100147"></a>ActionResponse delete(String networkId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p29043529"><a name="p29043529"></a><a name="p29043529"></a>DELETE /v2.0/networks/{network_id}</p>
<p id="p1399015043418"><a name="p1399015043418"></a><a name="p1399015043418"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row60065170"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p33440573"><a name="p33440573"></a><a name="p33440573"></a>Network get(String networkId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p24331897"><a name="p24331897"></a><a name="p24331897"></a>GET /v2.0/networks/{network_id}</p>
<p id="p9376195716344"><a name="p9376195716344"></a><a name="p9376195716344"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row17660485"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p21213148"><a name="p21213148"></a><a name="p21213148"></a>List&lt;? extends Network&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p40543448"><a name="p40543448"></a><a name="p40543448"></a>GET /v2.0/networks</p>
<p id="p11146115424215"><a name="p11146115424215"></a><a name="p11146115424215"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8802931104712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3187144164717"><a name="p3187144164717"></a><a name="p3187144164717"></a>List&lt;? extends Network&gt; list(Map&lt;String, String&gt;filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1084064564720"><a name="p1084064564720"></a><a name="p1084064564720"></a>GET /v2.0/networks</p>
<p id="p1631316430"><a name="p1631316430"></a><a name="p1631316430"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row29346720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p28274094"><a name="p28274094"></a><a name="p28274094"></a>Network update(String networkId, NetworkUpdate network)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8500244"><a name="p8500244"></a><a name="p8500244"></a>PUT /v2.0/networks/{network_id}</p>
<p id="p1552181014434"><a name="p1552181014434"></a><a name="p1552181014434"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_network_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9393336"><td class="cellrowborder" rowspan="6" valign="top" width="29.222922292229224%" headers="mcps1.1.4.1.1 "><p id="p22662742"><a name="p22662742"></a><a name="p22662742"></a>PortService</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.1.4.1.2 "><p id="p23742817"><a name="p23742817"></a><a name="p23742817"></a>Port create(Port port)</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.4.1.3 "><p id="p44120000"><a name="p44120000"></a><a name="p44120000"></a>POST /v2.0/ports</p>
<p id="p152236311266"><a name="p152236311266"></a><a name="p152236311266"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row61535683"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18334396"><a name="p18334396"></a><a name="p18334396"></a>ActionResponse delete(String portId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8691069"><a name="p8691069"></a><a name="p8691069"></a>DELETE /v2.0/ports/{port_id}</p>
<p id="p15316114011267"><a name="p15316114011267"></a><a name="p15316114011267"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11110760"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p27556393"><a name="p27556393"></a><a name="p27556393"></a>Port get(String portId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17475399"><a name="p17475399"></a><a name="p17475399"></a>GET /v2.0/ports/{port_id}</p>
<p id="p1764484672614"><a name="p1764484672614"></a><a name="p1764484672614"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row23060868"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p55991032"><a name="p55991032"></a><a name="p55991032"></a>List&lt;? extends Port&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38979707"><a name="p38979707"></a><a name="p38979707"></a>GET /v2.0/ports</p>
<p id="p17187528266"><a name="p17187528266"></a><a name="p17187528266"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15273051"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p29157627"><a name="p29157627"></a><a name="p29157627"></a>List&lt;? extends Port&gt; list(PortListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12957567"><a name="p12957567"></a><a name="p12957567"></a>GET /v2.0/ports?network_id={network_id}</p>
<p id="p73143013272"><a name="p73143013272"></a><a name="p73143013272"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row49509242"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p50825680"><a name="p50825680"></a><a name="p50825680"></a>Port update(Port port)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23239422"><a name="p23239422"></a><a name="p23239422"></a>PUT /v2.0/ports/{port_id}</p>
<p id="p1392105132710"><a name="p1392105132710"></a><a name="p1392105132710"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_port02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7828214"><td class="cellrowborder" rowspan="9" valign="top" width="29.222922292229224%" headers="mcps1.1.4.1.1 "><p id="p30105629"><a name="p30105629"></a><a name="p30105629"></a>RouterService</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.1.4.1.2 "><p id="p22636847"><a name="p22636847"></a><a name="p22636847"></a>RouterInterface attachInterface(String routerId, AttachInterfaceType type, String portOrSubnetId)</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.4.1.3 "><p id="p21645334"><a name="p21645334"></a><a name="p21645334"></a>PUT /v2.0/routers/{router_id}/add_router_interface</p>
<p id="p28261213271"><a name="p28261213271"></a><a name="p28261213271"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row60590285"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8866062"><a name="p8866062"></a><a name="p8866062"></a>Router create(Router router)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p47062423"><a name="p47062423"></a><a name="p47062423"></a>POST /v2.0/routers</p>
<p id="p571616183271"><a name="p571616183271"></a><a name="p571616183271"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20908631"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15877536"><a name="p15877536"></a><a name="p15877536"></a>Router create(String name, boolean adminStateUp)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11012038"><a name="p11012038"></a><a name="p11012038"></a>POST /v2.0/routers</p>
<p id="p3589172816273"><a name="p3589172816273"></a><a name="p3589172816273"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31999479"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41820978"><a name="p41820978"></a><a name="p41820978"></a>ActionResponse delete(String routerId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p32056062"><a name="p32056062"></a><a name="p32056062"></a>DELETE /v2.0/routers/{router_id}</p>
<p id="p7461934172720"><a name="p7461934172720"></a><a name="p7461934172720"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20069106"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14984857"><a name="p14984857"></a><a name="p14984857"></a>RouterInterface detachInterface(String routerId, String subnetId, String portId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5813925"><a name="p5813925"></a><a name="p5813925"></a>PUT /v2.0/routers/{router_id}/remove_router_interface</p>
<p id="p16887175672717"><a name="p16887175672717"></a><a name="p16887175672717"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52325333"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10493555"><a name="p10493555"></a><a name="p10493555"></a>Router get(String routerId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p44671593"><a name="p44671593"></a><a name="p44671593"></a>GET /v2.0/routers/{router_id}</p>
<p id="p74271446289"><a name="p74271446289"></a><a name="p74271446289"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row66500021"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17792611"><a name="p17792611"></a><a name="p17792611"></a>List&lt;? extends Router&gt;list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p31915390"><a name="p31915390"></a><a name="p31915390"></a>GET /v2.0/routers</p>
<p id="p1465191142819"><a name="p1465191142819"></a><a name="p1465191142819"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18803055"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p46652504"><a name="p46652504"></a><a name="p46652504"></a>Router toggleAdminStateUp(String routerId, boolean adminStateUp)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p20756449"><a name="p20756449"></a><a name="p20756449"></a>PUT /v2.0/routers/{router_id}</p>
<p id="p190812186282"><a name="p190812186282"></a><a name="p190812186282"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row52590313"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p31956933"><a name="p31956933"></a><a name="p31956933"></a>Router update(Router router)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p38374806"><a name="p38374806"></a><a name="p38374806"></a>PUT /v2.0/routers/{router_id}</p>
<p id="p44812259283"><a name="p44812259283"></a><a name="p44812259283"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_router_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9828942"><td class="cellrowborder" rowspan="4" valign="top" width="29.222922292229224%" headers="mcps1.1.4.1.1 "><p id="p57946857"><a name="p57946857"></a><a name="p57946857"></a>SecurityGroupRuleService</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.1.4.1.2 "><p id="p63183853"><a name="p63183853"></a><a name="p63183853"></a>SecurityGroupRule create(SecurityGroupRule rule)</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.4.1.3 "><p id="p17618432"><a name="p17618432"></a><a name="p17618432"></a>POST /v2.0/security-group-rules</p>
<p id="p410610324285"><a name="p410610324285"></a><a name="p410610324285"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0008.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row24348168"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26044600"><a name="p26044600"></a><a name="p26044600"></a>void delete(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p29237836"><a name="p29237836"></a><a name="p29237836"></a>DELETE /v2.0/security-group-rules/{security-group-rules-id}</p>
<p id="p12668103817282"><a name="p12668103817282"></a><a name="p12668103817282"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0009.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row61813935"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p40872853"><a name="p40872853"></a><a name="p40872853"></a>SecurityGroupRule get(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p22366803"><a name="p22366803"></a><a name="p22366803"></a>GET /v2.0/security-group-rules/{security-group-rules-id}</p>
<p id="p21735312813"><a name="p21735312813"></a><a name="p21735312813"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0007.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row67083507"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p65055018"><a name="p65055018"></a><a name="p65055018"></a>List&lt;? extends SecurityGroupRule&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34965068"><a name="p34965068"></a><a name="p34965068"></a>GET /v2.0/security-group-rules</p>
<p id="p6292135932817"><a name="p6292135932817"></a><a name="p6292135932817"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0006.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46250162"><td class="cellrowborder" rowspan="4" valign="top" width="29.222922292229224%" headers="mcps1.1.4.1.1 "><p id="p55275618"><a name="p55275618"></a><a name="p55275618"></a>SecurityGroupService</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.1.4.1.2 "><p id="p48140083"><a name="p48140083"></a><a name="p48140083"></a>SecurityGroup create(SecurityGroup securityGroup)</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.4.1.3 "><p id="p7032652"><a name="p7032652"></a><a name="p7032652"></a>POST /v2.0/security-groups</p>
<p id="p1059146152913"><a name="p1059146152913"></a><a name="p1059146152913"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row63293876"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26530317"><a name="p26530317"></a><a name="p26530317"></a>ActionResponse delete(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1472067"><a name="p1472067"></a><a name="p1472067"></a>DELETE /v2.0/security-groups/{security-group-id}</p>
<p id="p738361492916"><a name="p738361492916"></a><a name="p738361492916"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row13248604"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66503975"><a name="p66503975"></a><a name="p66503975"></a>SecurityGroup get(String id)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18112899"><a name="p18112899"></a><a name="p18112899"></a>GET /v2.0/security-groups/{security-group-id}</p>
<p id="p49091921132914"><a name="p49091921132914"></a><a name="p49091921132914"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row28798367"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p50966358"><a name="p50966358"></a><a name="p50966358"></a>List&lt;? extends SecurityGroup&gt;list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p34634354"><a name="p34634354"></a><a name="p34634354"></a>GET /v2.0/security-groups</p>
<p id="p97616281299"><a name="p97616281299"></a><a name="p97616281299"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_sg02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row43273738"><td class="cellrowborder" rowspan="7" valign="top" width="29.222922292229224%" headers="mcps1.1.4.1.1 "><p id="p15511864"><a name="p15511864"></a><a name="p15511864"></a>SubnetService</p>
</td>
<td class="cellrowborder" valign="top" width="36.773677367736774%" headers="mcps1.1.4.1.2 "><p id="p48501438"><a name="p48501438"></a><a name="p48501438"></a>Subnet create(Subnet subnet)</p>
</td>
<td class="cellrowborder" valign="top" width="34.003400340034005%" headers="mcps1.1.4.1.3 "><p id="p36302405"><a name="p36302405"></a><a name="p36302405"></a>POST /v2.0/subnets</p>
<p id="p93551652202911"><a name="p93551652202911"></a><a name="p93551652202911"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0003.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row58286192"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p23561115"><a name="p23561115"></a><a name="p23561115"></a>ActionResponse delete(String subnetId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p29402138"><a name="p29402138"></a><a name="p29402138"></a>DELETE /v2.0/subnets/{subnet_id}</p>
<p id="p141781638153011"><a name="p141781638153011"></a><a name="p141781638153011"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0005.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row63292653"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p26431238"><a name="p26431238"></a><a name="p26431238"></a>Subnet get(String subnetId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p60555495"><a name="p60555495"></a><a name="p60555495"></a>GET /v2.0/subnets/{subnet_id}</p>
<p id="p6171115853013"><a name="p6171115853013"></a><a name="p6171115853013"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0002.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8128546"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p54432515"><a name="p54432515"></a><a name="p54432515"></a>List&lt;? extends Subnet&gt;list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p46957633"><a name="p46957633"></a><a name="p46957633"></a>GET /v2.0/subnets</p>
<p id="p2448683114"><a name="p2448683114"></a><a name="p2448683114"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1562619102055"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1462741014517"><a name="p1462741014517"></a><a name="p1462741014517"></a>List&lt;? extends Subnet&gt;list(Map&lt;String,String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p962791018520"><a name="p962791018520"></a><a name="p962791018520"></a>GET /v2.0/subnets</p>
<p id="p183271213113116"><a name="p183271213113116"></a><a name="p183271213113116"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0001.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19965518"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6594274"><a name="p6594274"></a><a name="p6594274"></a>Subnet update(String subnetId, Subnet subnet)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p64374149"><a name="p64374149"></a><a name="p64374149"></a>PUT /v2.0/subnets/{subnet_id}</p>
<p id="p0125122073118"><a name="p0125122073118"></a><a name="p0125122073118"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42496437"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19659381"><a name="p19659381"></a><a name="p19659381"></a>Subnet update(Subnet subnet)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p48906009"><a name="p48906009"></a><a name="p48906009"></a>PUT /v2.0/subnets/{subnet_id}</p>
<p id="p16265027183112"><a name="p16265027183112"></a><a name="p16265027183112"></a><a href="https://support.huaweicloud.com/api-vpc/vpc_subnet02_0004.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

