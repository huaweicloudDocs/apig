# 更新VPC通道<a name="ZH-CN_TOPIC_0000001082221229"></a>

## 功能介绍<a name="zh-cn_topic_0118924574_section173482301428"></a>

更新指定VPC通道的参数。

## URI<a name="zh-cn_topic_0118924574_section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924574_table1439319294431"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924574_row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924574_p14361448204314"><a name="zh-cn_topic_0118924574_p14361448204314"></a><a name="zh-cn_topic_0118924574_p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924574_p1936174864316"><a name="zh-cn_topic_0118924574_p1936174864316"></a><a name="zh-cn_topic_0118924574_p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924574_row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924574_p1236111482435"><a name="zh-cn_topic_0118924574_p1236111482435"></a><a name="zh-cn_topic_0118924574_p1236111482435"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924574_p11361848184318"><a name="zh-cn_topic_0118924574_p11361848184318"></a><a name="zh-cn_topic_0118924574_p11361848184318"></a>/v1.0/apigw/vpc-channels/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924574_table18784710"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924574_row37287554"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924574_p393051"><a name="zh-cn_topic_0118924574_p393051"></a><a name="zh-cn_topic_0118924574_p393051"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924574_p31837140"><a name="zh-cn_topic_0118924574_p31837140"></a><a name="zh-cn_topic_0118924574_p31837140"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924574_p28671509"><a name="zh-cn_topic_0118924574_p28671509"></a><a name="zh-cn_topic_0118924574_p28671509"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924574_p40690887"><a name="zh-cn_topic_0118924574_p40690887"></a><a name="zh-cn_topic_0118924574_p40690887"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924574_row7627537"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p13850780"><a name="zh-cn_topic_0118924574_p13850780"></a><a name="zh-cn_topic_0118924574_p13850780"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p48171408"><a name="zh-cn_topic_0118924574_p48171408"></a><a name="zh-cn_topic_0118924574_p48171408"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p9569939"><a name="zh-cn_topic_0118924574_p9569939"></a><a name="zh-cn_topic_0118924574_p9569939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p36967632"><a name="zh-cn_topic_0118924574_p36967632"></a><a name="zh-cn_topic_0118924574_p36967632"></a>VPC通道的编号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924574_section73637302425"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924574_table1136319301429"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924574_row748813306425"><th class="cellrowborder" valign="top" width="15.46154615461546%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924574_p9488143084210"><a name="zh-cn_topic_0118924574_p9488143084210"></a><a name="zh-cn_topic_0118924574_p9488143084210"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924574_p148843017426"><a name="zh-cn_topic_0118924574_p148843017426"></a><a name="zh-cn_topic_0118924574_p148843017426"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924574_p9488830164214"><a name="zh-cn_topic_0118924574_p9488830164214"></a><a name="zh-cn_topic_0118924574_p9488830164214"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924574_p1048813014421"><a name="zh-cn_topic_0118924574_p1048813014421"></a><a name="zh-cn_topic_0118924574_p1048813014421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924574_row2012102914318"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p9051148"><a name="zh-cn_topic_0118924574_p9051148"></a><a name="zh-cn_topic_0118924574_p9051148"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p62054412"><a name="zh-cn_topic_0118924574_p62054412"></a><a name="zh-cn_topic_0118924574_p62054412"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p12740424339"><a name="zh-cn_topic_0118924574_p12740424339"></a><a name="zh-cn_topic_0118924574_p12740424339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p13931103183318"><a name="zh-cn_topic_0118924574_p13931103183318"></a><a name="zh-cn_topic_0118924574_p13931103183318"></a>VPC通道的名称。</p>
<p id="zh-cn_topic_0118924574_p37858559"><a name="zh-cn_topic_0118924574_p37858559"></a><a name="zh-cn_topic_0118924574_p37858559"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“-”、“_”组成，且只能以英文或中文开头。</p>
<div class="note" id="zh-cn_topic_0118924574_note690163615371"><a name="zh-cn_topic_0118924574_note690163615371"></a><a name="zh-cn_topic_0118924574_note690163615371"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118924574_p09053643719"><a name="zh-cn_topic_0118924574_p09053643719"></a><a name="zh-cn_topic_0118924574_p09053643719"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row81211629183115"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p4509019"><a name="zh-cn_topic_0118924574_p4509019"></a><a name="zh-cn_topic_0118924574_p4509019"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p29686297"><a name="zh-cn_topic_0118924574_p29686297"></a><a name="zh-cn_topic_0118924574_p29686297"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p82741042143312"><a name="zh-cn_topic_0118924574_p82741042143312"></a><a name="zh-cn_topic_0118924574_p82741042143312"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p96821415145419"><a name="zh-cn_topic_0118924574_p96821415145419"></a><a name="zh-cn_topic_0118924574_p96821415145419"></a>VPC通道的类型。</p>
<a name="zh-cn_topic_0118924574_ul168321565414"></a><a name="zh-cn_topic_0118924574_ul168321565414"></a><ul id="zh-cn_topic_0118924574_ul168321565414"><li>2：API网关内置支持负载均衡功能的快速通道类型</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row469315159546"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p4697171515412"><a name="zh-cn_topic_0118924574_p4697171515412"></a><a name="zh-cn_topic_0118924574_p4697171515412"></a>member_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p1370151513547"><a name="zh-cn_topic_0118924574_p1370151513547"></a><a name="zh-cn_topic_0118924574_p1370151513547"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p16703151535416"><a name="zh-cn_topic_0118924574_p16703151535416"></a><a name="zh-cn_topic_0118924574_p16703151535416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p1770651512541"><a name="zh-cn_topic_0118924574_p1770651512541"></a><a name="zh-cn_topic_0118924574_p1770651512541"></a>VPC通道的成员类型。</p>
<a name="zh-cn_topic_0118924574_ul1570617157543"></a><a name="zh-cn_topic_0118924574_ul1570617157543"></a><ul id="zh-cn_topic_0118924574_ul1570617157543"><li>ip（暂不支持）</li><li>instance</li></ul>
<p id="zh-cn_topic_0118924574_p87151615115419"><a name="zh-cn_topic_0118924574_p87151615115419"></a><a name="zh-cn_topic_0118924574_p87151615115419"></a>仅VPC通道类型为2时有效，缺省为instance。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row1612192923111"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p49099023"><a name="zh-cn_topic_0118924574_p49099023"></a><a name="zh-cn_topic_0118924574_p49099023"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p17597936"><a name="zh-cn_topic_0118924574_p17597936"></a><a name="zh-cn_topic_0118924574_p17597936"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p929014217338"><a name="zh-cn_topic_0118924574_p929014217338"></a><a name="zh-cn_topic_0118924574_p929014217338"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p49461931193318"><a name="zh-cn_topic_0118924574_p49461931193318"></a><a name="zh-cn_topic_0118924574_p49461931193318"></a>VPC通道中主机的端口号。</p>
<p id="zh-cn_topic_0118924574_p1373317153543"><a name="zh-cn_topic_0118924574_p1373317153543"></a><a name="zh-cn_topic_0118924574_p1373317153543"></a>取值范围1 ~ 65535，仅VPC通道类型为2时有效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row17121132912318"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p192983401416"><a name="zh-cn_topic_0118924574_p192983401416"></a><a name="zh-cn_topic_0118924574_p192983401416"></a>balance_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p182985416144"><a name="zh-cn_topic_0118924574_p182985416144"></a><a name="zh-cn_topic_0118924574_p182985416144"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p6290114214331"><a name="zh-cn_topic_0118924574_p6290114214331"></a><a name="zh-cn_topic_0118924574_p6290114214331"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p2748101511544"><a name="zh-cn_topic_0118924574_p2748101511544"></a><a name="zh-cn_topic_0118924574_p2748101511544"></a>分发算法。</p>
<a name="zh-cn_topic_0118924574_ul1374871511544"></a><a name="zh-cn_topic_0118924574_ul1374871511544"></a><ul id="zh-cn_topic_0118924574_ul1374871511544"><li>1：加权轮询（wrr）</li><li>2：加权最少连接（wleastconn）</li><li>3：源地址哈希（source）</li><li>4：URI哈希（uri）</li></ul>
<p id="zh-cn_topic_0118924574_p5946153116333"><a name="zh-cn_topic_0118924574_p5946153116333"></a><a name="zh-cn_topic_0118924574_p5946153116333"></a>仅VPC通道类型为2时有效，缺省为1。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row91212298312"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p8845107161418"><a name="zh-cn_topic_0118924574_p8845107161418"></a><a name="zh-cn_topic_0118924574_p8845107161418"></a>vpc_health_config</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p188451179141"><a name="zh-cn_topic_0118924574_p188451179141"></a><a name="zh-cn_topic_0118924574_p188451179141"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p122908425332"><a name="zh-cn_topic_0118924574_p122908425332"></a><a name="zh-cn_topic_0118924574_p122908425332"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p8946531183318"><a name="zh-cn_topic_0118924574_p8946531183318"></a><a name="zh-cn_topic_0118924574_p8946531183318"></a>健康检查详情，仅VPC通道类型为2时有效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row1949584023816"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p54951240193817"><a name="zh-cn_topic_0118924574_p54951240193817"></a><a name="zh-cn_topic_0118924574_p54951240193817"></a>vpc_instances</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p249574012387"><a name="zh-cn_topic_0118924574_p249574012387"></a><a name="zh-cn_topic_0118924574_p249574012387"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p7495134011385"><a name="zh-cn_topic_0118924574_p7495134011385"></a><a name="zh-cn_topic_0118924574_p7495134011385"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p14959403387"><a name="zh-cn_topic_0118924574_p14959403387"></a><a name="zh-cn_topic_0118924574_p14959403387"></a>后端实例列表，VPC通道类型为1时，有且仅有1个后端实例。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  健康检查详情

<a name="zh-cn_topic_0118924574_table56131171473"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924574_row1561341712474"><th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924574_p11613171794715"><a name="zh-cn_topic_0118924574_p11613171794715"></a><a name="zh-cn_topic_0118924574_p11613171794715"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.131313131313133%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924574_p1461341719471"><a name="zh-cn_topic_0118924574_p1461341719471"></a><a name="zh-cn_topic_0118924574_p1461341719471"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.131313131313133%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924574_p1361310173475"><a name="zh-cn_topic_0118924574_p1361310173475"></a><a name="zh-cn_topic_0118924574_p1361310173475"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.58585858585859%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924574_p1962861718474"><a name="zh-cn_topic_0118924574_p1962861718474"></a><a name="zh-cn_topic_0118924574_p1962861718474"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924574_row46281317124714"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p1562871714717"><a name="zh-cn_topic_0118924574_p1562871714717"></a><a name="zh-cn_topic_0118924574_p1562871714717"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p146282176479"><a name="zh-cn_topic_0118924574_p146282176479"></a><a name="zh-cn_topic_0118924574_p146282176479"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p1862819174475"><a name="zh-cn_topic_0118924574_p1862819174475"></a><a name="zh-cn_topic_0118924574_p1862819174475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><div class="p" id="zh-cn_topic_0118924574_p17838131515411"><a name="zh-cn_topic_0118924574_p17838131515411"></a><a name="zh-cn_topic_0118924574_p17838131515411"></a>使用以下协议，对VPC中主机执行健康检查。<a name="zh-cn_topic_0118924574_ul19904951155719"></a><a name="zh-cn_topic_0118924574_ul19904951155719"></a><ul id="zh-cn_topic_0118924574_ul19904951155719"><li>TCP</li><li>HTTP</li><li>HTTPS</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row7628217124717"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p0628171711477"><a name="zh-cn_topic_0118924574_p0628171711477"></a><a name="zh-cn_topic_0118924574_p0628171711477"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p1782432775013"><a name="zh-cn_topic_0118924574_p1782432775013"></a><a name="zh-cn_topic_0118924574_p1782432775013"></a>protocol = http时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p10644017184710"><a name="zh-cn_topic_0118924574_p10644017184710"></a><a name="zh-cn_topic_0118924574_p10644017184710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p15591010195011"><a name="zh-cn_topic_0118924574_p15591010195011"></a><a name="zh-cn_topic_0118924574_p15591010195011"></a>健康检查时的目标路径。</p>
<div class="note" id="zh-cn_topic_0118924574_note38431529153919"><a name="zh-cn_topic_0118924574_note38431529153919"></a><a name="zh-cn_topic_0118924574_note38431529153919"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118924574_p18843122918398"><a name="zh-cn_topic_0118924574_p18843122918398"></a><a name="zh-cn_topic_0118924574_p18843122918398"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row10644151704717"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p46440172472"><a name="zh-cn_topic_0118924574_p46440172472"></a><a name="zh-cn_topic_0118924574_p46440172472"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p14644181754720"><a name="zh-cn_topic_0118924574_p14644181754720"></a><a name="zh-cn_topic_0118924574_p14644181754720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p19644617104710"><a name="zh-cn_topic_0118924574_p19644617104710"></a><a name="zh-cn_topic_0118924574_p19644617104710"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p198780155542"><a name="zh-cn_topic_0118924574_p198780155542"></a><a name="zh-cn_topic_0118924574_p198780155542"></a>健康检查的目标端口，缺省时为VPC中主机的端口号。</p>
<p id="zh-cn_topic_0118924574_p1887861565412"><a name="zh-cn_topic_0118924574_p1887861565412"></a><a name="zh-cn_topic_0118924574_p1887861565412"></a>取值范围1 ~ 65535。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row56601917164716"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p76604177474"><a name="zh-cn_topic_0118924574_p76604177474"></a><a name="zh-cn_topic_0118924574_p76604177474"></a>threshold_normal</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p4660117134717"><a name="zh-cn_topic_0118924574_p4660117134717"></a><a name="zh-cn_topic_0118924574_p4660117134717"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p196608172477"><a name="zh-cn_topic_0118924574_p196608172477"></a><a name="zh-cn_topic_0118924574_p196608172477"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p1315411125313"><a name="zh-cn_topic_0118924574_p1315411125313"></a><a name="zh-cn_topic_0118924574_p1315411125313"></a>正常阈值。</p>
<p id="zh-cn_topic_0118924574_p28941515105412"><a name="zh-cn_topic_0118924574_p28941515105412"></a><a name="zh-cn_topic_0118924574_p28941515105412"></a>判定VPC通道中主机正常的依据为：连续检查<em id="zh-cn_topic_0118924574_i421224922811"><a name="zh-cn_topic_0118924574_i421224922811"></a><a name="zh-cn_topic_0118924574_i421224922811"></a>x</em>成功，x为您设置的正常阈值。</p>
<p id="zh-cn_topic_0118924574_p148984158547"><a name="zh-cn_topic_0118924574_p148984158547"></a><a name="zh-cn_topic_0118924574_p148984158547"></a>取值范围2 ~ 10</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row1266061794714"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p196601017124713"><a name="zh-cn_topic_0118924574_p196601017124713"></a><a name="zh-cn_topic_0118924574_p196601017124713"></a>threshold_abnormal</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p206601417154713"><a name="zh-cn_topic_0118924574_p206601417154713"></a><a name="zh-cn_topic_0118924574_p206601417154713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p56601117104714"><a name="zh-cn_topic_0118924574_p56601117104714"></a><a name="zh-cn_topic_0118924574_p56601117104714"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p1091261514547"><a name="zh-cn_topic_0118924574_p1091261514547"></a><a name="zh-cn_topic_0118924574_p1091261514547"></a>异常阙值。</p>
<p id="zh-cn_topic_0118924574_p79167352531"><a name="zh-cn_topic_0118924574_p79167352531"></a><a name="zh-cn_topic_0118924574_p79167352531"></a>判定VPC通道中主机异常的依据为：连续检查<em id="zh-cn_topic_0118924574_i37296135294"><a name="zh-cn_topic_0118924574_i37296135294"></a><a name="zh-cn_topic_0118924574_i37296135294"></a>x失败</em>，x为您设置的异常阈值。</p>
<p id="zh-cn_topic_0118924574_p1591621511546"><a name="zh-cn_topic_0118924574_p1591621511546"></a><a name="zh-cn_topic_0118924574_p1591621511546"></a>取值范围2 ~ 10。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row7675121714474"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p66751817104717"><a name="zh-cn_topic_0118924574_p66751817104717"></a><a name="zh-cn_topic_0118924574_p66751817104717"></a>time_out</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p367521764713"><a name="zh-cn_topic_0118924574_p367521764713"></a><a name="zh-cn_topic_0118924574_p367521764713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p36751017184719"><a name="zh-cn_topic_0118924574_p36751017184719"></a><a name="zh-cn_topic_0118924574_p36751017184719"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p1511311311562"><a name="zh-cn_topic_0118924574_p1511311311562"></a><a name="zh-cn_topic_0118924574_p1511311311562"></a>超时时间：检查期间，无响应的时间，单位为秒。必须小于time_interval字段取值。</p>
<p id="zh-cn_topic_0118924574_p6100155285117"><a name="zh-cn_topic_0118924574_p6100155285117"></a><a name="zh-cn_topic_0118924574_p6100155285117"></a>取值范围2 ~ 30。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row146754172472"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p2675171734717"><a name="zh-cn_topic_0118924574_p2675171734717"></a><a name="zh-cn_topic_0118924574_p2675171734717"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p18675111734711"><a name="zh-cn_topic_0118924574_p18675111734711"></a><a name="zh-cn_topic_0118924574_p18675111734711"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p26751317174716"><a name="zh-cn_topic_0118924574_p26751317174716"></a><a name="zh-cn_topic_0118924574_p26751317174716"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p958312467512"><a name="zh-cn_topic_0118924574_p958312467512"></a><a name="zh-cn_topic_0118924574_p958312467512"></a>间隔时间：连续两次检查的间隔时间，单位为秒。必须大于time_out字段取值。</p>
<p id="zh-cn_topic_0118924574_p106781254125110"><a name="zh-cn_topic_0118924574_p106781254125110"></a><a name="zh-cn_topic_0118924574_p106781254125110"></a>取值范围5 ~ 300。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row927095444819"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p1027035412488"><a name="zh-cn_topic_0118924574_p1027035412488"></a><a name="zh-cn_topic_0118924574_p1027035412488"></a>http_code</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p7270195418482"><a name="zh-cn_topic_0118924574_p7270195418482"></a><a name="zh-cn_topic_0118924574_p7270195418482"></a>protocol = http时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p9270135474815"><a name="zh-cn_topic_0118924574_p9270135474815"></a><a name="zh-cn_topic_0118924574_p9270135474815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p15281310185519"><a name="zh-cn_topic_0118924574_p15281310185519"></a><a name="zh-cn_topic_0118924574_p15281310185519"></a>检查目标HTTP响应时，判断成功使用的HTTP响应码。</p>
<p id="zh-cn_topic_0118924574_p1144417511111"><a name="zh-cn_topic_0118924574_p1144417511111"></a><a name="zh-cn_topic_0118924574_p1144417511111"></a>取值范围为100到599之前的任意整数值，支持如下三种格式：</p>
<a name="zh-cn_topic_0118924574_ul343965120114"></a><a name="zh-cn_topic_0118924574_ul343965120114"></a><ul id="zh-cn_topic_0118924574_ul343965120114"><li>多个值，如：200,201,202</li><li>一系列值，如：200-299</li><li>组合值，如：201,202,210-299</li></ul>
</td>
</tr>
</tbody>
</table>

**表 5**  后端实例列表

<a name="zh-cn_topic_0118924574_table6144132024717"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924574_row15144122054719"><th class="cellrowborder" valign="top" width="15.46154615461546%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924574_p41441620124712"><a name="zh-cn_topic_0118924574_p41441620124712"></a><a name="zh-cn_topic_0118924574_p41441620124712"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924574_p14144820104719"><a name="zh-cn_topic_0118924574_p14144820104719"></a><a name="zh-cn_topic_0118924574_p14144820104719"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924574_p71601720114710"><a name="zh-cn_topic_0118924574_p71601720114710"></a><a name="zh-cn_topic_0118924574_p71601720114710"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924574_p1716072074719"><a name="zh-cn_topic_0118924574_p1716072074719"></a><a name="zh-cn_topic_0118924574_p1716072074719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924574_row816019209472"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p11160192010473"><a name="zh-cn_topic_0118924574_p11160192010473"></a><a name="zh-cn_topic_0118924574_p11160192010473"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p916052018474"><a name="zh-cn_topic_0118924574_p916052018474"></a><a name="zh-cn_topic_0118924574_p916052018474"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p1916032024714"><a name="zh-cn_topic_0118924574_p1916032024714"></a><a name="zh-cn_topic_0118924574_p1916032024714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p3261416125418"><a name="zh-cn_topic_0118924574_p3261416125418"></a><a name="zh-cn_topic_0118924574_p3261416125418"></a>后端实例的名称。</p>
<p id="zh-cn_topic_0118924574_p1029151665411"><a name="zh-cn_topic_0118924574_p1029151665411"></a><a name="zh-cn_topic_0118924574_p1029151665411"></a>支持汉字，英文，数字，“-”,“_”,“.”，1 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0118924574_note329016115419"><a name="zh-cn_topic_0118924574_note329016115419"></a><a name="zh-cn_topic_0118924574_note329016115419"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118924574_p03081612549"><a name="zh-cn_topic_0118924574_p03081612549"></a><a name="zh-cn_topic_0118924574_p03081612549"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row171743206475"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p31740206478"><a name="zh-cn_topic_0118924574_p31740206478"></a><a name="zh-cn_topic_0118924574_p31740206478"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p1174162084716"><a name="zh-cn_topic_0118924574_p1174162084716"></a><a name="zh-cn_topic_0118924574_p1174162084716"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p1217432012470"><a name="zh-cn_topic_0118924574_p1217432012470"></a><a name="zh-cn_topic_0118924574_p1217432012470"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p3435162546"><a name="zh-cn_topic_0118924574_p3435162546"></a><a name="zh-cn_topic_0118924574_p3435162546"></a>后端实例的编号。</p>
<p id="zh-cn_topic_0118924574_p118250135519"><a name="zh-cn_topic_0118924574_p118250135519"></a><a name="zh-cn_topic_0118924574_p118250135519"></a>支持英文，数字，“-”,“_”，1 ~ 64字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row4191162015475"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924574_p17191112094711"><a name="zh-cn_topic_0118924574_p17191112094711"></a><a name="zh-cn_topic_0118924574_p17191112094711"></a>weight</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924574_p131911920174712"><a name="zh-cn_topic_0118924574_p131911920174712"></a><a name="zh-cn_topic_0118924574_p131911920174712"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924574_p161911220194720"><a name="zh-cn_topic_0118924574_p161911220194720"></a><a name="zh-cn_topic_0118924574_p161911220194720"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924574_p1133512255618"><a name="zh-cn_topic_0118924574_p1133512255618"></a><a name="zh-cn_topic_0118924574_p1133512255618"></a>权重值。</p>
<p id="zh-cn_topic_0118924574_p66216167546"><a name="zh-cn_topic_0118924574_p66216167546"></a><a name="zh-cn_topic_0118924574_p66216167546"></a>权重值越大，转发到该后端实例的请求数量越多。</p>
<p id="zh-cn_topic_0118924574_p14631916155415"><a name="zh-cn_topic_0118924574_p14631916155415"></a><a name="zh-cn_topic_0118924574_p14631916155415"></a>取值范围1 ~ 100，仅VPC通道类型为2时有效。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "balance_strategy": 1,
  "name": "vpc_001",
  "port": 15565,
  "type": 2,
  "member_type": "instance",
  "vpc_health_config": {
    "http_code": "205",
    "path": "/hc",
    "port": 15563,
    "protocol": "http",
    "threshold_abnormal": 5,
    "threshold_normal": 5,
    "time_interval": 200,
    "time_out": 30
  },
  "vpc_instances": [
    {
      "instance_id": "instance01",
      "instance_name": "instance_name01",
      "weight": 10
    }
  ]
}
```

## 响应消息<a name="zh-cn_topic_0118924574_section9395153012420"></a>

**表 6**  参数说明

<a name="zh-cn_topic_0118924574_table7395123013420"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924574_row114881330104215"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924574_p19488153019429"><a name="zh-cn_topic_0118924574_p19488153019429"></a><a name="zh-cn_topic_0118924574_p19488153019429"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924574_p248853014422"><a name="zh-cn_topic_0118924574_p248853014422"></a><a name="zh-cn_topic_0118924574_p248853014422"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924574_p64882308421"><a name="zh-cn_topic_0118924574_p64882308421"></a><a name="zh-cn_topic_0118924574_p64882308421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924574_row12488203074215"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p1448813305421"><a name="zh-cn_topic_0118924574_p1448813305421"></a><a name="zh-cn_topic_0118924574_p1448813305421"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p18488163024218"><a name="zh-cn_topic_0118924574_p18488163024218"></a><a name="zh-cn_topic_0118924574_p18488163024218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p25696563"><a name="zh-cn_topic_0118924574_p25696563"></a><a name="zh-cn_topic_0118924574_p25696563"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row17488133012421"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p1585685914587"><a name="zh-cn_topic_0118924574_p1585685914587"></a><a name="zh-cn_topic_0118924574_p1585685914587"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p4488183013424"><a name="zh-cn_topic_0118924574_p4488183013424"></a><a name="zh-cn_topic_0118924574_p4488183013424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p60351493"><a name="zh-cn_topic_0118924574_p60351493"></a><a name="zh-cn_topic_0118924574_p60351493"></a>VPC通道的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row748812305426"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p19871155912585"><a name="zh-cn_topic_0118924574_p19871155912585"></a><a name="zh-cn_topic_0118924574_p19871155912585"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p64881305424"><a name="zh-cn_topic_0118924574_p64881305424"></a><a name="zh-cn_topic_0118924574_p64881305424"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p917613163546"><a name="zh-cn_topic_0118924574_p917613163546"></a><a name="zh-cn_topic_0118924574_p917613163546"></a>VPC通道的类型。</p>
<a name="zh-cn_topic_0118924574_ul141791016115417"></a><a name="zh-cn_topic_0118924574_ul141791016115417"></a><ul id="zh-cn_topic_0118924574_ul141791016115417"><li>2：API网关内置支持负载均衡功能的快速通道类型</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row7187121617547"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p91911016155413"><a name="zh-cn_topic_0118924574_p91911016155413"></a><a name="zh-cn_topic_0118924574_p91911016155413"></a>member_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p181945166544"><a name="zh-cn_topic_0118924574_p181945166544"></a><a name="zh-cn_topic_0118924574_p181945166544"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p5196141685410"><a name="zh-cn_topic_0118924574_p5196141685410"></a><a name="zh-cn_topic_0118924574_p5196141685410"></a>VPC通道的成员类型。</p>
<a name="zh-cn_topic_0118924574_ul9198116125412"></a><a name="zh-cn_topic_0118924574_ul9198116125412"></a><ul id="zh-cn_topic_0118924574_ul9198116125412"><li>ip（暂不支持）</li><li>instance</li></ul>
<p id="zh-cn_topic_0118924574_p10206916205413"><a name="zh-cn_topic_0118924574_p10206916205413"></a><a name="zh-cn_topic_0118924574_p10206916205413"></a>仅VPC通道类型为2时有效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row138095017017"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p14809406014"><a name="zh-cn_topic_0118924574_p14809406014"></a><a name="zh-cn_topic_0118924574_p14809406014"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p5809305016"><a name="zh-cn_topic_0118924574_p5809305016"></a><a name="zh-cn_topic_0118924574_p5809305016"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p12663581620"><a name="zh-cn_topic_0118924574_p12663581620"></a><a name="zh-cn_topic_0118924574_p12663581620"></a>VPC通道的状态。</p>
<a name="zh-cn_topic_0118924574_ul15791839184416"></a><a name="zh-cn_topic_0118924574_ul15791839184416"></a><ul id="zh-cn_topic_0118924574_ul15791839184416"><li>1：正常</li><li>2：异常</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row31998111201"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p151995112018"><a name="zh-cn_topic_0118924574_p151995112018"></a><a name="zh-cn_topic_0118924574_p151995112018"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p15199011306"><a name="zh-cn_topic_0118924574_p15199011306"></a><a name="zh-cn_topic_0118924574_p15199011306"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p16681305"><a name="zh-cn_topic_0118924574_p16681305"></a><a name="zh-cn_topic_0118924574_p16681305"></a>VPC通道中主机的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row05591488016"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p135594817016"><a name="zh-cn_topic_0118924574_p135594817016"></a><a name="zh-cn_topic_0118924574_p135594817016"></a>balance_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p14559178309"><a name="zh-cn_topic_0118924574_p14559178309"></a><a name="zh-cn_topic_0118924574_p14559178309"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p22981401418"><a name="zh-cn_topic_0118924574_p22981401418"></a><a name="zh-cn_topic_0118924574_p22981401418"></a>分发算法。</p>
<a name="zh-cn_topic_0118924574_ul31881612450"></a><a name="zh-cn_topic_0118924574_ul31881612450"></a><ul id="zh-cn_topic_0118924574_ul31881612450"><li>1：加权轮询（wrr）</li><li>2：加权最少连接（wleastconn）</li><li>3：源地址哈希（source）</li><li>4：URI哈希（uri）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row109961654185911"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924574_p19996135415590"><a name="zh-cn_topic_0118924574_p19996135415590"></a><a name="zh-cn_topic_0118924574_p19996135415590"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924574_p20996554195919"><a name="zh-cn_topic_0118924574_p20996554195919"></a><a name="zh-cn_topic_0118924574_p20996554195919"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924574_p198451273146"><a name="zh-cn_topic_0118924574_p198451273146"></a><a name="zh-cn_topic_0118924574_p198451273146"></a>VPC通道的创建时间。</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "name": "vpc_001",
  "type": 2,
  "member_type": "instance",
  "port": 15565,
  "balance_strategy": 1,
  "id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
  "create_time": "2018-07-27T12:30:48.027484Z",
  "status": 1
}
```

## 状态码<a name="zh-cn_topic_0118924574_section338043011426"></a>

**表 7**  返回消息说明

<a name="zh-cn_topic_0118924574_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924574_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924574_p174881730194216"><a name="zh-cn_topic_0118924574_p174881730194216"></a><a name="zh-cn_topic_0118924574_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924574_p848863018429"><a name="zh-cn_topic_0118924574_p848863018429"></a><a name="zh-cn_topic_0118924574_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924574_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924574_p7488163084211"><a name="zh-cn_topic_0118924574_p7488163084211"></a><a name="zh-cn_topic_0118924574_p7488163084211"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924574_p948803015424"><a name="zh-cn_topic_0118924574_p948803015424"></a><a name="zh-cn_topic_0118924574_p948803015424"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924574_p14488113015426"><a name="zh-cn_topic_0118924574_p14488113015426"></a><a name="zh-cn_topic_0118924574_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924574_p164881130154211"><a name="zh-cn_topic_0118924574_p164881130154211"></a><a name="zh-cn_topic_0118924574_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924574_p24883304428"><a name="zh-cn_topic_0118924574_p24883304428"></a><a name="zh-cn_topic_0118924574_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924574_p1848810308429"><a name="zh-cn_topic_0118924574_p1848810308429"></a><a name="zh-cn_topic_0118924574_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924574_p6488133064210"><a name="zh-cn_topic_0118924574_p6488133064210"></a><a name="zh-cn_topic_0118924574_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924574_p10488193018426"><a name="zh-cn_topic_0118924574_p10488193018426"></a><a name="zh-cn_topic_0118924574_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924574_p144883304428"><a name="zh-cn_topic_0118924574_p144883304428"></a><a name="zh-cn_topic_0118924574_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924574_p4488103094212"><a name="zh-cn_topic_0118924574_p4488103094212"></a><a name="zh-cn_topic_0118924574_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924574_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924574_p17488163014423"><a name="zh-cn_topic_0118924574_p17488163014423"></a><a name="zh-cn_topic_0118924574_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924574_p048813014216"><a name="zh-cn_topic_0118924574_p048813014216"></a><a name="zh-cn_topic_0118924574_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

