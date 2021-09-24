# 对象模型<a name="ZH-CN_TOPIC_0000001082221221"></a>

本节介绍签名密钥与API的绑定关系的对象模型，如下表所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  签名密钥与API绑定关系对象模型

<a name="zh-cn_topic_0118924552_table27410541"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924552_row28527726"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924552_p29044451"><a name="zh-cn_topic_0118924552_p29044451"></a><a name="zh-cn_topic_0118924552_p29044451"></a><strong id="zh-cn_topic_0118924552_b60073473"><a name="zh-cn_topic_0118924552_b60073473"></a><a name="zh-cn_topic_0118924552_b60073473"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924552_p34113110"><a name="zh-cn_topic_0118924552_p34113110"></a><a name="zh-cn_topic_0118924552_p34113110"></a><strong id="zh-cn_topic_0118924552_b38582535"><a name="zh-cn_topic_0118924552_b38582535"></a><a name="zh-cn_topic_0118924552_b38582535"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924552_p38177670"><a name="zh-cn_topic_0118924552_p38177670"></a><a name="zh-cn_topic_0118924552_p38177670"></a><strong id="zh-cn_topic_0118924552_b8054718"><a name="zh-cn_topic_0118924552_b8054718"></a><a name="zh-cn_topic_0118924552_b8054718"></a>说明</strong></p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924552_p48452384"><a name="zh-cn_topic_0118924552_p48452384"></a><a name="zh-cn_topic_0118924552_p48452384"></a><strong id="zh-cn_topic_0118924552_b33418278"><a name="zh-cn_topic_0118924552_b33418278"></a><a name="zh-cn_topic_0118924552_b33418278"></a>操作类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924552_p22525974"><a name="zh-cn_topic_0118924552_p22525974"></a><a name="zh-cn_topic_0118924552_p22525974"></a><strong id="zh-cn_topic_0118924552_b1977561513569"><a name="zh-cn_topic_0118924552_b1977561513569"></a><a name="zh-cn_topic_0118924552_b1977561513569"></a>是否必选</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924552_row46872675"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924552_p38590344"><a name="zh-cn_topic_0118924552_p38590344"></a><a name="zh-cn_topic_0118924552_p38590344"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924552_p38810145"><a name="zh-cn_topic_0118924552_p38810145"></a><a name="zh-cn_topic_0118924552_p38810145"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924552_p56614039"><a name="zh-cn_topic_0118924552_p56614039"></a><a name="zh-cn_topic_0118924552_p56614039"></a>绑定关系的ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924552_p22334417"><a name="zh-cn_topic_0118924552_p22334417"></a><a name="zh-cn_topic_0118924552_p22334417"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924552_p64257335"><a name="zh-cn_topic_0118924552_p64257335"></a><a name="zh-cn_topic_0118924552_p64257335"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924552_row41445111"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924552_p1610827"><a name="zh-cn_topic_0118924552_p1610827"></a><a name="zh-cn_topic_0118924552_p1610827"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924552_p63368192"><a name="zh-cn_topic_0118924552_p63368192"></a><a name="zh-cn_topic_0118924552_p63368192"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924552_p32549950"><a name="zh-cn_topic_0118924552_p32549950"></a><a name="zh-cn_topic_0118924552_p32549950"></a>API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924552_p19300268"><a name="zh-cn_topic_0118924552_p19300268"></a><a name="zh-cn_topic_0118924552_p19300268"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924552_p19817842"><a name="zh-cn_topic_0118924552_p19817842"></a><a name="zh-cn_topic_0118924552_p19817842"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924552_row44142854"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924552_p18801412"><a name="zh-cn_topic_0118924552_p18801412"></a><a name="zh-cn_topic_0118924552_p18801412"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924552_p46519407"><a name="zh-cn_topic_0118924552_p46519407"></a><a name="zh-cn_topic_0118924552_p46519407"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924552_p9975598"><a name="zh-cn_topic_0118924552_p9975598"></a><a name="zh-cn_topic_0118924552_p9975598"></a>签名密钥编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924552_p2717098"><a name="zh-cn_topic_0118924552_p2717098"></a><a name="zh-cn_topic_0118924552_p2717098"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924552_p18758346"><a name="zh-cn_topic_0118924552_p18758346"></a><a name="zh-cn_topic_0118924552_p18758346"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924552_row34607387"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924552_p51734957"><a name="zh-cn_topic_0118924552_p51734957"></a><a name="zh-cn_topic_0118924552_p51734957"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924552_p29781975"><a name="zh-cn_topic_0118924552_p29781975"></a><a name="zh-cn_topic_0118924552_p29781975"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924552_p63529794"><a name="zh-cn_topic_0118924552_p63529794"></a><a name="zh-cn_topic_0118924552_p63529794"></a>环境编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924552_p45639702"><a name="zh-cn_topic_0118924552_p45639702"></a><a name="zh-cn_topic_0118924552_p45639702"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924552_p5828345"><a name="zh-cn_topic_0118924552_p5828345"></a><a name="zh-cn_topic_0118924552_p5828345"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924552_row52455113"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924552_p21005769"><a name="zh-cn_topic_0118924552_p21005769"></a><a name="zh-cn_topic_0118924552_p21005769"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924552_p23745709"><a name="zh-cn_topic_0118924552_p23745709"></a><a name="zh-cn_topic_0118924552_p23745709"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924552_p44354270"><a name="zh-cn_topic_0118924552_p44354270"></a><a name="zh-cn_topic_0118924552_p44354270"></a>绑定时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924552_p35926083"><a name="zh-cn_topic_0118924552_p35926083"></a><a name="zh-cn_topic_0118924552_p35926083"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924552_p24331588"><a name="zh-cn_topic_0118924552_p24331588"></a><a name="zh-cn_topic_0118924552_p24331588"></a>否</p>
</td>
</tr>
</tbody>
</table>

