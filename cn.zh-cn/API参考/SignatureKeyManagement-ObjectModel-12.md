# 对象模型<a name="ZH-CN_TOPIC_0000001081837307"></a>

本节介绍签名密钥的对象模型，如下表所示：

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  签名密钥模型

<a name="zh-cn_topic_0118924546_table1751917"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924546_row53502816"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924546_p38760878"><a name="zh-cn_topic_0118924546_p38760878"></a><a name="zh-cn_topic_0118924546_p38760878"></a><strong id="zh-cn_topic_0118924546_b13303587"><a name="zh-cn_topic_0118924546_b13303587"></a><a name="zh-cn_topic_0118924546_b13303587"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924546_p3848775"><a name="zh-cn_topic_0118924546_p3848775"></a><a name="zh-cn_topic_0118924546_p3848775"></a><strong id="zh-cn_topic_0118924546_b34638975"><a name="zh-cn_topic_0118924546_b34638975"></a><a name="zh-cn_topic_0118924546_b34638975"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924546_p54293586"><a name="zh-cn_topic_0118924546_p54293586"></a><a name="zh-cn_topic_0118924546_p54293586"></a><strong id="zh-cn_topic_0118924546_b18880231"><a name="zh-cn_topic_0118924546_b18880231"></a><a name="zh-cn_topic_0118924546_b18880231"></a>说明</strong></p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924546_p52903732"><a name="zh-cn_topic_0118924546_p52903732"></a><a name="zh-cn_topic_0118924546_p52903732"></a><strong id="zh-cn_topic_0118924546_b6371542"><a name="zh-cn_topic_0118924546_b6371542"></a><a name="zh-cn_topic_0118924546_b6371542"></a>操作类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924546_p46332887"><a name="zh-cn_topic_0118924546_p46332887"></a><a name="zh-cn_topic_0118924546_p46332887"></a><strong id="zh-cn_topic_0118924546_b41208319563"><a name="zh-cn_topic_0118924546_b41208319563"></a><a name="zh-cn_topic_0118924546_b41208319563"></a>是否必选</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924546_row20916077"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924546_p16480716"><a name="zh-cn_topic_0118924546_p16480716"></a><a name="zh-cn_topic_0118924546_p16480716"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924546_p59869652"><a name="zh-cn_topic_0118924546_p59869652"></a><a name="zh-cn_topic_0118924546_p59869652"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924546_p17603628"><a name="zh-cn_topic_0118924546_p17603628"></a><a name="zh-cn_topic_0118924546_p17603628"></a>签名密钥的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924546_p16607740"><a name="zh-cn_topic_0118924546_p16607740"></a><a name="zh-cn_topic_0118924546_p16607740"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924546_p3049709"><a name="zh-cn_topic_0118924546_p3049709"></a><a name="zh-cn_topic_0118924546_p3049709"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924546_row27447385"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924546_p8645726"><a name="zh-cn_topic_0118924546_p8645726"></a><a name="zh-cn_topic_0118924546_p8645726"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924546_p29215191"><a name="zh-cn_topic_0118924546_p29215191"></a><a name="zh-cn_topic_0118924546_p29215191"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924546_p17620269"><a name="zh-cn_topic_0118924546_p17620269"></a><a name="zh-cn_topic_0118924546_p17620269"></a>签名密钥的名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924546_p17955655"><a name="zh-cn_topic_0118924546_p17955655"></a><a name="zh-cn_topic_0118924546_p17955655"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924546_p45121933"><a name="zh-cn_topic_0118924546_p45121933"></a><a name="zh-cn_topic_0118924546_p45121933"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924546_row3444221"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924546_p10546481"><a name="zh-cn_topic_0118924546_p10546481"></a><a name="zh-cn_topic_0118924546_p10546481"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924546_p48958662"><a name="zh-cn_topic_0118924546_p48958662"></a><a name="zh-cn_topic_0118924546_p48958662"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924546_p6228708"><a name="zh-cn_topic_0118924546_p6228708"></a><a name="zh-cn_topic_0118924546_p6228708"></a>签名密钥的key</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924546_p34763314"><a name="zh-cn_topic_0118924546_p34763314"></a><a name="zh-cn_topic_0118924546_p34763314"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924546_p64365016"><a name="zh-cn_topic_0118924546_p64365016"></a><a name="zh-cn_topic_0118924546_p64365016"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924546_row42414236"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924546_p13001082"><a name="zh-cn_topic_0118924546_p13001082"></a><a name="zh-cn_topic_0118924546_p13001082"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924546_p46454725"><a name="zh-cn_topic_0118924546_p46454725"></a><a name="zh-cn_topic_0118924546_p46454725"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924546_p4736356"><a name="zh-cn_topic_0118924546_p4736356"></a><a name="zh-cn_topic_0118924546_p4736356"></a>签名密钥的密钥</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924546_p48100544"><a name="zh-cn_topic_0118924546_p48100544"></a><a name="zh-cn_topic_0118924546_p48100544"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924546_p3829952"><a name="zh-cn_topic_0118924546_p3829952"></a><a name="zh-cn_topic_0118924546_p3829952"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924546_row34469569"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924546_p40571699"><a name="zh-cn_topic_0118924546_p40571699"></a><a name="zh-cn_topic_0118924546_p40571699"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924546_p65082173"><a name="zh-cn_topic_0118924546_p65082173"></a><a name="zh-cn_topic_0118924546_p65082173"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924546_p37164680"><a name="zh-cn_topic_0118924546_p37164680"></a><a name="zh-cn_topic_0118924546_p37164680"></a>创建时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924546_p57549116"><a name="zh-cn_topic_0118924546_p57549116"></a><a name="zh-cn_topic_0118924546_p57549116"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924546_p30966783"><a name="zh-cn_topic_0118924546_p30966783"></a><a name="zh-cn_topic_0118924546_p30966783"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924546_row10265599"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924546_p26207199"><a name="zh-cn_topic_0118924546_p26207199"></a><a name="zh-cn_topic_0118924546_p26207199"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924546_p42408355"><a name="zh-cn_topic_0118924546_p42408355"></a><a name="zh-cn_topic_0118924546_p42408355"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924546_p12524724"><a name="zh-cn_topic_0118924546_p12524724"></a><a name="zh-cn_topic_0118924546_p12524724"></a>更新时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924546_p7869689"><a name="zh-cn_topic_0118924546_p7869689"></a><a name="zh-cn_topic_0118924546_p7869689"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924546_p33465050"><a name="zh-cn_topic_0118924546_p33465050"></a><a name="zh-cn_topic_0118924546_p33465050"></a>-</p>
</td>
</tr>
</tbody>
</table>

