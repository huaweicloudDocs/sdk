# MRS<a name="sdk_11_0018"></a>

基于MRS v1.1 API的SDK接口如下，调用方式请参考示例代码。

<a name="table5810621818403"></a>
<table><thead align="left"><tr id="row1740636518403"><th class="cellrowborder" valign="top" width="28.910000000000004%" id="mcps1.1.4.1.1"><p id="p62949318403"><a name="p62949318403"></a><a name="p62949318403"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="35.92%" id="mcps1.1.4.1.2"><p id="p5098895718403"><a name="p5098895718403"></a><a name="p5098895718403"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.17%" id="mcps1.1.4.1.3"><p id="p3646482918403"><a name="p3646482918403"></a><a name="p3646482918403"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row5974801018403"><td class="cellrowborder" rowspan="5" valign="top" width="28.910000000000004%" headers="mcps1.1.4.1.1 "><p id="p511893511210"><a name="p511893511210"></a><a name="p511893511210"></a>ClusterService</p>
</td>
<td class="cellrowborder" valign="top" width="35.92%" headers="mcps1.1.4.1.2 "><p id="p5641153154212"><a name="p5641153154212"></a><a name="p5641153154212"></a>MapReduceClusterCreateResult createAndRunJob(MapReduceClusterCreate cluster, MapReduceJobExeCreate jobExe)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p5055643218403"><a name="p5055643218403"></a><a name="p5055643218403"></a>POST /v1.1/{project_id}/run-job-flow</p>
</td>
</tr>
<tr id="row5235470818403"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p150284524219"><a name="p150284524219"></a><a name="p150284524219"></a>ActionResponse expand(String clusterId, int amount)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3607478618403"><a name="p3607478618403"></a><a name="p3607478618403"></a>PUT /v1.1/{project_id}/cluster_infos/{cluster_id}</p>
</td>
</tr>
<tr id="row5623762218403"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p5895357018403"><a name="p5895357018403"></a><a name="p5895357018403"></a>ActionResponse reduce(String clusterId, int amount, List&lt;String&gt; includes, List&lt;String&gt; excludes)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1050983318403"><a name="p1050983318403"></a><a name="p1050983318403"></a>PUT /v1.1/{project_id}/cluster_infos/{cluster_id}</p>
</td>
</tr>
<tr id="row2747963918403"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p88069594427"><a name="p88069594427"></a><a name="p88069594427"></a>MapReduceClusterInfo get(String clusterId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3950781118403"><a name="p3950781118403"></a><a name="p3950781118403"></a>GET /v1.1/{project_id}/cluster_infos/{cluster_id}</p>
</td>
</tr>
<tr id="row2002597918403"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p630913513432"><a name="p630913513432"></a><a name="p630913513432"></a>ActionResponse delete(String clusterId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5840609918403"><a name="p5840609918403"></a><a name="p5840609918403"></a>DELETE /v1.1/{project_id}/clusters/{cluster_id}</p>
</td>
</tr>
<tr id="row5603250818403"><td class="cellrowborder" rowspan="3" valign="top" width="28.910000000000004%" headers="mcps1.1.4.1.1 "><p id="p1926616710133"><a name="p1926616710133"></a><a name="p1926616710133"></a>JobExeServiceImpl</p>
</td>
<td class="cellrowborder" valign="top" width="35.92%" headers="mcps1.1.4.1.2 "><p id="p13248912174318"><a name="p13248912174318"></a><a name="p13248912174318"></a>MapReduceJobExe create(MapReduceJobExeCreate jobExeCreate)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p2470468618403"><a name="p2470468618403"></a><a name="p2470468618403"></a>POST /v1.1/{project_id}/jobs/submit-job</p>
</td>
</tr>
<tr id="row4533315118403"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1066871714436"><a name="p1066871714436"></a><a name="p1066871714436"></a>List&lt;? extends MapReduceJobExe&gt; list(JobExeListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p431991118403"><a name="p431991118403"></a><a name="p431991118403"></a>GET /v1.1/{project_id}/job-exes</p>
</td>
</tr>
<tr id="row3887919918403"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p6220739918403"><a name="p6220739918403"></a><a name="p6220739918403"></a>MapReduceJobExe get(String jobExeId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p563453518403"><a name="p563453518403"></a><a name="p563453518403"></a>GET /v1.1/{project_id}/job-exes/{job_exe_id}</p>
</td>
</tr>
<tr id="row4425667318403"><td class="cellrowborder" valign="top" width="28.910000000000004%" headers="mcps1.1.4.1.1 "><p id="p1393575618403"><a name="p1393575618403"></a><a name="p1393575618403"></a>JobExecutionService</p>
</td>
<td class="cellrowborder" valign="top" width="35.92%" headers="mcps1.1.4.1.2 "><p id="p1361212317438"><a name="p1361212317438"></a><a name="p1361212317438"></a>ActionResponse delete(String jobExecutionId)</p>
</td>
<td class="cellrowborder" valign="top" width="35.17%" headers="mcps1.1.4.1.3 "><p id="p5509092518403"><a name="p5509092518403"></a><a name="p5509092518403"></a>DELETE /v1.1/{project_id}/job-executions/{job_execution_id}</p>
</td>
</tr>
</tbody>
</table>

