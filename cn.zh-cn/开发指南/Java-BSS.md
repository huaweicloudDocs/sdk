# BSS<a name="sdk_11_0025"></a>

基于BSS v1.0 API的SDK接口如下，调用方式请参考示例代码。

>![](public_sys-resources/icon-note.gif) **说明：** 
>如下接口的API链接有面向合作伙伴和面向客户之分，若链接为“合作伙伴运营能力”表明该链接是面向合作伙伴的API接口链接，若链接为“客户运营能力”表明该链接是面向客户的API接口链接。

<a name="table187413011207"></a>
<table><thead align="left"><tr id="row941153119203"><th class="cellrowborder" valign="top" width="26.45735426457354%" id="mcps1.1.4.1.1"><p id="p1741103120200"><a name="p1741103120200"></a><a name="p1741103120200"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.67613238676132%" id="mcps1.1.4.1.2"><p id="p1741163172011"><a name="p1741163172011"></a><a name="p1741163172011"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.86651334866514%" id="mcps1.1.4.1.3"><p id="p1841103114208"><a name="p1841103114208"></a><a name="p1841103114208"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row1382061123212"><td class="cellrowborder" rowspan="3" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p12424311209"><a name="p12424311209"></a><a name="p12424311209"></a>Customer Management</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p24216312207"><a name="p24216312207"></a><a name="p24216312207"></a>CheckUserRsp checkUser(String domainID, CheckUserReq req)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p194263120206"><a name="p194263120206"></a><a name="p194263120206"></a>POST /v1.0/{partner_id}/partner/customer-mgr/check-user</p>
<p id="p04283102015"><a name="p04283102015"></a><a name="p04283102015"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0083753561.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row17831313103213"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p134213132012"><a name="p134213132012"></a><a name="p134213132012"></a>CreateCustomerRsp createCustomer(String domainID, CreateCustomerReq req)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p194283172012"><a name="p194283172012"></a><a name="p194283172012"></a>POST /v1.0/{partner_id}/partner/customer-mgr/customer</p>
<p id="p1421231142011"><a name="p1421231142011"></a><a name="p1421231142011"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0080030911.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row186031113103212"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3421231192019"><a name="p3421231192019"></a><a name="p3421231192019"></a>QueryCustomerInfoListRsp queryCustomerInfoList(String domainID, QueryCustomerInfoListReq req)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p5421231122011"><a name="p5421231122011"></a><a name="p5421231122011"></a>POST /v1.0/{partner_id}/partner/customer-mgr/query</p>
<p id="p1042133132010"><a name="p1042133132010"></a><a name="p1042133132010"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0077254158.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1257983923214"><td class="cellrowborder" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p444103162010"><a name="p444103162010"></a><a name="p444103162010"></a>Realname Auth</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p74423112010"><a name="p74423112010"></a><a name="p74423112010"></a>QueryRealnameAuthReviewResultRsp queryRealnameAuthReviewResult(String domainID, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p9441831142011"><a name="p9441831142011"></a><a name="p9441831142011"></a>GET /v1.0/{partner_id}/partner/customer-mgr/realname-auth/result</p>
<p id="p24453162013"><a name="p24453162013"></a><a name="p24453162013"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00007.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row14902758333"><td class="cellrowborder" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p9421831162018"><a name="p9421831162018"></a><a name="p9421831162018"></a>Enquiry</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p104233162016"><a name="p104233162016"></a><a name="p104233162016"></a>QueryRatingRsp queryRating(String domainID, QueryRatingReq req)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p17422316201"><a name="p17422316201"></a><a name="p17422316201"></a>POST /v1.0/{domain_id}/customer/product-mgr/query-rating</p>
<p id="p342143110201"><a name="p342143110201"></a><a name="p342143110201"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0078731101.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p5366192563416"><a name="p5366192563416"></a><a name="p5366192563416"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0078731101.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row280617265339"><td class="cellrowborder" rowspan="6" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p542153132013"><a name="p542153132013"></a><a name="p542153132013"></a>Period Order</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p442123114207"><a name="p442123114207"></a><a name="p442123114207"></a>QueryOrdersListRsp queryOrdersList(String domainID, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p16421631102019"><a name="p16421631102019"></a><a name="p16421631102019"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/detail</p>
<p id="p64233162011"><a name="p64233162011"></a><a name="p64233162011"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0083740673.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p18737145817346"><a name="p18737145817346"></a><a name="p18737145817346"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0083740673.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row3408271332"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p149984512012"><a name="p149984512012"></a><a name="p149984512012"></a>QueryOrderDetailRsp queryOrderDetail(String domainID, String orderId, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1243173122010"><a name="p1243173122010"></a><a name="p1243173122010"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/{order_id}</p>
<p id="p1431831172020"><a name="p1431831172020"></a><a name="p1431831172020"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746564.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p97781637183910"><a name="p97781637183910"></a><a name="p97781637183910"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746564.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row14451727143310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174313310205"><a name="p174313310205"></a><a name="p174313310205"></a>OrderPayRsp orderPay(String domainID, OrderPayReq req)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p12431931132020"><a name="p12431931132020"></a><a name="p12431931132020"></a>POST /v1.0/{domain_id}/customer/order-mgr/order/pay</p>
<p id="p94313111202"><a name="p94313111202"></a><a name="p94313111202"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p6349143474013"><a name="p6349143474013"></a><a name="p6349143474013"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row13256128143310"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3852314111915"><a name="p3852314111915"></a><a name="p3852314111915"></a>OrderActionsRsp orderActions(String domainID, Map&lt;String, String&gt; filteringParams, OrderActionsReq req)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1431931132013"><a name="p1431931132013"></a><a name="p1431931132013"></a>PUT /v1.0/{domain_id}/customer/order-mgr/orders/actions</p>
<p id="p16431331162017"><a name="p16431331162017"></a><a name="p16431331162017"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0079992470.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row18552028163312"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p144383112013"><a name="p144383112013"></a><a name="p144383112013"></a>QueryRefundOrderRsp queryRefundOrder(String domainID, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p043931142011"><a name="p043931142011"></a><a name="p043931142011"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/refund-order</p>
<p id="p174317310203"><a name="p174317310203"></a><a name="p174317310203"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0112435250.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1786952810336"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10438318202"><a name="p10438318202"></a><a name="p10438318202"></a>QueryResourcesRsp queryResources(String domainID, String orderId,  Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1143183119208"><a name="p1143183119208"></a><a name="p1143183119208"></a>GET /v1.0/{domain_id}/common/order-mgr/orders-resource/{order_id}</p>
<p id="p134383117207"><a name="p134383117207"></a><a name="p134383117207"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00001.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1385624332216"><a name="p1385624332216"></a><a name="p1385624332216"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00001.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row73373163410"><td class="cellrowborder" rowspan="5" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p1843123119203"><a name="p1843123119203"></a><a name="p1843123119203"></a>Period Resource</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p1343103142011"><a name="p1343103142011"></a><a name="p1343103142011"></a>queryResourcesList(String domainID, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p164319313207"><a name="p164319313207"></a><a name="p164319313207"></a>GET /v1.0/{domain_id}/common/order-mgr/resources/detail</p>
<p id="p2035383115013"><a name="p2035383115013"></a><a name="p2035383115013"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0084961226.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1835333119011"><a name="p1835333119011"></a><a name="p1835333119011"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0084961226.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row736517318341"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p543103110209"><a name="p543103110209"></a><a name="p543103110209"></a>OrderRenewByResourceIdRsp orderRenewByResourceId(OrderRenewByResourceIdReq req, String domainID)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p194463172019"><a name="p194463172019"></a><a name="p194463172019"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/renew</p>
<p id="p1644133113206"><a name="p1644133113206"></a><a name="p1644133113206"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0082522029.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p16592113872616"><a name="p16592113872616"></a><a name="p16592113872616"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522029.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row127501733341"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3441931172017"><a name="p3441931172017"></a><a name="p3441931172017"></a>OrderDeleteByResourceIdRsp orderDeleteByResourceId(String domainID, OrderDeleteByResourceIdReq req)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p744133114208"><a name="p744133114208"></a><a name="p744133114208"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/delete</p>
<p id="p124416311201"><a name="p124416311201"></a><a name="p124416311201"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p139307154283"><a name="p139307154283"></a><a name="p139307154283"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row6621249341"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p174411319203"><a name="p174411319203"></a><a name="p174411319203"></a>AutoRenewRsp autoRenew(String domainID, String resourceId, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p174410317209"><a name="p174410317209"></a><a name="p174410317209"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/{resource_id}/actions</p>
<p id="p6441131122011"><a name="p6441131122011"></a><a name="p6441131122011"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00002.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1443019122920"><a name="p1443019122920"></a><a name="p1443019122920"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00002.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row1420034193415"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1744331202015"><a name="p1744331202015"></a><a name="p1744331202015"></a>CancelAutoRenewRsp cancelAutoRenew(String domainID, String resourceId, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p18447313205"><a name="p18447313205"></a><a name="p18447313205"></a>DELETE /v1.0/{domain_id}/common/order-mgr/resources/{resource_id}/actions</p>
<p id="p1144103117209"><a name="p1144103117209"></a><a name="p1144103117209"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00003.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p9774839114018"><a name="p9774839114018"></a><a name="p9774839114018"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00003.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row17248133910346"><td class="cellrowborder" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p942113192018"><a name="p942113192018"></a><a name="p942113192018"></a>Pay-Per-Use Resource</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p12429314204"><a name="p12429314204"></a><a name="p12429314204"></a>QueryCustomerResourceRsp queryCustomerResource(String domainID, QueryCustomerResourceReq req)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p19421531122018"><a name="p19421531122018"></a><a name="p19421531122018"></a>POST /v1.0/{partner_id}/partner/customer-mgr/customer-resource/query-resources</p>
<p id="p194213112015"><a name="p194213112015"></a><a name="p194213112015"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0079744790.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1441113110206"><td class="cellrowborder" rowspan="3" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p124119315209"><a name="p124119315209"></a><a name="p124119315209"></a>Bill</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p1841231152013"><a name="p1841231152013"></a><a name="p1841231152013"></a>QueryMonthlySumRsp queryMonthlySum(String domainID, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p642193111200"><a name="p642193111200"></a><a name="p642193111200"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/monthly-sum</p>
<p id="p242183162011"><a name="p242183162011"></a><a name="p242183162011"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0109708205.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row94203122018"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1942331172018"><a name="p1942331172018"></a><a name="p1942331172018"></a>QueryResRecordRsp queryResRecord(String domainID, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1242203110202"><a name="p1242203110202"></a><a name="p1242203110202"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/res-records</p>
<p id="p842231152016"><a name="p842231152016"></a><a name="p842231152016"></a><a href="https://support.huaweicloud.com/api-oce/mbc_00005.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row3421531182011"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10427310207"><a name="p10427310207"></a><a name="p10427310207"></a>QueryResFeeRecordRsp queryResFeeRecord(String domainID, Map&lt;String, String&gt; filteringParams)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p14211312206"><a name="p14211312206"></a><a name="p14211312206"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/res-fee-records</p>
<p id="p1542173102014"><a name="p1542173102014"></a><a name="p1542173102014"></a><a href="https://support.huaweicloud.com/api-oce/mbc_00002.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row344331182019"><td class="cellrowborder" valign="top" width="26.45735426457354%" headers="mcps1.1.4.1.1 "><p id="p194418311200"><a name="p194418311200"></a><a name="p194418311200"></a>Utilities</p>
</td>
<td class="cellrowborder" valign="top" width="38.67613238676132%" headers="mcps1.1.4.1.2 "><p id="p194433115203"><a name="p194433115203"></a><a name="p194433115203"></a>SendVerificationCodeRsp sendVerificationCode(String domainID, SendVerificationCodeReq req)</p>
</td>
<td class="cellrowborder" valign="top" width="34.86651334866514%" headers="mcps1.1.4.1.3 "><p id="p344143114202"><a name="p344143114202"></a><a name="p344143114202"></a>POST /v1.0/{partner_id}/partner/common-mgr/verificationcode</p>
<p id="p94443119203"><a name="p94443119203"></a><a name="p94443119203"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0118172609.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
</tbody>
</table>

