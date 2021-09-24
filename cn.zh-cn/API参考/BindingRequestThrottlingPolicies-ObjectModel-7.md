# 对象模型<a name="ZH-CN_TOPIC_0000001082221197"></a>

本节介绍流控策略与API的绑定关系的对象模型，如下表所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  流控策略限定关系对象模型

<a name="zh-cn_topic_0118922262_table64652501"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922262_row15393610"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118922262_p38922887"><a name="zh-cn_topic_0118922262_p38922887"></a><a name="zh-cn_topic_0118922262_p38922887"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118922262_p65746124"><a name="zh-cn_topic_0118922262_p65746124"></a><a name="zh-cn_topic_0118922262_p65746124"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118922262_p23835842"><a name="zh-cn_topic_0118922262_p23835842"></a><a name="zh-cn_topic_0118922262_p23835842"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118922262_p51655056"><a name="zh-cn_topic_0118922262_p51655056"></a><a name="zh-cn_topic_0118922262_p51655056"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118922262_p23310047"><a name="zh-cn_topic_0118922262_p23310047"></a><a name="zh-cn_topic_0118922262_p23310047"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922262_row9065687"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922262_p63232031"><a name="zh-cn_topic_0118922262_p63232031"></a><a name="zh-cn_topic_0118922262_p63232031"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922262_p21520863"><a name="zh-cn_topic_0118922262_p21520863"></a><a name="zh-cn_topic_0118922262_p21520863"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922262_p65468352"><a name="zh-cn_topic_0118922262_p65468352"></a><a name="zh-cn_topic_0118922262_p65468352"></a>绑定关系的ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922262_p1336297"><a name="zh-cn_topic_0118922262_p1336297"></a><a name="zh-cn_topic_0118922262_p1336297"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922262_p41131267"><a name="zh-cn_topic_0118922262_p41131267"></a><a name="zh-cn_topic_0118922262_p41131267"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922262_row34637090"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922262_p54140904"><a name="zh-cn_topic_0118922262_p54140904"></a><a name="zh-cn_topic_0118922262_p54140904"></a>throttle_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922262_p23337074"><a name="zh-cn_topic_0118922262_p23337074"></a><a name="zh-cn_topic_0118922262_p23337074"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922262_p11254824"><a name="zh-cn_topic_0118922262_p11254824"></a><a name="zh-cn_topic_0118922262_p11254824"></a>流控策略的ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922262_p39225588"><a name="zh-cn_topic_0118922262_p39225588"></a><a name="zh-cn_topic_0118922262_p39225588"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922262_p23156027"><a name="zh-cn_topic_0118922262_p23156027"></a><a name="zh-cn_topic_0118922262_p23156027"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922262_row7077657"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922262_p36419367"><a name="zh-cn_topic_0118922262_p36419367"></a><a name="zh-cn_topic_0118922262_p36419367"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922262_p64287589"><a name="zh-cn_topic_0118922262_p64287589"></a><a name="zh-cn_topic_0118922262_p64287589"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922262_p39912187"><a name="zh-cn_topic_0118922262_p39912187"></a><a name="zh-cn_topic_0118922262_p39912187"></a>API的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922262_p11661714"><a name="zh-cn_topic_0118922262_p11661714"></a><a name="zh-cn_topic_0118922262_p11661714"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922262_p5074769"><a name="zh-cn_topic_0118922262_p5074769"></a><a name="zh-cn_topic_0118922262_p5074769"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922262_row45672928"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922262_p8519663"><a name="zh-cn_topic_0118922262_p8519663"></a><a name="zh-cn_topic_0118922262_p8519663"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922262_p19004091"><a name="zh-cn_topic_0118922262_p19004091"></a><a name="zh-cn_topic_0118922262_p19004091"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922262_p62936363"><a name="zh-cn_topic_0118922262_p62936363"></a><a name="zh-cn_topic_0118922262_p62936363"></a>绑定的环境编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922262_p64680615"><a name="zh-cn_topic_0118922262_p64680615"></a><a name="zh-cn_topic_0118922262_p64680615"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922262_p4638488"><a name="zh-cn_topic_0118922262_p4638488"></a><a name="zh-cn_topic_0118922262_p4638488"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922262_row41746400"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922262_p26015259"><a name="zh-cn_topic_0118922262_p26015259"></a><a name="zh-cn_topic_0118922262_p26015259"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922262_p26861247"><a name="zh-cn_topic_0118922262_p26861247"></a><a name="zh-cn_topic_0118922262_p26861247"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922262_p28277362"><a name="zh-cn_topic_0118922262_p28277362"></a><a name="zh-cn_topic_0118922262_p28277362"></a>绑定时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922262_p8765023"><a name="zh-cn_topic_0118922262_p8765023"></a><a name="zh-cn_topic_0118922262_p8765023"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922262_p38878252"><a name="zh-cn_topic_0118922262_p38878252"></a><a name="zh-cn_topic_0118922262_p38878252"></a>-</p>
</td>
</tr>
</tbody>
</table>

