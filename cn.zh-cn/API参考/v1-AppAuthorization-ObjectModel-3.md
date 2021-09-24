# 对象模型<a name="ZH-CN_TOPIC_0000001082135175"></a>

本节介绍APP与API之间的授权关系的对象模型，如下表所示。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  APP授权关系对象模型

<a name="zh-cn_topic_0225568841_table33491166"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568841_row43749103"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0225568841_p54016492"><a name="zh-cn_topic_0225568841_p54016492"></a><a name="zh-cn_topic_0225568841_p54016492"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0225568841_p13259721"><a name="zh-cn_topic_0225568841_p13259721"></a><a name="zh-cn_topic_0225568841_p13259721"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0225568841_p295598"><a name="zh-cn_topic_0225568841_p295598"></a><a name="zh-cn_topic_0225568841_p295598"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0225568841_p23943492"><a name="zh-cn_topic_0225568841_p23943492"></a><a name="zh-cn_topic_0225568841_p23943492"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0225568841_p60374706"><a name="zh-cn_topic_0225568841_p60374706"></a><a name="zh-cn_topic_0225568841_p60374706"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568841_row58513057"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568841_p41937209"><a name="zh-cn_topic_0225568841_p41937209"></a><a name="zh-cn_topic_0225568841_p41937209"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568841_p41470753"><a name="zh-cn_topic_0225568841_p41470753"></a><a name="zh-cn_topic_0225568841_p41470753"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568841_p3687809"><a name="zh-cn_topic_0225568841_p3687809"></a><a name="zh-cn_topic_0225568841_p3687809"></a>授权关系的ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568841_p30277122"><a name="zh-cn_topic_0225568841_p30277122"></a><a name="zh-cn_topic_0225568841_p30277122"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568841_p36527819"><a name="zh-cn_topic_0225568841_p36527819"></a><a name="zh-cn_topic_0225568841_p36527819"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568841_row60314923"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568841_p53670580"><a name="zh-cn_topic_0225568841_p53670580"></a><a name="zh-cn_topic_0225568841_p53670580"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568841_p52349722"><a name="zh-cn_topic_0225568841_p52349722"></a><a name="zh-cn_topic_0225568841_p52349722"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568841_p12469060"><a name="zh-cn_topic_0225568841_p12469060"></a><a name="zh-cn_topic_0225568841_p12469060"></a>APP的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568841_p3360922"><a name="zh-cn_topic_0225568841_p3360922"></a><a name="zh-cn_topic_0225568841_p3360922"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568841_p3799302"><a name="zh-cn_topic_0225568841_p3799302"></a><a name="zh-cn_topic_0225568841_p3799302"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568841_row34193718"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568841_p18227803"><a name="zh-cn_topic_0225568841_p18227803"></a><a name="zh-cn_topic_0225568841_p18227803"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568841_p57097"><a name="zh-cn_topic_0225568841_p57097"></a><a name="zh-cn_topic_0225568841_p57097"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568841_p4624871"><a name="zh-cn_topic_0225568841_p4624871"></a><a name="zh-cn_topic_0225568841_p4624871"></a>api的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568841_p39070237"><a name="zh-cn_topic_0225568841_p39070237"></a><a name="zh-cn_topic_0225568841_p39070237"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568841_p10572628"><a name="zh-cn_topic_0225568841_p10572628"></a><a name="zh-cn_topic_0225568841_p10572628"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568841_row28044791"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568841_p57035602"><a name="zh-cn_topic_0225568841_p57035602"></a><a name="zh-cn_topic_0225568841_p57035602"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568841_p56481025"><a name="zh-cn_topic_0225568841_p56481025"></a><a name="zh-cn_topic_0225568841_p56481025"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568841_p11560301"><a name="zh-cn_topic_0225568841_p11560301"></a><a name="zh-cn_topic_0225568841_p11560301"></a>环境编号（发布环境）</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568841_p63969149"><a name="zh-cn_topic_0225568841_p63969149"></a><a name="zh-cn_topic_0225568841_p63969149"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568841_p14118553"><a name="zh-cn_topic_0225568841_p14118553"></a><a name="zh-cn_topic_0225568841_p14118553"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568841_row59958120"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568841_p24769538"><a name="zh-cn_topic_0225568841_p24769538"></a><a name="zh-cn_topic_0225568841_p24769538"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568841_p60175581"><a name="zh-cn_topic_0225568841_p60175581"></a><a name="zh-cn_topic_0225568841_p60175581"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568841_p42383905"><a name="zh-cn_topic_0225568841_p42383905"></a><a name="zh-cn_topic_0225568841_p42383905"></a>授权时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568841_p10544244"><a name="zh-cn_topic_0225568841_p10544244"></a><a name="zh-cn_topic_0225568841_p10544244"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568841_p48777473"><a name="zh-cn_topic_0225568841_p48777473"></a><a name="zh-cn_topic_0225568841_p48777473"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568841_row36344076"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568841_p58189024"><a name="zh-cn_topic_0225568841_p58189024"></a><a name="zh-cn_topic_0225568841_p58189024"></a>auth_role</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568841_p15690497"><a name="zh-cn_topic_0225568841_p15690497"></a><a name="zh-cn_topic_0225568841_p15690497"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568841_p62970710"><a name="zh-cn_topic_0225568841_p62970710"></a><a name="zh-cn_topic_0225568841_p62970710"></a>授权者</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568841_p353863"><a name="zh-cn_topic_0225568841_p353863"></a><a name="zh-cn_topic_0225568841_p353863"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568841_p28662974"><a name="zh-cn_topic_0225568841_p28662974"></a><a name="zh-cn_topic_0225568841_p28662974"></a>-</p>
</td>
</tr>
</tbody>
</table>

