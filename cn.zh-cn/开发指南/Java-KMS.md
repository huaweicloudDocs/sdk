# KMS<a name="sdk_11_0015"></a>

基于KMS v1.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table138844"></a>
<table><thead align="left"><tr id="row35094160"><th class="cellrowborder" valign="top" width="28.48%" id="mcps1.1.4.1.1"><p id="p24054701"><a name="p24054701"></a><a name="p24054701"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.34%" id="mcps1.1.4.1.2"><p id="p2273746"><a name="p2273746"></a><a name="p2273746"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="35.18%" id="mcps1.1.4.1.3"><p id="p49955752"><a name="p49955752"></a><a name="p49955752"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row19884118"><td class="cellrowborder" rowspan="9" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p759913216714"><a name="p759913216714"></a><a name="p759913216714"></a>KeyService</p>
</td>
<td class="cellrowborder" valign="top" width="36.34%" headers="mcps1.1.4.1.2 "><p id="p173041815122115"><a name="p173041815122115"></a><a name="p173041815122115"></a>Key create(KeyCreate keyCreate)</p>
</td>
<td class="cellrowborder" valign="top" width="35.18%" headers="mcps1.1.4.1.3 "><p id="p5733201195735"><a name="p5733201195735"></a><a name="p5733201195735"></a>POST /v1.0/{project_id}/kms/create-key</p>
</td>
</tr>
<tr id="row53255854"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15672223182116"><a name="p15672223182116"></a><a name="p15672223182116"></a>Keys list(KeyListOptions options)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18754042195735"><a name="p18754042195735"></a><a name="p18754042195735"></a>POST /v1.0/{project_id}/kms/list-keys</p>
</td>
</tr>
<tr id="row14242537"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p149713518214"><a name="p149713518214"></a><a name="p149713518214"></a>Key get(String keyId, String sequence)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p48597341195735"><a name="p48597341195735"></a><a name="p48597341195735"></a>POST /v1.0/{project_id}/kms/describe-key</p>
</td>
</tr>
<tr id="row66441544"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p53846086195626"><a name="p53846086195626"></a><a name="p53846086195626"></a>Key disable(String keyId, String sequence)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p61090501195735"><a name="p61090501195735"></a><a name="p61090501195735"></a>POST /v1.0/{project_id}/kms/disable-key</p>
</td>
</tr>
<tr id="row62271039"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p62220609195626"><a name="p62220609195626"></a><a name="p62220609195626"></a>Key enable(String keyId, String sequence)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p41798854195735"><a name="p41798854195735"></a><a name="p41798854195735"></a>POST /v1.0/{project_id}/kms/enable-key</p>
</td>
</tr>
<tr id="row40084941"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p60340921195626"><a name="p60340921195626"></a><a name="p60340921195626"></a>Key scheduleDeletion(String keyId, Integer pendingDays, String sequence)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3940345195735"><a name="p3940345195735"></a><a name="p3940345195735"></a>POST /v1.0/{project_id}/kms/schedule-key-deletion</p>
</td>
</tr>
<tr id="row46070087"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p540839192216"><a name="p540839192216"></a><a name="p540839192216"></a>Key cancelDeletion(String keyId, String sequence)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p53939651195735"><a name="p53939651195735"></a><a name="p53939651195735"></a>POST /v1.0/{project_id}/kms/cancel-key-deletion</p>
</td>
</tr>
<tr id="row588929"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4753433195626"><a name="p4753433195626"></a><a name="p4753433195626"></a>Integer getKeyCreatedAmount()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p63320334195735"><a name="p63320334195735"></a><a name="p63320334195735"></a>GET /v1.0/{project_id}/kms/user-instances</p>
</td>
</tr>
<tr id="row13286310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1021522418228"><a name="p1021522418228"></a><a name="p1021522418228"></a>List&lt;Quota&gt; quotas()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p56733964195735"><a name="p56733964195735"></a><a name="p56733964195735"></a>GET /v1.0/{project_id}/kms/user-quotas</p>
</td>
</tr>
<tr id="row40742509"><td class="cellrowborder" rowspan="5" valign="top" width="28.48%" headers="mcps1.1.4.1.1 "><p id="p56662262195833"><a name="p56662262195833"></a><a name="p56662262195833"></a>CryptoService</p>
</td>
<td class="cellrowborder" valign="top" width="36.34%" headers="mcps1.1.4.1.2 "><p id="p0392173372212"><a name="p0392173372212"></a><a name="p0392173372212"></a>String generateRandomString(String sequence)</p>
</td>
<td class="cellrowborder" valign="top" width="35.18%" headers="mcps1.1.4.1.3 "><p id="p20000251195735"><a name="p20000251195735"></a><a name="p20000251195735"></a>POST /v1.0/{project_id}/kms/gen-random</p>
</td>
</tr>
<tr id="row18774354"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18997362195626"><a name="p18997362195626"></a><a name="p18997362195626"></a>DEK createDEK(String keyId, HashMap&lt;String, Object&gt; encryptionContext, String sequence)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17559515195735"><a name="p17559515195735"></a><a name="p17559515195735"></a>POST /v1.0/{project_id}/kms/create-datakey</p>
</td>
</tr>
<tr id="row35520730"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p938018491222"><a name="p938018491222"></a><a name="p938018491222"></a>DEK createDEKWithoutPlaintext(String keyId, HashMap&lt;String, Object&gt; encryptionContext, String sequence)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p50202424195735"><a name="p50202424195735"></a><a name="p50202424195735"></a>POST /v1.0/{project_id}/kms/create-datakey-without-plaintext</p>
</td>
</tr>
<tr id="row43163346"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p52517086195626"><a name="p52517086195626"></a><a name="p52517086195626"></a>EncryptedDEK encryptDEK(EncryptDEK encrypt)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p23236581195735"><a name="p23236581195735"></a><a name="p23236581195735"></a>POST /v1.0/{project_id}/kms/encrypt-datakey</p>
</td>
</tr>
<tr id="row24889743"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p32903283195626"><a name="p32903283195626"></a><a name="p32903283195626"></a>DecryptedDEK decryptDEK(DecryptDEK decrypt)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p28034494195735"><a name="p28034494195735"></a><a name="p28034494195735"></a>POST /v1.0/{project_id}/kms/decrypt-datakey</p>
</td>
</tr>
</tbody>
</table>

