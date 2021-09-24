# 查询自定义认证列表<a name="ZH-CN_TOPIC_0000001081837327"></a>

## 功能介绍<a name="zh-cn_topic_0221111191_section66524352"></a>

查询自定义认证列表

## URI<a name="zh-cn_topic_0221111191_section61848258"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0221111191_table27084002"></a>
<table><thead align="left"><tr id="zh-cn_topic_0221111191_row40355780"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0221111191_p47592766"><a name="zh-cn_topic_0221111191_p47592766"></a><a name="zh-cn_topic_0221111191_p47592766"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0221111191_p29808828"><a name="zh-cn_topic_0221111191_p29808828"></a><a name="zh-cn_topic_0221111191_p29808828"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0221111191_row65704871"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0221111191_p20494310"><a name="zh-cn_topic_0221111191_p20494310"></a><a name="zh-cn_topic_0221111191_p20494310"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0221111191_p49426402"><a name="zh-cn_topic_0221111191_p49426402"></a><a name="zh-cn_topic_0221111191_p49426402"></a>/v1.0/apigw/authorizers[?page_size, page_no, id, name, type]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、name、type、page\_size、page\_no

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0221111191_table40608407"></a>
<table><thead align="left"><tr id="zh-cn_topic_0221111191_row2467029"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0221111191_p65611664"><a name="zh-cn_topic_0221111191_p65611664"></a><a name="zh-cn_topic_0221111191_p65611664"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0221111191_p12944543"><a name="zh-cn_topic_0221111191_p12944543"></a><a name="zh-cn_topic_0221111191_p12944543"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0221111191_p41875051"><a name="zh-cn_topic_0221111191_p41875051"></a><a name="zh-cn_topic_0221111191_p41875051"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0221111191_p36435931"><a name="zh-cn_topic_0221111191_p36435931"></a><a name="zh-cn_topic_0221111191_p36435931"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0221111191_row65629271"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0221111191_p14370760"><a name="zh-cn_topic_0221111191_p14370760"></a><a name="zh-cn_topic_0221111191_p14370760"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0221111191_p23180950"><a name="zh-cn_topic_0221111191_p23180950"></a><a name="zh-cn_topic_0221111191_p23180950"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0221111191_p65717672"><a name="zh-cn_topic_0221111191_p65717672"></a><a name="zh-cn_topic_0221111191_p65717672"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0221111191_p21531239"><a name="zh-cn_topic_0221111191_p21531239"></a><a name="zh-cn_topic_0221111191_p21531239"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row59563426"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0221111191_p59908239"><a name="zh-cn_topic_0221111191_p59908239"></a><a name="zh-cn_topic_0221111191_p59908239"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0221111191_p20729180"><a name="zh-cn_topic_0221111191_p20729180"></a><a name="zh-cn_topic_0221111191_p20729180"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0221111191_p1342001"><a name="zh-cn_topic_0221111191_p1342001"></a><a name="zh-cn_topic_0221111191_p1342001"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0221111191_p41593271"><a name="zh-cn_topic_0221111191_p41593271"></a><a name="zh-cn_topic_0221111191_p41593271"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row1950610612123"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0221111191_p5507865123"><a name="zh-cn_topic_0221111191_p5507865123"></a><a name="zh-cn_topic_0221111191_p5507865123"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0221111191_p1657343911316"><a name="zh-cn_topic_0221111191_p1657343911316"></a><a name="zh-cn_topic_0221111191_p1657343911316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0221111191_p272194191318"><a name="zh-cn_topic_0221111191_p272194191318"></a><a name="zh-cn_topic_0221111191_p272194191318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0221111191_p8507116201218"><a name="zh-cn_topic_0221111191_p8507116201218"></a><a name="zh-cn_topic_0221111191_p8507116201218"></a>类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row8058788"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0221111191_p48782101"><a name="zh-cn_topic_0221111191_p48782101"></a><a name="zh-cn_topic_0221111191_p48782101"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0221111191_p59036110"><a name="zh-cn_topic_0221111191_p59036110"></a><a name="zh-cn_topic_0221111191_p59036110"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0221111191_p17195640"><a name="zh-cn_topic_0221111191_p17195640"></a><a name="zh-cn_topic_0221111191_p17195640"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0221111191_p50669627"><a name="zh-cn_topic_0221111191_p50669627"></a><a name="zh-cn_topic_0221111191_p50669627"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row53373461"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0221111191_p28283055"><a name="zh-cn_topic_0221111191_p28283055"></a><a name="zh-cn_topic_0221111191_p28283055"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0221111191_p9226101"><a name="zh-cn_topic_0221111191_p9226101"></a><a name="zh-cn_topic_0221111191_p9226101"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0221111191_p9116753"><a name="zh-cn_topic_0221111191_p9116753"></a><a name="zh-cn_topic_0221111191_p9116753"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0221111191_p259496"><a name="zh-cn_topic_0221111191_p259496"></a><a name="zh-cn_topic_0221111191_p259496"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0221111191_section19763417"></a>

无

## 响应消息<a name="zh-cn_topic_0221111191_section57332943"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0221111191_table37289116"></a>
<table><thead align="left"><tr id="zh-cn_topic_0221111191_row8457713"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0221111191_p13986137"><a name="zh-cn_topic_0221111191_p13986137"></a><a name="zh-cn_topic_0221111191_p13986137"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0221111191_p59135289"><a name="zh-cn_topic_0221111191_p59135289"></a><a name="zh-cn_topic_0221111191_p59135289"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0221111191_p25229114"><a name="zh-cn_topic_0221111191_p25229114"></a><a name="zh-cn_topic_0221111191_p25229114"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0221111191_row30292355"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p37761725"><a name="zh-cn_topic_0221111191_p37761725"></a><a name="zh-cn_topic_0221111191_p37761725"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p38800912"><a name="zh-cn_topic_0221111191_p38800912"></a><a name="zh-cn_topic_0221111191_p38800912"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p9238141511415"><a name="zh-cn_topic_0221111191_p9238141511415"></a><a name="zh-cn_topic_0221111191_p9238141511415"></a>满足条件的自定义认证总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row33033276"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p58449682"><a name="zh-cn_topic_0221111191_p58449682"></a><a name="zh-cn_topic_0221111191_p58449682"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p36803838"><a name="zh-cn_topic_0221111191_p36803838"></a><a name="zh-cn_topic_0221111191_p36803838"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p28320869"><a name="zh-cn_topic_0221111191_p28320869"></a><a name="zh-cn_topic_0221111191_p28320869"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row53561235"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p43492801"><a name="zh-cn_topic_0221111191_p43492801"></a><a name="zh-cn_topic_0221111191_p43492801"></a>authorizer_list</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p33255967"><a name="zh-cn_topic_0221111191_p33255967"></a><a name="zh-cn_topic_0221111191_p33255967"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p9378773"><a name="zh-cn_topic_0221111191_p9378773"></a><a name="zh-cn_topic_0221111191_p9378773"></a>自定义认证列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  authorizer\_list参数说明

<a name="zh-cn_topic_0221111191_table2803298"></a>
<table><thead align="left"><tr id="zh-cn_topic_0221111191_row9258659"><th class="cellrowborder" valign="top" width="20.02%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0221111191_p11753897"><a name="zh-cn_topic_0221111191_p11753897"></a><a name="zh-cn_topic_0221111191_p11753897"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.98%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0221111191_p12541637"><a name="zh-cn_topic_0221111191_p12541637"></a><a name="zh-cn_topic_0221111191_p12541637"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0221111191_p9239644"><a name="zh-cn_topic_0221111191_p9239644"></a><a name="zh-cn_topic_0221111191_p9239644"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0221111191_row10213720"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p22005025"><a name="zh-cn_topic_0221111191_p22005025"></a><a name="zh-cn_topic_0221111191_p22005025"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p37576606"><a name="zh-cn_topic_0221111191_p37576606"></a><a name="zh-cn_topic_0221111191_p37576606"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p23806264"><a name="zh-cn_topic_0221111191_p23806264"></a><a name="zh-cn_topic_0221111191_p23806264"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row12929787"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p40679818"><a name="zh-cn_topic_0221111191_p40679818"></a><a name="zh-cn_topic_0221111191_p40679818"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p6730986"><a name="zh-cn_topic_0221111191_p6730986"></a><a name="zh-cn_topic_0221111191_p6730986"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p4183116625"><a name="zh-cn_topic_0221111191_p4183116625"></a><a name="zh-cn_topic_0221111191_p4183116625"></a>自定义认证的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row7942236"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p078091916016"><a name="zh-cn_topic_0221111191_p078091916016"></a><a name="zh-cn_topic_0221111191_p078091916016"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p43191612927"><a name="zh-cn_topic_0221111191_p43191612927"></a><a name="zh-cn_topic_0221111191_p43191612927"></a></p>
<p id="zh-cn_topic_0221111191_p1131817121824"><a name="zh-cn_topic_0221111191_p1131817121824"></a><a name="zh-cn_topic_0221111191_p1131817121824"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p174157561811"><a name="zh-cn_topic_0221111191_p174157561811"></a><a name="zh-cn_topic_0221111191_p174157561811"></a>自定义认证类型：</p>
<a name="zh-cn_topic_0221111191_ul04151356316"></a><a name="zh-cn_topic_0221111191_ul04151356316"></a><ul id="zh-cn_topic_0221111191_ul04151356316"><li>FRONTEND：前端</li><li>BACKEND：后端</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row26358777"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p14730142317016"><a name="zh-cn_topic_0221111191_p14730142317016"></a><a name="zh-cn_topic_0221111191_p14730142317016"></a>authorizer_type</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p398200"><a name="zh-cn_topic_0221111191_p398200"></a><a name="zh-cn_topic_0221111191_p398200"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p10821651114"><a name="zh-cn_topic_0221111191_p10821651114"></a><a name="zh-cn_topic_0221111191_p10821651114"></a>只能为：FUNC</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row21852379"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p1530418271701"><a name="zh-cn_topic_0221111191_p1530418271701"></a><a name="zh-cn_topic_0221111191_p1530418271701"></a>authorizer_uri</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p36223141827"><a name="zh-cn_topic_0221111191_p36223141827"></a><a name="zh-cn_topic_0221111191_p36223141827"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p13462546519"><a name="zh-cn_topic_0221111191_p13462546519"></a><a name="zh-cn_topic_0221111191_p13462546519"></a>函数urn</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row17074768"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p1404467010"><a name="zh-cn_topic_0221111191_p1404467010"></a><a name="zh-cn_topic_0221111191_p1404467010"></a>identities</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p1289301726"><a name="zh-cn_topic_0221111191_p1289301726"></a><a name="zh-cn_topic_0221111191_p1289301726"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p3687421212"><a name="zh-cn_topic_0221111191_p3687421212"></a><a name="zh-cn_topic_0221111191_p3687421212"></a>认证来源</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row23864751"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p176566481901"><a name="zh-cn_topic_0221111191_p176566481901"></a><a name="zh-cn_topic_0221111191_p176566481901"></a>ttl</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p2566123613220"><a name="zh-cn_topic_0221111191_p2566123613220"></a><a name="zh-cn_topic_0221111191_p2566123613220"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p11732173710119"><a name="zh-cn_topic_0221111191_p11732173710119"></a><a name="zh-cn_topic_0221111191_p11732173710119"></a>缓存时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row19473624"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p13273951706"><a name="zh-cn_topic_0221111191_p13273951706"></a><a name="zh-cn_topic_0221111191_p13273951706"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p2062812416220"><a name="zh-cn_topic_0221111191_p2062812416220"></a><a name="zh-cn_topic_0221111191_p2062812416220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p112028271314"><a name="zh-cn_topic_0221111191_p112028271314"></a><a name="zh-cn_topic_0221111191_p112028271314"></a>用户数据</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row168471214124017"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p19764828113"><a name="zh-cn_topic_0221111191_p19764828113"></a><a name="zh-cn_topic_0221111191_p19764828113"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p64189201"><a name="zh-cn_topic_0221111191_p64189201"></a><a name="zh-cn_topic_0221111191_p64189201"></a>Time</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p31942831"><a name="zh-cn_topic_0221111191_p31942831"></a><a name="zh-cn_topic_0221111191_p31942831"></a>创建时间</p>
</td>
</tr>
</tbody>
</table>

**表 5**  identities参数说明

<a name="zh-cn_topic_0221111191_table19554526582"></a>
<table><thead align="left"><tr id="zh-cn_topic_0221111191_row65535215818"><th class="cellrowborder" valign="top" width="20.02%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0221111191_p1555145245815"><a name="zh-cn_topic_0221111191_p1555145245815"></a><a name="zh-cn_topic_0221111191_p1555145245815"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.98%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0221111191_p135555214586"><a name="zh-cn_topic_0221111191_p135555214586"></a><a name="zh-cn_topic_0221111191_p135555214586"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0221111191_p135535214586"><a name="zh-cn_topic_0221111191_p135535214586"></a><a name="zh-cn_topic_0221111191_p135535214586"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0221111191_row25525218586"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p146251519115919"><a name="zh-cn_topic_0221111191_p146251519115919"></a><a name="zh-cn_topic_0221111191_p146251519115919"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p165525265811"><a name="zh-cn_topic_0221111191_p165525265811"></a><a name="zh-cn_topic_0221111191_p165525265811"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p1097423515913"><a name="zh-cn_topic_0221111191_p1097423515913"></a><a name="zh-cn_topic_0221111191_p1097423515913"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row125565225812"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0221111191_p10536132655914"><a name="zh-cn_topic_0221111191_p10536132655914"></a><a name="zh-cn_topic_0221111191_p10536132655914"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0221111191_p655452205813"><a name="zh-cn_topic_0221111191_p655452205813"></a><a name="zh-cn_topic_0221111191_p655452205813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0221111191_p692424514593"><a name="zh-cn_topic_0221111191_p692424514593"></a><a name="zh-cn_topic_0221111191_p692424514593"></a>参数位置：</p>
<a name="zh-cn_topic_0221111191_ul5924194585913"></a><a name="zh-cn_topic_0221111191_ul5924194585913"></a><ul id="zh-cn_topic_0221111191_ul5924194585913"><li>HEADER：头</li><li>QUERY：query</li></ul>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
    "total":1,
    "size":1,
    "authorizer_list":[
        {
            "name":"Authorizer_9dlh",
            "type":"FRONTEND",
            "authorizer_type":"FUNC",
            "authorizer_uri":"urn:fss:regionexample:dbb5762c88f045c6a1427a952bcae284:function:default:test111",
            "identities":[
                {
                    "name":"Authorization",
                    "location":"HEADER",
                }
            ],
            "ttl":10,
            "user_data":"aaaa",
            "id":"7345e3fe4047491ebd8ecb0acd665a4c",
            "create_time":"2020-01-19T11:48:56Z"
        }
    ]
}
```

## 状态码<a name="zh-cn_topic_0221111191_section43653029"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0221111191_table61067539"></a>
<table><thead align="left"><tr id="zh-cn_topic_0221111191_row16541512"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0221111191_p64794090"><a name="zh-cn_topic_0221111191_p64794090"></a><a name="zh-cn_topic_0221111191_p64794090"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0221111191_p13829924"><a name="zh-cn_topic_0221111191_p13829924"></a><a name="zh-cn_topic_0221111191_p13829924"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0221111191_row46482079"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0221111191_p6952067"><a name="zh-cn_topic_0221111191_p6952067"></a><a name="zh-cn_topic_0221111191_p6952067"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0221111191_p73578115452"><a name="zh-cn_topic_0221111191_p73578115452"></a><a name="zh-cn_topic_0221111191_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row34892078"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0221111191_p7686078"><a name="zh-cn_topic_0221111191_p7686078"></a><a name="zh-cn_topic_0221111191_p7686078"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0221111191_p48128109554"><a name="zh-cn_topic_0221111191_p48128109554"></a><a name="zh-cn_topic_0221111191_p48128109554"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row33115333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0221111191_p65096331"><a name="zh-cn_topic_0221111191_p65096331"></a><a name="zh-cn_topic_0221111191_p65096331"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0221111191_p9203142078"><a name="zh-cn_topic_0221111191_p9203142078"></a><a name="zh-cn_topic_0221111191_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row9258873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0221111191_p11771280"><a name="zh-cn_topic_0221111191_p11771280"></a><a name="zh-cn_topic_0221111191_p11771280"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0221111191_p13949586"><a name="zh-cn_topic_0221111191_p13949586"></a><a name="zh-cn_topic_0221111191_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0221111191_row58437416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0221111191_p35810232"><a name="zh-cn_topic_0221111191_p35810232"></a><a name="zh-cn_topic_0221111191_p35810232"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0221111191_p14947689"><a name="zh-cn_topic_0221111191_p14947689"></a><a name="zh-cn_topic_0221111191_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

