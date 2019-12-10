# Python-RTS<a name="ZH-CN_TOPIC_0070868145"></a>

基于RTS v1 API的SDK接口如下，调用方式举例：conn.orchestration.create\_stack\(\)。

<a name="table157611310191613"></a>
<table><thead align="left"><tr id="row4835131011611"><th class="cellrowborder" valign="top" width="19.351935193519353%" id="mcps1.1.4.1.1"><p id="p108351310121619"><a name="p108351310121619"></a><a name="p108351310121619"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.2037203720372%" id="mcps1.1.4.1.2"><p id="p683541020166"><a name="p683541020166"></a><a name="p683541020166"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="43.444344434443444%" id="mcps1.1.4.1.3"><p id="p18835181031615"><a name="p18835181031615"></a><a name="p18835181031615"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row8835141031614"><td class="cellrowborder" rowspan="8" valign="top" width="19.351935193519353%" headers="mcps1.1.4.1.1 "><p id="p1835510201620"><a name="p1835510201620"></a><a name="p1835510201620"></a>Stack Operations</p>
</td>
<td class="cellrowborder" valign="top" width="37.2037203720372%" headers="mcps1.1.4.1.2 "><p id="p7835710111619"><a name="p7835710111619"></a><a name="p7835710111619"></a>create_stack(self, preview=False, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="43.444344434443444%" headers="mcps1.1.4.1.3 "><p id="p13835191061612"><a name="p13835191061612"></a><a name="p13835191061612"></a>POST /v1/{tenant_id}/stacks</p>
</td>
</tr>
<tr id="row168351110131617"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9835010141619"><a name="p9835010141619"></a><a name="p9835010141619"></a>find_stack(self, name_or_id, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p118361210151619"><a name="p118361210151619"></a><a name="p118361210151619"></a>GET /v1/{tenant_id}/stacks</p>
</td>
</tr>
<tr id="row6836181012162"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p158361110121613"><a name="p158361110121613"></a><a name="p158361110121613"></a>stacks(self, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p483616102166"><a name="p483616102166"></a><a name="p483616102166"></a>GET /v1/{tenant_id}/stacks</p>
</td>
</tr>
<tr id="row183671016162"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p38362010201614"><a name="p38362010201614"></a><a name="p38362010201614"></a>get_stack(self, stack)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17836151012167"><a name="p17836151012167"></a><a name="p17836151012167"></a>GET /v1/{tenant_id}/stacks/{stack_name}/{stack_id}</p>
</td>
</tr>
<tr id="row1283691010163"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1883611001617"><a name="p1883611001617"></a><a name="p1883611001617"></a>update_stack(self, stack, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18836111013165"><a name="p18836111013165"></a><a name="p18836111013165"></a>PUT /v1/{tenant_id}/stacks/{stack_name}/{stack_id}</p>
</td>
</tr>
<tr id="row1183681014162"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p88361210201615"><a name="p88361210201615"></a><a name="p88361210201615"></a>delete_stack(self, stack, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p138361210111611"><a name="p138361210111611"></a><a name="p138361210111611"></a>DELETE /v1/{tenant_id}/stacks/{stack_id}</p>
</td>
</tr>
<tr id="row18361410101619"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p583651081612"><a name="p583651081612"></a><a name="p583651081612"></a>check_stack(self, stack)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p15836171091617"><a name="p15836171091617"></a><a name="p15836171091617"></a>POST /v1/{tenant_id}/stacks/{stack_name}/{stack_id}/actions</p>
</td>
</tr>
<tr id="row13836181071615"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1283613104168"><a name="p1283613104168"></a><a name="p1283613104168"></a>resources(self, stack, **query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14836191015169"><a name="p14836191015169"></a><a name="p14836191015169"></a>GET /v1/{tenant_id}/stacks/{stack_name}/{stack_id}/resources</p>
</td>
</tr>
<tr id="row7836710151619"><td class="cellrowborder" rowspan="3" valign="top" width="19.351935193519353%" headers="mcps1.1.4.1.1 "><p id="p1483671071614"><a name="p1483671071614"></a><a name="p1483671071614"></a>Software_config Operations</p>
</td>
<td class="cellrowborder" valign="top" width="37.2037203720372%" headers="mcps1.1.4.1.2 "><p id="p1783613108167"><a name="p1783613108167"></a><a name="p1783613108167"></a>create_software_config(self, **attrs)</p>
</td>
<td class="cellrowborder" valign="top" width="43.444344434443444%" headers="mcps1.1.4.1.3 "><p id="p1883611021620"><a name="p1883611021620"></a><a name="p1883611021620"></a>POST /v1/{tenant_id}/software_configs</p>
</td>
</tr>
<tr id="row4836810181619"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p20836171019161"><a name="p20836171019161"></a><a name="p20836171019161"></a>get_software_config(self, software_config)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1083611018163"><a name="p1083611018163"></a><a name="p1083611018163"></a>GET /v1/{tenant_id}/software_configs/{config_id}</p>
</td>
</tr>
<tr id="row483611091618"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p118361109164"><a name="p118361109164"></a><a name="p118361109164"></a>delete_software_config(self, software_config, ignore_missing=True)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9836191091614"><a name="p9836191091614"></a><a name="p9836191091614"></a>DELETE /v1/{tenant_id}/software_configs/{config_id}</p>
</td>
</tr>
</tbody>
</table>

