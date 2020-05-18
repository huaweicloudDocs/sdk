# KMS<a name="sdk_12_0015"></a>

基于KMS v1.0 API的SDK接口如下，调用方式举例：conn.kms.create\_key\(\)

<a name="table39221624"></a>
<table><thead align="left"><tr id="row33048293"><th class="cellrowborder" valign="top" width="27.310000000000002%" id="mcps1.1.4.1.1"><p id="p59666077"><a name="p59666077"></a><a name="p59666077"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.559999999999995%" id="mcps1.1.4.1.2"><p id="p1114082"><a name="p1114082"></a><a name="p1114082"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.13%" id="mcps1.1.4.1.3"><p id="p23131803"><a name="p23131803"></a><a name="p23131803"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row61736753"><td class="cellrowborder" rowspan="7" valign="top" width="27.310000000000002%" headers="mcps1.1.4.1.1 "><p id="p39998624"><a name="p39998624"></a><a name="p39998624"></a>Key Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.559999999999995%" headers="mcps1.1.4.1.2 "><p id="p26855499195149"><a name="p26855499195149"></a><a name="p26855499195149"></a>create_key(**kwargs)</p>
</td>
<td class="cellrowborder" valign="top" width="36.13%" headers="mcps1.1.4.1.3 "><p id="p609468519537"><a name="p609468519537"></a><a name="p609468519537"></a>POST /v1.0/{project_id}/kms/create-key</p>
</td>
</tr>
<tr id="row2077973"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p48979633195149"><a name="p48979633195149"></a><a name="p48979633195149"></a>keys(**query)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1384058119537"><a name="p1384058119537"></a><a name="p1384058119537"></a>POST /v1.0/{project_id}/kms/list-keys</p>
</td>
</tr>
<tr id="row61803142"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4236947195149"><a name="p4236947195149"></a><a name="p4236947195149"></a>describe_key(key, **kwargs)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p2345440619537"><a name="p2345440619537"></a><a name="p2345440619537"></a>POST /v1.0/{project_id}/kms/describe-key</p>
</td>
</tr>
<tr id="row718904119517"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1726700195149"><a name="p1726700195149"></a><a name="p1726700195149"></a>disable_key(key, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5261055319537"><a name="p5261055319537"></a><a name="p5261055319537"></a>POST /v1.0/{project_id}/kms/disable-key</p>
</td>
</tr>
<tr id="row44335988195112"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p50804863195149"><a name="p50804863195149"></a><a name="p50804863195149"></a>enable_key(key, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3393222719537"><a name="p3393222719537"></a><a name="p3393222719537"></a>POST /v1.0/{project_id}/kms/enable-key</p>
</td>
</tr>
<tr id="row45293474195118"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p59761303195149"><a name="p59761303195149"></a><a name="p59761303195149"></a>schedule_deletion_key(key, pending_days, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4053172619537"><a name="p4053172619537"></a><a name="p4053172619537"></a>POST /v1.0/{project_id}/kms/schedule-key-deletion</p>
</td>
</tr>
<tr id="row25529125195115"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12337608195149"><a name="p12337608195149"></a><a name="p12337608195149"></a>cancel_deletion_key(key, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1972814019537"><a name="p1972814019537"></a><a name="p1972814019537"></a>POST /v1.0/{project_id}/kms/cancel-key-deletion</p>
</td>
</tr>
<tr id="row7933109195124"><td class="cellrowborder" valign="top" width="27.310000000000002%" headers="mcps1.1.4.1.1 "><p id="p27503491195124"><a name="p27503491195124"></a><a name="p27503491195124"></a>random Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.559999999999995%" headers="mcps1.1.4.1.2 "><p id="p1528491195149"><a name="p1528491195149"></a><a name="p1528491195149"></a>gen_random(**params)</p>
</td>
<td class="cellrowborder" valign="top" width="36.13%" headers="mcps1.1.4.1.3 "><p id="p2051788319537"><a name="p2051788319537"></a><a name="p2051788319537"></a>POST /v1.0/{project_id}/kms/gen-random</p>
</td>
</tr>
<tr id="row23251077195124"><td class="cellrowborder" rowspan="4" valign="top" width="27.310000000000002%" headers="mcps1.1.4.1.1 "><p id="p20915575195338"><a name="p20915575195338"></a><a name="p20915575195338"></a>DataKey Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.559999999999995%" headers="mcps1.1.4.1.2 "><p id="p40528549195149"><a name="p40528549195149"></a><a name="p40528549195149"></a>create_datakey(key, **params)</p>
</td>
<td class="cellrowborder" valign="top" width="36.13%" headers="mcps1.1.4.1.3 "><p id="p5936892319537"><a name="p5936892319537"></a><a name="p5936892319537"></a>POST /v1.0/{project_id}/kms/create-datakey</p>
</td>
</tr>
<tr id="row47322695195124"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p17412256195149"><a name="p17412256195149"></a><a name="p17412256195149"></a>create_datakey_wo_plain(key, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6183660019537"><a name="p6183660019537"></a><a name="p6183660019537"></a>POST /v1.0/{project_id}/kms/create-datakey-without-plaintext</p>
</td>
</tr>
<tr id="row12714617195124"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p9959374195149"><a name="p9959374195149"></a><a name="p9959374195149"></a>encrypt_datakey(datakey, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p4883402119537"><a name="p4883402119537"></a><a name="p4883402119537"></a>POST /v1.0/{project_id}/kms/encrypt-datakey</p>
</td>
</tr>
<tr id="row10562234195126"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p12627053195149"><a name="p12627053195149"></a><a name="p12627053195149"></a>decrypt_datakey(datakey, **params)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3230406219537"><a name="p3230406219537"></a><a name="p3230406219537"></a>POST /v1.0/{project_id}/kms/decrypt-datakey</p>
</td>
</tr>
<tr id="row38456283195126"><td class="cellrowborder" valign="top" width="27.310000000000002%" headers="mcps1.1.4.1.1 "><p id="p63855888195126"><a name="p63855888195126"></a><a name="p63855888195126"></a>InstanceNumber Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.559999999999995%" headers="mcps1.1.4.1.2 "><p id="p11207293195149"><a name="p11207293195149"></a><a name="p11207293195149"></a>get_instance_number()</p>
</td>
<td class="cellrowborder" valign="top" width="36.13%" headers="mcps1.1.4.1.3 "><p id="p6155914119537"><a name="p6155914119537"></a><a name="p6155914119537"></a>GET /v1.0/{project_id}/kms/user-instances</p>
</td>
</tr>
<tr id="row56468703195126"><td class="cellrowborder" valign="top" width="27.310000000000002%" headers="mcps1.1.4.1.1 "><p id="p24324583195424"><a name="p24324583195424"></a><a name="p24324583195424"></a>Quota Operations</p>
</td>
<td class="cellrowborder" valign="top" width="36.559999999999995%" headers="mcps1.1.4.1.2 "><p id="p46844638195149"><a name="p46844638195149"></a><a name="p46844638195149"></a>get_quota()</p>
</td>
<td class="cellrowborder" valign="top" width="36.13%" headers="mcps1.1.4.1.3 "><p id="p4789274019537"><a name="p4789274019537"></a><a name="p4789274019537"></a>GET /v1.0/{project_id}/kms/user-quotas</p>
</td>
</tr>
</tbody>
</table>

