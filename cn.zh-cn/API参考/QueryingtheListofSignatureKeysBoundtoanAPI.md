# 查看API绑定的签名密钥列表<a name="ZH-CN_TOPIC_0000001082221223"></a>

## 功能介绍<a name="zh-cn_topic_0118924556_section5517300"></a>

查询某个API绑定的签名密钥列表。每个API在每个环境上应该最多只会绑定一个签名密钥。

## URI<a name="zh-cn_topic_0118924556_section49655705"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924556_table20364239"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924556_row13477612"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924556_p17944826"><a name="zh-cn_topic_0118924556_p17944826"></a><a name="zh-cn_topic_0118924556_p17944826"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924556_p44244812"><a name="zh-cn_topic_0118924556_p44244812"></a><a name="zh-cn_topic_0118924556_p44244812"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924556_row27060043"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924556_p44379870"><a name="zh-cn_topic_0118924556_p44379870"></a><a name="zh-cn_topic_0118924556_p44379870"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924556_p37999726"><a name="zh-cn_topic_0118924556_p37999726"></a><a name="zh-cn_topic_0118924556_p37999726"></a>/v1.0/apigw/sign-bindings/binded-signs[?page_no, page_size, api_id, sign_id, sign_name,env_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：api\_id、sign\_id、sign\_name、env\_id、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924556_table11837592"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924556_row47015449"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924556_p50155053"><a name="zh-cn_topic_0118924556_p50155053"></a><a name="zh-cn_topic_0118924556_p50155053"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924556_p36027493"><a name="zh-cn_topic_0118924556_p36027493"></a><a name="zh-cn_topic_0118924556_p36027493"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924556_p32545834"><a name="zh-cn_topic_0118924556_p32545834"></a><a name="zh-cn_topic_0118924556_p32545834"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924556_p18966883"><a name="zh-cn_topic_0118924556_p18966883"></a><a name="zh-cn_topic_0118924556_p18966883"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924556_row59922553"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924556_p21888595"><a name="zh-cn_topic_0118924556_p21888595"></a><a name="zh-cn_topic_0118924556_p21888595"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924556_p28145753"><a name="zh-cn_topic_0118924556_p28145753"></a><a name="zh-cn_topic_0118924556_p28145753"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924556_p65213557"><a name="zh-cn_topic_0118924556_p65213557"></a><a name="zh-cn_topic_0118924556_p65213557"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924556_p47806732"><a name="zh-cn_topic_0118924556_p47806732"></a><a name="zh-cn_topic_0118924556_p47806732"></a>API的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row27607410"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924556_p21607760"><a name="zh-cn_topic_0118924556_p21607760"></a><a name="zh-cn_topic_0118924556_p21607760"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924556_p5398110"><a name="zh-cn_topic_0118924556_p5398110"></a><a name="zh-cn_topic_0118924556_p5398110"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924556_p34593732"><a name="zh-cn_topic_0118924556_p34593732"></a><a name="zh-cn_topic_0118924556_p34593732"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924556_p50628907"><a name="zh-cn_topic_0118924556_p50628907"></a><a name="zh-cn_topic_0118924556_p50628907"></a>签名密钥的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row53006982"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924556_p65707153"><a name="zh-cn_topic_0118924556_p65707153"></a><a name="zh-cn_topic_0118924556_p65707153"></a>sign_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924556_p20679152"><a name="zh-cn_topic_0118924556_p20679152"></a><a name="zh-cn_topic_0118924556_p20679152"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924556_p64398604"><a name="zh-cn_topic_0118924556_p64398604"></a><a name="zh-cn_topic_0118924556_p64398604"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924556_p48904396"><a name="zh-cn_topic_0118924556_p48904396"></a><a name="zh-cn_topic_0118924556_p48904396"></a>签名密钥的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row37486381"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924556_p16498015"><a name="zh-cn_topic_0118924556_p16498015"></a><a name="zh-cn_topic_0118924556_p16498015"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924556_p61270825"><a name="zh-cn_topic_0118924556_p61270825"></a><a name="zh-cn_topic_0118924556_p61270825"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924556_p63989812"><a name="zh-cn_topic_0118924556_p63989812"></a><a name="zh-cn_topic_0118924556_p63989812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924556_p15792296"><a name="zh-cn_topic_0118924556_p15792296"></a><a name="zh-cn_topic_0118924556_p15792296"></a>环境编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924556_section44248161"></a>

无

## 响应消息<a name="zh-cn_topic_0118924556_section27331307"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924556_table9287199"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924556_row24571637"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924556_p44145606"><a name="zh-cn_topic_0118924556_p44145606"></a><a name="zh-cn_topic_0118924556_p44145606"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924556_p19024372"><a name="zh-cn_topic_0118924556_p19024372"></a><a name="zh-cn_topic_0118924556_p19024372"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924556_p64579174"><a name="zh-cn_topic_0118924556_p64579174"></a><a name="zh-cn_topic_0118924556_p64579174"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924556_row63530629"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p45707320"><a name="zh-cn_topic_0118924556_p45707320"></a><a name="zh-cn_topic_0118924556_p45707320"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p11305448"><a name="zh-cn_topic_0118924556_p11305448"></a><a name="zh-cn_topic_0118924556_p11305448"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p43326076"><a name="zh-cn_topic_0118924556_p43326076"></a><a name="zh-cn_topic_0118924556_p43326076"></a>本次查询满足条件的签名密钥总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row54390367"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p43543621"><a name="zh-cn_topic_0118924556_p43543621"></a><a name="zh-cn_topic_0118924556_p43543621"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p37372419"><a name="zh-cn_topic_0118924556_p37372419"></a><a name="zh-cn_topic_0118924556_p37372419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p7267138"><a name="zh-cn_topic_0118924556_p7267138"></a><a name="zh-cn_topic_0118924556_p7267138"></a>本次查询返回的签名密钥列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row65404250"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p63252860"><a name="zh-cn_topic_0118924556_p63252860"></a><a name="zh-cn_topic_0118924556_p63252860"></a>bindings</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p23208051"><a name="zh-cn_topic_0118924556_p23208051"></a><a name="zh-cn_topic_0118924556_p23208051"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p804007"><a name="zh-cn_topic_0118924556_p804007"></a><a name="zh-cn_topic_0118924556_p804007"></a>本次查询返回的签名密钥列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  bindings参数说明

<a name="zh-cn_topic_0118924556_table65124607"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924556_row33193740"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924556_p4338391"><a name="zh-cn_topic_0118924556_p4338391"></a><a name="zh-cn_topic_0118924556_p4338391"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924556_p15865395"><a name="zh-cn_topic_0118924556_p15865395"></a><a name="zh-cn_topic_0118924556_p15865395"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924556_p10028615"><a name="zh-cn_topic_0118924556_p10028615"></a><a name="zh-cn_topic_0118924556_p10028615"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924556_row7011516"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p31061946"><a name="zh-cn_topic_0118924556_p31061946"></a><a name="zh-cn_topic_0118924556_p31061946"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p32989672"><a name="zh-cn_topic_0118924556_p32989672"></a><a name="zh-cn_topic_0118924556_p32989672"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p54917742"><a name="zh-cn_topic_0118924556_p54917742"></a><a name="zh-cn_topic_0118924556_p54917742"></a>绑定关系的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row24497634"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p38151328"><a name="zh-cn_topic_0118924556_p38151328"></a><a name="zh-cn_topic_0118924556_p38151328"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p3249867"><a name="zh-cn_topic_0118924556_p3249867"></a><a name="zh-cn_topic_0118924556_p3249867"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p61912650"><a name="zh-cn_topic_0118924556_p61912650"></a><a name="zh-cn_topic_0118924556_p61912650"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row20342941"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p37165494"><a name="zh-cn_topic_0118924556_p37165494"></a><a name="zh-cn_topic_0118924556_p37165494"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p57614999"><a name="zh-cn_topic_0118924556_p57614999"></a><a name="zh-cn_topic_0118924556_p57614999"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p36303337"><a name="zh-cn_topic_0118924556_p36303337"></a><a name="zh-cn_topic_0118924556_p36303337"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row58294579"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p24240497"><a name="zh-cn_topic_0118924556_p24240497"></a><a name="zh-cn_topic_0118924556_p24240497"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p17323251"><a name="zh-cn_topic_0118924556_p17323251"></a><a name="zh-cn_topic_0118924556_p17323251"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p61006114"><a name="zh-cn_topic_0118924556_p61006114"></a><a name="zh-cn_topic_0118924556_p61006114"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row12184117"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p47389458"><a name="zh-cn_topic_0118924556_p47389458"></a><a name="zh-cn_topic_0118924556_p47389458"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p13340879"><a name="zh-cn_topic_0118924556_p13340879"></a><a name="zh-cn_topic_0118924556_p13340879"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p6869396"><a name="zh-cn_topic_0118924556_p6869396"></a><a name="zh-cn_topic_0118924556_p6869396"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row61824570"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p41734239"><a name="zh-cn_topic_0118924556_p41734239"></a><a name="zh-cn_topic_0118924556_p41734239"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p25030176"><a name="zh-cn_topic_0118924556_p25030176"></a><a name="zh-cn_topic_0118924556_p25030176"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p14178407"><a name="zh-cn_topic_0118924556_p14178407"></a><a name="zh-cn_topic_0118924556_p14178407"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row60496799"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p1293671"><a name="zh-cn_topic_0118924556_p1293671"></a><a name="zh-cn_topic_0118924556_p1293671"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p37678503"><a name="zh-cn_topic_0118924556_p37678503"></a><a name="zh-cn_topic_0118924556_p37678503"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p32059912"><a name="zh-cn_topic_0118924556_p32059912"></a><a name="zh-cn_topic_0118924556_p32059912"></a>签名密钥的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row20103756"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p17791553"><a name="zh-cn_topic_0118924556_p17791553"></a><a name="zh-cn_topic_0118924556_p17791553"></a>sign_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p31829674"><a name="zh-cn_topic_0118924556_p31829674"></a><a name="zh-cn_topic_0118924556_p31829674"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p28066800"><a name="zh-cn_topic_0118924556_p28066800"></a><a name="zh-cn_topic_0118924556_p28066800"></a>签名密钥的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row51274609"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p59602636"><a name="zh-cn_topic_0118924556_p59602636"></a><a name="zh-cn_topic_0118924556_p59602636"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p63084216"><a name="zh-cn_topic_0118924556_p63084216"></a><a name="zh-cn_topic_0118924556_p63084216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p9547868"><a name="zh-cn_topic_0118924556_p9547868"></a><a name="zh-cn_topic_0118924556_p9547868"></a>签名密钥的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row18821955"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p48183407"><a name="zh-cn_topic_0118924556_p48183407"></a><a name="zh-cn_topic_0118924556_p48183407"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p10541928"><a name="zh-cn_topic_0118924556_p10541928"></a><a name="zh-cn_topic_0118924556_p10541928"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p48589845"><a name="zh-cn_topic_0118924556_p48589845"></a><a name="zh-cn_topic_0118924556_p48589845"></a>签名密钥的密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row34655427"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p55626202"><a name="zh-cn_topic_0118924556_p55626202"></a><a name="zh-cn_topic_0118924556_p55626202"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p9428505"><a name="zh-cn_topic_0118924556_p9428505"></a><a name="zh-cn_topic_0118924556_p9428505"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p25511465"><a name="zh-cn_topic_0118924556_p25511465"></a><a name="zh-cn_topic_0118924556_p25511465"></a>API所属环境的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row28276599"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p8703171"><a name="zh-cn_topic_0118924556_p8703171"></a><a name="zh-cn_topic_0118924556_p8703171"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p33868211"><a name="zh-cn_topic_0118924556_p33868211"></a><a name="zh-cn_topic_0118924556_p33868211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p58970543"><a name="zh-cn_topic_0118924556_p58970543"></a><a name="zh-cn_topic_0118924556_p58970543"></a>API所属环境的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row60972846"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p39853480"><a name="zh-cn_topic_0118924556_p39853480"></a><a name="zh-cn_topic_0118924556_p39853480"></a>binding_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p6906467"><a name="zh-cn_topic_0118924556_p6906467"></a><a name="zh-cn_topic_0118924556_p6906467"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p22552967"><a name="zh-cn_topic_0118924556_p22552967"></a><a name="zh-cn_topic_0118924556_p22552967"></a>绑定时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row4895143611364"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924556_p289616365369"><a name="zh-cn_topic_0118924556_p289616365369"></a><a name="zh-cn_topic_0118924556_p289616365369"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924556_p8896113633612"><a name="zh-cn_topic_0118924556_p8896113633612"></a><a name="zh-cn_topic_0118924556_p8896113633612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924556_p14896123613366"><a name="zh-cn_topic_0118924556_p14896123613366"></a><a name="zh-cn_topic_0118924556_p14896123613366"></a>API的发布编号</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 2,
  "size": 2,
  "bindings": [
    {
      "id": "4588ec6f5dab4f67b298dc693f58029e",
      "api_id": "d85c502a-f916-47e8-bba0-50537a2d1af2",
      "api_name": "aaa",
      "api_remark": "",
      "group_name": "asd",
      "api_type": 1,
      "sign_id": "3a793b65a9034bdfae08924f149bfb4a",
      "sign_name": "signature01",
      "sign_key": "abcd_1234",
      "sign_secret": "******",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "binding_time": "2018-02-07T07: 08: 51Z",
      "publish_id": "3a793b65a9034bdfae08924f149bfsda"
    },
    {
      "id": "d8426fb090e442c4a56a35e451bea085",
      "api_id": "3c6769c6-ec61-4b45-b478-c60310dbaa1b",
      "api_name": "bbb",
      "api_remark": "",
      "group_name": "asd",
      "api_type": 1,
      "sign_id": "3a793b65a9034bdfae08924f149bfb4a",
      "sign_name": "signature01",
      "sign_key": "abcd_1234",
      "sign_secret": "******",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "binding_time": "2018-02-07T03: 17: 26Z",
      "publish_id": "3a793b65a9034bdfae08924f149bfsda"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0118924556_section62689135"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924556_table41624107"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924556_row66873984"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924556_p48083630"><a name="zh-cn_topic_0118924556_p48083630"></a><a name="zh-cn_topic_0118924556_p48083630"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924556_p22139981"><a name="zh-cn_topic_0118924556_p22139981"></a><a name="zh-cn_topic_0118924556_p22139981"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924556_row33918813"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924556_p63069309"><a name="zh-cn_topic_0118924556_p63069309"></a><a name="zh-cn_topic_0118924556_p63069309"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924556_p50988816"><a name="zh-cn_topic_0118924556_p50988816"></a><a name="zh-cn_topic_0118924556_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row7954866"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924556_p40364423"><a name="zh-cn_topic_0118924556_p40364423"></a><a name="zh-cn_topic_0118924556_p40364423"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924556_p48292816"><a name="zh-cn_topic_0118924556_p48292816"></a><a name="zh-cn_topic_0118924556_p48292816"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row31982164"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924556_p40418471"><a name="zh-cn_topic_0118924556_p40418471"></a><a name="zh-cn_topic_0118924556_p40418471"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924556_p52670690"><a name="zh-cn_topic_0118924556_p52670690"></a><a name="zh-cn_topic_0118924556_p52670690"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row4274166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924556_p10663202"><a name="zh-cn_topic_0118924556_p10663202"></a><a name="zh-cn_topic_0118924556_p10663202"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924556_p58413001"><a name="zh-cn_topic_0118924556_p58413001"></a><a name="zh-cn_topic_0118924556_p58413001"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row55954967"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924556_p36058501"><a name="zh-cn_topic_0118924556_p36058501"></a><a name="zh-cn_topic_0118924556_p36058501"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924556_p35057443"><a name="zh-cn_topic_0118924556_p35057443"></a><a name="zh-cn_topic_0118924556_p35057443"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924556_row47081531"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924556_p55507685"><a name="zh-cn_topic_0118924556_p55507685"></a><a name="zh-cn_topic_0118924556_p55507685"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924556_p6744143"><a name="zh-cn_topic_0118924556_p6744143"></a><a name="zh-cn_topic_0118924556_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

