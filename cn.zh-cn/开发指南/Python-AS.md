# Python-AS<a name="ZH-CN_TOPIC_0072142410"></a>

基于AS v1 API的SDK接口如下，调用方式举例：conn.auto\_scaling.create\_group\(\)

<a name="table22377509173456"></a>
<table><thead align="left"><tr id="row31280221173456"><th class="cellrowborder" valign="top" width="17.849999999999998%" id="mcps1.1.4.1.1"><p id="p50669961173456"><a name="p50669961173456"></a><a name="p50669961173456"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39.93%" id="mcps1.1.4.1.2"><p id="p10626137173456"><a name="p10626137173456"></a><a name="p10626137173456"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="42.22%" id="mcps1.1.4.1.3"><p id="p55410741173456"><a name="p55410741173456"></a><a name="p55410741173456"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row59085062173456"><td class="cellrowborder" rowspan="7" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p56380605175740"><a name="p56380605175740"></a><a name="p56380605175740"></a>Group Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p7686851895"><a name="p7686851895"></a><a name="p7686851895"></a>create_group(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p622635071895"><a name="p622635071895"></a><a name="p622635071895"></a>POST /autoscaling-api/v1/{project_id}/scaling_group</p>
<p id="p153885443406"><a name="p153885443406"></a><a name="p153885443406"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063023.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row39651246175759"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p245052231895"><a name="p245052231895"></a><a name="p245052231895"></a>groups(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p387660761895"><a name="p387660761895"></a><a name="p387660761895"></a>GET /autoscaling-api/v1/{project_id}/scaling_group</p>
<p id="p191376174317"><a name="p191376174317"></a><a name="p191376174317"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063030.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3700652418010"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p76382191895"><a name="p76382191895"></a><a name="p76382191895"></a>get_group(self, group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p147160081895"><a name="p147160081895"></a><a name="p147160081895"></a>GET /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p416819910433"><a name="p416819910433"></a><a name="p416819910433"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063073.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5729000518014"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p576609811895"><a name="p576609811895"></a><a name="p576609811895"></a>update_group(self, group, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p400278761895"><a name="p400278761895"></a><a name="p400278761895"></a>PUT /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p1120101214310"><a name="p1120101214310"></a><a name="p1120101214310"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063036.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3088701173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p550752101895"><a name="p550752101895"></a><a name="p550752101895"></a>delete_group(self, group, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p319070141895"><a name="p319070141895"></a><a name="p319070141895"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p2751201454319"><a name="p2751201454319"></a><a name="p2751201454319"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063041.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row51841891173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p405462631895"><a name="p405462631895"></a><a name="p405462631895"></a>resume_group(self, group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p630218651895"><a name="p630218651895"></a><a name="p630218651895"></a>POST /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}/action</p>
<p id="p162109185431"><a name="p162109185431"></a><a name="p162109185431"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063017.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row33834419173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4088229618918"><a name="p4088229618918"></a><a name="p4088229618918"></a>pause_group(self, group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2313165218918"><a name="p2313165218918"></a><a name="p2313165218918"></a>POST /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}/action</p>
<p id="p6629125884610"><a name="p6629125884610"></a><a name="p6629125884610"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063017.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row35075245173456"><td class="cellrowborder" rowspan="5" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p1083981918115"><a name="p1083981918115"></a><a name="p1083981918115"></a>Config Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p1865003718918"><a name="p1865003718918"></a><a name="p1865003718918"></a>create_config(self, name, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p3425804818918"><a name="p3425804818918"></a><a name="p3425804818918"></a>POST /autoscaling-api/v1/{project_id}/scaling_configuration</p>
<p id="p16607132318435"><a name="p16607132318435"></a><a name="p16607132318435"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063055.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row42544890173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p962005218918"><a name="p962005218918"></a><a name="p962005218918"></a>configs(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4102674318918"><a name="p4102674318918"></a><a name="p4102674318918"></a>GET /autoscaling-api/v1/{project_id}/scaling_configuration</p>
<p id="p5967112716438"><a name="p5967112716438"></a><a name="p5967112716438"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063056.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row48955445173456"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4505160118918"><a name="p4505160118918"></a><a name="p4505160118918"></a>get_config(self, config)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2530104618918"><a name="p2530104618918"></a><a name="p2530104618918"></a>GET /autoscaling-api/v1/{project_id}/scaling_configuration/{scaling_configuration_id}</p>
<p id="p1510633110434"><a name="p1510633110434"></a><a name="p1510633110434"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063052.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1022652718232"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5663428918918"><a name="p5663428918918"></a><a name="p5663428918918"></a>delete_config(self, config, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2397467418918"><a name="p2397467418918"></a><a name="p2397467418918"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_configuration/{scaling_configuration_id}</p>
<p id="p54732335431"><a name="p54732335431"></a><a name="p54732335431"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063060.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6515000718253"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2923334518918"><a name="p2923334518918"></a><a name="p2923334518918"></a>batch_delete_configs(self, configs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1909072918918"><a name="p1909072918918"></a><a name="p1909072918918"></a>POST /autoscaling-api/v1/{project_id}/scaling_configurations</p>
<p id="p988143664312"><a name="p988143664312"></a><a name="p988143664312"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063049.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row144860671831"><td class="cellrowborder" rowspan="4" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p4664355718332"><a name="p4664355718332"></a><a name="p4664355718332"></a>Instance Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p2560674218918"><a name="p2560674218918"></a><a name="p2560674218918"></a>instances(self, group, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p6088022218918"><a name="p6088022218918"></a><a name="p6088022218918"></a>GET /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/list</p>
<p id="p89931385430"><a name="p89931385430"></a><a name="p89931385430"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063045.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row638903301846"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2272321318918"><a name="p2272321318918"></a><a name="p2272321318918"></a>remove_instance(self, instance, delete_instance=False, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2864099218918"><a name="p2864099218918"></a><a name="p2864099218918"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_group_instance/{instance_id}</p>
<p id="p04644114318"><a name="p04644114318"></a><a name="p04644114318"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063059.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3166059718354"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p842663618918"><a name="p842663618918"></a><a name="p842663618918"></a>batch_add_instances(self, group, instances)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1146889818918"><a name="p1146889818918"></a><a name="p1146889818918"></a>POST /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/action</p>
<p id="p5315143124319"><a name="p5315143124319"></a><a name="p5315143124319"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063053.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row241237431849"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3932819018918"><a name="p3932819018918"></a><a name="p3932819018918"></a>batch_remove_instances(self, group, instances, delete_instance=False)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3146685118918"><a name="p3146685118918"></a><a name="p3146685118918"></a>POST /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/action</p>
<p id="p16423846204318"><a name="p16423846204318"></a><a name="p16423846204318"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063053.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row296146318412"><td class="cellrowborder" rowspan="8" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p2907311018454"><a name="p2907311018454"></a><a name="p2907311018454"></a>Policy Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p1974373118931"><a name="p1974373118931"></a><a name="p1974373118931"></a>create_policy(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p5573834818931"><a name="p5573834818931"></a><a name="p5573834818931"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy</p>
<p id="p3480104810439"><a name="p3480104810439"></a><a name="p3480104810439"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063062.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row732382918414"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3239298418931"><a name="p3239298418931"></a><a name="p3239298418931"></a>update_policy(self, policy, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p658607318931"><a name="p658607318931"></a><a name="p658607318931"></a>PUT /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p96271850164314"><a name="p96271850164314"></a><a name="p96271850164314"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063080.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row394420831843"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3651858018931"><a name="p3651858018931"></a><a name="p3651858018931"></a>policies(self, group, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p521501618931"><a name="p521501618931"></a><a name="p521501618931"></a>GET /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_group_id}/list</p>
<p id="p12688125219436"><a name="p12688125219436"></a><a name="p12688125219436"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0134002033.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row188667151840"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4365031518931"><a name="p4365031518931"></a><a name="p4365031518931"></a>get_policy(self, policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4601463518931"><a name="p4601463518931"></a><a name="p4601463518931"></a>GET /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p17603857174316"><a name="p17603857174316"></a><a name="p17603857174316"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063043.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row82645618357"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5734596218931"><a name="p5734596218931"></a><a name="p5734596218931"></a>execute_policy(self, policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1451136018931"><a name="p1451136018931"></a><a name="p1451136018931"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}/action</p>
<p id="p15679059194313"><a name="p15679059194313"></a><a name="p15679059194313"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063075.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2241504318351"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4269021418931"><a name="p4269021418931"></a><a name="p4269021418931"></a>resume_policy(self, policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3535534118931"><a name="p3535534118931"></a><a name="p3535534118931"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}/action</p>
<p id="p18635124414"><a name="p18635124414"></a><a name="p18635124414"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063075.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4097530818257"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p423983718931"><a name="p423983718931"></a><a name="p423983718931"></a>pause_policy(self, policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p788249318931"><a name="p788249318931"></a><a name="p788249318931"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}/action</p>
<p id="p175367474415"><a name="p175367474415"></a><a name="p175367474415"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063075.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6377785318518"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4208440218931"><a name="p4208440218931"></a><a name="p4208440218931"></a>delete_policy(self, policy, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5339341518931"><a name="p5339341518931"></a><a name="p5339341518931"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p7727124214333"><a name="p7727124214333"></a><a name="p7727124214333"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063065.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5837080718515"><td class="cellrowborder" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p686197818545"><a name="p686197818545"></a><a name="p686197818545"></a>Activity Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p65864418931"><a name="p65864418931"></a><a name="p65864418931"></a>activities(self, group, **query)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p5335018318931"><a name="p5335018318931"></a><a name="p5335018318931"></a>GET /autoscaling-api/v1/{project_id}/scaling_activity_log/{scaling_group_id}</p>
<p id="p421113911447"><a name="p421113911447"></a><a name="p421113911447"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063071.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5914831518513"><td class="cellrowborder" rowspan="2" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p943666018558"><a name="p943666018558"></a><a name="p943666018558"></a>Quota Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p3625125418931"><a name="p3625125418931"></a><a name="p3625125418931"></a>quotas(self, group=None)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p5067049818931"><a name="p5067049818931"></a><a name="p5067049818931"></a>GET /autoscaling-api/v1/{project_id}/quotas</p>
<p id="p1120161294419"><a name="p1120161294419"></a><a name="p1120161294419"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063063.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5435092518344"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2891791118931"><a name="p2891791118931"></a><a name="p2891791118931"></a>quotas(self, group=None)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6064947718931"><a name="p6064947718931"></a><a name="p6064947718931"></a>GET /autoscaling-api/v1/{project_id}/quotas/{scaling_group_id}</p>
<p id="p16112615164412"><a name="p16112615164412"></a><a name="p16112615164412"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063020.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5938115194343"><td class="cellrowborder" rowspan="7" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p15346396194528"><a name="p15346396194528"></a><a name="p15346396194528"></a>Lifecycle_hook Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p18293056194438"><a name="p18293056194438"></a><a name="p18293056194438"></a>create_lifecycle_hook(self, group, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p3687875319456"><a name="p3687875319456"></a><a name="p3687875319456"></a>POST /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}</p>
<p id="p15981161714414"><a name="p15981161714414"></a><a name="p15981161714414"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063074.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row60045887194350"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p66243524194438"><a name="p66243524194438"></a><a name="p66243524194438"></a>lifecycle_hooks(self, group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4591939819456"><a name="p4591939819456"></a><a name="p4591939819456"></a>GET /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/list</p>
<p id="p823516233448"><a name="p823516233448"></a><a name="p823516233448"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063069.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row543643119440"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p40803932194438"><a name="p40803932194438"></a><a name="p40803932194438"></a>get_lifecycle_hook(self, group, lifecycle_hook)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6555185519456"><a name="p6555185519456"></a><a name="p6555185519456"></a>GET /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p184202634417"><a name="p184202634417"></a><a name="p184202634417"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063031.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row3214790119446"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42260154194438"><a name="p42260154194438"></a><a name="p42260154194438"></a>update_lifecycle_hook(self, group, lifecycle_hook, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1456465219456"><a name="p1456465219456"></a><a name="p1456465219456"></a>PUT /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p14339828114415"><a name="p14339828114415"></a><a name="p14339828114415"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063040.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row46319886194410"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p29561995194438"><a name="p29561995194438"></a><a name="p29561995194438"></a>delete_lifecycle_hook(self, group, lifecycle_hook)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2789275019456"><a name="p2789275019456"></a><a name="p2789275019456"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p16831163113448"><a name="p16831163113448"></a><a name="p16831163113448"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063026.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8755774194413"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p36116865194438"><a name="p36116865194438"></a><a name="p36116865194438"></a>call_back_instance(self, group, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4378989319456"><a name="p4378989319456"></a><a name="p4378989319456"></a>PUT /autoscaling-api/v1/{project_id}/scaling_instance_hook/{scaling_group_id}/callback</p>
<p id="p5193153413442"><a name="p5193153413442"></a><a name="p5193153413442"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063028.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row33667636194418"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p46369100194438"><a name="p46369100194438"></a><a name="p46369100194438"></a>get_group_hanging_instance(self, group,  **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4164236819456"><a name="p4164236819456"></a><a name="p4164236819456"></a>GET /autoscaling-api/v1/{project_id}/scaling_instance_hook/{scaling_group_id}/list{?instance_id}</p>
<p id="p425213754419"><a name="p425213754419"></a><a name="p425213754419"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063081.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row575217348373"><td class="cellrowborder" rowspan="3" valign="top" width="17.849999999999998%" headers="mcps1.1.4.1.1 "><p id="p7353114619374"><a name="p7353114619374"></a><a name="p7353114619374"></a>Notification Operations</p>
</td>
<td class="cellrowborder" valign="top" width="39.93%" headers="mcps1.1.4.1.2 "><p id="p1688192317384"><a name="p1688192317384"></a><a name="p1688192317384"></a>create_notification(self, group, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="42.22%" headers="mcps1.1.4.1.3 "><p id="p19879113314191"><a name="p19879113314191"></a><a name="p19879113314191"></a>PUT /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}</p>
<p id="p1837718407191"><a name="p1837718407191"></a><a name="p1837718407191"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063033.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row332943873712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p988152323819"><a name="p988152323819"></a><a name="p988152323819"></a>notifications(self, group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17687126171910"><a name="p17687126171910"></a><a name="p17687126171910"></a>GET /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}</p>
<p id="p088720416192"><a name="p088720416192"></a><a name="p088720416192"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063054.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6845941113712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p78811023203817"><a name="p78811023203817"></a><a name="p78811023203817"></a>delete_notification(self, group, topic)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p141701710180"><a name="p141701710180"></a><a name="p141701710180"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}/{topic_urn}</p>
<p id="p1512744121920"><a name="p1512744121920"></a><a name="p1512744121920"></a><a href="https://support.huaweicloud.com/api-as/zh-cn_topic_0043063035.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

