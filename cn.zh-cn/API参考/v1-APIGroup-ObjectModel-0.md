# 对象模型<a name="ZH-CN_TOPIC_0000001082135157"></a>

本节介绍API分组的对象模型，如下表所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  分组对象模型

<a name="zh-cn_topic_0225568805_table19700793"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568805_row8739679"><th class="cellrowborder" valign="top" width="20.407959204079592%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0225568805_p36825378"><a name="zh-cn_topic_0225568805_p36825378"></a><a name="zh-cn_topic_0225568805_p36825378"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.328367163283673%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0225568805_p30065613"><a name="zh-cn_topic_0225568805_p30065613"></a><a name="zh-cn_topic_0225568805_p30065613"></a>数据类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.66663333666634%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0225568805_p19395593"><a name="zh-cn_topic_0225568805_p19395593"></a><a name="zh-cn_topic_0225568805_p19395593"></a>参数说明</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885711%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0225568805_p27539197"><a name="zh-cn_topic_0225568805_p27539197"></a><a name="zh-cn_topic_0225568805_p27539197"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0225568805_p16082514"><a name="zh-cn_topic_0225568805_p16082514"></a><a name="zh-cn_topic_0225568805_p16082514"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568805_row27615280"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p22245182"><a name="zh-cn_topic_0225568805_p22245182"></a><a name="zh-cn_topic_0225568805_p22245182"></a>ID</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p57029284"><a name="zh-cn_topic_0225568805_p57029284"></a><a name="zh-cn_topic_0225568805_p57029284"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p55969291"><a name="zh-cn_topic_0225568805_p55969291"></a><a name="zh-cn_topic_0225568805_p55969291"></a>API分组编号</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p37218714"><a name="zh-cn_topic_0225568805_p37218714"></a><a name="zh-cn_topic_0225568805_p37218714"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p61925882"><a name="zh-cn_topic_0225568805_p61925882"></a><a name="zh-cn_topic_0225568805_p61925882"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row20462032"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p46811884"><a name="zh-cn_topic_0225568805_p46811884"></a><a name="zh-cn_topic_0225568805_p46811884"></a>NAME</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p33666220"><a name="zh-cn_topic_0225568805_p33666220"></a><a name="zh-cn_topic_0225568805_p33666220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p42609272"><a name="zh-cn_topic_0225568805_p42609272"></a><a name="zh-cn_topic_0225568805_p42609272"></a>API分组名称</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p28799033"><a name="zh-cn_topic_0225568805_p28799033"></a><a name="zh-cn_topic_0225568805_p28799033"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p51020375"><a name="zh-cn_topic_0225568805_p51020375"></a><a name="zh-cn_topic_0225568805_p51020375"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row56530196"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p15543176"><a name="zh-cn_topic_0225568805_p15543176"></a><a name="zh-cn_topic_0225568805_p15543176"></a>STATUS</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p51037707"><a name="zh-cn_topic_0225568805_p51037707"></a><a name="zh-cn_topic_0225568805_p51037707"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p40413640"><a name="zh-cn_topic_0225568805_p40413640"></a><a name="zh-cn_topic_0225568805_p40413640"></a>API分组状态</p>
<a name="zh-cn_topic_0225568805_ul53721145134416"></a><a name="zh-cn_topic_0225568805_ul53721145134416"></a><ul id="zh-cn_topic_0225568805_ul53721145134416"><li>1 正常状态</li><li>2 禁用状态</li><li>3 已删除</li></ul>
<p id="zh-cn_topic_0225568805_p6772746"><a name="zh-cn_topic_0225568805_p6772746"></a><a name="zh-cn_topic_0225568805_p6772746"></a>默认值1</p>
<p id="zh-cn_topic_0225568805_p60954720"><a name="zh-cn_topic_0225568805_p60954720"></a><a name="zh-cn_topic_0225568805_p60954720"></a><strong id="zh-cn_topic_0225568805_b11721568"><a name="zh-cn_topic_0225568805_b11721568"></a><a name="zh-cn_topic_0225568805_b11721568"></a>该字段暂时废弃</strong></p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p9922958"><a name="zh-cn_topic_0225568805_p9922958"></a><a name="zh-cn_topic_0225568805_p9922958"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p65562173"><a name="zh-cn_topic_0225568805_p65562173"></a><a name="zh-cn_topic_0225568805_p65562173"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row53188653"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p13313599"><a name="zh-cn_topic_0225568805_p13313599"></a><a name="zh-cn_topic_0225568805_p13313599"></a>SL_DOMAIN</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p4659750"><a name="zh-cn_topic_0225568805_p4659750"></a><a name="zh-cn_topic_0225568805_p4659750"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p41895498"><a name="zh-cn_topic_0225568805_p41895498"></a><a name="zh-cn_topic_0225568805_p41895498"></a>API分组的子域名，由API网关分配，用户不可填写和修改</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p38092178"><a name="zh-cn_topic_0225568805_p38092178"></a><a name="zh-cn_topic_0225568805_p38092178"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p65567591"><a name="zh-cn_topic_0225568805_p65567591"></a><a name="zh-cn_topic_0225568805_p65567591"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row53237409"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p17262900"><a name="zh-cn_topic_0225568805_p17262900"></a><a name="zh-cn_topic_0225568805_p17262900"></a>PROJECT_ID</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p56117639"><a name="zh-cn_topic_0225568805_p56117639"></a><a name="zh-cn_topic_0225568805_p56117639"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p49234882"><a name="zh-cn_topic_0225568805_p49234882"></a><a name="zh-cn_topic_0225568805_p49234882"></a>创建该API分组的租户编号，即API分组的所有者</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p28602510"><a name="zh-cn_topic_0225568805_p28602510"></a><a name="zh-cn_topic_0225568805_p28602510"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p35101970"><a name="zh-cn_topic_0225568805_p35101970"></a><a name="zh-cn_topic_0225568805_p35101970"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row4491218298"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p1149618594"><a name="zh-cn_topic_0225568805_p1149618594"></a><a name="zh-cn_topic_0225568805_p1149618594"></a>DOMAIN_NAME</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p194931817917"><a name="zh-cn_topic_0225568805_p194931817917"></a><a name="zh-cn_topic_0225568805_p194931817917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p13497181298"><a name="zh-cn_topic_0225568805_p13497181298"></a><a name="zh-cn_topic_0225568805_p13497181298"></a>创建该API分组的租户名称</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 ">&nbsp;&nbsp;</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 ">&nbsp;&nbsp;</td>
</tr>
<tr id="zh-cn_topic_0225568805_row47482281"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p20859573"><a name="zh-cn_topic_0225568805_p20859573"></a><a name="zh-cn_topic_0225568805_p20859573"></a>REGISTER_TIME</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p11903886"><a name="zh-cn_topic_0225568805_p11903886"></a><a name="zh-cn_topic_0225568805_p11903886"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p24690715"><a name="zh-cn_topic_0225568805_p24690715"></a><a name="zh-cn_topic_0225568805_p24690715"></a>API分组创建时间，由系统默认生成</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p53790917"><a name="zh-cn_topic_0225568805_p53790917"></a><a name="zh-cn_topic_0225568805_p53790917"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p62097011"><a name="zh-cn_topic_0225568805_p62097011"></a><a name="zh-cn_topic_0225568805_p62097011"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row22002191"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p37347071"><a name="zh-cn_topic_0225568805_p37347071"></a><a name="zh-cn_topic_0225568805_p37347071"></a>UPDATE_TIME</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p5213928"><a name="zh-cn_topic_0225568805_p5213928"></a><a name="zh-cn_topic_0225568805_p5213928"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p19674993"><a name="zh-cn_topic_0225568805_p19674993"></a><a name="zh-cn_topic_0225568805_p19674993"></a>最近一次修改时间</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p50170562"><a name="zh-cn_topic_0225568805_p50170562"></a><a name="zh-cn_topic_0225568805_p50170562"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p37283716"><a name="zh-cn_topic_0225568805_p37283716"></a><a name="zh-cn_topic_0225568805_p37283716"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row9126"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p739284"><a name="zh-cn_topic_0225568805_p739284"></a><a name="zh-cn_topic_0225568805_p739284"></a>REMARK</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p59882054"><a name="zh-cn_topic_0225568805_p59882054"></a><a name="zh-cn_topic_0225568805_p59882054"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p18608229"><a name="zh-cn_topic_0225568805_p18608229"></a><a name="zh-cn_topic_0225568805_p18608229"></a>描述，简述该API分组的功能、作用等</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p30871576"><a name="zh-cn_topic_0225568805_p30871576"></a><a name="zh-cn_topic_0225568805_p30871576"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p17569736"><a name="zh-cn_topic_0225568805_p17569736"></a><a name="zh-cn_topic_0225568805_p17569736"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568805_row23909898"><td class="cellrowborder" valign="top" width="20.407959204079592%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568805_p57653567"><a name="zh-cn_topic_0225568805_p57653567"></a><a name="zh-cn_topic_0225568805_p57653567"></a>THROTTLE_ID</p>
</td>
<td class="cellrowborder" valign="top" width="16.328367163283673%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568805_p39427365"><a name="zh-cn_topic_0225568805_p39427365"></a><a name="zh-cn_topic_0225568805_p39427365"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.66663333666634%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568805_p39500003"><a name="zh-cn_topic_0225568805_p39500003"></a><a name="zh-cn_topic_0225568805_p39500003"></a>流控策略编号，限定该分组在一定时间内可以被访问的次数</p>
<div class="note" id="zh-cn_topic_0225568805_note20704858144716"><a name="zh-cn_topic_0225568805_note20704858144716"></a><a name="zh-cn_topic_0225568805_note20704858144716"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568805_p97048585476"><a name="zh-cn_topic_0225568805_p97048585476"></a><a name="zh-cn_topic_0225568805_p97048585476"></a>该字段表示该分组下的所有API单位时间内总共能够访问多少次，并非表示每个API单位时间内分别能够访问多少次。</p>
</div></div>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885711%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568805_p42431218"><a name="zh-cn_topic_0225568805_p42431218"></a><a name="zh-cn_topic_0225568805_p42431218"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568805_p14376643"><a name="zh-cn_topic_0225568805_p14376643"></a><a name="zh-cn_topic_0225568805_p14376643"></a>-</p>
</td>
</tr>
</tbody>
</table>

