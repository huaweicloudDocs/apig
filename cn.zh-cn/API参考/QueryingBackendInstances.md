# 查看后端实例列表（云服务器列表）<a name="ZH-CN_TOPIC_0000001081837321"></a>

## 功能介绍<a name="zh-cn_topic_0118924580_section173482301428"></a>

查看指定VPC通道的云服务器列表。

## URI<a name="zh-cn_topic_0118924580_section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924580_table1439319294431"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924580_row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924580_p14361448204314"><a name="zh-cn_topic_0118924580_p14361448204314"></a><a name="zh-cn_topic_0118924580_p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924580_p1936174864316"><a name="zh-cn_topic_0118924580_p1936174864316"></a><a name="zh-cn_topic_0118924580_p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924580_row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924580_p1236111482435"><a name="zh-cn_topic_0118924580_p1236111482435"></a><a name="zh-cn_topic_0118924580_p1236111482435"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924580_p11361848184318"><a name="zh-cn_topic_0118924580_p11361848184318"></a><a name="zh-cn_topic_0118924580_p11361848184318"></a>/v1.0/apigw/vpc-channels/{id}/members[?page_size, page_no, name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：name、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924580_table18784710"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924580_row37287554"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924580_p393051"><a name="zh-cn_topic_0118924580_p393051"></a><a name="zh-cn_topic_0118924580_p393051"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924580_p31837140"><a name="zh-cn_topic_0118924580_p31837140"></a><a name="zh-cn_topic_0118924580_p31837140"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924580_p28671509"><a name="zh-cn_topic_0118924580_p28671509"></a><a name="zh-cn_topic_0118924580_p28671509"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924580_p40690887"><a name="zh-cn_topic_0118924580_p40690887"></a><a name="zh-cn_topic_0118924580_p40690887"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924580_row7627537"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924580_p13850780"><a name="zh-cn_topic_0118924580_p13850780"></a><a name="zh-cn_topic_0118924580_p13850780"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924580_p48171408"><a name="zh-cn_topic_0118924580_p48171408"></a><a name="zh-cn_topic_0118924580_p48171408"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924580_p9569939"><a name="zh-cn_topic_0118924580_p9569939"></a><a name="zh-cn_topic_0118924580_p9569939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924580_p36967632"><a name="zh-cn_topic_0118924580_p36967632"></a><a name="zh-cn_topic_0118924580_p36967632"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row1176054812130"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924580_p20478948151317"><a name="zh-cn_topic_0118924580_p20478948151317"></a><a name="zh-cn_topic_0118924580_p20478948151317"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924580_p13478164813136"><a name="zh-cn_topic_0118924580_p13478164813136"></a><a name="zh-cn_topic_0118924580_p13478164813136"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924580_p447812481138"><a name="zh-cn_topic_0118924580_p447812481138"></a><a name="zh-cn_topic_0118924580_p447812481138"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924580_p174783483134"><a name="zh-cn_topic_0118924580_p174783483134"></a><a name="zh-cn_topic_0118924580_p174783483134"></a>云服务器的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row676014486132"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924580_p7510848191318"><a name="zh-cn_topic_0118924580_p7510848191318"></a><a name="zh-cn_topic_0118924580_p7510848191318"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924580_p14525148121311"><a name="zh-cn_topic_0118924580_p14525148121311"></a><a name="zh-cn_topic_0118924580_p14525148121311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924580_p195251848201320"><a name="zh-cn_topic_0118924580_p195251848201320"></a><a name="zh-cn_topic_0118924580_p195251848201320"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924580_p1352504881313"><a name="zh-cn_topic_0118924580_p1352504881313"></a><a name="zh-cn_topic_0118924580_p1352504881313"></a>每页显示的云服务器数量，默认值：20。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row476016485136"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924580_p85251248181312"><a name="zh-cn_topic_0118924580_p85251248181312"></a><a name="zh-cn_topic_0118924580_p85251248181312"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924580_p652516485136"><a name="zh-cn_topic_0118924580_p652516485136"></a><a name="zh-cn_topic_0118924580_p652516485136"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924580_p852517485135"><a name="zh-cn_topic_0118924580_p852517485135"></a><a name="zh-cn_topic_0118924580_p852517485135"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924580_p25417483136"><a name="zh-cn_topic_0118924580_p25417483136"></a><a name="zh-cn_topic_0118924580_p25417483136"></a>页码，默认值：1。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924580_section842814271492"></a>

无

## 响应消息<a name="zh-cn_topic_0118924580_section312285311219"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924580_table12122155310121"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924580_row18122953181219"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924580_p81221153141210"><a name="zh-cn_topic_0118924580_p81221153141210"></a><a name="zh-cn_topic_0118924580_p81221153141210"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924580_p131371353101214"><a name="zh-cn_topic_0118924580_p131371353101214"></a><a name="zh-cn_topic_0118924580_p131371353101214"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924580_p10137753191214"><a name="zh-cn_topic_0118924580_p10137753191214"></a><a name="zh-cn_topic_0118924580_p10137753191214"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924580_row713716535122"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p19137153181215"><a name="zh-cn_topic_0118924580_p19137153181215"></a><a name="zh-cn_topic_0118924580_p19137153181215"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p7137253101216"><a name="zh-cn_topic_0118924580_p7137253101216"></a><a name="zh-cn_topic_0118924580_p7137253101216"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p71374537124"><a name="zh-cn_topic_0118924580_p71374537124"></a><a name="zh-cn_topic_0118924580_p71374537124"></a>符合条件的云服务器总数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row1713745311216"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p81371753181211"><a name="zh-cn_topic_0118924580_p81371753181211"></a><a name="zh-cn_topic_0118924580_p81371753181211"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p201531553141213"><a name="zh-cn_topic_0118924580_p201531553141213"></a><a name="zh-cn_topic_0118924580_p201531553141213"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p5153105315128"><a name="zh-cn_topic_0118924580_p5153105315128"></a><a name="zh-cn_topic_0118924580_p5153105315128"></a>本次查询返回的列表长度。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row3153553121217"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p715375371210"><a name="zh-cn_topic_0118924580_p715375371210"></a><a name="zh-cn_topic_0118924580_p715375371210"></a>vpc_instances</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p14153115311217"><a name="zh-cn_topic_0118924580_p14153115311217"></a><a name="zh-cn_topic_0118924580_p14153115311217"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p20153553201215"><a name="zh-cn_topic_0118924580_p20153553201215"></a><a name="zh-cn_topic_0118924580_p20153553201215"></a>本次查询到的云服务器列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  后端实例详情

<a name="zh-cn_topic_0118924580_table369051818103"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924580_row96971418151018"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924580_p166988187108"><a name="zh-cn_topic_0118924580_p166988187108"></a><a name="zh-cn_topic_0118924580_p166988187108"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924580_p070151881014"><a name="zh-cn_topic_0118924580_p070151881014"></a><a name="zh-cn_topic_0118924580_p070151881014"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924580_p10702181861014"><a name="zh-cn_topic_0118924580_p10702181861014"></a><a name="zh-cn_topic_0118924580_p10702181861014"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924580_row2706518171010"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p270971851011"><a name="zh-cn_topic_0118924580_p270971851011"></a><a name="zh-cn_topic_0118924580_p270971851011"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p1671171818106"><a name="zh-cn_topic_0118924580_p1671171818106"></a><a name="zh-cn_topic_0118924580_p1671171818106"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p3714618121013"><a name="zh-cn_topic_0118924580_p3714618121013"></a><a name="zh-cn_topic_0118924580_p3714618121013"></a>后端实例对象的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row15715518131012"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p19715171861018"><a name="zh-cn_topic_0118924580_p19715171861018"></a><a name="zh-cn_topic_0118924580_p19715171861018"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p1671861831013"><a name="zh-cn_topic_0118924580_p1671861831013"></a><a name="zh-cn_topic_0118924580_p1671861831013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p147215185105"><a name="zh-cn_topic_0118924580_p147215185105"></a><a name="zh-cn_topic_0118924580_p147215185105"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row372213185106"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p16724018171016"><a name="zh-cn_topic_0118924580_p16724018171016"></a><a name="zh-cn_topic_0118924580_p16724018171016"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p872671812109"><a name="zh-cn_topic_0118924580_p872671812109"></a><a name="zh-cn_topic_0118924580_p872671812109"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p10729141841011"><a name="zh-cn_topic_0118924580_p10729141841011"></a><a name="zh-cn_topic_0118924580_p10729141841011"></a>后端实例对象的状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row5731191831020"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p77322018111010"><a name="zh-cn_topic_0118924580_p77322018111010"></a><a name="zh-cn_topic_0118924580_p77322018111010"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p673391861012"><a name="zh-cn_topic_0118924580_p673391861012"></a><a name="zh-cn_topic_0118924580_p673391861012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p1373511811019"><a name="zh-cn_topic_0118924580_p1373511811019"></a><a name="zh-cn_topic_0118924580_p1373511811019"></a>云服务器的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row8735201813105"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p073814186107"><a name="zh-cn_topic_0118924580_p073814186107"></a><a name="zh-cn_topic_0118924580_p073814186107"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p1741141831010"><a name="zh-cn_topic_0118924580_p1741141831010"></a><a name="zh-cn_topic_0118924580_p1741141831010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p1274310188106"><a name="zh-cn_topic_0118924580_p1274310188106"></a><a name="zh-cn_topic_0118924580_p1274310188106"></a>云服务器的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row2988816867"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p274681831019"><a name="zh-cn_topic_0118924580_p274681831019"></a><a name="zh-cn_topic_0118924580_p274681831019"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p14748918131010"><a name="zh-cn_topic_0118924580_p14748918131010"></a><a name="zh-cn_topic_0118924580_p14748918131010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p1975041814109"><a name="zh-cn_topic_0118924580_p1975041814109"></a><a name="zh-cn_topic_0118924580_p1975041814109"></a>云服务器的主机地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row1075001891019"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p975113187104"><a name="zh-cn_topic_0118924580_p975113187104"></a><a name="zh-cn_topic_0118924580_p975113187104"></a>weight</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p5753171818103"><a name="zh-cn_topic_0118924580_p5753171818103"></a><a name="zh-cn_topic_0118924580_p5753171818103"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p3754118181010"><a name="zh-cn_topic_0118924580_p3754118181010"></a><a name="zh-cn_topic_0118924580_p3754118181010"></a>权重值。</p>
<p id="zh-cn_topic_0118924580_p4755131810102"><a name="zh-cn_topic_0118924580_p4755131810102"></a><a name="zh-cn_topic_0118924580_p4755131810102"></a>权重值越大，转发到该云服务器的请求数量越多。</p>
<p id="zh-cn_topic_0118924580_p167561218151018"><a name="zh-cn_topic_0118924580_p167561218151018"></a><a name="zh-cn_topic_0118924580_p167561218151018"></a>取值范围1 ~ 100。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row197570189109"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924580_p11759018171013"><a name="zh-cn_topic_0118924580_p11759018171013"></a><a name="zh-cn_topic_0118924580_p11759018171013"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924580_p16761191851016"><a name="zh-cn_topic_0118924580_p16761191851016"></a><a name="zh-cn_topic_0118924580_p16761191851016"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924580_p7762181812105"><a name="zh-cn_topic_0118924580_p7762181812105"></a><a name="zh-cn_topic_0118924580_p7762181812105"></a>云服务器增加到VPC通道的时间。</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 2,
  "size": 2,
  "vpc_instances": [
    {
      "instance_id": "instance02",
      "instance_name": "instance_name02",
      "host": "127.0.0.2",
      "weight": 10,
      "id": "680e42fab429447ca23b9623107523d9",
      "vpc_id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
      "status": 1,
      "create_time": "2018-07-27T12:42:32Z"
    },
    {
      "instance_id": "instance01",
      "instance_name": "instance_name01",
      "host": "127.0.0.1",
      "weight": 10,
      "id": "c3bc73605a8b400793363c87574fbad7",
      "vpc_id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
      "status": 1,
      "create_time": "2018-07-27T12:30:48Z"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0118924580_section338043011426"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924580_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924580_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924580_p174881730194216"><a name="zh-cn_topic_0118924580_p174881730194216"></a><a name="zh-cn_topic_0118924580_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924580_p848863018429"><a name="zh-cn_topic_0118924580_p848863018429"></a><a name="zh-cn_topic_0118924580_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924580_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924580_p7488163084211"><a name="zh-cn_topic_0118924580_p7488163084211"></a><a name="zh-cn_topic_0118924580_p7488163084211"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924580_p948803015424"><a name="zh-cn_topic_0118924580_p948803015424"></a><a name="zh-cn_topic_0118924580_p948803015424"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924580_p14488113015426"><a name="zh-cn_topic_0118924580_p14488113015426"></a><a name="zh-cn_topic_0118924580_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924580_p164881130154211"><a name="zh-cn_topic_0118924580_p164881130154211"></a><a name="zh-cn_topic_0118924580_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924580_p24883304428"><a name="zh-cn_topic_0118924580_p24883304428"></a><a name="zh-cn_topic_0118924580_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924580_p1848810308429"><a name="zh-cn_topic_0118924580_p1848810308429"></a><a name="zh-cn_topic_0118924580_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924580_p6488133064210"><a name="zh-cn_topic_0118924580_p6488133064210"></a><a name="zh-cn_topic_0118924580_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924580_p10488193018426"><a name="zh-cn_topic_0118924580_p10488193018426"></a><a name="zh-cn_topic_0118924580_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924580_p144883304428"><a name="zh-cn_topic_0118924580_p144883304428"></a><a name="zh-cn_topic_0118924580_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924580_p4488103094212"><a name="zh-cn_topic_0118924580_p4488103094212"></a><a name="zh-cn_topic_0118924580_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924580_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924580_p17488163014423"><a name="zh-cn_topic_0118924580_p17488163014423"></a><a name="zh-cn_topic_0118924580_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924580_p048813014216"><a name="zh-cn_topic_0118924580_p048813014216"></a><a name="zh-cn_topic_0118924580_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

