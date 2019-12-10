# Java-DMS<a name="ZH-CN_TOPIC_0079300123"></a>

基于DMS v1.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table4466452219112"></a>
<table><thead align="left"><tr id="row1883931919112"><th class="cellrowborder" valign="top" width="11%" id="mcps1.1.4.1.1"><p id="p33735697152039"><a name="p33735697152039"></a><a name="p33735697152039"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="39%" id="mcps1.1.4.1.2"><p id="p2273746"><a name="p2273746"></a><a name="p2273746"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.4.1.3"><p id="p49955752"><a name="p49955752"></a><a name="p49955752"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row415976919112"><td class="cellrowborder" rowspan="4" valign="top" width="11%" headers="mcps1.1.4.1.1 "><p id="p139698819112"><a name="p139698819112"></a><a name="p139698819112"></a>QueueService</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p8272509294"><a name="p8272509294"></a><a name="p8272509294"></a>Queue create(String name, String description)</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.4.1.3 "><p id="p3883369919112"><a name="p3883369919112"></a><a name="p3883369919112"></a>POST /v1.0/{project_id}/queues</p>
</td>
</tr>
<tr id="row1395897519112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p984913632910"><a name="p984913632910"></a><a name="p984913632910"></a>List&lt;? extends Queue&gt; list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4834510619112"><a name="p4834510619112"></a><a name="p4834510619112"></a>GET /v1.0/{project_id}/queues</p>
</td>
</tr>
<tr id="row3245277819112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p204221312132916"><a name="p204221312132916"></a><a name="p204221312132916"></a>Queue get(String queueId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5336099019112"><a name="p5336099019112"></a><a name="p5336099019112"></a>GET /v1.0/{project_id}/queues/{queue_id}</p>
</td>
</tr>
<tr id="row1048686619112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4412980819112"><a name="p4412980819112"></a><a name="p4412980819112"></a>ActionResponse delete(String queueId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1774469919112"><a name="p1774469919112"></a><a name="p1774469919112"></a>DELETE /v1.0/{project_id}/queues/{queue_id}</p>
</td>
</tr>
<tr id="row2548456419112"><td class="cellrowborder" rowspan="3" valign="top" width="11%" headers="mcps1.1.4.1.1 "><p id="p136812410110"><a name="p136812410110"></a><a name="p136812410110"></a>ConsumerGroupService</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p3604880619112"><a name="p3604880619112"></a><a name="p3604880619112"></a>ConsumerGroup create(String queueId, String consumerGroupName)</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.4.1.3 "><p id="p3427213519112"><a name="p3427213519112"></a><a name="p3427213519112"></a>POST /v1.0/{project_id}/queues/{queue_id}/groups</p>
</td>
</tr>
<tr id="row4001376219112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17742510113013"><a name="p17742510113013"></a><a name="p17742510113013"></a>List&lt;ConsumerGroup&gt; list(String queueId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p42185719112"><a name="p42185719112"></a><a name="p42185719112"></a>GET /v1.0/{project_id}/queues/{queue_id}/groups</p>
</td>
</tr>
<tr id="row379671819112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p41631417173018"><a name="p41631417173018"></a><a name="p41631417173018"></a>ActionResponse delete(String queueId, String consumerGroupId)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1288246919112"><a name="p1288246919112"></a><a name="p1288246919112"></a>DELETE /v1.0/{project_id}/queues/{queue_id}/groups/{consumer_group_id}</p>
</td>
</tr>
<tr id="row4883336519112"><td class="cellrowborder" rowspan="3" valign="top" width="11%" headers="mcps1.1.4.1.1 "><p id="p6318850119112"><a name="p6318850119112"></a><a name="p6318850119112"></a>QueueMessageService</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p12281113115302"><a name="p12281113115302"></a><a name="p12281113115302"></a>ActionResponse produce(String queueId, QueueMessage message)</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.4.1.3 "><p id="p4830378619112"><a name="p4830378619112"></a><a name="p4830378619112"></a>POST /v1.0/{project_id}/queues/{queue_id}/messages</p>
</td>
</tr>
<tr id="row3208089019112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p024455353110"><a name="p024455353110"></a><a name="p024455353110"></a>List&lt;QueueMessageWithHandler&gt; consume(String queueId, String consumerGroupId, Integer maxMessages, Integer timeWait)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2932559119112"><a name="p2932559119112"></a><a name="p2932559119112"></a>GET /v1.0/{project_id}/queues/{queue_id}/groups/{consumer_group_id}/messages</p>
</td>
</tr>
<tr id="row6260373519112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3773773719112"><a name="p3773773719112"></a><a name="p3773773719112"></a>ConsumeConfirmResponse confirmConsuming(String queueId, String consumerGroupId,Map&lt;String, ConsumeStatus&gt; consumeResult)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3685787219112"><a name="p3685787219112"></a><a name="p3685787219112"></a>POST /v1.0/{project_id}/queues/{queue_id}/groups/{consumer_group_id}/ack</p>
</td>
</tr>
<tr id="row6328539919112"><td class="cellrowborder" valign="top" width="11%" headers="mcps1.1.4.1.1 "><p id="p2584370419112"><a name="p2584370419112"></a><a name="p2584370419112"></a>MessageQueueQuotaService</p>
</td>
<td class="cellrowborder" valign="top" width="39%" headers="mcps1.1.4.1.2 "><p id="p593514219416"><a name="p593514219416"></a><a name="p593514219416"></a>List&lt;Quota&gt; get()</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.4.1.3 "><p id="p4355487519112"><a name="p4355487519112"></a><a name="p4355487519112"></a>GET /v1.0/{project_id}/quotas/dms</p>
</td>
</tr>
</tbody>
</table>

