# 查询已购买的API分组列表<a name="ZH-CN_TOPIC_0000001082135127"></a>

## 功能介绍<a name="zh-cn_topic_0118924522_section24315590"></a>

租户可以查询自己已购买的API分组列表。

## URI<a name="zh-cn_topic_0118924522_section17513719"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924522_table48054825"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924522_row26116789"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924522_p35085151"><a name="zh-cn_topic_0118924522_p35085151"></a><a name="zh-cn_topic_0118924522_p35085151"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924522_p23325002"><a name="zh-cn_topic_0118924522_p23325002"></a><a name="zh-cn_topic_0118924522_p23325002"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924522_row10277022"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924522_p27132417"><a name="zh-cn_topic_0118924522_p27132417"></a><a name="zh-cn_topic_0118924522_p27132417"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924522_p50242206"><a name="zh-cn_topic_0118924522_p50242206"></a><a name="zh-cn_topic_0118924522_p50242206"></a>/v1.0/apigw/purchases/groups[?page_size, page_no, id, group_id, group_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、group\_id 、group\_name 、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924522_table3383718"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924522_row57199365"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924522_p2637004"><a name="zh-cn_topic_0118924522_p2637004"></a><a name="zh-cn_topic_0118924522_p2637004"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924522_p12270800"><a name="zh-cn_topic_0118924522_p12270800"></a><a name="zh-cn_topic_0118924522_p12270800"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924522_p54410744"><a name="zh-cn_topic_0118924522_p54410744"></a><a name="zh-cn_topic_0118924522_p54410744"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924522_p45194157"><a name="zh-cn_topic_0118924522_p45194157"></a><a name="zh-cn_topic_0118924522_p45194157"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924522_row36848086"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924522_p31904988"><a name="zh-cn_topic_0118924522_p31904988"></a><a name="zh-cn_topic_0118924522_p31904988"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924522_p34167206"><a name="zh-cn_topic_0118924522_p34167206"></a><a name="zh-cn_topic_0118924522_p34167206"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924522_p16080284"><a name="zh-cn_topic_0118924522_p16080284"></a><a name="zh-cn_topic_0118924522_p16080284"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924522_p27434664"><a name="zh-cn_topic_0118924522_p27434664"></a><a name="zh-cn_topic_0118924522_p27434664"></a>订购关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row45585384"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924522_p1428653"><a name="zh-cn_topic_0118924522_p1428653"></a><a name="zh-cn_topic_0118924522_p1428653"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924522_p48612091"><a name="zh-cn_topic_0118924522_p48612091"></a><a name="zh-cn_topic_0118924522_p48612091"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924522_p45265273"><a name="zh-cn_topic_0118924522_p45265273"></a><a name="zh-cn_topic_0118924522_p45265273"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924522_p42608463"><a name="zh-cn_topic_0118924522_p42608463"></a><a name="zh-cn_topic_0118924522_p42608463"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row47931851"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924522_p57274713"><a name="zh-cn_topic_0118924522_p57274713"></a><a name="zh-cn_topic_0118924522_p57274713"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924522_p8740180"><a name="zh-cn_topic_0118924522_p8740180"></a><a name="zh-cn_topic_0118924522_p8740180"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924522_p36865955"><a name="zh-cn_topic_0118924522_p36865955"></a><a name="zh-cn_topic_0118924522_p36865955"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924522_p33352367"><a name="zh-cn_topic_0118924522_p33352367"></a><a name="zh-cn_topic_0118924522_p33352367"></a>API分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row55921708"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924522_p33364523"><a name="zh-cn_topic_0118924522_p33364523"></a><a name="zh-cn_topic_0118924522_p33364523"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924522_p18171838"><a name="zh-cn_topic_0118924522_p18171838"></a><a name="zh-cn_topic_0118924522_p18171838"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924522_p62632782"><a name="zh-cn_topic_0118924522_p62632782"></a><a name="zh-cn_topic_0118924522_p62632782"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924522_p40090562"><a name="zh-cn_topic_0118924522_p40090562"></a><a name="zh-cn_topic_0118924522_p40090562"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row25270741"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924522_p33664155"><a name="zh-cn_topic_0118924522_p33664155"></a><a name="zh-cn_topic_0118924522_p33664155"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924522_p42442041"><a name="zh-cn_topic_0118924522_p42442041"></a><a name="zh-cn_topic_0118924522_p42442041"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924522_p15253336"><a name="zh-cn_topic_0118924522_p15253336"></a><a name="zh-cn_topic_0118924522_p15253336"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924522_p27560736"><a name="zh-cn_topic_0118924522_p27560736"></a><a name="zh-cn_topic_0118924522_p27560736"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924522_section23405748"></a>

无

## 响应消息<a name="zh-cn_topic_0118924522_section16817402"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924522_table15288659"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924522_row8923449"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924522_p51710807"><a name="zh-cn_topic_0118924522_p51710807"></a><a name="zh-cn_topic_0118924522_p51710807"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924522_p27825849"><a name="zh-cn_topic_0118924522_p27825849"></a><a name="zh-cn_topic_0118924522_p27825849"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924522_p39301320"><a name="zh-cn_topic_0118924522_p39301320"></a><a name="zh-cn_topic_0118924522_p39301320"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924522_row29290347"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p23707915"><a name="zh-cn_topic_0118924522_p23707915"></a><a name="zh-cn_topic_0118924522_p23707915"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p41292943"><a name="zh-cn_topic_0118924522_p41292943"></a><a name="zh-cn_topic_0118924522_p41292943"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p56394080"><a name="zh-cn_topic_0118924522_p56394080"></a><a name="zh-cn_topic_0118924522_p56394080"></a>满足查询条件的分组总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row37784672"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p40659598"><a name="zh-cn_topic_0118924522_p40659598"></a><a name="zh-cn_topic_0118924522_p40659598"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p5093181"><a name="zh-cn_topic_0118924522_p5093181"></a><a name="zh-cn_topic_0118924522_p5093181"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p9894549"><a name="zh-cn_topic_0118924522_p9894549"></a><a name="zh-cn_topic_0118924522_p9894549"></a>本次查询返回的分组个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row21942079"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p32477990"><a name="zh-cn_topic_0118924522_p32477990"></a><a name="zh-cn_topic_0118924522_p32477990"></a>purchases</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p13471562"><a name="zh-cn_topic_0118924522_p13471562"></a><a name="zh-cn_topic_0118924522_p13471562"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p17454738"><a name="zh-cn_topic_0118924522_p17454738"></a><a name="zh-cn_topic_0118924522_p17454738"></a>本次查询返回的分组列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  purchases参数说明

<a name="zh-cn_topic_0118924522_table22874919"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924522_row35974848"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924522_p28281558"><a name="zh-cn_topic_0118924522_p28281558"></a><a name="zh-cn_topic_0118924522_p28281558"></a><strong id="zh-cn_topic_0118924522_b53207438"><a name="zh-cn_topic_0118924522_b53207438"></a><a name="zh-cn_topic_0118924522_b53207438"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924522_p14835218"><a name="zh-cn_topic_0118924522_p14835218"></a><a name="zh-cn_topic_0118924522_p14835218"></a><strong id="zh-cn_topic_0118924522_b66408105"><a name="zh-cn_topic_0118924522_b66408105"></a><a name="zh-cn_topic_0118924522_b66408105"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924522_p10347445"><a name="zh-cn_topic_0118924522_p10347445"></a><a name="zh-cn_topic_0118924522_p10347445"></a><strong id="zh-cn_topic_0118924522_b26018149"><a name="zh-cn_topic_0118924522_b26018149"></a><a name="zh-cn_topic_0118924522_b26018149"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924522_row27095299"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p47235577"><a name="zh-cn_topic_0118924522_p47235577"></a><a name="zh-cn_topic_0118924522_p47235577"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p876528"><a name="zh-cn_topic_0118924522_p876528"></a><a name="zh-cn_topic_0118924522_p876528"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p3889935"><a name="zh-cn_topic_0118924522_p3889935"></a><a name="zh-cn_topic_0118924522_p3889935"></a>订购关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row35009422"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p17190909"><a name="zh-cn_topic_0118924522_p17190909"></a><a name="zh-cn_topic_0118924522_p17190909"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p50286377"><a name="zh-cn_topic_0118924522_p50286377"></a><a name="zh-cn_topic_0118924522_p50286377"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p46664697"><a name="zh-cn_topic_0118924522_p46664697"></a><a name="zh-cn_topic_0118924522_p46664697"></a>分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row17329090"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p61479044"><a name="zh-cn_topic_0118924522_p61479044"></a><a name="zh-cn_topic_0118924522_p61479044"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p13746654"><a name="zh-cn_topic_0118924522_p13746654"></a><a name="zh-cn_topic_0118924522_p13746654"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p39737209"><a name="zh-cn_topic_0118924522_p39737209"></a><a name="zh-cn_topic_0118924522_p39737209"></a>分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row22090566"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p44505445"><a name="zh-cn_topic_0118924522_p44505445"></a><a name="zh-cn_topic_0118924522_p44505445"></a>group_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p48171288"><a name="zh-cn_topic_0118924522_p48171288"></a><a name="zh-cn_topic_0118924522_p48171288"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p9560264"><a name="zh-cn_topic_0118924522_p9560264"></a><a name="zh-cn_topic_0118924522_p9560264"></a>分组描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row18933514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p57219647"><a name="zh-cn_topic_0118924522_p57219647"></a><a name="zh-cn_topic_0118924522_p57219647"></a>order_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p4279845"><a name="zh-cn_topic_0118924522_p4279845"></a><a name="zh-cn_topic_0118924522_p4279845"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p11123171"><a name="zh-cn_topic_0118924522_p11123171"></a><a name="zh-cn_topic_0118924522_p11123171"></a>订购时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row32999683"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p55728698"><a name="zh-cn_topic_0118924522_p55728698"></a><a name="zh-cn_topic_0118924522_p55728698"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p17730652"><a name="zh-cn_topic_0118924522_p17730652"></a><a name="zh-cn_topic_0118924522_p17730652"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p26896723"><a name="zh-cn_topic_0118924522_p26896723"></a><a name="zh-cn_topic_0118924522_p26896723"></a>生效时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row40743922"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p11923395"><a name="zh-cn_topic_0118924522_p11923395"></a><a name="zh-cn_topic_0118924522_p11923395"></a>expire_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p26270940"><a name="zh-cn_topic_0118924522_p26270940"></a><a name="zh-cn_topic_0118924522_p26270940"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p47571430"><a name="zh-cn_topic_0118924522_p47571430"></a><a name="zh-cn_topic_0118924522_p47571430"></a>过期时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row25489693"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p51399251"><a name="zh-cn_topic_0118924522_p51399251"></a><a name="zh-cn_topic_0118924522_p51399251"></a>group_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p2589773"><a name="zh-cn_topic_0118924522_p2589773"></a><a name="zh-cn_topic_0118924522_p2589773"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p8445043"><a name="zh-cn_topic_0118924522_p8445043"></a><a name="zh-cn_topic_0118924522_p8445043"></a>分组访问域名列表，查询列表时不返回</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row8896531"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p49530407"><a name="zh-cn_topic_0118924522_p49530407"></a><a name="zh-cn_topic_0118924522_p49530407"></a>quota_left</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p52540060"><a name="zh-cn_topic_0118924522_p52540060"></a><a name="zh-cn_topic_0118924522_p52540060"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p27886490"><a name="zh-cn_topic_0118924522_p27886490"></a><a name="zh-cn_topic_0118924522_p27886490"></a>剩余访问次数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row49651819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p62374408"><a name="zh-cn_topic_0118924522_p62374408"></a><a name="zh-cn_topic_0118924522_p62374408"></a>quota_used</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p19162306"><a name="zh-cn_topic_0118924522_p19162306"></a><a name="zh-cn_topic_0118924522_p19162306"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p8642944"><a name="zh-cn_topic_0118924522_p8642944"></a><a name="zh-cn_topic_0118924522_p8642944"></a>已使用访问次数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row10677636"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p59582212"><a name="zh-cn_topic_0118924522_p59582212"></a><a name="zh-cn_topic_0118924522_p59582212"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p61429885"><a name="zh-cn_topic_0118924522_p61429885"></a><a name="zh-cn_topic_0118924522_p61429885"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p9764758"><a name="zh-cn_topic_0118924522_p9764758"></a><a name="zh-cn_topic_0118924522_p9764758"></a>生成的APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row20773958"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924522_p4969010"><a name="zh-cn_topic_0118924522_p4969010"></a><a name="zh-cn_topic_0118924522_p4969010"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924522_p66945555"><a name="zh-cn_topic_0118924522_p66945555"></a><a name="zh-cn_topic_0118924522_p66945555"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924522_p53880913"><a name="zh-cn_topic_0118924522_p53880913"></a><a name="zh-cn_topic_0118924522_p53880913"></a>生成的APP的secret</p>
</td>
</tr>
</tbody>
</table>

响应参数样例：

```
{
	"total": 3,
	"size": 3,
	"purchases": [{
		"id": "615af8d9-f31d-4cdf-8807-b191dc969a07",
		"group_id": "f0585333-5722-4878-b7fa-31ae00b6ae3a",
		"group_name": "api_group_003",
		"group_remark": "分组003",
		"group_domains": null,
		"quota_used": 0,
		"quota_left": 2000000000,
		"order_time": "2017-12-29T06:22:46Z",
		"start_time": "2018-01-01T00:00:00Z",
		"expire_time": "2019-01-01T00:00:00Z",
		"app_key": "0e242685-661d-4254-a8bb-be9a92b04785",
		"app_secret": "******"
	},
	{
		"id": "9d0bdab1-a553-4bc9-be8c-a2e6c08e4d13",
		"group_id": "02a8ab3c-b278-4de5-a096-852829671ae7",
		"group_name": "api_group_002",
		"group_remark": "分组002",
		"group_domains": null,
		"quota_used": 0,
		"quota_left": 2000000000,
		"order_time": "2017-12-29T06:22:46Z",
		"start_time": "2018-01-01T00:00:00Z",
		"expire_time": "2019-01-01T00:00:00Z",
		"app_key": "0e242685-661d-4254-a8bb-be9a92b04785",
		"app_secret": "******"
	},
	{
		"id": "3f30d49b-220f-4b11-9e94-c2fd3c1cc587",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"group_name": "api_group_001",
		"group_remark": "分组001",
		"group_domains": null,
		"quota_used": 0,
		"quota_left": 2000000000,
		"order_time": "2017-12-29T06:16:03Z",
		"start_time": "2018-01-01T00:00:00Z",
		"expire_time": "2019-01-01T00:00:00Z",
		"app_key": "0e242685-661d-4254-a8bb-be9a92b04785",
		"app_secret": "******"
	}]
}
```

## 状态码<a name="zh-cn_topic_0118924522_section9325140"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924522_table34711240"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924522_row25122570"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924522_p21662275"><a name="zh-cn_topic_0118924522_p21662275"></a><a name="zh-cn_topic_0118924522_p21662275"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924522_p9813849"><a name="zh-cn_topic_0118924522_p9813849"></a><a name="zh-cn_topic_0118924522_p9813849"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924522_row56724275"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924522_p31263545"><a name="zh-cn_topic_0118924522_p31263545"></a><a name="zh-cn_topic_0118924522_p31263545"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924522_p49319253"><a name="zh-cn_topic_0118924522_p49319253"></a><a name="zh-cn_topic_0118924522_p49319253"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row41220093"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924522_p50493266"><a name="zh-cn_topic_0118924522_p50493266"></a><a name="zh-cn_topic_0118924522_p50493266"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924522_p63422768"><a name="zh-cn_topic_0118924522_p63422768"></a><a name="zh-cn_topic_0118924522_p63422768"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row33934001"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924522_p64299566"><a name="zh-cn_topic_0118924522_p64299566"></a><a name="zh-cn_topic_0118924522_p64299566"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924522_p40882376"><a name="zh-cn_topic_0118924522_p40882376"></a><a name="zh-cn_topic_0118924522_p40882376"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924522_row32397067"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924522_p6916762"><a name="zh-cn_topic_0118924522_p6916762"></a><a name="zh-cn_topic_0118924522_p6916762"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924522_p6744143"><a name="zh-cn_topic_0118924522_p6744143"></a><a name="zh-cn_topic_0118924522_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

