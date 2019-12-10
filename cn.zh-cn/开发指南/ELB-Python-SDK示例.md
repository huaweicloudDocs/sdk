# ELB Python SDK示例<a name="ZH-CN_TOPIC_0072126391"></a>

SDK与RESTful API一一对应，SDK最新版本支持的接口列表，以及SDK和API的对应关系，请参考[这里](Python-ELB.md)。

在使用ELB SDK的时候，SDK支持的参数细节，请参考ELB API[描述](https://support.huaweicloud.com/api-elb/zh-cn_topic_0022480177.html)。

增强型负载均衡ELB v2 Python SDK支持如下资源对象的操作，资源对象的“增改查删”代码示例如下：

<a name="table2317742153910"></a>
<table><thead align="left"><tr id="row105381942173916"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="p95381642123916"><a name="p95381642123916"></a><a name="p95381642123916"></a>资源对象</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="p11538144216391"><a name="p11538144216391"></a><a name="p11538144216391"></a>“增改查删”代码样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row35383428392"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1353817422399"><a name="p1353817422399"></a><a name="p1353817422399"></a>loadbalacner</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p35381042203918"><a name="p35381042203918"></a><a name="p35381042203918"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/LoadBalancer.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row753894210391"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1353804263917"><a name="p1353804263917"></a><a name="p1353804263917"></a>listener</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p125381842103911"><a name="p125381842103911"></a><a name="p125381842103911"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/Listener.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row115381742143915"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1853864214398"><a name="p1853864214398"></a><a name="p1853864214398"></a>pool</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p145381842113914"><a name="p145381842113914"></a><a name="p145381842113914"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/Pool.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1538142123913"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p19538164283911"><a name="p19538164283911"></a><a name="p19538164283911"></a>member</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p13538174219393"><a name="p13538174219393"></a><a name="p13538174219393"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/Member.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row17538942103918"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p15538114213917"><a name="p15538114213917"></a><a name="p15538114213917"></a>healthmonitor</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p2053854218397"><a name="p2053854218397"></a><a name="p2053854218397"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/healthmonitor.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row353814273915"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1253844223911"><a name="p1253844223911"></a><a name="p1253844223911"></a>certificate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p55381426392"><a name="p55381426392"></a><a name="p55381426392"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/certification.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row35385422395"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p6538194218398"><a name="p6538194218398"></a><a name="p6538194218398"></a>l7policy</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p5538342143913"><a name="p5538342143913"></a><a name="p5538342143913"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/l7policy.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row0538114212398"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1453814214392"><a name="p1453814214392"></a><a name="p1453814214392"></a>l7rule</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p95381142143913"><a name="p95381142143913"></a><a name="p95381142143913"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/l7rule.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row1154094214397"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p20540142113914"><a name="p20540142113914"></a><a name="p20540142113914"></a>whitelist</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p19540154293917"><a name="p19540154293917"></a><a name="p19540154293917"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/network/WhiteList.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
</tbody>
</table>

经典型负载均衡ELB v1 Python SDK支持如下资源对象的操作，资源对象的“增改查删”代码示例如下：

<a name="table438184210394"></a>
<table><thead align="left"><tr id="row5540174219399"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="p05406423391"><a name="p05406423391"></a><a name="p05406423391"></a>资源对象</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="p175401442113911"><a name="p175401442113911"></a><a name="p175401442113911"></a>“增改查删”代码样例</p>
</th>
</tr>
</thead>
<tbody><tr id="row195401742183916"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p7540154212396"><a name="p7540154212396"></a><a name="p7540154212396"></a>loadbalacner</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p19540142193910"><a name="p19540142193910"></a><a name="p19540142193910"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/elb/v1/loadbalancer.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row2540114263919"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1754084273914"><a name="p1754084273914"></a><a name="p1754084273914"></a>listener</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p18540134210395"><a name="p18540134210395"></a><a name="p18540134210395"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/elb/v1/listener.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row75401442183911"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p4540154217394"><a name="p4540154217394"></a><a name="p4540154217394"></a>member</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p15540124253910"><a name="p15540124253910"></a><a name="p15540124253910"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/elb/v1/member.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row8540742163916"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p6540134216399"><a name="p6540134216399"></a><a name="p6540134216399"></a>healthcheck</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p14540342183910"><a name="p14540342183910"></a><a name="p14540342183910"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/elb/v1/healthcheck.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
<tr id="row18540542143918"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p85404425398"><a name="p85404425398"></a><a name="p85404425398"></a>certificate</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p654016426399"><a name="p654016426399"></a><a name="p654016426399"></a><a href="https://github.com/huaweicloud/huaweicloud-sdk-python/blob/master/examples/elb/v1/certificate.py" target="_blank" rel="noopener noreferrer">代码</a></p>
</td>
</tr>
</tbody>
</table>

