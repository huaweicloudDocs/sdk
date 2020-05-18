# BSS<a name="sdk_13_0011"></a>

基于BSS v1.0 API的SDK接口如下，调用方式请参考示例代码。

>![](public_sys-resources/icon-note.gif) **说明：**   
>如下接口的API链接有面向合作伙伴和面向客户之分，若链接为“合作伙伴运营能力”表明该链接是面向合作伙伴的API接口链接，若链接为“客户运营能力”表明该链接是面向客户的API接口链接。  

<a name="table94971342195618"></a>
<table><thead align="left"><tr id="row107201342165614"><th class="cellrowborder" valign="top" width="26.037396260373956%" id="mcps1.1.4.1.1"><p id="p1072044212568"><a name="p1072044212568"></a><a name="p1072044212568"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="37.186281371862805%" id="mcps1.1.4.1.2"><p id="p187202428561"><a name="p187202428561"></a><a name="p187202428561"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="36.77632236776322%" id="mcps1.1.4.1.3"><p id="p20720142125619"><a name="p20720142125619"></a><a name="p20720142125619"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row3720174205619"><td class="cellrowborder" rowspan="3" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p87203421561"><a name="p87203421561"></a><a name="p87203421561"></a>Customer Management</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p107201842105615"><a name="p107201842105615"></a><a name="p107201842105615"></a>func CheckCustomerRegisterInfo(client *gophercloud.ServiceClient, opts CheckCustomerRegisterInfoBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p187201042165612"><a name="p187201042165612"></a><a name="p187201042165612"></a>POST /v1.0/{partner_id}/partner/customer-mgr/check-user</p>
<p id="p5720104255619"><a name="p5720104255619"></a><a name="p5720104255619"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0083753561.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row15721164215565"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14721124285616"><a name="p14721124285616"></a><a name="p14721124285616"></a>func CreateCustomer(client *gophercloud.ServiceClient, opts CreateCustomerOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p16721124285610"><a name="p16721124285610"></a><a name="p16721124285610"></a>POST /v1.0/{partner_id}/partner/customer-mgr/customer</p>
<p id="p472184285610"><a name="p472184285610"></a><a name="p472184285610"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0080030911.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1972104215562"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p172164265615"><a name="p172164265615"></a><a name="p172164265615"></a>func QueryCustomer(client *gophercloud.ServiceClient, opts QueryCustomerOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p177214425566"><a name="p177214425566"></a><a name="p177214425566"></a>POST /v1.0/{partner_id}/partner/customer-mgr/query</p>
<p id="p1972119427566"><a name="p1972119427566"></a><a name="p1972119427566"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0077254158.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1272111421568"><td class="cellrowborder" rowspan="4" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p472112428564"><a name="p472112428564"></a><a name="p472112428564"></a>Realname Auth</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p2721942115613"><a name="p2721942115613"></a><a name="p2721942115613"></a>func IndividualRealNameAuth(client *gophercloud.ServiceClient, opts IndividualRealNameAuthOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p1772118420569"><a name="p1772118420569"></a><a name="p1772118420569"></a>POST /v1.0/{partner_id}/partner/customer-mgr/realname-auth/individual</p>
<p id="p1772113425564"><a name="p1772113425564"></a><a name="p1772113425564"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00004.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row117211542155617"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p972114215619"><a name="p972114215619"></a><a name="p972114215619"></a>func EnterpriseRealNameAuth(client *gophercloud.ServiceClient, opts EnterpriseRealNameAuthOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10721242145619"><a name="p10721242145619"></a><a name="p10721242145619"></a>POST /v1.0/{partner_id}/partner/customer-mgr/realname-auth/enterprise</p>
<p id="p872164225614"><a name="p872164225614"></a><a name="p872164225614"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00005.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1072114219561"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p27211429562"><a name="p27211429562"></a><a name="p27211429562"></a>func ChangeEnterpriseRealNameAuth(client *gophercloud.ServiceClient, opts ChangeEnterpriseRealNameAuthOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p17721442185617"><a name="p17721442185617"></a><a name="p17721442185617"></a>PUT /v1.0/{partner_id}/partner/customer-mgr/realname-auth/enterprise</p>
<p id="p972114428568"><a name="p972114428568"></a><a name="p972114428568"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00006.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1672194265616"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p27212042155619"><a name="p27212042155619"></a><a name="p27212042155619"></a>func QueryRealNameAuth(client *gophercloud.ServiceClient, opts QueryRealNameAuthOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p772111427562"><a name="p772111427562"></a><a name="p772111427562"></a>GET /v1.0/{partner_id}/partner/customer-mgr/realname-auth/result</p>
<p id="p172116423567"><a name="p172116423567"></a><a name="p172116423567"></a><a href="https://support.huaweicloud.com/api-bpconsole/mc_00007.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row187212042205620"><td class="cellrowborder" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p472184215618"><a name="p472184215618"></a><a name="p472184215618"></a>Enquiry</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p1772154213565"><a name="p1772154213565"></a><a name="p1772154213565"></a>func QueryRating(client *gophercloud.ServiceClient, opts QueryRatingOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p11721142105616"><a name="p11721142105616"></a><a name="p11721142105616"></a>POST /v1.0/{domain_id}/customer/product-mgr/query-rating</p>
<p id="p18721184217569"><a name="p18721184217569"></a><a name="p18721184217569"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0078731101.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p20721184210562"><a name="p20721184210562"></a><a name="p20721184210562"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0078731101.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row17212425569"><td class="cellrowborder" rowspan="7" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p127211542145616"><a name="p127211542145616"></a><a name="p127211542145616"></a>Period Order</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p157211942125613"><a name="p157211942125613"></a><a name="p157211942125613"></a>func QueryOrderList(client *gophercloud.ServiceClient, opts QueryOrderListBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p572112422564"><a name="p572112422564"></a><a name="p572112422564"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/detail</p>
<p id="p1872114220566"><a name="p1872114220566"></a><a name="p1872114220566"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0083740673.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p107211442175613"><a name="p107211442175613"></a><a name="p107211442175613"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0083740673.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row117229429569"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p0722942165619"><a name="p0722942165619"></a><a name="p0722942165619"></a>func QueryOrderDetail(client *gophercloud.ServiceClient, opts QueryOrderDetailBuilder, orderId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p7722142175618"><a name="p7722142175618"></a><a name="p7722142175618"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/{order_id}</p>
<p id="p1772214295612"><a name="p1772214295612"></a><a name="p1772214295612"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746564.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1472234210564"><a name="p1472234210564"></a><a name="p1472234210564"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746564.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row177221042135616"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1722134225620"><a name="p1722134225620"></a><a name="p1722134225620"></a>func PayPeriodOrder(client *gophercloud.ServiceClient, opts PayPeriodOrderBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p11722942155615"><a name="p11722942155615"></a><a name="p11722942155615"></a>POST /v1.0/{domain_id}/customer/order-mgr/order/pay</p>
<p id="p1072254275619"><a name="p1072254275619"></a><a name="p1072254275619"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p87221642195618"><a name="p87221642195618"></a><a name="p87221642195618"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0075746561.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row19722174219566"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16722184219566"><a name="p16722184219566"></a><a name="p16722184219566"></a>func UnsubscribePeriodOrder(client *gophercloud.ServiceClient, opts UnsubscribePeriodOrderBuilder, orderId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p117221042155613"><a name="p117221042155613"></a><a name="p117221042155613"></a>DELETE /v1.0/{domain_id}/customer/order-mgr/orders/{order_id}</p>
<p id="p177221642125618"><a name="p177221642125618"></a><a name="p177221642125618"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0076597539.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1172214429562"><a name="p1172214429562"></a><a name="p1172214429562"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0076597539.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row0722114215614"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p372234245613"><a name="p372234245613"></a><a name="p372234245613"></a>func CancelOrder(client *gophercloud.ServiceClient, opts CancelOrderBuilder,actionId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1872210420562"><a name="p1872210420562"></a><a name="p1872210420562"></a>PUT /v1.0/{domain_id}/customer/order-mgr/orders/actions</p>
<p id="p372224255610"><a name="p372224255610"></a><a name="p372224255610"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0079992470.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1172218424562"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1272220424566"><a name="p1272220424566"></a><a name="p1272220424566"></a>func QueryRefundOrderAmount(client *gophercloud.ServiceClient, opts QueryRefundOrderAmountBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p372294235614"><a name="p372294235614"></a><a name="p372294235614"></a>GET /v1.0/{domain_id}/common/order-mgr/orders/refund-order</p>
<p id="p1872224215563"><a name="p1872224215563"></a><a name="p1872224215563"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0112435250.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row67221542135611"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p4722342115612"><a name="p4722342115612"></a><a name="p4722342115612"></a>func QueryResourceStatusByOrderId(client *gophercloud.ServiceClient, opts QueryResourceStatusByOrderIdBuilder, orderId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1872211428564"><a name="p1872211428564"></a><a name="p1872211428564"></a>GET /v1.0/{domain_id}/common/order-mgr/orders-resource/{order_id}</p>
<p id="p572224275619"><a name="p572224275619"></a><a name="p572224275619"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00001.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1722642205620"><a name="p1722642205620"></a><a name="p1722642205620"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00001.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row1272214275616"><td class="cellrowborder" rowspan="5" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p12722742195615"><a name="p12722742195615"></a><a name="p12722742195615"></a>Period Resource</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p197222042105620"><a name="p197222042105620"></a><a name="p197222042105620"></a>func QueryCustomerPeriodResourcesList(client *gophercloud.ServiceClient, opts QueryCustomerPeriodResourcesListOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p107223426564"><a name="p107223426564"></a><a name="p107223426564"></a>GET /v1.0/{domain_id}/common/order-mgr/resources/detail</p>
<p id="p1872254275612"><a name="p1872254275612"></a><a name="p1872254275612"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0084961226.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p6722144210560"><a name="p6722144210560"></a><a name="p6722144210560"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0084961226.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row157221142175614"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p16722042175611"><a name="p16722042175611"></a><a name="p16722042175611"></a>func RenewSubscriptionByResourceId(client *gophercloud.ServiceClient, opts RenewSubscriptionByResourceIdOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p167221142115610"><a name="p167221142115610"></a><a name="p167221142115610"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/renew</p>
<p id="p10722442145610"><a name="p10722442145610"></a><a name="p10722442145610"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0082522029.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1472215428567"><a name="p1472215428567"></a><a name="p1472215428567"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522029.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row13723194211561"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p372394212565"><a name="p372394212565"></a><a name="p372394212565"></a>func UnsubscribeByResourceId(client *gophercloud.ServiceClient, opts UnsubscribeByResourceIdOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1872374255618"><a name="p1872374255618"></a><a name="p1872374255618"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/delete</p>
<p id="p17723154285615"><a name="p17723154285615"></a><a name="p17723154285615"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p8723184214561"><a name="p8723184214561"></a><a name="p8723184214561"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0082522030.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row7723194212564"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p11723124220569"><a name="p11723124220569"></a><a name="p11723124220569"></a>func EnableAutoRenew(client *gophercloud.ServiceClient, opts EnableAutoRenewOptsBuilder,resourceId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p10723442125619"><a name="p10723442125619"></a><a name="p10723442125619"></a>POST /v1.0/{domain_id}/common/order-mgr/resources/{resource_id}/actions</p>
<p id="p157235422566"><a name="p157235422566"></a><a name="p157235422566"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00002.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p5723124255617"><a name="p5723124255617"></a><a name="p5723124255617"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00002.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row1372324215565"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p772344255619"><a name="p772344255619"></a><a name="p772344255619"></a>func DisableAutoRenew(client *gophercloud.ServiceClient, opts DisableAutoRenewOptsBuilder,resourceId string)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p177233426564"><a name="p177233426564"></a><a name="p177233426564"></a>DELETE /v1.0/{domain_id}/common/order-mgr/resources/{resource_id}/actions</p>
<p id="p972304216567"><a name="p972304216567"></a><a name="p972304216567"></a><a href="https://support.huaweicloud.com/api-bpconsole/api_order_00003.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
<p id="p1972394245611"><a name="p1972394245611"></a><a name="p1972394245611"></a><a href="https://support.huaweicloud.com/api-oce/api_order_00003.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row4723154214569"><td class="cellrowborder" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p16723124219564"><a name="p16723124219564"></a><a name="p16723124219564"></a>Pay-Per-Use Resource</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p1372384219567"><a name="p1372384219567"></a><a name="p1372384219567"></a>func QueryCustomerResource(client *gophercloud.ServiceClient, opts QueryCustomerResourceOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p172318428568"><a name="p172318428568"></a><a name="p172318428568"></a>POST /v1.0/{partner_id}/partner/customer-mgr/customer-resource/query-resources</p>
<p id="p1472324295616"><a name="p1472324295616"></a><a name="p1472324295616"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0079744790.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
<tr id="row1272304214562"><td class="cellrowborder" rowspan="3" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p57236429566"><a name="p57236429566"></a><a name="p57236429566"></a>Bill</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p137231442105613"><a name="p137231442105613"></a><a name="p137231442105613"></a>func QueryMonthlyExpenditureSummary(client *gophercloud.ServiceClient, opts QueryMonthlyExpenditureSummaryOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p1723124275612"><a name="p1723124275612"></a><a name="p1723124275612"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/monthly-sum</p>
<p id="p272315423563"><a name="p272315423563"></a><a name="p272315423563"></a><a href="https://support.huaweicloud.com/api-oce/zh-cn_topic_0109708205.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row117231542105610"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p1272334295614"><a name="p1272334295614"></a><a name="p1272334295614"></a>func QueryResourceUsageDetails(client *gophercloud.ServiceClient, opts QueryResourceUsageDetailsOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p6723174245613"><a name="p6723174245613"></a><a name="p6723174245613"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/res-records</p>
<p id="p1372317427561"><a name="p1372317427561"></a><a name="p1372317427561"></a><a href="https://support.huaweicloud.com/api-oce/mbc_00005.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row9723144210561"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p14723194285616"><a name="p14723194285616"></a><a name="p14723194285616"></a>func QueryResourceUsageRecord(client *gophercloud.ServiceClient, opts QueryResourceUsageRecordOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1072311420561"><a name="p1072311420561"></a><a name="p1072311420561"></a>GET /v1.0/{domain_id}/customer/account-mgr/bill/res-fee-records</p>
<p id="p172314220566"><a name="p172314220566"></a><a name="p172314220566"></a><a href="https://support.huaweicloud.com/api-oce/mbc_00002.html" target="_blank" rel="noopener noreferrer">链接（客户运营能力）</a></p>
</td>
</tr>
<tr id="row072324215610"><td class="cellrowborder" valign="top" width="26.037396260373956%" headers="mcps1.1.4.1.1 "><p id="p11723124211566"><a name="p11723124211566"></a><a name="p11723124211566"></a>Utilities</p>
</td>
<td class="cellrowborder" valign="top" width="37.186281371862805%" headers="mcps1.1.4.1.2 "><p id="p18723164211561"><a name="p18723164211561"></a><a name="p18723164211561"></a>func SendVerificationCode(client *gophercloud.ServiceClient, opts SendVerificationCodeOptsBuilder)</p>
</td>
<td class="cellrowborder" valign="top" width="36.77632236776322%" headers="mcps1.1.4.1.3 "><p id="p6723134265610"><a name="p6723134265610"></a><a name="p6723134265610"></a>POST /v1.0/{partner_id}/partner/common-mgr/verificationcode</p>
<p id="p1572314219567"><a name="p1572314219567"></a><a name="p1572314219567"></a><a href="https://support.huaweicloud.com/api-bpconsole/zh-cn_topic_0118172609.html" target="_blank" rel="noopener noreferrer">链接（合作伙伴运营能力）</a></p>
</td>
</tr>
</tbody>
</table>

