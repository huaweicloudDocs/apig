# 查询分组列表<a name="ZH-CN_TOPIC_0000001081837257"></a>

## 功能介绍<a name="zh-cn_topic_0118921490_section46949754"></a>

查询API分组列表。

如果是租户操作，则查询该租户下所有的分组；如果是管理员操作，则查询的是所有租户的分组。

## URI<a name="zh-cn_topic_0118921490_section19894605"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921490_table51530049"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921490_row67004532"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921490_p58658025"><a name="zh-cn_topic_0118921490_p58658025"></a><a name="zh-cn_topic_0118921490_p58658025"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921490_p53679570"><a name="zh-cn_topic_0118921490_p53679570"></a><a name="zh-cn_topic_0118921490_p53679570"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921490_row53077912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921490_p4343586"><a name="zh-cn_topic_0118921490_p4343586"></a><a name="zh-cn_topic_0118921490_p4343586"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921490_p16286168"><a name="zh-cn_topic_0118921490_p16286168"></a><a name="zh-cn_topic_0118921490_p16286168"></a>/v1.0/apigw/api-groups[?page_size, page_no, id, name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、name、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921490_table40608407"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921490_row2467029"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921490_p65611664"><a name="zh-cn_topic_0118921490_p65611664"></a><a name="zh-cn_topic_0118921490_p65611664"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921490_p12944543"><a name="zh-cn_topic_0118921490_p12944543"></a><a name="zh-cn_topic_0118921490_p12944543"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921490_p41875051"><a name="zh-cn_topic_0118921490_p41875051"></a><a name="zh-cn_topic_0118921490_p41875051"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921490_p36435931"><a name="zh-cn_topic_0118921490_p36435931"></a><a name="zh-cn_topic_0118921490_p36435931"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921490_row65629271"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921490_p14370760"><a name="zh-cn_topic_0118921490_p14370760"></a><a name="zh-cn_topic_0118921490_p14370760"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921490_p23180950"><a name="zh-cn_topic_0118921490_p23180950"></a><a name="zh-cn_topic_0118921490_p23180950"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921490_p65717672"><a name="zh-cn_topic_0118921490_p65717672"></a><a name="zh-cn_topic_0118921490_p65717672"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921490_p21531239"><a name="zh-cn_topic_0118921490_p21531239"></a><a name="zh-cn_topic_0118921490_p21531239"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row59563426"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921490_p59908239"><a name="zh-cn_topic_0118921490_p59908239"></a><a name="zh-cn_topic_0118921490_p59908239"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921490_p20729180"><a name="zh-cn_topic_0118921490_p20729180"></a><a name="zh-cn_topic_0118921490_p20729180"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921490_p1342001"><a name="zh-cn_topic_0118921490_p1342001"></a><a name="zh-cn_topic_0118921490_p1342001"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921490_p41593271"><a name="zh-cn_topic_0118921490_p41593271"></a><a name="zh-cn_topic_0118921490_p41593271"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row8058788"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921490_p48782101"><a name="zh-cn_topic_0118921490_p48782101"></a><a name="zh-cn_topic_0118921490_p48782101"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921490_p59036110"><a name="zh-cn_topic_0118921490_p59036110"></a><a name="zh-cn_topic_0118921490_p59036110"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921490_p17195640"><a name="zh-cn_topic_0118921490_p17195640"></a><a name="zh-cn_topic_0118921490_p17195640"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921490_p50669627"><a name="zh-cn_topic_0118921490_p50669627"></a><a name="zh-cn_topic_0118921490_p50669627"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row53373461"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921490_p28283055"><a name="zh-cn_topic_0118921490_p28283055"></a><a name="zh-cn_topic_0118921490_p28283055"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921490_p9226101"><a name="zh-cn_topic_0118921490_p9226101"></a><a name="zh-cn_topic_0118921490_p9226101"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921490_p9116753"><a name="zh-cn_topic_0118921490_p9116753"></a><a name="zh-cn_topic_0118921490_p9116753"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921490_p259496"><a name="zh-cn_topic_0118921490_p259496"></a><a name="zh-cn_topic_0118921490_p259496"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row14184336124518"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921490_p7186103615458"><a name="zh-cn_topic_0118921490_p7186103615458"></a><a name="zh-cn_topic_0118921490_p7186103615458"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921490_p6186163619453"><a name="zh-cn_topic_0118921490_p6186163619453"></a><a name="zh-cn_topic_0118921490_p6186163619453"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921490_p61861736164517"><a name="zh-cn_topic_0118921490_p61861736164517"></a><a name="zh-cn_topic_0118921490_p61861736164517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921490_p12186203617455"><a name="zh-cn_topic_0118921490_p12186203617455"></a><a name="zh-cn_topic_0118921490_p12186203617455"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921490_section44833719"></a>

无

## 响应消息<a name="zh-cn_topic_0118921490_section7652604"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921490_table37289116"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921490_row8457713"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921490_p13986137"><a name="zh-cn_topic_0118921490_p13986137"></a><a name="zh-cn_topic_0118921490_p13986137"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921490_p59135289"><a name="zh-cn_topic_0118921490_p59135289"></a><a name="zh-cn_topic_0118921490_p59135289"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921490_p25229114"><a name="zh-cn_topic_0118921490_p25229114"></a><a name="zh-cn_topic_0118921490_p25229114"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921490_row30292355"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p37761725"><a name="zh-cn_topic_0118921490_p37761725"></a><a name="zh-cn_topic_0118921490_p37761725"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p38800912"><a name="zh-cn_topic_0118921490_p38800912"></a><a name="zh-cn_topic_0118921490_p38800912"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p55866147"><a name="zh-cn_topic_0118921490_p55866147"></a><a name="zh-cn_topic_0118921490_p55866147"></a>满足条件的分组总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row33033276"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p58449682"><a name="zh-cn_topic_0118921490_p58449682"></a><a name="zh-cn_topic_0118921490_p58449682"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p36803838"><a name="zh-cn_topic_0118921490_p36803838"></a><a name="zh-cn_topic_0118921490_p36803838"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p28320869"><a name="zh-cn_topic_0118921490_p28320869"></a><a name="zh-cn_topic_0118921490_p28320869"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row53561235"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p43492801"><a name="zh-cn_topic_0118921490_p43492801"></a><a name="zh-cn_topic_0118921490_p43492801"></a>groups</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p33255967"><a name="zh-cn_topic_0118921490_p33255967"></a><a name="zh-cn_topic_0118921490_p33255967"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p9378773"><a name="zh-cn_topic_0118921490_p9378773"></a><a name="zh-cn_topic_0118921490_p9378773"></a>分组列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  字典数据类型：分组字段说明

<a name="zh-cn_topic_0118921490_table17300097"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921490_row63268036"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921490_p24437261"><a name="zh-cn_topic_0118921490_p24437261"></a><a name="zh-cn_topic_0118921490_p24437261"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921490_p33261086"><a name="zh-cn_topic_0118921490_p33261086"></a><a name="zh-cn_topic_0118921490_p33261086"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921490_p9793440"><a name="zh-cn_topic_0118921490_p9793440"></a><a name="zh-cn_topic_0118921490_p9793440"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921490_row55071162"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p31579157"><a name="zh-cn_topic_0118921490_p31579157"></a><a name="zh-cn_topic_0118921490_p31579157"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p7774937"><a name="zh-cn_topic_0118921490_p7774937"></a><a name="zh-cn_topic_0118921490_p7774937"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p25790124"><a name="zh-cn_topic_0118921490_p25790124"></a><a name="zh-cn_topic_0118921490_p25790124"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row30784532"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p10519172"><a name="zh-cn_topic_0118921490_p10519172"></a><a name="zh-cn_topic_0118921490_p10519172"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p46746584"><a name="zh-cn_topic_0118921490_p46746584"></a><a name="zh-cn_topic_0118921490_p46746584"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p28376953"><a name="zh-cn_topic_0118921490_p28376953"></a><a name="zh-cn_topic_0118921490_p28376953"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row54065985"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p17268671"><a name="zh-cn_topic_0118921490_p17268671"></a><a name="zh-cn_topic_0118921490_p17268671"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p56585150"><a name="zh-cn_topic_0118921490_p56585150"></a><a name="zh-cn_topic_0118921490_p56585150"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p19994470"><a name="zh-cn_topic_0118921490_p19994470"></a><a name="zh-cn_topic_0118921490_p19994470"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row45732504"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p13345359"><a name="zh-cn_topic_0118921490_p13345359"></a><a name="zh-cn_topic_0118921490_p13345359"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p7232323"><a name="zh-cn_topic_0118921490_p7232323"></a><a name="zh-cn_topic_0118921490_p7232323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p48947291"><a name="zh-cn_topic_0118921490_p48947291"></a><a name="zh-cn_topic_0118921490_p48947291"></a>系统默认分配的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row65061826132915"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p18800341297"><a name="zh-cn_topic_0118921490_p18800341297"></a><a name="zh-cn_topic_0118921490_p18800341297"></a>sl_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p18242153613292"><a name="zh-cn_topic_0118921490_p18242153613292"></a><a name="zh-cn_topic_0118921490_p18242153613292"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p11203441112920"><a name="zh-cn_topic_0118921490_p11203441112920"></a><a name="zh-cn_topic_0118921490_p11203441112920"></a>系统默认分配的子域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row37872440"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p47768834"><a name="zh-cn_topic_0118921490_p47768834"></a><a name="zh-cn_topic_0118921490_p47768834"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p44070373"><a name="zh-cn_topic_0118921490_p44070373"></a><a name="zh-cn_topic_0118921490_p44070373"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p12930440"><a name="zh-cn_topic_0118921490_p12930440"></a><a name="zh-cn_topic_0118921490_p12930440"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row49265097"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p31049903"><a name="zh-cn_topic_0118921490_p31049903"></a><a name="zh-cn_topic_0118921490_p31049903"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p32014251"><a name="zh-cn_topic_0118921490_p32014251"></a><a name="zh-cn_topic_0118921490_p32014251"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p43017506"><a name="zh-cn_topic_0118921490_p43017506"></a><a name="zh-cn_topic_0118921490_p43017506"></a>最近修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row51613240"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p19922934"><a name="zh-cn_topic_0118921490_p19922934"></a><a name="zh-cn_topic_0118921490_p19922934"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p3144932"><a name="zh-cn_topic_0118921490_p3144932"></a><a name="zh-cn_topic_0118921490_p3144932"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p53412906"><a name="zh-cn_topic_0118921490_p53412906"></a><a name="zh-cn_topic_0118921490_p53412906"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row3429462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p9350971"><a name="zh-cn_topic_0118921490_p9350971"></a><a name="zh-cn_topic_0118921490_p9350971"></a>on_sell_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p19231164"><a name="zh-cn_topic_0118921490_p19231164"></a><a name="zh-cn_topic_0118921490_p19231164"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p14220483"><a name="zh-cn_topic_0118921490_p14220483"></a><a name="zh-cn_topic_0118921490_p14220483"></a>是否已上架云市场：</p>
<a name="zh-cn_topic_0118921490_ul60875483"></a><a name="zh-cn_topic_0118921490_ul60875483"></a><ul id="zh-cn_topic_0118921490_ul60875483"><li>1：已上架</li><li>2：未上架</li><li>3：审核中</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row1880511716455"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p63758800"><a name="zh-cn_topic_0118921490_p63758800"></a><a name="zh-cn_topic_0118921490_p63758800"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p64189201"><a name="zh-cn_topic_0118921490_p64189201"></a><a name="zh-cn_topic_0118921490_p64189201"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p31942831"><a name="zh-cn_topic_0118921490_p31942831"></a><a name="zh-cn_topic_0118921490_p31942831"></a>流控时长内分组下的API的总访问次数限制，默认不限，请根据服务的负载能力自行设置</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row642312418454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p66657312"><a name="zh-cn_topic_0118921490_p66657312"></a><a name="zh-cn_topic_0118921490_p66657312"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p30533155"><a name="zh-cn_topic_0118921490_p30533155"></a><a name="zh-cn_topic_0118921490_p30533155"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p57266528"><a name="zh-cn_topic_0118921490_p57266528"></a><a name="zh-cn_topic_0118921490_p57266528"></a>流控时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row011851416459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p5585767"><a name="zh-cn_topic_0118921490_p5585767"></a><a name="zh-cn_topic_0118921490_p5585767"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p49793976"><a name="zh-cn_topic_0118921490_p49793976"></a><a name="zh-cn_topic_0118921490_p49793976"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p6780221"><a name="zh-cn_topic_0118921490_p6780221"></a><a name="zh-cn_topic_0118921490_p6780221"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row1134681118458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p43834197"><a name="zh-cn_topic_0118921490_p43834197"></a><a name="zh-cn_topic_0118921490_p43834197"></a>url_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p60909101"><a name="zh-cn_topic_0118921490_p60909101"></a><a name="zh-cn_topic_0118921490_p60909101"></a>Array of <a href="#zh-cn_topic_0118921490_table9811220">UrlDomainsResp</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p34690133"><a name="zh-cn_topic_0118921490_p34690133"></a><a name="zh-cn_topic_0118921490_p34690133"></a>分组上绑定的独立域名列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  UrlDomainsResp

<a name="zh-cn_topic_0118921490_table9811220"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921490_row18394177"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921490_p13533375"><a name="zh-cn_topic_0118921490_p13533375"></a><a name="zh-cn_topic_0118921490_p13533375"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921490_p22461630"><a name="zh-cn_topic_0118921490_p22461630"></a><a name="zh-cn_topic_0118921490_p22461630"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921490_p7452774"><a name="zh-cn_topic_0118921490_p7452774"></a><a name="zh-cn_topic_0118921490_p7452774"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921490_row66803806"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p42399182"><a name="zh-cn_topic_0118921490_p42399182"></a><a name="zh-cn_topic_0118921490_p42399182"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p11781727"><a name="zh-cn_topic_0118921490_p11781727"></a><a name="zh-cn_topic_0118921490_p11781727"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p14795832"><a name="zh-cn_topic_0118921490_p14795832"></a><a name="zh-cn_topic_0118921490_p14795832"></a>域名编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row66053632"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p48743961"><a name="zh-cn_topic_0118921490_p48743961"></a><a name="zh-cn_topic_0118921490_p48743961"></a>domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p55946767"><a name="zh-cn_topic_0118921490_p55946767"></a><a name="zh-cn_topic_0118921490_p55946767"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p35394249"><a name="zh-cn_topic_0118921490_p35394249"></a><a name="zh-cn_topic_0118921490_p35394249"></a>访问域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row50112787"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p32603951"><a name="zh-cn_topic_0118921490_p32603951"></a><a name="zh-cn_topic_0118921490_p32603951"></a>cname_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p23674371"><a name="zh-cn_topic_0118921490_p23674371"></a><a name="zh-cn_topic_0118921490_p23674371"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p38575928"><a name="zh-cn_topic_0118921490_p38575928"></a><a name="zh-cn_topic_0118921490_p38575928"></a>域名cname状态：</p>
<a name="zh-cn_topic_0118921490_ul11639038"></a><a name="zh-cn_topic_0118921490_ul11639038"></a><ul id="zh-cn_topic_0118921490_ul11639038"><li>1：未解析</li><li>2：解析中</li><li>3：解析成功</li><li>4：解析失败</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row11732266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p10789489"><a name="zh-cn_topic_0118921490_p10789489"></a><a name="zh-cn_topic_0118921490_p10789489"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p1533408"><a name="zh-cn_topic_0118921490_p1533408"></a><a name="zh-cn_topic_0118921490_p1533408"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p57097248"><a name="zh-cn_topic_0118921490_p57097248"></a><a name="zh-cn_topic_0118921490_p57097248"></a>SSL证书编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row967016619319"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921490_p667011623113"><a name="zh-cn_topic_0118921490_p667011623113"></a><a name="zh-cn_topic_0118921490_p667011623113"></a>ssl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921490_p967017623110"><a name="zh-cn_topic_0118921490_p967017623110"></a><a name="zh-cn_topic_0118921490_p967017623110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921490_p76701261314"><a name="zh-cn_topic_0118921490_p76701261314"></a><a name="zh-cn_topic_0118921490_p76701261314"></a>SSL证书名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"groups": [{
		"id": "02a8ab3c-b278-4de5-a096-852829671ae7",
		"name": "api_group_002",
		"status": 1,
		"sl_domain": "19e62eca-43d9-4ce2-a478-b3f48e67fb91.apigw.example.com",
                "sl_domains": ["19e62eca-43d9-4ce2-a478-b3f48e67fb91.apigw.example.com","19e62eca-43d9-4ce2-a478-b3f48e67fb91.apigw.example.cn"],
		"remark": "分组002",
		"register_time": "2017-12-28T11:57:35Z",
		"update_time": "2017-12-28T11:57:35Z",
		"on_sell_status": 2
	},
	{
		"id": "73c58022-f20d-495a-a188-85d718647f09",
		"name": "api_group_001",
		"status": 1,
		"sl_domain": "c4c230d1-a8f2-4816-b9df-09ac5989180c.apigw.example.com",
                "sl_domains": ["c4c230d1-a8f2-4816-b9df-09ac5989180c.apigw.example.com","c4c230d1-a8f2-4816-b9df-09ac5989180c.apigw.example.cn"],
		"remark": "分组001",
		"register_time": "2017-12-28T11:57:27Z",
		"update_time": "2017-12-28T11:57:27Z",
		"on_sell_status": 2
	}]
}
```

## 状态码<a name="zh-cn_topic_0118921490_section850289"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0118921490_table24836589"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921490_row45772199"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921490_p16560630"><a name="zh-cn_topic_0118921490_p16560630"></a><a name="zh-cn_topic_0118921490_p16560630"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921490_p66342678"><a name="zh-cn_topic_0118921490_p66342678"></a><a name="zh-cn_topic_0118921490_p66342678"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921490_row5047855"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921490_p6223080"><a name="zh-cn_topic_0118921490_p6223080"></a><a name="zh-cn_topic_0118921490_p6223080"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921490_p50988816"><a name="zh-cn_topic_0118921490_p50988816"></a><a name="zh-cn_topic_0118921490_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row40331444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921490_p45621557"><a name="zh-cn_topic_0118921490_p45621557"></a><a name="zh-cn_topic_0118921490_p45621557"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921490_p18594143614553"><a name="zh-cn_topic_0118921490_p18594143614553"></a><a name="zh-cn_topic_0118921490_p18594143614553"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row39228080"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921490_p23357924"><a name="zh-cn_topic_0118921490_p23357924"></a><a name="zh-cn_topic_0118921490_p23357924"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921490_p9203142078"><a name="zh-cn_topic_0118921490_p9203142078"></a><a name="zh-cn_topic_0118921490_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921490_row49384039"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921490_p40684231"><a name="zh-cn_topic_0118921490_p40684231"></a><a name="zh-cn_topic_0118921490_p40684231"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921490_p14947689"><a name="zh-cn_topic_0118921490_p14947689"></a><a name="zh-cn_topic_0118921490_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

