# 查询签名密钥列表<a name="ZH-CN_TOPIC_0000001082135211"></a>

## 功能介绍<a name="zh-cn_topic_0225568939_section59423210"></a>

查询所有签名密钥的信息。

## URI<a name="zh-cn_topic_0225568939_section65046848"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568939_table25351940"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568939_row16714936"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568939_p11732565"><a name="zh-cn_topic_0225568939_p11732565"></a><a name="zh-cn_topic_0225568939_p11732565"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568939_p10813690"><a name="zh-cn_topic_0225568939_p10813690"></a><a name="zh-cn_topic_0225568939_p10813690"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568939_row3493712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568939_p14555262"><a name="zh-cn_topic_0225568939_p14555262"></a><a name="zh-cn_topic_0225568939_p14555262"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568939_p38125613"><a name="zh-cn_topic_0225568939_p38125613"></a><a name="zh-cn_topic_0225568939_p38125613"></a>/v1/{project_id}/apigw/instances/{instance_id}/signs[?page_size, page_no, id, name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、name。

## 请求消息<a name="zh-cn_topic_0225568939_section48550723"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0225568939_table55384250"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568939_row4272454"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568939_p10524464"><a name="zh-cn_topic_0225568939_p10524464"></a><a name="zh-cn_topic_0225568939_p10524464"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.22%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568939_p47175238"><a name="zh-cn_topic_0225568939_p47175238"></a><a name="zh-cn_topic_0225568939_p47175238"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="22.189999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568939_p63097970"><a name="zh-cn_topic_0225568939_p63097970"></a><a name="zh-cn_topic_0225568939_p63097970"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.59%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568939_p10661913"><a name="zh-cn_topic_0225568939_p10661913"></a><a name="zh-cn_topic_0225568939_p10661913"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568939_row188211598505"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568939_p55878963"><a name="zh-cn_topic_0225568939_p55878963"></a><a name="zh-cn_topic_0225568939_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568939_p29902160"><a name="zh-cn_topic_0225568939_p29902160"></a><a name="zh-cn_topic_0225568939_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.189999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568939_p6155914"><a name="zh-cn_topic_0225568939_p6155914"></a><a name="zh-cn_topic_0225568939_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.59%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568939_p28867016"><a name="zh-cn_topic_0225568939_p28867016"></a><a name="zh-cn_topic_0225568939_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row13240155918509"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568939_p1780913159538"><a name="zh-cn_topic_0225568939_p1780913159538"></a><a name="zh-cn_topic_0225568939_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568939_p9809215115310"><a name="zh-cn_topic_0225568939_p9809215115310"></a><a name="zh-cn_topic_0225568939_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.189999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568939_p1280914152538"><a name="zh-cn_topic_0225568939_p1280914152538"></a><a name="zh-cn_topic_0225568939_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.59%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568939_p1880914157537"><a name="zh-cn_topic_0225568939_p1880914157537"></a><a name="zh-cn_topic_0225568939_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row58308645"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568939_p25379838"><a name="zh-cn_topic_0225568939_p25379838"></a><a name="zh-cn_topic_0225568939_p25379838"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568939_p42501003"><a name="zh-cn_topic_0225568939_p42501003"></a><a name="zh-cn_topic_0225568939_p42501003"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.189999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568939_p20029237"><a name="zh-cn_topic_0225568939_p20029237"></a><a name="zh-cn_topic_0225568939_p20029237"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.59%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568939_p11755491"><a name="zh-cn_topic_0225568939_p11755491"></a><a name="zh-cn_topic_0225568939_p11755491"></a>签名密钥编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row38690559"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568939_p46927599"><a name="zh-cn_topic_0225568939_p46927599"></a><a name="zh-cn_topic_0225568939_p46927599"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568939_p43039192"><a name="zh-cn_topic_0225568939_p43039192"></a><a name="zh-cn_topic_0225568939_p43039192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.189999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568939_p63622497"><a name="zh-cn_topic_0225568939_p63622497"></a><a name="zh-cn_topic_0225568939_p63622497"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.59%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568939_p53148594"><a name="zh-cn_topic_0225568939_p53148594"></a><a name="zh-cn_topic_0225568939_p53148594"></a>签名密钥名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row458525365119"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568939_p8585195325117"><a name="zh-cn_topic_0225568939_p8585195325117"></a><a name="zh-cn_topic_0225568939_p8585195325117"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568939_p95851539513"><a name="zh-cn_topic_0225568939_p95851539513"></a><a name="zh-cn_topic_0225568939_p95851539513"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="22.189999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568939_p358519531511"><a name="zh-cn_topic_0225568939_p358519531511"></a><a name="zh-cn_topic_0225568939_p358519531511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.59%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568939_p135851153155112"><a name="zh-cn_topic_0225568939_p135851153155112"></a><a name="zh-cn_topic_0225568939_p135851153155112"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0225568939_section40294460"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568939_table15236082"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568939_row62596037"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568939_p37114228"><a name="zh-cn_topic_0225568939_p37114228"></a><a name="zh-cn_topic_0225568939_p37114228"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568939_p53462516"><a name="zh-cn_topic_0225568939_p53462516"></a><a name="zh-cn_topic_0225568939_p53462516"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568939_p35496557"><a name="zh-cn_topic_0225568939_p35496557"></a><a name="zh-cn_topic_0225568939_p35496557"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568939_row56648838"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p25153127"><a name="zh-cn_topic_0225568939_p25153127"></a><a name="zh-cn_topic_0225568939_p25153127"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p24137401"><a name="zh-cn_topic_0225568939_p24137401"></a><a name="zh-cn_topic_0225568939_p24137401"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p8972451"><a name="zh-cn_topic_0225568939_p8972451"></a><a name="zh-cn_topic_0225568939_p8972451"></a>符合条件的签名密钥的数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row13643201"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p31357507"><a name="zh-cn_topic_0225568939_p31357507"></a><a name="zh-cn_topic_0225568939_p31357507"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p56930162"><a name="zh-cn_topic_0225568939_p56930162"></a><a name="zh-cn_topic_0225568939_p56930162"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p47940405"><a name="zh-cn_topic_0225568939_p47940405"></a><a name="zh-cn_topic_0225568939_p47940405"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row28810466"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p51946399"><a name="zh-cn_topic_0225568939_p51946399"></a><a name="zh-cn_topic_0225568939_p51946399"></a>signs</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p46908772"><a name="zh-cn_topic_0225568939_p46908772"></a><a name="zh-cn_topic_0225568939_p46908772"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p41514202"><a name="zh-cn_topic_0225568939_p41514202"></a><a name="zh-cn_topic_0225568939_p41514202"></a>本次查询到的签名密钥列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  signs参数说明

<a name="zh-cn_topic_0225568939_table7207208"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568939_row46987248"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568939_p47870772"><a name="zh-cn_topic_0225568939_p47870772"></a><a name="zh-cn_topic_0225568939_p47870772"></a><strong id="zh-cn_topic_0225568939_b28183768"><a name="zh-cn_topic_0225568939_b28183768"></a><a name="zh-cn_topic_0225568939_b28183768"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568939_p1183873"><a name="zh-cn_topic_0225568939_p1183873"></a><a name="zh-cn_topic_0225568939_p1183873"></a><strong id="zh-cn_topic_0225568939_b10654865"><a name="zh-cn_topic_0225568939_b10654865"></a><a name="zh-cn_topic_0225568939_b10654865"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568939_p57737722"><a name="zh-cn_topic_0225568939_p57737722"></a><a name="zh-cn_topic_0225568939_p57737722"></a><strong id="zh-cn_topic_0225568939_b49877454"><a name="zh-cn_topic_0225568939_b49877454"></a><a name="zh-cn_topic_0225568939_b49877454"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568939_row13541953"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p23156380"><a name="zh-cn_topic_0225568939_p23156380"></a><a name="zh-cn_topic_0225568939_p23156380"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p63727496"><a name="zh-cn_topic_0225568939_p63727496"></a><a name="zh-cn_topic_0225568939_p63727496"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p61653548"><a name="zh-cn_topic_0225568939_p61653548"></a><a name="zh-cn_topic_0225568939_p61653548"></a>签名密钥的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row18011027"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p49607103"><a name="zh-cn_topic_0225568939_p49607103"></a><a name="zh-cn_topic_0225568939_p49607103"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p58752440"><a name="zh-cn_topic_0225568939_p58752440"></a><a name="zh-cn_topic_0225568939_p58752440"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p61327205"><a name="zh-cn_topic_0225568939_p61327205"></a><a name="zh-cn_topic_0225568939_p61327205"></a>签名密钥的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row15073939"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p13029546"><a name="zh-cn_topic_0225568939_p13029546"></a><a name="zh-cn_topic_0225568939_p13029546"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p48760297"><a name="zh-cn_topic_0225568939_p48760297"></a><a name="zh-cn_topic_0225568939_p48760297"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p57270009"><a name="zh-cn_topic_0225568939_p57270009"></a><a name="zh-cn_topic_0225568939_p57270009"></a>签名密钥的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row45668039"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p8123667"><a name="zh-cn_topic_0225568939_p8123667"></a><a name="zh-cn_topic_0225568939_p8123667"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p54037251"><a name="zh-cn_topic_0225568939_p54037251"></a><a name="zh-cn_topic_0225568939_p54037251"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p14941183"><a name="zh-cn_topic_0225568939_p14941183"></a><a name="zh-cn_topic_0225568939_p14941183"></a>签名密钥的密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row252926"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p20487032"><a name="zh-cn_topic_0225568939_p20487032"></a><a name="zh-cn_topic_0225568939_p20487032"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p48836915"><a name="zh-cn_topic_0225568939_p48836915"></a><a name="zh-cn_topic_0225568939_p48836915"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p63476055"><a name="zh-cn_topic_0225568939_p63476055"></a><a name="zh-cn_topic_0225568939_p63476055"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row34413583"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p36036834"><a name="zh-cn_topic_0225568939_p36036834"></a><a name="zh-cn_topic_0225568939_p36036834"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p33302450"><a name="zh-cn_topic_0225568939_p33302450"></a><a name="zh-cn_topic_0225568939_p33302450"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p13143910"><a name="zh-cn_topic_0225568939_p13143910"></a><a name="zh-cn_topic_0225568939_p13143910"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row13274195918612"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568939_p52361752033"><a name="zh-cn_topic_0225568939_p52361752033"></a><a name="zh-cn_topic_0225568939_p52361752033"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568939_p12236185032"><a name="zh-cn_topic_0225568939_p12236185032"></a><a name="zh-cn_topic_0225568939_p12236185032"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568939_p17236557312"><a name="zh-cn_topic_0225568939_p17236557312"></a><a name="zh-cn_topic_0225568939_p17236557312"></a>绑定的API数量</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"signs": [{
		"name": "signature01",
		"sign_key": "abcd_1234",
		"sign_secret": "******",
		"id": "3a793b65a9034bdfae08924f149bfb4a",
		"create_time": "2018-02-06T12:17:36Z",
		"update_time": "2018-02-07T02:00:27.964766Z",
                "bind_num":1
	},
	{
		"name": "sada",
		"sign_key": "asdasdasdasda",
		"sign_secret": "******",
		"id": "51ce490901f4411fa54eb06d33bd7218",
		"create_time": "2018-02-06T11:53:08Z",
		"update_time": "2018-02-06T11:53:08Z",
                "bind_num":1
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568939_section34303324"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568939_table65819597"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568939_row38654893"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568939_p44038594"><a name="zh-cn_topic_0225568939_p44038594"></a><a name="zh-cn_topic_0225568939_p44038594"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568939_p26098194"><a name="zh-cn_topic_0225568939_p26098194"></a><a name="zh-cn_topic_0225568939_p26098194"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568939_row33775564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568939_p51466179"><a name="zh-cn_topic_0225568939_p51466179"></a><a name="zh-cn_topic_0225568939_p51466179"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568939_p8010999"><a name="zh-cn_topic_0225568939_p8010999"></a><a name="zh-cn_topic_0225568939_p8010999"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row4990131"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568939_p1547468"><a name="zh-cn_topic_0225568939_p1547468"></a><a name="zh-cn_topic_0225568939_p1547468"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568939_p58236118"><a name="zh-cn_topic_0225568939_p58236118"></a><a name="zh-cn_topic_0225568939_p58236118"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row54363021"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568939_p41328579"><a name="zh-cn_topic_0225568939_p41328579"></a><a name="zh-cn_topic_0225568939_p41328579"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568939_p59280573"><a name="zh-cn_topic_0225568939_p59280573"></a><a name="zh-cn_topic_0225568939_p59280573"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568939_row63763111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568939_p64538371"><a name="zh-cn_topic_0225568939_p64538371"></a><a name="zh-cn_topic_0225568939_p64538371"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568939_p60225559"><a name="zh-cn_topic_0225568939_p60225559"></a><a name="zh-cn_topic_0225568939_p60225559"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

