# TMS<a name="sdk_11_0026"></a>

基于TMS v1.0 API的SDK接口如下，调用方式请参考示例代码。

<a name="table8484916201010"></a>
<table><thead align="left"><tr id="row157021316171019"><th class="cellrowborder" valign="top" width="26.14261426142614%" id="mcps1.1.4.1.1"><p id="p157026162107"><a name="p157026162107"></a><a name="p157026162107"></a>Interface</p>
</th>
<th class="cellrowborder" valign="top" width="38.89388938893889%" id="mcps1.1.4.1.2"><p id="p370211618107"><a name="p370211618107"></a><a name="p370211618107"></a>Method</p>
</th>
<th class="cellrowborder" valign="top" width="34.96349634963496%" id="mcps1.1.4.1.3"><p id="p1670231681013"><a name="p1670231681013"></a><a name="p1670231681013"></a>API</p>
</th>
</tr>
</thead>
<tbody><tr id="row970281614107"><td class="cellrowborder" rowspan="5" valign="top" width="26.14261426142614%" headers="mcps1.1.4.1.1 "><p id="p27531024204112"><a name="p27531024204112"></a><a name="p27531024204112"></a>TagService</p>
</td>
<td class="cellrowborder" valign="top" width="38.89388938893889%" headers="mcps1.1.4.1.2 "><p id="p1637371218419"><a name="p1637371218419"></a><a name="p1637371218419"></a>String create(List&lt;PredefineTagRequest&gt; tagList)</p>
</td>
<td class="cellrowborder" valign="top" width="34.96349634963496%" headers="mcps1.1.4.1.3 "><p id="p2373121214118"><a name="p2373121214118"></a><a name="p2373121214118"></a>POST /v1.0/predefine_tags/action</p>
<p id="p749083113619"><a name="p749083113619"></a><a name="p749083113619"></a><a href="https://support.huaweicloud.com/api-tms/zh-cn_topic_0056765935.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row11702121671016"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p10373612144110"><a name="p10373612144110"></a><a name="p10373612144110"></a>String dekete(List&lt;PredefineTagRequest&gt; tagList)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p183738124418"><a name="p183738124418"></a><a name="p183738124418"></a>POST/v1.0/predefine_tags/action</p>
<p id="p732212391611"><a name="p732212391611"></a><a name="p732212391611"></a><a href="https://support.huaweicloud.com/api-tms/zh-cn_topic_0056765935.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row370341612101"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p83741312124113"><a name="p83741312124113"></a><a name="p83741312124113"></a>PredefineTags list()</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p3374161234113"><a name="p3374161234113"></a><a name="p3374161234113"></a>GET/v1.0/predefine_tags</p>
<p id="p8669456611"><a name="p8669456611"></a><a name="p8669456611"></a><a href="https://support.huaweicloud.com/api-tms/zh-cn_topic_0056765936.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row19703716191017"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p837441217414"><a name="p837441217414"></a><a name="p837441217414"></a>PredefineTags list(TagFilterOption option)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p13741120411"><a name="p13741120411"></a><a name="p13741120411"></a>GET/v1.0/predefine_tags</p>
<p id="p61444501761"><a name="p61444501761"></a><a name="p61444501761"></a><a href="https://support.huaweicloud.com/api-tms/zh-cn_topic_0056765936.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
<tr id="row1070320164101"><td class="cellrowborder" valign="top" headers="mcps1.1.4.1.1 "><p id="p53742125419"><a name="p53742125419"></a><a name="p53742125419"></a>ActionResponse modify(PredefineTagRequest oldTag, PredefineTagRequest newTag)</p>
</td>
<td class="cellrowborder" valign="top" headers="mcps1.1.4.1.2 "><p id="p1837431244112"><a name="p1837431244112"></a><a name="p1837431244112"></a>PUT/v1.0/predefine_tags</p>
<p id="p91213572611"><a name="p91213572611"></a><a name="p91213572611"></a><a href="https://support.huaweicloud.com/api-tms/zh-cn_topic_0060929630.html" target="_blank" rel="noopener noreferrer">链接</a></p>
</td>
</tr>
</tbody>
</table>

