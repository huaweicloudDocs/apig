# 对象模型<a name="ZH-CN_TOPIC_0000001082221189"></a>

本节介绍环境的对象模型。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  环境管理对象模型

<a name="zh-cn_topic_0118922243_table61885012"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922243_row33851179"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118922243_p57590974"><a name="zh-cn_topic_0118922243_p57590974"></a><a name="zh-cn_topic_0118922243_p57590974"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118922243_p34357326"><a name="zh-cn_topic_0118922243_p34357326"></a><a name="zh-cn_topic_0118922243_p34357326"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118922243_p31480002"><a name="zh-cn_topic_0118922243_p31480002"></a><a name="zh-cn_topic_0118922243_p31480002"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118922243_p66852227"><a name="zh-cn_topic_0118922243_p66852227"></a><a name="zh-cn_topic_0118922243_p66852227"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118922243_p46321272"><a name="zh-cn_topic_0118922243_p46321272"></a><a name="zh-cn_topic_0118922243_p46321272"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922243_row61035529"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922243_p44930848"><a name="zh-cn_topic_0118922243_p44930848"></a><a name="zh-cn_topic_0118922243_p44930848"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922243_p15520034"><a name="zh-cn_topic_0118922243_p15520034"></a><a name="zh-cn_topic_0118922243_p15520034"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922243_p49163257"><a name="zh-cn_topic_0118922243_p49163257"></a><a name="zh-cn_topic_0118922243_p49163257"></a>环境ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922243_p22800909"><a name="zh-cn_topic_0118922243_p22800909"></a><a name="zh-cn_topic_0118922243_p22800909"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922243_p34934341"><a name="zh-cn_topic_0118922243_p34934341"></a><a name="zh-cn_topic_0118922243_p34934341"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922243_row45973618"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922243_p32875612"><a name="zh-cn_topic_0118922243_p32875612"></a><a name="zh-cn_topic_0118922243_p32875612"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922243_p45678943"><a name="zh-cn_topic_0118922243_p45678943"></a><a name="zh-cn_topic_0118922243_p45678943"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922243_p9006882"><a name="zh-cn_topic_0118922243_p9006882"></a><a name="zh-cn_topic_0118922243_p9006882"></a>环境名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922243_p58468813"><a name="zh-cn_topic_0118922243_p58468813"></a><a name="zh-cn_topic_0118922243_p58468813"></a>CUR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922243_p38353417"><a name="zh-cn_topic_0118922243_p38353417"></a><a name="zh-cn_topic_0118922243_p38353417"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922243_row9636437"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922243_p42353900"><a name="zh-cn_topic_0118922243_p42353900"></a><a name="zh-cn_topic_0118922243_p42353900"></a>alias</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922243_p8113896"><a name="zh-cn_topic_0118922243_p8113896"></a><a name="zh-cn_topic_0118922243_p8113896"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922243_p53245873"><a name="zh-cn_topic_0118922243_p53245873"></a><a name="zh-cn_topic_0118922243_p53245873"></a>环境别名</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922243_p17948462"><a name="zh-cn_topic_0118922243_p17948462"></a><a name="zh-cn_topic_0118922243_p17948462"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922243_p44539336"><a name="zh-cn_topic_0118922243_p44539336"></a><a name="zh-cn_topic_0118922243_p44539336"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922243_row65309707"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922243_p55594906"><a name="zh-cn_topic_0118922243_p55594906"></a><a name="zh-cn_topic_0118922243_p55594906"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922243_p6893562"><a name="zh-cn_topic_0118922243_p6893562"></a><a name="zh-cn_topic_0118922243_p6893562"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922243_p21507667"><a name="zh-cn_topic_0118922243_p21507667"></a><a name="zh-cn_topic_0118922243_p21507667"></a>创建环境的租户编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922243_p64399436"><a name="zh-cn_topic_0118922243_p64399436"></a><a name="zh-cn_topic_0118922243_p64399436"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922243_p48971789"><a name="zh-cn_topic_0118922243_p48971789"></a><a name="zh-cn_topic_0118922243_p48971789"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922243_row38092920"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922243_p65627705"><a name="zh-cn_topic_0118922243_p65627705"></a><a name="zh-cn_topic_0118922243_p65627705"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922243_p14243927"><a name="zh-cn_topic_0118922243_p14243927"></a><a name="zh-cn_topic_0118922243_p14243927"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922243_p12907449"><a name="zh-cn_topic_0118922243_p12907449"></a><a name="zh-cn_topic_0118922243_p12907449"></a>创建环境时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922243_p38870472"><a name="zh-cn_topic_0118922243_p38870472"></a><a name="zh-cn_topic_0118922243_p38870472"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922243_p61500523"><a name="zh-cn_topic_0118922243_p61500523"></a><a name="zh-cn_topic_0118922243_p61500523"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922243_row16633800"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118922243_p5160549"><a name="zh-cn_topic_0118922243_p5160549"></a><a name="zh-cn_topic_0118922243_p5160549"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118922243_p15351306"><a name="zh-cn_topic_0118922243_p15351306"></a><a name="zh-cn_topic_0118922243_p15351306"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118922243_p35496288"><a name="zh-cn_topic_0118922243_p35496288"></a><a name="zh-cn_topic_0118922243_p35496288"></a>描述信息</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118922243_p56627086"><a name="zh-cn_topic_0118922243_p56627086"></a><a name="zh-cn_topic_0118922243_p56627086"></a>CUR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118922243_p23391293"><a name="zh-cn_topic_0118922243_p23391293"></a><a name="zh-cn_topic_0118922243_p23391293"></a>否</p>
</td>
</tr>
</tbody>
</table>

