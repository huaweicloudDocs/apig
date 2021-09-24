# 对象模型<a name="ZH-CN_TOPIC_0000001081976123"></a>

本节介绍特殊流控的对象模型，如下表所示：

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  特殊流控对象模型

<a name="zh-cn_topic_0118922269_table20320369"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922269_row1070821"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118922269_p19627639"><a name="zh-cn_topic_0118922269_p19627639"></a><a name="zh-cn_topic_0118922269_p19627639"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118922269_p46334942"><a name="zh-cn_topic_0118922269_p46334942"></a><a name="zh-cn_topic_0118922269_p46334942"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118922269_p62142850"><a name="zh-cn_topic_0118922269_p62142850"></a><a name="zh-cn_topic_0118922269_p62142850"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118922269_p406090"><a name="zh-cn_topic_0118922269_p406090"></a><a name="zh-cn_topic_0118922269_p406090"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118922269_p32893343"><a name="zh-cn_topic_0118922269_p32893343"></a><a name="zh-cn_topic_0118922269_p32893343"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922269_row47115112"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922269_p58227726"><a name="zh-cn_topic_0118922269_p58227726"></a><a name="zh-cn_topic_0118922269_p58227726"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922269_p18825336"><a name="zh-cn_topic_0118922269_p18825336"></a><a name="zh-cn_topic_0118922269_p18825336"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922269_p48457230"><a name="zh-cn_topic_0118922269_p48457230"></a><a name="zh-cn_topic_0118922269_p48457230"></a>特殊配置的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922269_p32721594"><a name="zh-cn_topic_0118922269_p32721594"></a><a name="zh-cn_topic_0118922269_p32721594"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922269_p33203425"><a name="zh-cn_topic_0118922269_p33203425"></a><a name="zh-cn_topic_0118922269_p33203425"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922269_row30395375"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922269_p46106333"><a name="zh-cn_topic_0118922269_p46106333"></a><a name="zh-cn_topic_0118922269_p46106333"></a>strategy_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922269_p43625467"><a name="zh-cn_topic_0118922269_p43625467"></a><a name="zh-cn_topic_0118922269_p43625467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922269_p44001905"><a name="zh-cn_topic_0118922269_p44001905"></a><a name="zh-cn_topic_0118922269_p44001905"></a>流控策略编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922269_p7384552"><a name="zh-cn_topic_0118922269_p7384552"></a><a name="zh-cn_topic_0118922269_p7384552"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922269_p61277831"><a name="zh-cn_topic_0118922269_p61277831"></a><a name="zh-cn_topic_0118922269_p61277831"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922269_row14629574"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922269_p44144821"><a name="zh-cn_topic_0118922269_p44144821"></a><a name="zh-cn_topic_0118922269_p44144821"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922269_p18960737"><a name="zh-cn_topic_0118922269_p18960737"></a><a name="zh-cn_topic_0118922269_p18960737"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922269_p59424689"><a name="zh-cn_topic_0118922269_p59424689"></a><a name="zh-cn_topic_0118922269_p59424689"></a>生效的特殊对象的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922269_p48670477"><a name="zh-cn_topic_0118922269_p48670477"></a><a name="zh-cn_topic_0118922269_p48670477"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922269_p49994590"><a name="zh-cn_topic_0118922269_p49994590"></a><a name="zh-cn_topic_0118922269_p49994590"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922269_row47298134"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922269_p5943665"><a name="zh-cn_topic_0118922269_p5943665"></a><a name="zh-cn_topic_0118922269_p5943665"></a>instance_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922269_p11674869"><a name="zh-cn_topic_0118922269_p11674869"></a><a name="zh-cn_topic_0118922269_p11674869"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922269_p6140296"><a name="zh-cn_topic_0118922269_p6140296"></a><a name="zh-cn_topic_0118922269_p6140296"></a>对象类型APP/USER</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922269_p27602005"><a name="zh-cn_topic_0118922269_p27602005"></a><a name="zh-cn_topic_0118922269_p27602005"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922269_p21169922"><a name="zh-cn_topic_0118922269_p21169922"></a><a name="zh-cn_topic_0118922269_p21169922"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922269_row56311572"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922269_p64943477"><a name="zh-cn_topic_0118922269_p64943477"></a><a name="zh-cn_topic_0118922269_p64943477"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922269_p25930250"><a name="zh-cn_topic_0118922269_p25930250"></a><a name="zh-cn_topic_0118922269_p25930250"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922269_p19975483"><a name="zh-cn_topic_0118922269_p19975483"></a><a name="zh-cn_topic_0118922269_p19975483"></a>特殊对象在流控时间内能够访问API的最大次数限制</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922269_p7401458"><a name="zh-cn_topic_0118922269_p7401458"></a><a name="zh-cn_topic_0118922269_p7401458"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922269_p62647188"><a name="zh-cn_topic_0118922269_p62647188"></a><a name="zh-cn_topic_0118922269_p62647188"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922269_row26953786"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922269_p35773034"><a name="zh-cn_topic_0118922269_p35773034"></a><a name="zh-cn_topic_0118922269_p35773034"></a>apply_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922269_p11934651"><a name="zh-cn_topic_0118922269_p11934651"></a><a name="zh-cn_topic_0118922269_p11934651"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922269_p27182676"><a name="zh-cn_topic_0118922269_p27182676"></a><a name="zh-cn_topic_0118922269_p27182676"></a>设置的时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922269_p54313182"><a name="zh-cn_topic_0118922269_p54313182"></a><a name="zh-cn_topic_0118922269_p54313182"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922269_p37291649"><a name="zh-cn_topic_0118922269_p37291649"></a><a name="zh-cn_topic_0118922269_p37291649"></a>-</p>
</td>
</tr>
</tbody>
</table>

