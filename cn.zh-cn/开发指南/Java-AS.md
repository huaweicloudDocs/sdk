# AS<a name="sdk_11_0007"></a>

基于AS v1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table10151546101313"></a>
<table><thead align="left"><tr id="row6151346191310"><th class="cellrowborder" valign="top" width="28.48%" id="mcps1.1.4.1.1"><p id="p01511946141318"><a name="p01511946141318"></a><a name="p01511946141318"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.58%" id="mcps1.1.4.1.2"><p id="p915114612139"><a name="p915114612139"></a><a name="p915114612139"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="32.940000000000005%" id="mcps1.1.4.1.3"><p id="p5151194620133"><a name="p5151194620133"></a><a name="p5151194620133"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row11519462133"><td class="cellrowborder" rowspan="7" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p4151446131310"><a name="p4151446131310"></a><a name="p4151446131310"></a>AutoScalingGroupServic</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p14151174661319"><a name="p14151174661319"></a><a name="p14151174661319"></a>String create(ScalingGroupCreate group)</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p1063616444309"><a name="p1063616444309"></a><a name="p1063616444309"></a>POST /autoscaling-api/v1/{project_id}/scaling_group</p>
<p id="p61511646141320"><a name="p61511646141320"></a><a name="p61511646141320"></a><a href="https://support.huaweicloud.com/api-as/as_06_0201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1715194611138"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p61513464136"><a name="p61513464136"></a><a name="p61513464136"></a>List&lt;? extends ScalingGroup&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1151104691319"><a name="p1151104691319"></a><a name="p1151104691319"></a>GET /autoscaling-api/v1/{project_id}/scaling_group</p>
<p id="p1594462902217"><a name="p1594462902217"></a><a name="p1594462902217"></a><a href="https://support.huaweicloud.com/api-as/as_06_0102.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row41511146101312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p101511546171315"><a name="p101511546171315"></a><a name="p101511546171315"></a>ScalingGroup get(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p161518463133"><a name="p161518463133"></a><a name="p161518463133"></a>GET /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p1364610341226"><a name="p1364610341226"></a><a name="p1364610341226"></a><a href="https://support.huaweicloud.com/api-as/as_06_0103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row715113469138"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8151104615131"><a name="p8151104615131"></a><a name="p8151104615131"></a>String update(String groupId, ScalingGroupUpdate group)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2152446141311"><a name="p2152446141311"></a><a name="p2152446141311"></a>PUT /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}</p>
<p id="p7725237182213"><a name="p7725237182213"></a><a name="p7725237182213"></a><a href="https://support.huaweicloud.com/api-as/as_06_0104.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row8152746111310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p71526465133"><a name="p71526465133"></a><a name="p71526465133"></a>ActionResponse delete(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p8152546111310"><a name="p8152546111310"></a><a name="p8152546111310"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id</p>
<p id="p454314408226"><a name="p454314408226"></a><a name="p454314408226"></a><a href="https://support.huaweicloud.com/api-as/as_06_0105.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21521846131313"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p31521146121316"><a name="p31521146121316"></a><a name="p31521146121316"></a>ActionResponse resume(String groupId)</p>
<p id="p14152546131311"><a name="p14152546131311"></a><a name="p14152546131311"></a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15152114617133"><a name="p15152114617133"></a><a name="p15152114617133"></a>POST /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}/action</p>
<p id="p197301647102216"><a name="p197301647102216"></a><a name="p197301647102216"></a><a href="https://support.huaweicloud.com/api-as/as_06_0106.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row61522467132"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p8152114611319"><a name="p8152114611319"></a><a name="p8152114611319"></a>ActionResponse pause(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15152194691316"><a name="p15152194691316"></a><a name="p15152194691316"></a>POST /autoscaling-api/v1/{project_id}/scaling_group/{scaling_group_id}/action</p>
<p id="p691144919222"><a name="p691144919222"></a><a name="p691144919222"></a><a href="https://support.huaweicloud.com/api-as/as_06_0106.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18152946131320"><td class="cellrowborder" rowspan="5" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p115204610137"><a name="p115204610137"></a><a name="p115204610137"></a>AutoScalingConfigService</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p51529467132"><a name="p51529467132"></a><a name="p51529467132"></a>String create(ScalingConfigCreate config)</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p615224619137"><a name="p615224619137"></a><a name="p615224619137"></a>POST /autoscaling-api/v1/{project_id}/scaling_configuration</p>
<p id="p7761175213228"><a name="p7761175213228"></a><a name="p7761175213228"></a><a href="https://support.huaweicloud.com/api-as/as_06_0201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15152546171310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17152144612132"><a name="p17152144612132"></a><a name="p17152144612132"></a>List&lt;? extends ScalingConfig&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1096694912235"><a name="p1096694912235"></a><a name="p1096694912235"></a>GET /autoscaling-api/v1/{project_id}/scaling_configuration</p>
<p id="p1215274651311"><a name="p1215274651311"></a><a name="p1215274651311"></a><a href="https://support.huaweicloud.com/api-as/as_06_0202.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6152146121311"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p171521446181311"><a name="p171521446181311"></a><a name="p171521446181311"></a>ScalingConfig get(String configId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7152946181313"><a name="p7152946181313"></a><a name="p7152946181313"></a>GET /autoscaling-api/v1/{project_id}/scaling_configuration/{scaling_configuration_id}</p>
<p id="p1580805152314"><a name="p1580805152314"></a><a name="p1580805152314"></a><a href="https://support.huaweicloud.com/api-as/as_06_0203.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row181521546151315"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p91521146131310"><a name="p91521146131310"></a><a name="p91521146131310"></a>ActionResponse delete(String configId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15152144618131"><a name="p15152144618131"></a><a name="p15152144618131"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_configuration/{scaling_configuration_id}</p>
<p id="p814645432311"><a name="p814645432311"></a><a name="p814645432311"></a><a href="https://support.huaweicloud.com/api-as/as_06_0204.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row7152846141314"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p171529464134"><a name="p171529464134"></a><a name="p171529464134"></a>ActionResponse delete(List&lt;String&gt; configIds)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p101526461131"><a name="p101526461131"></a><a name="p101526461131"></a>POST /autoscaling-api/v1/{project_id}/scaling_configurations</p>
<p id="p560125722317"><a name="p560125722317"></a><a name="p560125722317"></a><a href="https://support.huaweicloud.com/api-as/as_06_0205.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row9152104691314"><td class="cellrowborder" rowspan="4" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p9152246171313"><a name="p9152246171313"></a><a name="p9152246171313"></a>AutoScalingGroupInstanceService</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p1615219465134"><a name="p1615219465134"></a><a name="p1615219465134"></a>List&lt;? extends ScalingGroupInstance&gt; list(String groupId, ScalingGroupInstanceListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p2153146131315"><a name="p2153146131315"></a><a name="p2153146131315"></a>GET /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/list</p>
<p id="p582819596232"><a name="p582819596232"></a><a name="p582819596232"></a><a href="https://support.huaweicloud.com/api-as/as_06_0301.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1415334618132"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0153446111312"><a name="p0153446111312"></a><a name="p0153446111312"></a>ActionResponse delete(String instanceId, boolean deleteInstance)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p228242012314"><a name="p228242012314"></a><a name="p228242012314"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_group_instance/{instance_id}</p>
<p id="p1162575313164"><a name="p1162575313164"></a><a name="p1162575313164"></a><a href="https://support.huaweicloud.com/api-as/as_06_0302.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row6153144621318"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p815334619137"><a name="p815334619137"></a><a name="p815334619137"></a>ActionResponse batchAdd(String groupId, List&lt;String&gt; instanceIds, boolean deleteInstance)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p515354610133"><a name="p515354610133"></a><a name="p515354610133"></a>POST /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/action</p>
<p id="p1742865102412"><a name="p1742865102412"></a><a name="p1742865102412"></a><a href="https://support.huaweicloud.com/api-as/as_06_0303.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row161531346141315"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p315311469135"><a name="p315311469135"></a><a name="p315311469135"></a>ActionResponse batchRemove(String groupId, List&lt;String&gt; instanceIds, boolean deleteInstance)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1415334618134"><a name="p1415334618134"></a><a name="p1415334618134"></a>POST /autoscaling-api/v1/{project_id}/scaling_group_instance/{scaling_group_id}/action</p>
<p id="p69931710102412"><a name="p69931710102412"></a><a name="p69931710102412"></a><a href="https://support.huaweicloud.com/api-as/as_06_0303.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row915354631311"><td class="cellrowborder" rowspan="8" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p151531846171313"><a name="p151531846171313"></a><a name="p151531846171313"></a>AutoScalingPolicyService</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p91531446121317"><a name="p91531446121317"></a><a name="p91531446121317"></a>String create(ScalingPolicyCreateUpdate policy)</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p9153046151315"><a name="p9153046151315"></a><a name="p9153046151315"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy</p>
<p id="p342111811244"><a name="p342111811244"></a><a name="p342111811244"></a><a href="https://support.huaweicloud.com/api-as/as_06_0401.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row2153846171311"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10153154619138"><a name="p10153154619138"></a><a name="p10153154619138"></a>String update(ScalingPolicyCreateUpdate policy)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15153184631317"><a name="p15153184631317"></a><a name="p15153184631317"></a>PUT /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p16810514112418"><a name="p16810514112418"></a><a name="p16810514112418"></a><a href="https://support.huaweicloud.com/api-as/as_06_0403.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21531446161314"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p31531646141314"><a name="p31531646141314"></a><a name="p31531646141314"></a>List&lt;? extends ScalingPolicy&gt; list(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p151530466131"><a name="p151530466131"></a><a name="p151530466131"></a>GET /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_group_id}/list</p>
<p id="p2991517142413"><a name="p2991517142413"></a><a name="p2991517142413"></a><a href="https://support.huaweicloud.com/api-as/as_06_0405.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11153546161315"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19154646201313"><a name="p19154646201313"></a><a name="p19154646201313"></a>ScalingPolicy get(String policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1415411464134"><a name="p1415411464134"></a><a name="p1415411464134"></a>GET /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p194401320132413"><a name="p194401320132413"></a><a name="p194401320132413"></a><a href="https://support.huaweicloud.com/api-as/as_06_0407.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1915444619132"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11543464133"><a name="p11543464133"></a><a name="p11543464133"></a>ActionResponse execute(String policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p19154946161313"><a name="p19154946161313"></a><a name="p19154946161313"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}/action</p>
<p id="p13690192312417"><a name="p13690192312417"></a><a name="p13690192312417"></a><a href="https://support.huaweicloud.com/api-as/as_06_0409.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row415444671310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15154154621318"><a name="p15154154621318"></a><a name="p15154154621318"></a>ActionResponse resume(String policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p201544464137"><a name="p201544464137"></a><a name="p201544464137"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}/action</p>
<p id="p16173626182415"><a name="p16173626182415"></a><a name="p16173626182415"></a><a href="https://support.huaweicloud.com/api-as/as_06_0409.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31541946181316"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2154174616137"><a name="p2154174616137"></a><a name="p2154174616137"></a>ActionResponse pause(String policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5154164619132"><a name="p5154164619132"></a><a name="p5154164619132"></a>POST /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}/action</p>
<p id="p1218619554326"><a name="p1218619554326"></a><a name="p1218619554326"></a><a href="https://support.huaweicloud.com/api-as/as_06_0409.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row215454651316"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17154446171316"><a name="p17154446171316"></a><a name="p17154446171316"></a>ActionResponse delete(String policyId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1715444671320"><a name="p1715444671320"></a><a name="p1715444671320"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_policy/{scaling_policy_id}</p>
<p id="p1525343412249"><a name="p1525343412249"></a><a name="p1525343412249"></a><a href="https://support.huaweicloud.com/api-as/as_06_0410.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row18154164617131"><td class="cellrowborder" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p13154114613135"><a name="p13154114613135"></a><a name="p13154114613135"></a>AutoScalingActivityLogService</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p1915434611315"><a name="p1915434611315"></a><a name="p1915434611315"></a>list(String groupId, ScalingActivityLogListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p101542464139"><a name="p101542464139"></a><a name="p101542464139"></a>GET /autoscaling-api/v1/{project_id}/scaling_activity_log/{scaling_group_id}</p>
<p id="p8414436142414"><a name="p8414436142414"></a><a name="p8414436142414"></a><a href="https://support.huaweicloud.com/api-as/as_06_0601.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row31541246101311"><td class="cellrowborder" rowspan="2" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p21541946101319"><a name="p21541946101319"></a><a name="p21541946101319"></a>AutoScalingQuotaService</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p1315434651315"><a name="p1315434651315"></a><a name="p1315434651315"></a>List&lt;Quota&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p13154946101311"><a name="p13154946101311"></a><a name="p13154946101311"></a>GET /autoscaling-api/v1/{project_id}/quotas</p>
<p id="p1785213972411"><a name="p1785213972411"></a><a name="p1785213972411"></a><a href="https://support.huaweicloud.com/api-as/as_06_0701.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row315411463138"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p19154346161315"><a name="p19154346161315"></a><a name="p19154346161315"></a>List&lt;Quota&gt; list(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7154174611137"><a name="p7154174611137"></a><a name="p7154174611137"></a>GET /autoscaling-api/v1/{project_id}/quotas/{scaling_group_id}</p>
<p id="p151111042202411"><a name="p151111042202411"></a><a name="p151111042202411"></a><a href="https://support.huaweicloud.com/api-as/as_06_0702.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5154646111318"><td class="cellrowborder" rowspan="7" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p161551546191315"><a name="p161551546191315"></a><a name="p161551546191315"></a>AutoScalingLifecycleHookService</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p8155174613136"><a name="p8155174613136"></a><a name="p8155174613136"></a>ASAutoScalingLifecycleHook create(ASAutoScalingLifecycleHook lifecycleHook, String groupId)</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p1515524612132"><a name="p1515524612132"></a><a name="p1515524612132"></a>POST /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}</p>
<p id="p2010819456246"><a name="p2010819456246"></a><a name="p2010819456246"></a><a href="https://support.huaweicloud.com/api-as/as_06_0201.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row715594618138"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4155546111310"><a name="p4155546111310"></a><a name="p4155546111310"></a>List&lt;? extends ASAutoScalingLifecycleHook&gt; list(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p91551846191310"><a name="p91551846191310"></a><a name="p91551846191310"></a>GET /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/list</p>
<p id="p16643486244"><a name="p16643486244"></a><a name="p16643486244"></a><a href="https://support.huaweicloud.com/api-as/as_06_0102.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row815510468138"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p121551046191317"><a name="p121551046191317"></a><a name="p121551046191317"></a>ASAutoScalingLifecycleHook list(String groupId, String lifecycleHookName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11155134616139"><a name="p11155134616139"></a><a name="p11155134616139"></a>GET /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p946615032410"><a name="p946615032410"></a><a name="p946615032410"></a><a href="https://support.huaweicloud.com/api-as/as_06_0103.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row5155346171319"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p141553464136"><a name="p141553464136"></a><a name="p141553464136"></a>ActionResponse delete(String groupId, String lifecycleHookName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13155246111314"><a name="p13155246111314"></a><a name="p13155246111314"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p77565562417"><a name="p77565562417"></a><a name="p77565562417"></a><a href="https://support.huaweicloud.com/api-as/as_06_0904.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row21555463135"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1015584621318"><a name="p1015584621318"></a><a name="p1015584621318"></a>ASAutoScalingLifecycleHook update(String groupId, String lifecycleHookName, ASAutoScalingLifecycleHook lifecycleHook)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2015512465134"><a name="p2015512465134"></a><a name="p2015512465134"></a>PUT /autoscaling-api/v1/{project_id}/scaling_lifecycle_hook/{scaling_group_id}/{lifecycle_hook_name}</p>
<p id="p159385572247"><a name="p159385572247"></a><a name="p159385572247"></a><a href="https://support.huaweicloud.com/api-as/as_06_0907.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row20155144612135"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1155134612131"><a name="p1155134612131"></a><a name="p1155134612131"></a>List&lt;? extends AutoScalingInstanceHangupInfo&gt; scalingInstanceHangup(String groupId, ScalingInstanceOptions instanceId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1315574611131"><a name="p1315574611131"></a><a name="p1315574611131"></a>GET /autoscaling-api/v1/{project_id}/scaling_instance_hook/{scaling_group_id}/list</p>
<p id="p206431819259"><a name="p206431819259"></a><a name="p206431819259"></a><a href="https://support.huaweicloud.com/api-as/as_06_0907.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row15155114661312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1415554612131"><a name="p1415554612131"></a><a name="p1415554612131"></a>ActionResponse scalingInstanceHookCallback(String groupId, ASAutoScalingLifecycleInstanceCallback lifecycleInstanceCallback)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12155746151315"><a name="p12155746151315"></a><a name="p12155746151315"></a>PUT /autoscaling-api/v1/{project_id}/scaling_instance_hook/{scaling_group_id}/callback</p>
<p id="p4434114202515"><a name="p4434114202515"></a><a name="p4434114202515"></a><a href="https://support.huaweicloud.com/api-as/as_06_0906.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row912618831810"><td class="cellrowborder" rowspan="3" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p2246162491816"><a name="p2246162491816"></a><a name="p2246162491816"></a>AutoScalingInformService</p>
</td>
<td class="cellrowborder" valign="top" width="38.58%" headers="mcps1.1.4.1.2 "><p id="p8126138191810"><a name="p8126138191810"></a><a name="p8126138191810"></a>ASAutoScalingInform deploy(String groupId, ASAutoScalingInform info)</p>
</td>
<td class="cellrowborder" valign="top" width="32.940000000000005%" headers="mcps1.1.4.1.3 "><p id="p19879113314191"><a name="p19879113314191"></a><a name="p19879113314191"></a>PUT /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}</p>
<p id="p1837718407191"><a name="p1837718407191"></a><a name="p1837718407191"></a><a href="https://support.huaweicloud.com/api-as/as_06_0801.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row4647612161819"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3647612111812"><a name="p3647612111812"></a><a name="p3647612111812"></a>ASAutoScalingTopics list(String groupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17687126171910"><a name="p17687126171910"></a><a name="p17687126171910"></a>GET /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}</p>
<p id="p088720416192"><a name="p088720416192"></a><a name="p088720416192"></a><a href="https://support.huaweicloud.com/api-as/as_06_0802.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row131661711180"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2161617131819"><a name="p2161617131819"></a><a name="p2161617131819"></a>ActionResponse delete(String groupId, String topicUrn)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p141701710180"><a name="p141701710180"></a><a name="p141701710180"></a>DELETE /autoscaling-api/v1/{project_id}/scaling_notification/{scaling_group_id}/{topic_urn}</p>
<p id="p1512744121920"><a name="p1512744121920"></a><a name="p1512744121920"></a><a href="https://support.huaweicloud.com/api-as/as_06_0803.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

