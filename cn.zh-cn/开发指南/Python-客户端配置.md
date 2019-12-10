# Python 客户端配置<a name="ZH-CN_TOPIC_0111241269"></a>

SDK支持的自定义功能，用户可以通过配置进行开启或者关闭。

示例代码：

```
conn = connection.Connection(auth_url=auth_url,
                             user_domain_id=userDomainId,
                             project_id=projectId,
                             username=username,
                             password=password,
                             verify=False)
```

当前支持的自定义参数如下：

<a name="table2960834219313"></a>
<table><thead align="left"><tr id="row3681197319313"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="p5949226519313"><a name="p5949226519313"></a><a name="p5949226519313"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.2"><p id="p5414419019313"><a name="p5414419019313"></a><a name="p5414419019313"></a>默认值</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.3"><p id="p2360329219313"><a name="p2360329219313"></a><a name="p2360329219313"></a>功能描述</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="p3281847419313"><a name="p3281847419313"></a><a name="p3281847419313"></a>备注</p>
</th>
</tr>
</thead>
<tbody><tr id="row2693081019313"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="p3391202019313"><a name="p3391202019313"></a><a name="p3391202019313"></a>verify</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="p675589164646"><a name="p675589164646"></a><a name="p675589164646"></a>True</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="p3088153319313"><a name="p3088153319313"></a><a name="p3088153319313"></a>SSL检查</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="p1837622019313"><a name="p1837622019313"></a><a name="p1837622019313"></a>建议打开</p>
</td>
</tr>
</tbody>
</table>

