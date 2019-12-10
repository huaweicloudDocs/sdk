# Java-CTS<a name="ZH-CN_TOPIC_0079300118"></a>

基于CTS v1.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table66289298171154"></a>
<table><thead align="left"><tr id="row18804775171458"><th class="cellrowborder" valign="top" width="21.959999999999997%" id="mcps1.1.4.1.1"><p id="p5720345017156"><a name="p5720345017156"></a><a name="p5720345017156"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="44.91%" id="mcps1.1.4.1.2"><p id="p296787817156"><a name="p296787817156"></a><a name="p296787817156"></a>method</p>
</th>
<th class="cellrowborder" valign="top" width="33.129999999999995%" id="mcps1.1.4.1.3"><p id="p3907156217156"><a name="p3907156217156"></a><a name="p3907156217156"></a>API URL</p>
</th>
</tr>
</thead>
<tbody><tr id="row8386953171154"><td class="cellrowborder" rowspan="4" valign="top" width="21.959999999999997%" headers="mcps1.1.4.1.1 "><p id="p156041350115817"><a name="p156041350115817"></a><a name="p156041350115817"></a>TrackerService</p>
</td>
<td class="cellrowborder" valign="top" width="44.91%" headers="mcps1.1.4.1.2 "><p id="p12966142317617"><a name="p12966142317617"></a><a name="p12966142317617"></a>Tracker create(String bucketName, String filePrefixName)</p>
</td>
<td class="cellrowborder" valign="top" width="33.129999999999995%" headers="mcps1.1.4.1.3 "><p id="p47975060171117"><a name="p47975060171117"></a><a name="p47975060171117"></a>POST /v1.0/{project_id}/tracker</p>
</td>
</tr>
<tr id="row21080418171154"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4514173219612"><a name="p4514173219612"></a><a name="p4514173219612"></a>Tracker get(String trackerName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12880774171117"><a name="p12880774171117"></a><a name="p12880774171117"></a>GET /v1.0/{project_id}/tracker{?tracker_name}</p>
</td>
</tr>
<tr id="row11888958171154"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p61952322171117"><a name="p61952322171117"></a><a name="p61952322171117"></a>Tracker update(TrackerUpdate update)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p52082168171117"><a name="p52082168171117"></a><a name="p52082168171117"></a>PUT /v1.0/{project_id}/tracker/{?tracker_name}</p>
</td>
</tr>
<tr id="row27092199171154"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p02383468610"><a name="p02383468610"></a><a name="p02383468610"></a>ActionResponse delete(String trackerName)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2083177171117"><a name="p2083177171117"></a><a name="p2083177171117"></a>DELETE /v1.0/{project_id}/tracker{?tracker_name}</p>
</td>
</tr>
<tr id="row18259241171154"><td class="cellrowborder" valign="top" width="21.959999999999997%" headers="mcps1.1.4.1.1 "><p id="p750516795919"><a name="p750516795919"></a><a name="p750516795919"></a>TraceService</p>
</td>
<td class="cellrowborder" valign="top" width="44.91%" headers="mcps1.1.4.1.2 "><p id="p2596477417113"><a name="p2596477417113"></a><a name="p2596477417113"></a>List&lt;Trace&gt; list(String trackerName, TraceListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" width="33.129999999999995%" headers="mcps1.1.4.1.3 "><p id="p2277192917113"><a name="p2277192917113"></a><a name="p2277192917113"></a>GET /v2.0/{project_id}/{tracker_name}/trace{?trace_id,service_type,resource_type,resource_id,resource_name,trace_name,trace_rating,user,limit,from,to,next}</p>
</td>
</tr>
</tbody>
</table>

