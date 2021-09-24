# 对象模型<a name="ZH-CN_TOPIC_0000001081976135"></a>

管理系统的默认配置，管理员可以根据系统的实际运行情况对这些配置的值进行修改。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  系统配置对象模型

<a name="zh-cn_topic_0118924527_table61320436"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924527_row48730629"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924527_p54866914"><a name="zh-cn_topic_0118924527_p54866914"></a><a name="zh-cn_topic_0118924527_p54866914"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924527_p15035039"><a name="zh-cn_topic_0118924527_p15035039"></a><a name="zh-cn_topic_0118924527_p15035039"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924527_p9878628"><a name="zh-cn_topic_0118924527_p9878628"></a><a name="zh-cn_topic_0118924527_p9878628"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924527_p61971418"><a name="zh-cn_topic_0118924527_p61971418"></a><a name="zh-cn_topic_0118924527_p61971418"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924527_p53628968"><a name="zh-cn_topic_0118924527_p53628968"></a><a name="zh-cn_topic_0118924527_p53628968"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924527_row48979191"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p7891567"><a name="zh-cn_topic_0118924527_p7891567"></a><a name="zh-cn_topic_0118924527_p7891567"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p35237175"><a name="zh-cn_topic_0118924527_p35237175"></a><a name="zh-cn_topic_0118924527_p35237175"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p35638903"><a name="zh-cn_topic_0118924527_p35638903"></a><a name="zh-cn_topic_0118924527_p35638903"></a>配置项的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p1070040"><a name="zh-cn_topic_0118924527_p1070040"></a><a name="zh-cn_topic_0118924527_p1070040"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p19564417"><a name="zh-cn_topic_0118924527_p19564417"></a><a name="zh-cn_topic_0118924527_p19564417"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row41862033"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p35381498"><a name="zh-cn_topic_0118924527_p35381498"></a><a name="zh-cn_topic_0118924527_p35381498"></a>module_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p47329088"><a name="zh-cn_topic_0118924527_p47329088"></a><a name="zh-cn_topic_0118924527_p47329088"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p8450890"><a name="zh-cn_topic_0118924527_p8450890"></a><a name="zh-cn_topic_0118924527_p8450890"></a>配置项所属的模块名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p13433472"><a name="zh-cn_topic_0118924527_p13433472"></a><a name="zh-cn_topic_0118924527_p13433472"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p14369484"><a name="zh-cn_topic_0118924527_p14369484"></a><a name="zh-cn_topic_0118924527_p14369484"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row62216492"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p6371121"><a name="zh-cn_topic_0118924527_p6371121"></a><a name="zh-cn_topic_0118924527_p6371121"></a>config_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p46298815"><a name="zh-cn_topic_0118924527_p46298815"></a><a name="zh-cn_topic_0118924527_p46298815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p59216509"><a name="zh-cn_topic_0118924527_p59216509"></a><a name="zh-cn_topic_0118924527_p59216509"></a>配置项的名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p31807891"><a name="zh-cn_topic_0118924527_p31807891"></a><a name="zh-cn_topic_0118924527_p31807891"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p26302378"><a name="zh-cn_topic_0118924527_p26302378"></a><a name="zh-cn_topic_0118924527_p26302378"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row35394813"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p48407608"><a name="zh-cn_topic_0118924527_p48407608"></a><a name="zh-cn_topic_0118924527_p48407608"></a>config_value</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p28702151"><a name="zh-cn_topic_0118924527_p28702151"></a><a name="zh-cn_topic_0118924527_p28702151"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p43172883"><a name="zh-cn_topic_0118924527_p43172883"></a><a name="zh-cn_topic_0118924527_p43172883"></a>配置项的值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p7342595"><a name="zh-cn_topic_0118924527_p7342595"></a><a name="zh-cn_topic_0118924527_p7342595"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p57879295"><a name="zh-cn_topic_0118924527_p57879295"></a><a name="zh-cn_topic_0118924527_p57879295"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row51151614"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p49640056"><a name="zh-cn_topic_0118924527_p49640056"></a><a name="zh-cn_topic_0118924527_p49640056"></a>can_special</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p61421619"><a name="zh-cn_topic_0118924527_p61421619"></a><a name="zh-cn_topic_0118924527_p61421619"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p9095255"><a name="zh-cn_topic_0118924527_p9095255"></a><a name="zh-cn_topic_0118924527_p9095255"></a>是否支持特殊配置</p>
<a name="zh-cn_topic_0118924527_ul14748431"></a><a name="zh-cn_topic_0118924527_ul14748431"></a><ul id="zh-cn_topic_0118924527_ul14748431"><li>1:  支持特殊配置</li><li>2：不支持特殊配置</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p60585650"><a name="zh-cn_topic_0118924527_p60585650"></a><a name="zh-cn_topic_0118924527_p60585650"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p8490598"><a name="zh-cn_topic_0118924527_p8490598"></a><a name="zh-cn_topic_0118924527_p8490598"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row9306521"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p15630751"><a name="zh-cn_topic_0118924527_p15630751"></a><a name="zh-cn_topic_0118924527_p15630751"></a>remarks</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p58131325"><a name="zh-cn_topic_0118924527_p58131325"></a><a name="zh-cn_topic_0118924527_p58131325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p11016924"><a name="zh-cn_topic_0118924527_p11016924"></a><a name="zh-cn_topic_0118924527_p11016924"></a>对配置项的描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p19955684"><a name="zh-cn_topic_0118924527_p19955684"></a><a name="zh-cn_topic_0118924527_p19955684"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p5797692"><a name="zh-cn_topic_0118924527_p5797692"></a><a name="zh-cn_topic_0118924527_p5797692"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row52179229"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p65768049"><a name="zh-cn_topic_0118924527_p65768049"></a><a name="zh-cn_topic_0118924527_p65768049"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p25611753"><a name="zh-cn_topic_0118924527_p25611753"></a><a name="zh-cn_topic_0118924527_p25611753"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p61286126"><a name="zh-cn_topic_0118924527_p61286126"></a><a name="zh-cn_topic_0118924527_p61286126"></a>更新时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p65229159"><a name="zh-cn_topic_0118924527_p65229159"></a><a name="zh-cn_topic_0118924527_p65229159"></a>RU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p49070525"><a name="zh-cn_topic_0118924527_p49070525"></a><a name="zh-cn_topic_0118924527_p49070525"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row38981542"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p3388305"><a name="zh-cn_topic_0118924527_p3388305"></a><a name="zh-cn_topic_0118924527_p3388305"></a>match_regexp</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p6017293"><a name="zh-cn_topic_0118924527_p6017293"></a><a name="zh-cn_topic_0118924527_p6017293"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p17638721"><a name="zh-cn_topic_0118924527_p17638721"></a><a name="zh-cn_topic_0118924527_p17638721"></a>配置项的值应该满足的规则</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p19450326"><a name="zh-cn_topic_0118924527_p19450326"></a><a name="zh-cn_topic_0118924527_p19450326"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p31972596"><a name="zh-cn_topic_0118924527_p31972596"></a><a name="zh-cn_topic_0118924527_p31972596"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924527_row19317909"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924527_p21246802"><a name="zh-cn_topic_0118924527_p21246802"></a><a name="zh-cn_topic_0118924527_p21246802"></a>encrypt_flag</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924527_p43269420"><a name="zh-cn_topic_0118924527_p43269420"></a><a name="zh-cn_topic_0118924527_p43269420"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924527_p15162122"><a name="zh-cn_topic_0118924527_p15162122"></a><a name="zh-cn_topic_0118924527_p15162122"></a>config_value字段是否加密</p>
<a name="zh-cn_topic_0118924527_ul2241374"></a><a name="zh-cn_topic_0118924527_ul2241374"></a><ul id="zh-cn_topic_0118924527_ul2241374"><li>1：加密</li><li>2：不加密</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924527_p8818839"><a name="zh-cn_topic_0118924527_p8818839"></a><a name="zh-cn_topic_0118924527_p8818839"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924527_p43237328"><a name="zh-cn_topic_0118924527_p43237328"></a><a name="zh-cn_topic_0118924527_p43237328"></a>-</p>
</td>
</tr>
</tbody>
</table>

