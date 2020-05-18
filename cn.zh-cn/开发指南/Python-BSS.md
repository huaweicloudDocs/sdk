# BSS<a name="sdk_12_0025"></a>

基于BSS v1.0 API的SDK接口如下，调用方式请参考示例代码。

>![](public_sys-resources/icon-note.gif) **说明：**   
>如下接口的API链接有面向合作伙伴和面向客户之分，若链接为“合作伙伴运营能力”表明该链接是面向合作伙伴的API接口链接，若链接为“客户运营能力”表明该链接是面向客户的API接口链接。  

<a name="table115681513182717"></a>
<table><thead align="left"><tr id="row2834191311272"><th class="cellrowborder" valign="top" width="26.987301269873008%" id="mcps1.1.4.1.1"><p id="p128341813112716"><a name="p128341813112716"></a><a name="p128341813112716"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="36.44635536446355%" id="mcps1.1.4.1.2"><p id="p7834101372716"><a name="p7834101372716"></a><a name="p7834101372716"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.566343365663435%" id="mcps1.1.4.1.3"><p id="p4834201317271"><a name="p4834201317271"></a><a name="p4834201317271"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row14834113192716"><td class="cellrowborder" rowspan="3" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p7834113172719"><a name="p7834113172719"></a><a name="p7834113172719"></a>Customer Management</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p3834113122714"><a name="p3834113122714"></a><a name="p3834113122714"></a>check_customer_register_info(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p15834131317271"><a name="p15834131317271"></a><a name="p15834131317271"></a>POST /v1.0/{partner_id}/partner/customer-mgr/check-user</p>
<p id="p188347133274"><a name="p188347133274"></a><a name="p188347133274"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0083753561.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row8834161315276"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p2834161352718"><a name="p2834161352718"></a><a name="p2834161352718"></a>create_customer(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p283421317279"><a name="p283421317279"></a><a name="p283421317279"></a>POST /v1.0/{partner_id}/partner/customer-mgr/customer</p>
<p id="p10834191322718"><a name="p10834191322718"></a><a name="p10834191322718"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0080030911.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row138341613192715"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p68341113192714"><a name="p68341113192714"></a><a name="p68341113192714"></a>query_customer_list(userDomainId, **data)</p>
<p id="p1834313182715"><a name="p1834313182715"></a><a name="p1834313182715"></a></p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p183411138273"><a name="p183411138273"></a><a name="p183411138273"></a>POST /v1.0/{partner_id}/partner/customer-mgr/query</p>
<p id="p1783441302717"><a name="p1783441302717"></a><a name="p1783441302717"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0077254158.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1283441319275"><td class="cellrowborder" rowspan="4" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p183431312274"><a name="p183431312274"></a><a name="p183431312274"></a>Realname Auth</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p19834181312271"><a name="p19834181312271"></a><a name="p19834181312271"></a>individual_realname_auth(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p1683420138278"><a name="p1683420138278"></a><a name="p1683420138278"></a>POST /v1.0/{partner_id}/partner/customer-mgr/realname-auth/individual</p>
<p id="p138341136271"><a name="p138341136271"></a><a name="p138341136271"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00004.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row483415133276"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7834181312276"><a name="p7834181312276"></a><a name="p7834181312276"></a>enterprise_realname_auth(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7834713112717"><a name="p7834713112717"></a><a name="p7834713112717"></a>POST /v1.0/{partner_id}/partner/customer-mgr/realname-auth/enterprise</p>
<p id="p883414139277"><a name="p883414139277"></a><a name="p883414139277"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00005.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row9834513112710"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p3835713172712"><a name="p3835713172712"></a><a name="p3835713172712"></a>change_enterprise_realname_auth(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p28351913112718"><a name="p28351913112718"></a><a name="p28351913112718"></a>PUT /v1.0/{partner_id}/partner/customer-mgr/realname-auth/enterprise</p>
<p id="p1283521315277"><a name="p1283521315277"></a><a name="p1283521315277"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00006.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row4835181318278"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p15835413182713"><a name="p15835413182713"></a><a name="p15835413182713"></a>query_realname_auth(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p0835161302715"><a name="p0835161302715"></a><a name="p0835161302715"></a>GET /v1.0/{partner_id}/partner/customer-mgr/realname-auth/result</p>
<p id="p12835513202719"><a name="p12835513202719"></a><a name="p12835513202719"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00007.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row198359134276"><td class="cellrowborder" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p128350135275"><a name="p128350135275"></a><a name="p128350135275"></a>Enquiry</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p188351513202711"><a name="p188351513202711"></a><a name="p188351513202711"></a>query_rating(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p19835913192716"><a name="p19835913192716"></a><a name="p19835913192716"></a>POST /v1.0/{domain_id}/customer/product-mgr/query-rating</p>
<p id="p17835913102710"><a name="p17835913102710"></a><a name="p17835913102710"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0078731101.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p4835013162719"><a name="p4835013162719"></a><a name="p4835013162719"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0078731101.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row10835513122714"><td class="cellrowborder" rowspan="7" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p68358130270"><a name="p68358130270"></a><a name="p68358130270"></a>Period Order</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p38352130278"><a name="p38352130278"></a><a name="p38352130278"></a>query_order_list(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p1183531314276"><a name="p1183531314276"></a><a name="p1183531314276"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/detail</p>
<p id="p58351313122712"><a name="p58351313122712"></a><a name="p58351313122712"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0083740673.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p28351513142712"><a name="p28351513142712"></a><a name="p28351513142712"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0083740673.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row9835101352720"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p158351413162712"><a name="p158351413162712"></a><a name="p158351413162712"></a>query_order_detail(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p208351713132715"><a name="p208351713132715"></a><a name="p208351713132715"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/{order_id}</p>
<p id="p1983521392717"><a name="p1983521392717"></a><a name="p1983521392717"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746564.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1983515136279"><a name="p1983515136279"></a><a name="p1983515136279"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746564.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row1783517139271"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p188351413112719"><a name="p188351413112719"></a><a name="p188351413112719"></a>pay_period_order(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p783551392715"><a name="p783551392715"></a><a name="p783551392715"></a>POST /v1.0/{domain_id}/customer/order-mgr/order/pay</p>
<p id="p18835191318275"><a name="p18835191318275"></a><a name="p18835191318275"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1883521362710"><a name="p1883521362710"></a><a name="p1883521362710"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row68351013122712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p118351613102710"><a name="p118351613102710"></a><a name="p118351613102710"></a>unsubscribe_period_order(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p208363139278"><a name="p208363139278"></a><a name="p208363139278"></a>DELETE /v1.0/{domain_id}/customer/order-mgr/orders/{order_id}</p>
<p id="p11836513102710"><a name="p11836513102710"></a><a name="p11836513102710"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0076597539.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p883671322717"><a name="p883671322717"></a><a name="p883671322717"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0076597539.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row108361113162714"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p683621315278"><a name="p683621315278"></a><a name="p683621315278"></a>cancel_order(userDomainId, orderId="xxxxxxxxxx", action_id="cancel")</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3836171311275"><a name="p3836171311275"></a><a name="p3836171311275"></a>PUT /v1.0/{domain_id}/customer/order-mgr/orders/actions</p>
<p id="p118361213142710"><a name="p118361213142710"></a><a name="p118361213142710"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0079992470.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1783631312717"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1183621311273"><a name="p1183621311273"></a><a name="p1183621311273"></a>query_refund_order_amount(domain_id=userDomainId, order_id='xxxxxxxxxx')</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6836141313272"><a name="p6836141313272"></a><a name="p6836141313272"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/refund-order</p>
<p id="p68366131274"><a name="p68366131274"></a><a name="p68366131274"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0112435250.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row383615134271"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p7836141322717"><a name="p7836141322717"></a><a name="p7836141322717"></a>query_resource_status_by_orderId(userDomainId, order_id="xxxxxxxxxx")</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p178365132277"><a name="p178365132277"></a><a name="p178365132277"></a>GET /v1.0/{domain_id}/common/order-mgr/orders-resource/{order_id}</p>
<p id="p1783620131277"><a name="p1783620131277"></a><a name="p1783620131277"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00001.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1836111313272"><a name="p1836111313272"></a><a name="p1836111313272"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00001.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row9836171372720"><td class="cellrowborder" rowspan="5" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p158366139272"><a name="p158366139272"></a><a name="p158366139272"></a>Period Resourse</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p1083620131270"><a name="p1083620131270"></a><a name="p1083620131270"></a>query_customer_period_resources_list(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p08362131277"><a name="p08362131277"></a><a name="p08362131277"></a>GET /v1.0/{domain_id}/common/order-mgr/resources/detail</p>
<p id="p4836613122712"><a name="p4836613122712"></a><a name="p4836613122712"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0084961226.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p78365131278"><a name="p78365131278"></a><a name="p78365131278"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0084961226.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row98361213102712"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p383691332713"><a name="p383691332713"></a><a name="p383691332713"></a>renew_subscription_by_resourceId(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p483661319279"><a name="p483661319279"></a><a name="p483661319279"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/renew</p>
<p id="p1183618136271"><a name="p1183618136271"></a><a name="p1183618136271"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0082522029.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p2836101312279"><a name="p2836101312279"></a><a name="p2836101312279"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522029.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row08361213162714"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18836181372714"><a name="p18836181372714"></a><a name="p18836181372714"></a>unsubscribe_by_resourceId(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1583617139272"><a name="p1583617139272"></a><a name="p1583617139272"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/delete</p>
<p id="p1283691312714"><a name="p1283691312714"></a><a name="p1283691312714"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1483621392717"><a name="p1483621392717"></a><a name="p1483621392717"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row13837181332711"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p148375133277"><a name="p148375133277"></a><a name="p148375133277"></a>enable_auto_renew(userDomainId, resource_id="xxxxxxxxxxxxxx", action_id="autorenew")</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9837191310275"><a name="p9837191310275"></a><a name="p9837191310275"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/{resource_id}/actions</p>
<p id="p98371138274"><a name="p98371138274"></a><a name="p98371138274"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00002.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p683715138271"><a name="p683715138271"></a><a name="p683715138271"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00002.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row1183781312276"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0837413122715"><a name="p0837413122715"></a><a name="p0837413122715"></a>disable_auto_renew(userDomainId, resource_id="xxxxxxxxxxxx", action_id="autorenew")</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13837213142712"><a name="p13837213142712"></a><a name="p13837213142712"></a>DELETE /v1.0/{domain_id}/common/order-mgr/resources/{resource_id}/actions</p>
<p id="p18371713142718"><a name="p18371713142718"></a><a name="p18371713142718"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00003.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p583761382715"><a name="p583761382715"></a><a name="p583761382715"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00003.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row7837121372716"><td class="cellrowborder" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p38373138271"><a name="p38373138271"></a><a name="p38373138271"></a>Pay-Per-Use Resource</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p883751312277"><a name="p883751312277"></a><a name="p883751312277"></a>query_customer_resource(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p168377131272"><a name="p168377131272"></a><a name="p168377131272"></a>POST /v1.0/{partner_id}/partner/customer-mgr/customer-resource/query-resources</p>
<p id="p38373139277"><a name="p38373139277"></a><a name="p38373139277"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0079744790.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1383701312716"><td class="cellrowborder" rowspan="3" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p15837313202718"><a name="p15837313202718"></a><a name="p15837313202718"></a>Bill</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p1683771319276"><a name="p1683771319276"></a><a name="p1683771319276"></a>query_monthly_expenditure_summary(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p0837113152713"><a name="p0837113152713"></a><a name="p0837113152713"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/monthly-sum</p>
<p id="p118371613142714"><a name="p118371613142714"></a><a name="p118371613142714"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0109708205.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row1583781312272"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p68371513112713"><a name="p68371513112713"></a><a name="p68371513112713"></a>query_resource_usage_details(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1837213162714"><a name="p1837213162714"></a><a name="p1837213162714"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/res-records</p>
<p id="p17837191382716"><a name="p17837191382716"></a><a name="p17837191382716"></a><a href="https://support.huaweicloud.com/api-oce/mbc_00005.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row1483791342718"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p18371213192715"><a name="p18371213192715"></a><a name="p18371213192715"></a>query_resource_usage_record(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p9837101320276"><a name="p9837101320276"></a><a name="p9837101320276"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/res-fee-records</p>
<p id="p188371413192712"><a name="p188371413192712"></a><a name="p188371413192712"></a><a href="https://support.huaweicloud.com/api-oce/mbc_00002.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row15837131322716"><td class="cellrowborder" valign="top" width="26.987301269873008%" headers="mcps1.1.4.1.1 "><p id="p188371213152712"><a name="p188371213152712"></a><a name="p188371213152712"></a>Utilities</p>
</td>
<td class="cellrowborder" valign="top" width="36.44635536446355%" headers="mcps1.1.4.1.2 "><p id="p8837171310270"><a name="p8837171310270"></a><a name="p8837171310270"></a>send_verification_code(userDomainId, **data)</p>
</td>
<td class="cellrowborder" valign="top" width="36.566343365663435%" headers="mcps1.1.4.1.3 "><p id="p1783816139276"><a name="p1783816139276"></a><a name="p1783816139276"></a>POST /v1.0/{partner_id}/partner/common-mgr/verificationcode</p>
<p id="p188382138276"><a name="p188382138276"></a><a name="p188382138276"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0118172609.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
</tbody>
</table>

