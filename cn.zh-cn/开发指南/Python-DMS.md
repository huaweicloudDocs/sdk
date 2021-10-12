# DMS<a name="sdk_12_0017"></a>

基于DMS v1.0 API的SDK接口如下，调用方式举例：conn.dms.create\_queue\(\)

<a name="table5801246519410"></a>
<table><tbody><tr id="row5513745919410"><td class="cellrowborder" valign="top" width="27.310000000000002%"><p id="p3694923219410"><a name="p3694923219410"></a><a name="p3694923219410"></a>Interface</p>
</td>
<td class="cellrowborder" valign="top" width="35.809999999999995%"><p id="p4009780519410"><a name="p4009780519410"></a><a name="p4009780519410"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="36.88%"><p id="p2669675419410"><a name="p2669675419410"></a><a name="p2669675419410"></a>API</p>
</td>
</tr>
<tr id="row3894420019410"><td class="cellrowborder" rowspan="4" valign="top" width="27.310000000000002%"><p id="p36359719410"><a name="p36359719410"></a><a name="p36359719410"></a>Queue Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.809999999999995%"><p id="p2945137419410"><a name="p2945137419410"></a><a name="p2945137419410"></a>create_queue(**kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.88%"><p id="p3675112519410"><a name="p3675112519410"></a><a name="p3675112519410"></a>POST /v1.0/{project_id}/queues</p>
</td>
</tr>
<tr id="row6232466919410"><td class="cellrowborder" valign="top"><p id="p1513341319410"><a name="p1513341319410"></a><a name="p1513341319410"></a>queues()</p>
</td>
<td class="cellrowborder" valign="top"><p id="p1784691719410"><a name="p1784691719410"></a><a name="p1784691719410"></a>GET /v1.0/{project_id}/queues</p>
</td>
</tr>
<tr id="row2640453019410"><td class="cellrowborder" valign="top"><p id="p5839218619410"><a name="p5839218619410"></a><a name="p5839218619410"></a>get_queue(queue)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p3214663919410"><a name="p3214663919410"></a><a name="p3214663919410"></a>GET /v1.0/{project_id}/queues/{queue_id}</p>
</td>
</tr>
<tr id="row2088429719410"><td class="cellrowborder" valign="top"><p id="p1390652419410"><a name="p1390652419410"></a><a name="p1390652419410"></a>delete_queue(queue, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p5268663919410"><a name="p5268663919410"></a><a name="p5268663919410"></a>DELETE /v1.0/{project_id}/queues/{queue_id}</p>
</td>
</tr>
<tr id="row441770419410"><td class="cellrowborder" rowspan="3" valign="top" width="27.310000000000002%"><p id="p2228972619410"><a name="p2228972619410"></a><a name="p2228972619410"></a>Group Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.809999999999995%"><p id="p886585019410"><a name="p886585019410"></a><a name="p886585019410"></a>create_groups(queue, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.88%"><p id="p4704527919410"><a name="p4704527919410"></a><a name="p4704527919410"></a>POST /v1.0/{project_id}/queues/{queue_id}/groups</p>
</td>
</tr>
<tr id="row2075433319410"><td class="cellrowborder" valign="top"><p id="p337944619410"><a name="p337944619410"></a><a name="p337944619410"></a>groups(queue)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p529971519410"><a name="p529971519410"></a><a name="p529971519410"></a>GET /v1.0/{project_id}/queues/{queue_id}/groups</p>
</td>
</tr>
<tr id="row4769744119410"><td class="cellrowborder" valign="top"><p id="p3828751219410"><a name="p3828751219410"></a><a name="p3828751219410"></a>delete_group(queue, group)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p1428075919410"><a name="p1428075919410"></a><a name="p1428075919410"></a>DELETE /v1.0/{project_id}/queues/{queue_id}/groups/{consumer_group_id}</p>
</td>
</tr>
<tr id="row6141797419410"><td class="cellrowborder" rowspan="3" valign="top" width="27.310000000000002%"><p id="p879997319410"><a name="p879997319410"></a><a name="p879997319410"></a>Message Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.809999999999995%"><p id="p3983848919410"><a name="p3983848919410"></a><a name="p3983848919410"></a>send_messages(queue, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.88%"><p id="p569213819410"><a name="p569213819410"></a><a name="p569213819410"></a>POST /v1.0/{project_id}/queues/{queue_id}/messages</p>
</td>
</tr>
<tr id="row5122924519410"><td class="cellrowborder" valign="top"><p id="p5592820619410"><a name="p5592820619410"></a><a name="p5592820619410"></a>consume_message(queue, consume_group, **query)</p>
</td>
<td class="cellrowborder" valign="top"><p id="p3389087619410"><a name="p3389087619410"></a><a name="p3389087619410"></a>GET /v1.0/{project_id}/queues/{queue_id}/groups/{consumer_group_id}/messages</p>
</td>
</tr>
<tr id="row3658243319410"><td class="cellrowborder" valign="top"><p id="p1038710919410"><a name="p1038710919410"></a><a name="p1038710919410"></a>ack_consumed_message(consumed_message, status='success')</p>
</td>
<td class="cellrowborder" valign="top"><p id="p3604946419410"><a name="p3604946419410"></a><a name="p3604946419410"></a>POST /v1.0/{project_id}/queues/{queue_id}/groups/{consumer_group_id}/ack</p>
</td>
</tr>
<tr id="row13447964172729"><td class="cellrowborder" valign="top" width="27.310000000000002%"><p id="p53922812172729"><a name="p53922812172729"></a><a name="p53922812172729"></a>Quota Operations</p>
</td>
<td class="cellrowborder" valign="top" width="35.809999999999995%"><p id="p5671647172729"><a name="p5671647172729"></a><a name="p5671647172729"></a>quotas()</p>
</td>
<td class="cellrowborder" valign="top" width="36.88%"><p id="p56750271172729"><a name="p56750271172729"></a><a name="p56750271172729"></a>GET /v1.0/{project_id}/quotas/dms</p>
</td>
</tr>
</tbody>
</table>

