# Python-MRS<a name="ZH-CN_TOPIC_0079300131"></a>

基于MRS v1.1 API的SDK接口如下，调用方式举例：conn.map\_reduce.create\_cluster\_and\_run\_job\(\)

<a name="table40885158174529"></a>
<table><thead align="left"><tr id="row11079666174529"><th class="cellrowborder" valign="top" width="19.21%" id="mcps1.1.4.1.1"><p id="p12534220184352"><a name="p12534220184352"></a><a name="p12534220184352"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="34.900000000000006%" id="mcps1.1.4.1.2"><p id="p8638927184352"><a name="p8638927184352"></a><a name="p8638927184352"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="45.89%" id="mcps1.1.4.1.3"><p id="p28664466184352"><a name="p28664466184352"></a><a name="p28664466184352"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row46399827174529"><td class="cellrowborder" rowspan="5" valign="top" width="19.21%" headers="mcps1.1.4.1.1 "><p id="p289667174529"><a name="p289667174529"></a><a name="p289667174529"></a>Cluster Operations</p>
</td>
<td class="cellrowborder" valign="top" width="34.900000000000006%" headers="mcps1.1.4.1.2 "><p id="p23463084174529"><a name="p23463084174529"></a><a name="p23463084174529"></a>create_cluster_and_run_job(**cluster,**job)</p>
</td>
<td class="cellrowborder" valign="top" width="45.89%" headers="mcps1.1.4.1.3 "><p id="p21461621174529"><a name="p21461621174529"></a><a name="p21461621174529"></a>POST /v1.1/{project_id}/run-job-flow</p>
</td>
</tr>
<tr id="row58936861174529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9156409174529"><a name="p9156409174529"></a><a name="p9156409174529"></a>expand_cluster("cluster-id", expand_node_amount)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3471690174529"><a name="p3471690174529"></a><a name="p3471690174529"></a>PUT /v1.1/{project_id}/cluster_infos/{cluster_id}</p>
</td>
</tr>
<tr id="row31245218174529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p47834749174529"><a name="p47834749174529"></a><a name="p47834749174529"></a>reduce_cluster("cluster-id", reduce_node_amount, includes=includes, excludes=excludes)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p49409473174529"><a name="p49409473174529"></a><a name="p49409473174529"></a>PUT /v1.1/{project_id}/cluster_infos/{cluster_id}</p>
</td>
</tr>
<tr id="row42032073174529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p49154748174529"><a name="p49154748174529"></a><a name="p49154748174529"></a>get_cluster("cluster-id")</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p22111660174529"><a name="p22111660174529"></a><a name="p22111660174529"></a>GET /v1.1/{project_id}/cluster_infos/{cluster_id}</p>
</td>
</tr>
<tr id="row64787214174529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13272963174529"><a name="p13272963174529"></a><a name="p13272963174529"></a>delete_cluster("cluster-id")</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1368233174529"><a name="p1368233174529"></a><a name="p1368233174529"></a>DELETE /v1.1/{project_id}/clusters/{cluster_id}</p>
</td>
</tr>
<tr id="row47529574174529"><td class="cellrowborder" rowspan="3" valign="top" width="19.21%" headers="mcps1.1.4.1.1 "><p id="p24690281174529"><a name="p24690281174529"></a><a name="p24690281174529"></a>Job Operations</p>
</td>
<td class="cellrowborder" valign="top" width="34.900000000000006%" headers="mcps1.1.4.1.2 "><p id="p53755753174529"><a name="p53755753174529"></a><a name="p53755753174529"></a>exe_job(**exe)</p>
</td>
<td class="cellrowborder" valign="top" width="45.89%" headers="mcps1.1.4.1.3 "><p id="p59248717174529"><a name="p59248717174529"></a><a name="p59248717174529"></a>POST /v1.1/{project_id}/jobs/submit-job</p>
</td>
</tr>
<tr id="row63490885174529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p42488083174529"><a name="p42488083174529"></a><a name="p42488083174529"></a>job_exes(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18982673174529"><a name="p18982673174529"></a><a name="p18982673174529"></a>GET /v1.1/{project_id}/job-exes</p>
</td>
</tr>
<tr id="row36626329174529"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p13942691174529"><a name="p13942691174529"></a><a name="p13942691174529"></a>get_job_exe("job-exe-id")</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p55616177174529"><a name="p55616177174529"></a><a name="p55616177174529"></a>GET /v1.1/{project_id}/job-exes/{job_exe_id}</p>
</td>
</tr>
<tr id="row22409987174529"><td class="cellrowborder" valign="top" width="19.21%" headers="mcps1.1.4.1.1 "><p id="p10439565174529"><a name="p10439565174529"></a><a name="p10439565174529"></a>JobExecution Operations</p>
</td>
<td class="cellrowborder" valign="top" width="34.900000000000006%" headers="mcps1.1.4.1.2 "><p id="p3269654174529"><a name="p3269654174529"></a><a name="p3269654174529"></a>delete_job_execution("job-execution-id")</p>
</td>
<td class="cellrowborder" valign="top" width="45.89%" headers="mcps1.1.4.1.3 "><p id="p63515430174529"><a name="p63515430174529"></a><a name="p63515430174529"></a>DELETE /v1.1/{project_id}/job-executions/{job_execution_id}</p>
</td>
</tr>
</tbody>
</table>

