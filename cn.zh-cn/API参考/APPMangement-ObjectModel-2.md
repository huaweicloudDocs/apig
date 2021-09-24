# 对象模型<a name="ZH-CN_TOPIC_0000001081976099"></a>

本节介绍APP的对象模型，如下表所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  APP对象模型

<a name="zh-cn_topic_0118921757_table65094334"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921757_row66234065"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921757_p63359031"><a name="zh-cn_topic_0118921757_p63359031"></a><a name="zh-cn_topic_0118921757_p63359031"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921757_p31807923"><a name="zh-cn_topic_0118921757_p31807923"></a><a name="zh-cn_topic_0118921757_p31807923"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921757_p26304938"><a name="zh-cn_topic_0118921757_p26304938"></a><a name="zh-cn_topic_0118921757_p26304938"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921757_p50325254"><a name="zh-cn_topic_0118921757_p50325254"></a><a name="zh-cn_topic_0118921757_p50325254"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921757_p49813807"><a name="zh-cn_topic_0118921757_p49813807"></a><a name="zh-cn_topic_0118921757_p49813807"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921757_row8386572"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p8223750"><a name="zh-cn_topic_0118921757_p8223750"></a><a name="zh-cn_topic_0118921757_p8223750"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p62144004"><a name="zh-cn_topic_0118921757_p62144004"></a><a name="zh-cn_topic_0118921757_p62144004"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p499567"><a name="zh-cn_topic_0118921757_p499567"></a><a name="zh-cn_topic_0118921757_p499567"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p40464942"><a name="zh-cn_topic_0118921757_p40464942"></a><a name="zh-cn_topic_0118921757_p40464942"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p56434858"><a name="zh-cn_topic_0118921757_p56434858"></a><a name="zh-cn_topic_0118921757_p56434858"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row38151674"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p3277851"><a name="zh-cn_topic_0118921757_p3277851"></a><a name="zh-cn_topic_0118921757_p3277851"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p64179373"><a name="zh-cn_topic_0118921757_p64179373"></a><a name="zh-cn_topic_0118921757_p64179373"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p31146711"><a name="zh-cn_topic_0118921757_p31146711"></a><a name="zh-cn_topic_0118921757_p31146711"></a>名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p39855682"><a name="zh-cn_topic_0118921757_p39855682"></a><a name="zh-cn_topic_0118921757_p39855682"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p7084822"><a name="zh-cn_topic_0118921757_p7084822"></a><a name="zh-cn_topic_0118921757_p7084822"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row63763398"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p64561609"><a name="zh-cn_topic_0118921757_p64561609"></a><a name="zh-cn_topic_0118921757_p64561609"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p62107849"><a name="zh-cn_topic_0118921757_p62107849"></a><a name="zh-cn_topic_0118921757_p62107849"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p64679853"><a name="zh-cn_topic_0118921757_p64679853"></a><a name="zh-cn_topic_0118921757_p64679853"></a>状态：</p>
<a name="zh-cn_topic_0118921757_ul45247768"></a><a name="zh-cn_topic_0118921757_ul45247768"></a><ul id="zh-cn_topic_0118921757_ul45247768"><li>1：启用</li><li>2：禁用</li><li>3：已删除</li></ul>
<p id="zh-cn_topic_0118921757_p48104796"><a name="zh-cn_topic_0118921757_p48104796"></a><a name="zh-cn_topic_0118921757_p48104796"></a>默认1</p>
<p id="zh-cn_topic_0118921757_p30289988"><a name="zh-cn_topic_0118921757_p30289988"></a><a name="zh-cn_topic_0118921757_p30289988"></a><strong id="zh-cn_topic_0118921757_b4174443"><a name="zh-cn_topic_0118921757_b4174443"></a><a name="zh-cn_topic_0118921757_b4174443"></a>该字段已废弃</strong></p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p2585635"><a name="zh-cn_topic_0118921757_p2585635"></a><a name="zh-cn_topic_0118921757_p2585635"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p8109867"><a name="zh-cn_topic_0118921757_p8109867"></a><a name="zh-cn_topic_0118921757_p8109867"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row5879940"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p6513160"><a name="zh-cn_topic_0118921757_p6513160"></a><a name="zh-cn_topic_0118921757_p6513160"></a>appkey</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p57803952"><a name="zh-cn_topic_0118921757_p57803952"></a><a name="zh-cn_topic_0118921757_p57803952"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p51608549"><a name="zh-cn_topic_0118921757_p51608549"></a><a name="zh-cn_topic_0118921757_p51608549"></a>APP的key，全局唯一</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p19542926"><a name="zh-cn_topic_0118921757_p19542926"></a><a name="zh-cn_topic_0118921757_p19542926"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p39473172"><a name="zh-cn_topic_0118921757_p39473172"></a><a name="zh-cn_topic_0118921757_p39473172"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row19714229"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p53348688"><a name="zh-cn_topic_0118921757_p53348688"></a><a name="zh-cn_topic_0118921757_p53348688"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p26276476"><a name="zh-cn_topic_0118921757_p26276476"></a><a name="zh-cn_topic_0118921757_p26276476"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p48019808"><a name="zh-cn_topic_0118921757_p48019808"></a><a name="zh-cn_topic_0118921757_p48019808"></a>密钥</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p64399269"><a name="zh-cn_topic_0118921757_p64399269"></a><a name="zh-cn_topic_0118921757_p64399269"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p48958323"><a name="zh-cn_topic_0118921757_p48958323"></a><a name="zh-cn_topic_0118921757_p48958323"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row37971724"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p55810809"><a name="zh-cn_topic_0118921757_p55810809"></a><a name="zh-cn_topic_0118921757_p55810809"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p24381699"><a name="zh-cn_topic_0118921757_p24381699"></a><a name="zh-cn_topic_0118921757_p24381699"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p28760593"><a name="zh-cn_topic_0118921757_p28760593"></a><a name="zh-cn_topic_0118921757_p28760593"></a>APP所属租户编号，即APP的创建者</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p47906700"><a name="zh-cn_topic_0118921757_p47906700"></a><a name="zh-cn_topic_0118921757_p47906700"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p55237467"><a name="zh-cn_topic_0118921757_p55237467"></a><a name="zh-cn_topic_0118921757_p55237467"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row27375158"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p2795295"><a name="zh-cn_topic_0118921757_p2795295"></a><a name="zh-cn_topic_0118921757_p2795295"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p25092304"><a name="zh-cn_topic_0118921757_p25092304"></a><a name="zh-cn_topic_0118921757_p25092304"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p19210738"><a name="zh-cn_topic_0118921757_p19210738"></a><a name="zh-cn_topic_0118921757_p19210738"></a>描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p12565932"><a name="zh-cn_topic_0118921757_p12565932"></a><a name="zh-cn_topic_0118921757_p12565932"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p11207591"><a name="zh-cn_topic_0118921757_p11207591"></a><a name="zh-cn_topic_0118921757_p11207591"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row33759460"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p50161763"><a name="zh-cn_topic_0118921757_p50161763"></a><a name="zh-cn_topic_0118921757_p50161763"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p36570998"><a name="zh-cn_topic_0118921757_p36570998"></a><a name="zh-cn_topic_0118921757_p36570998"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p9460870"><a name="zh-cn_topic_0118921757_p9460870"></a><a name="zh-cn_topic_0118921757_p9460870"></a>注册时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p28132986"><a name="zh-cn_topic_0118921757_p28132986"></a><a name="zh-cn_topic_0118921757_p28132986"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p64179387"><a name="zh-cn_topic_0118921757_p64179387"></a><a name="zh-cn_topic_0118921757_p64179387"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921757_row40743571"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921757_p11894961"><a name="zh-cn_topic_0118921757_p11894961"></a><a name="zh-cn_topic_0118921757_p11894961"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921757_p23967824"><a name="zh-cn_topic_0118921757_p23967824"></a><a name="zh-cn_topic_0118921757_p23967824"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921757_p62345624"><a name="zh-cn_topic_0118921757_p62345624"></a><a name="zh-cn_topic_0118921757_p62345624"></a>更新时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921757_p16830768"><a name="zh-cn_topic_0118921757_p16830768"></a><a name="zh-cn_topic_0118921757_p16830768"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921757_p21114944"><a name="zh-cn_topic_0118921757_p21114944"></a><a name="zh-cn_topic_0118921757_p21114944"></a>-</p>
</td>
</tr>
</tbody>
</table>

