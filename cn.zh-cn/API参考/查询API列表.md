# 查询API列表<a name="apig-zh-api-180713031"></a>

## 功能介绍<a name="section31536236"></a>

查看API列表，返回API详细信息、发布信息等，但不能查看到后端服务信息。

## URI<a name="section15390672"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table4929521"></a>
<table><thead align="left"><tr id="row21328449"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p49882799"><a name="p49882799"></a><a name="p49882799"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p13974922"><a name="p13974922"></a><a name="p13974922"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row58226873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p18756261"><a name="p18756261"></a><a name="p18756261"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p42862133"><a name="p42862133"></a><a name="p42862133"></a>/v1.0/apigw/apis/[?page_size, page_no, id, name, group_id, req_protocol, req_method, req_uri, auth_type, env_id, type,status]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：id、name、group\_id、req\_protocol、req\_method、req\_uri、auth\_type、env\_id、type、status、page\_size、page\_no。  

## 请求消息<a name="section4298322"></a>

**表 2**  参数说明

<a name="table309072"></a>
<table><thead align="left"><tr id="row29526596"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p42844056"><a name="p42844056"></a><a name="p42844056"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p47816505"><a name="p47816505"></a><a name="p47816505"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p47931662"><a name="p47931662"></a><a name="p47931662"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p57259391"><a name="p57259391"></a><a name="p57259391"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7499126"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p3449432"><a name="p3449432"></a><a name="p3449432"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p10968591"><a name="p10968591"></a><a name="p10968591"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p16040707"><a name="p16040707"></a><a name="p16040707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p24228891"><a name="p24228891"></a><a name="p24228891"></a>API的编号</p>
</td>
</tr>
<tr id="row16733432"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p13230786"><a name="p13230786"></a><a name="p13230786"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p65060773"><a name="p65060773"></a><a name="p65060773"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p35431240"><a name="p35431240"></a><a name="p35431240"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p51358163"><a name="p51358163"></a><a name="p51358163"></a>API的名称</p>
</td>
</tr>
<tr id="row59570287"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p60463979"><a name="p60463979"></a><a name="p60463979"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p65744098"><a name="p65744098"></a><a name="p65744098"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p23671742"><a name="p23671742"></a><a name="p23671742"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p38362983"><a name="p38362983"></a><a name="p38362983"></a>API所属分组编号</p>
</td>
</tr>
<tr id="row9722532"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p49327594"><a name="p49327594"></a><a name="p49327594"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p36112177"><a name="p36112177"></a><a name="p36112177"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p39405216"><a name="p39405216"></a><a name="p39405216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p37705952"><a name="p37705952"></a><a name="p37705952"></a>请求协议</p>
</td>
</tr>
<tr id="row3809254"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p40114146"><a name="p40114146"></a><a name="p40114146"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p28020354"><a name="p28020354"></a><a name="p28020354"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p55056174"><a name="p55056174"></a><a name="p55056174"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p30365135"><a name="p30365135"></a><a name="p30365135"></a>请求方法</p>
</td>
</tr>
<tr id="row4850767"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p57367866"><a name="p57367866"></a><a name="p57367866"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p16285582"><a name="p16285582"></a><a name="p16285582"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p44063729"><a name="p44063729"></a><a name="p44063729"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p12392334"><a name="p12392334"></a><a name="p12392334"></a>请求路径</p>
</td>
</tr>
<tr id="row44422145"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p41423973"><a name="p41423973"></a><a name="p41423973"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p67007510"><a name="p67007510"></a><a name="p67007510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p58899195"><a name="p58899195"></a><a name="p58899195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p6105468"><a name="p6105468"></a><a name="p6105468"></a>授权类型</p>
</td>
</tr>
<tr id="row54949219"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p21701787"><a name="p21701787"></a><a name="p21701787"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p13014307"><a name="p13014307"></a><a name="p13014307"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p47525923"><a name="p47525923"></a><a name="p47525923"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p24394564"><a name="p24394564"></a><a name="p24394564"></a>发布的环境编号</p>
</td>
</tr>
<tr id="row18224488"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p66897437"><a name="p66897437"></a><a name="p66897437"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p49983302"><a name="p49983302"></a><a name="p49983302"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p22115660"><a name="p22115660"></a><a name="p22115660"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p46538006"><a name="p46538006"></a><a name="p46538006"></a>API类型</p>
</td>
</tr>
<tr id="row16188872"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p36230260"><a name="p36230260"></a><a name="p36230260"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p48969944"><a name="p48969944"></a><a name="p48969944"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p7142557"><a name="p7142557"></a><a name="p7142557"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p41676267"><a name="p41676267"></a><a name="p41676267"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row39542084"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p48792241"><a name="p48792241"></a><a name="p48792241"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p59857467"><a name="p59857467"></a><a name="p59857467"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p16616649"><a name="p16616649"></a><a name="p16616649"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p3771332"><a name="p3771332"></a><a name="p3771332"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="row136191246154813"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p26191463489"><a name="p26191463489"></a><a name="p26191463489"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1261984620484"><a name="p1261984620484"></a><a name="p1261984620484"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p261916461487"><a name="p261916461487"></a><a name="p261916461487"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p10619154674815"><a name="p10619154674815"></a><a name="p10619154674815"></a>指定需要精确匹配查找的资源名称</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section12619772"></a>

**表 3**  参数说明

<a name="table62034025"></a>
<table><thead align="left"><tr id="row12774732"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p28120399"><a name="p28120399"></a><a name="p28120399"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p63159826"><a name="p63159826"></a><a name="p63159826"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p15672253"><a name="p15672253"></a><a name="p15672253"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row61492985"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14875885"><a name="p14875885"></a><a name="p14875885"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64096066"><a name="p64096066"></a><a name="p64096066"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p24398880"><a name="p24398880"></a><a name="p24398880"></a>符合条件的API总数</p>
</td>
</tr>
<tr id="row18263329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2934686"><a name="p2934686"></a><a name="p2934686"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p36383032"><a name="p36383032"></a><a name="p36383032"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61344470"><a name="p61344470"></a><a name="p61344470"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="row15229322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p25615594"><a name="p25615594"></a><a name="p25615594"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p61597251"><a name="p61597251"></a><a name="p61597251"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p23321404"><a name="p23321404"></a><a name="p23321404"></a>本次查询到的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table8566044"></a>
<table><thead align="left"><tr id="row21338628"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p50707320"><a name="p50707320"></a><a name="p50707320"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13652219"><a name="p13652219"></a><a name="p13652219"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p32087992"><a name="p32087992"></a><a name="p32087992"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row48990549"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8811514"><a name="p8811514"></a><a name="p8811514"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42644048"><a name="p42644048"></a><a name="p42644048"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p31615870"><a name="p31615870"></a><a name="p31615870"></a>API编号</p>
</td>
</tr>
<tr id="row16107382"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29629597"><a name="p29629597"></a><a name="p29629597"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51187119"><a name="p51187119"></a><a name="p51187119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52515990"><a name="p52515990"></a><a name="p52515990"></a>API名称</p>
</td>
</tr>
<tr id="row2881869"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p32104846"><a name="p32104846"></a><a name="p32104846"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p50355735"><a name="p50355735"></a><a name="p50355735"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52282769"><a name="p52282769"></a><a name="p52282769"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row782880"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63413318"><a name="p63413318"></a><a name="p63413318"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p36205104"><a name="p36205104"></a><a name="p36205104"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46932294"><a name="p46932294"></a><a name="p46932294"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row19737470"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55231234"><a name="p55231234"></a><a name="p55231234"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44544999"><a name="p44544999"></a><a name="p44544999"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p51375189"><a name="p51375189"></a><a name="p51375189"></a>API的状态</p>
</td>
</tr>
<tr id="row59723518"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5766795"><a name="p5766795"></a><a name="p5766795"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64457269"><a name="p64457269"></a><a name="p64457269"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53656291"><a name="p53656291"></a><a name="p53656291"></a>API类型</p>
</td>
</tr>
<tr id="row13144575"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p58077679"><a name="p58077679"></a><a name="p58077679"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6671576"><a name="p6671576"></a><a name="p6671576"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3526753"><a name="p3526753"></a><a name="p3526753"></a>API版本</p>
</td>
</tr>
<tr id="row31740777"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20866117"><a name="p20866117"></a><a name="p20866117"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12433942"><a name="p12433942"></a><a name="p12433942"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p516420"><a name="p516420"></a><a name="p516420"></a>API访问协议</p>
</td>
</tr>
<tr id="row4647785"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40926317"><a name="p40926317"></a><a name="p40926317"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p26697344"><a name="p26697344"></a><a name="p26697344"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15001293"><a name="p15001293"></a><a name="p15001293"></a>API请求方式</p>
</td>
</tr>
<tr id="row793912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p64306892"><a name="p64306892"></a><a name="p64306892"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p41475757"><a name="p41475757"></a><a name="p41475757"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4093122"><a name="p4093122"></a><a name="p4093122"></a>API访问地址</p>
</td>
</tr>
<tr id="row36838099"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p31096082"><a name="p31096082"></a><a name="p31096082"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35754746"><a name="p35754746"></a><a name="p35754746"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10453298"><a name="p10453298"></a><a name="p10453298"></a>API认证方式</p>
</td>
</tr>
<tr id="row26970819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37152759"><a name="p37152759"></a><a name="p37152759"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56583503"><a name="p56583503"></a><a name="p56583503"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19861044"><a name="p19861044"></a><a name="p19861044"></a>API匹配方式</p>
</td>
</tr>
<tr id="row44531670"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50295545"><a name="p50295545"></a><a name="p50295545"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47407324"><a name="p47407324"></a><a name="p47407324"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14788007"><a name="p14788007"></a><a name="p14788007"></a>API注册时间</p>
</td>
</tr>
<tr id="row65983203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p43039263"><a name="p43039263"></a><a name="p43039263"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p63628246"><a name="p63628246"></a><a name="p63628246"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53614322"><a name="p53614322"></a><a name="p53614322"></a>API修改时间</p>
</td>
</tr>
<tr id="row12766858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p27482552"><a name="p27482552"></a><a name="p27482552"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11494206"><a name="p11494206"></a><a name="p11494206"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p58615493"><a name="p58615493"></a><a name="p58615493"></a>API描述</p>
</td>
</tr>
<tr id="row57777392"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p49457179"><a name="p49457179"></a><a name="p49457179"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p46608538"><a name="p46608538"></a><a name="p46608538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17195222"><a name="p17195222"></a><a name="p17195222"></a>后端类型</p>
</td>
</tr>
<tr id="row20539270"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53068135"><a name="p53068135"></a><a name="p53068135"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3551673"><a name="p3551673"></a><a name="p3551673"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19250083"><a name="p19250083"></a><a name="p19250083"></a>发布的环境名</p>
</td>
</tr>
<tr id="row39033025"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7558467"><a name="p7558467"></a><a name="p7558467"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8256114"><a name="p8256114"></a><a name="p8256114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p64765493"><a name="p64765493"></a><a name="p64765493"></a>发布的环境id</p>
</td>
</tr>
<tr id="row46018530"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p36513439"><a name="p36513439"></a><a name="p36513439"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4798564"><a name="p4798564"></a><a name="p4798564"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53139418"><a name="p53139418"></a><a name="p53139418"></a>发布记录的编号</p>
</td>
</tr>
<tr id="row29624732"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50793096"><a name="p50793096"></a><a name="p50793096"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20600108"><a name="p20600108"></a><a name="p20600108"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57996081"><a name="p57996081"></a><a name="p57996081"></a>是否需要编排</p>
</td>
</tr>
<tr id="row02521055181212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16252655131214"><a name="p16252655131214"></a><a name="p16252655131214"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17252195514120"><a name="p17252195514120"></a><a name="p17252195514120"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p0252955151218"><a name="p0252955151218"></a><a name="p0252955151218"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="row1455379135"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11455072136"><a name="p11455072136"></a><a name="p11455072136"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1145577181318"><a name="p1145577181318"></a><a name="p1145577181318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14455577139"><a name="p14455577139"></a><a name="p14455577139"></a>API的标签</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 3,
  "size": 3,
  "apis": [
    {
      "name": "test",
      "type": 1,
      "version": "V0.0.1",
      "req_protocol": "HTTPS",
      "req_method": "GET",
      "req_uri": "/test/{project_id}",
      "auth_type": "APP",
      "tag": "test",
      "cors": false,
      "match_mode": "NORMAL",
      "backend_type": "HTTP",
      "group_id": "f71f69876f90456ca6fd18ed012fdc11",
      "id": "81efcfd94b8747a0b21e8c04144a4e8c",
      "status": 1,
      "arrange_necessary": 2,
      "register_time": "2018-08-15T03:41:11Z",
      "update_time": "2018-08-15T03:41:11Z",
      "group_name": "group0002"
    },
    {
      "name": "bbbbb",
      "type": 1,
      "version": "0.0.1",
      "req_protocol": "HTTPS",
      "req_method": "GET",
      "req_uri": "/test002",
      "auth_type": "APP",
      "cors": false,
      "match_mode": "NORMAL",
      "backend_type": "MOCK",
      "remark": "aaa",
      "group_id": "70f1b578da9b4dfe889b4c33d1b995c2",
      "id": "91c26288acea4448be205265d77dae22",
      "status": 1,
      "arrange_necessary": 2,
      "register_time": "2018-07-27T11:54:24Z",
      "update_time": "2018-07-27T11:54:24Z",
      "group_name": "test001",
      "run_env_name": "RELEASE",
      "run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "publish_id": "a6e06a00c382436eb524fa2dd343cb6d"
    },
    {
      "name": "aaa",
      "type": 1,
      "version": "0.0.1",
      "req_protocol": "HTTPS",
      "req_method": "GET",
      "req_uri": "/test001",
      "auth_type": "APP",
      "cors": false,
      "match_mode": "NORMAL",
      "backend_type": "MOCK",
      "remark": "aaa",
      "group_id": "70f1b578da9b4dfe889b4c33d1b995c2",
      "id": "aebacac6095942b4b2dd2b209bb7b9bc",
      "status": 1,
      "arrange_necessary": 2,
      "register_time": "2018-07-27T11:23:34Z",
      "update_time": "2018-07-27T11:23:34Z",
      "group_name": "test001",
      "run_env_name": "RELEASE",
      "run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "publish_id": "1bc8b2b741a04bd4af3ef9d7cd003104"
    }
  ]
}
```

## 状态码<a name="section38684899"></a>

**表 5**  返回消息说明

<a name="table37042451"></a>
<table><thead align="left"><tr id="row40505160"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p59692522"><a name="p59692522"></a><a name="p59692522"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p3256100"><a name="p3256100"></a><a name="p3256100"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row62417567"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22658179"><a name="p22658179"></a><a name="p22658179"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row9031982"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p60501950"><a name="p60501950"></a><a name="p60501950"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1710898"><a name="p1710898"></a><a name="p1710898"></a>Bad Request</p>
</td>
</tr>
<tr id="row15398085"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p39285387"><a name="p39285387"></a><a name="p39285387"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row50671481"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p10749328"><a name="p10749328"></a><a name="p10749328"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p65389202"><a name="p65389202"></a><a name="p65389202"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

