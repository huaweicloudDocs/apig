# 查看签名密钥未绑定的API列表<a name="ZH-CN_TOPIC_0000001082221297"></a>

## 功能介绍<a name="zh-cn_topic_0225568942_section51759191"></a>

查询所有未绑定到该签名密钥上的API列表。需要API已经发布，未发布的API不予展示。

## URI<a name="zh-cn_topic_0225568942_section63179535"></a>

HTTP/HTTPS请求方法以及URI如表3-73所示。

**表 1**  HTTP/HTTPS请求方法以及

<a name="zh-cn_topic_0225568942_table42511059"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568942_row55091690"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568942_p33241899"><a name="zh-cn_topic_0225568942_p33241899"></a><a name="zh-cn_topic_0225568942_p33241899"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568942_p8239264"><a name="zh-cn_topic_0225568942_p8239264"></a><a name="zh-cn_topic_0225568942_p8239264"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568942_row63400625"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568942_p35177032"><a name="zh-cn_topic_0225568942_p35177032"></a><a name="zh-cn_topic_0225568942_p35177032"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568942_p30767306"><a name="zh-cn_topic_0225568942_p30767306"></a><a name="zh-cn_topic_0225568942_p30767306"></a>/v1/{project_id}/apigw/instances/{instance_id}/sign-bindings/unbinded-apis[?page_size, page_no, sign_id, env_id, api_id, api_name, group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：sign\_id、env\_id、api\_id、api\_name、group\_id、page\_size、page\_no。

## 请求消息<a name="zh-cn_topic_0225568942_section31744903"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0225568942_table5666522"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568942_row16340827"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568942_p48538593"><a name="zh-cn_topic_0225568942_p48538593"></a><a name="zh-cn_topic_0225568942_p48538593"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568942_p39311997"><a name="zh-cn_topic_0225568942_p39311997"></a><a name="zh-cn_topic_0225568942_p39311997"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568942_p30155156"><a name="zh-cn_topic_0225568942_p30155156"></a><a name="zh-cn_topic_0225568942_p30155156"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568942_p26648592"><a name="zh-cn_topic_0225568942_p26648592"></a><a name="zh-cn_topic_0225568942_p26648592"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568942_row10119141815116"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568942_p55878963"><a name="zh-cn_topic_0225568942_p55878963"></a><a name="zh-cn_topic_0225568942_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568942_p29902160"><a name="zh-cn_topic_0225568942_p29902160"></a><a name="zh-cn_topic_0225568942_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568942_p6155914"><a name="zh-cn_topic_0225568942_p6155914"></a><a name="zh-cn_topic_0225568942_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568942_p28867016"><a name="zh-cn_topic_0225568942_p28867016"></a><a name="zh-cn_topic_0225568942_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row843201705116"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568942_p1780913159538"><a name="zh-cn_topic_0225568942_p1780913159538"></a><a name="zh-cn_topic_0225568942_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568942_p9809215115310"><a name="zh-cn_topic_0225568942_p9809215115310"></a><a name="zh-cn_topic_0225568942_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568942_p1280914152538"><a name="zh-cn_topic_0225568942_p1280914152538"></a><a name="zh-cn_topic_0225568942_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568942_p1880914157537"><a name="zh-cn_topic_0225568942_p1880914157537"></a><a name="zh-cn_topic_0225568942_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row11052377"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568942_p22827350"><a name="zh-cn_topic_0225568942_p22827350"></a><a name="zh-cn_topic_0225568942_p22827350"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568942_p37076080"><a name="zh-cn_topic_0225568942_p37076080"></a><a name="zh-cn_topic_0225568942_p37076080"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568942_p50372494"><a name="zh-cn_topic_0225568942_p50372494"></a><a name="zh-cn_topic_0225568942_p50372494"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568942_p53640217"><a name="zh-cn_topic_0225568942_p53640217"></a><a name="zh-cn_topic_0225568942_p53640217"></a>安全密钥编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row12999906"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568942_p46359483"><a name="zh-cn_topic_0225568942_p46359483"></a><a name="zh-cn_topic_0225568942_p46359483"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568942_p64130612"><a name="zh-cn_topic_0225568942_p64130612"></a><a name="zh-cn_topic_0225568942_p64130612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568942_p27197045"><a name="zh-cn_topic_0225568942_p27197045"></a><a name="zh-cn_topic_0225568942_p27197045"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568942_p55477031"><a name="zh-cn_topic_0225568942_p55477031"></a><a name="zh-cn_topic_0225568942_p55477031"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row29531233"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568942_p43219711"><a name="zh-cn_topic_0225568942_p43219711"></a><a name="zh-cn_topic_0225568942_p43219711"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568942_p11135713"><a name="zh-cn_topic_0225568942_p11135713"></a><a name="zh-cn_topic_0225568942_p11135713"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568942_p29577584"><a name="zh-cn_topic_0225568942_p29577584"></a><a name="zh-cn_topic_0225568942_p29577584"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568942_p46974099"><a name="zh-cn_topic_0225568942_p46974099"></a><a name="zh-cn_topic_0225568942_p46974099"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row20113712"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568942_p18597965"><a name="zh-cn_topic_0225568942_p18597965"></a><a name="zh-cn_topic_0225568942_p18597965"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568942_p30040178"><a name="zh-cn_topic_0225568942_p30040178"></a><a name="zh-cn_topic_0225568942_p30040178"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568942_p17335368"><a name="zh-cn_topic_0225568942_p17335368"></a><a name="zh-cn_topic_0225568942_p17335368"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568942_p61987574"><a name="zh-cn_topic_0225568942_p61987574"></a><a name="zh-cn_topic_0225568942_p61987574"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row21017262"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568942_p24676693"><a name="zh-cn_topic_0225568942_p24676693"></a><a name="zh-cn_topic_0225568942_p24676693"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568942_p52655079"><a name="zh-cn_topic_0225568942_p52655079"></a><a name="zh-cn_topic_0225568942_p52655079"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568942_p37203022"><a name="zh-cn_topic_0225568942_p37203022"></a><a name="zh-cn_topic_0225568942_p37203022"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568942_p60654834"><a name="zh-cn_topic_0225568942_p60654834"></a><a name="zh-cn_topic_0225568942_p60654834"></a>API分组编号</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0225568942_section21200323"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568942_table34366064"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568942_row59541114"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568942_p58100907"><a name="zh-cn_topic_0225568942_p58100907"></a><a name="zh-cn_topic_0225568942_p58100907"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568942_p8553058"><a name="zh-cn_topic_0225568942_p8553058"></a><a name="zh-cn_topic_0225568942_p8553058"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568942_p21709060"><a name="zh-cn_topic_0225568942_p21709060"></a><a name="zh-cn_topic_0225568942_p21709060"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568942_row13603451"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p28137775"><a name="zh-cn_topic_0225568942_p28137775"></a><a name="zh-cn_topic_0225568942_p28137775"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p64567303"><a name="zh-cn_topic_0225568942_p64567303"></a><a name="zh-cn_topic_0225568942_p64567303"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p62569068"><a name="zh-cn_topic_0225568942_p62569068"></a><a name="zh-cn_topic_0225568942_p62569068"></a>满足查询条件的API的总个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row26250702"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p45932145"><a name="zh-cn_topic_0225568942_p45932145"></a><a name="zh-cn_topic_0225568942_p45932145"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p29516244"><a name="zh-cn_topic_0225568942_p29516244"></a><a name="zh-cn_topic_0225568942_p29516244"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p42005535"><a name="zh-cn_topic_0225568942_p42005535"></a><a name="zh-cn_topic_0225568942_p42005535"></a>本次查询返回的API列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row42505499"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p20393431"><a name="zh-cn_topic_0225568942_p20393431"></a><a name="zh-cn_topic_0225568942_p20393431"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p41255182"><a name="zh-cn_topic_0225568942_p41255182"></a><a name="zh-cn_topic_0225568942_p41255182"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p53335466"><a name="zh-cn_topic_0225568942_p53335466"></a><a name="zh-cn_topic_0225568942_p53335466"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="zh-cn_topic_0225568942_table10257154"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568942_row50958760"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568942_p34018899"><a name="zh-cn_topic_0225568942_p34018899"></a><a name="zh-cn_topic_0225568942_p34018899"></a><strong id="zh-cn_topic_0225568942_b37734636"><a name="zh-cn_topic_0225568942_b37734636"></a><a name="zh-cn_topic_0225568942_b37734636"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568942_p36606693"><a name="zh-cn_topic_0225568942_p36606693"></a><a name="zh-cn_topic_0225568942_p36606693"></a><strong id="zh-cn_topic_0225568942_b61024782"><a name="zh-cn_topic_0225568942_b61024782"></a><a name="zh-cn_topic_0225568942_b61024782"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568942_p44060270"><a name="zh-cn_topic_0225568942_p44060270"></a><a name="zh-cn_topic_0225568942_p44060270"></a><strong id="zh-cn_topic_0225568942_b60998111"><a name="zh-cn_topic_0225568942_b60998111"></a><a name="zh-cn_topic_0225568942_b60998111"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568942_row41899953"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p38453019"><a name="zh-cn_topic_0225568942_p38453019"></a><a name="zh-cn_topic_0225568942_p38453019"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p27686854"><a name="zh-cn_topic_0225568942_p27686854"></a><a name="zh-cn_topic_0225568942_p27686854"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p28042714"><a name="zh-cn_topic_0225568942_p28042714"></a><a name="zh-cn_topic_0225568942_p28042714"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row51057834"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p42043885"><a name="zh-cn_topic_0225568942_p42043885"></a><a name="zh-cn_topic_0225568942_p42043885"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p50111533"><a name="zh-cn_topic_0225568942_p50111533"></a><a name="zh-cn_topic_0225568942_p50111533"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p32502353"><a name="zh-cn_topic_0225568942_p32502353"></a><a name="zh-cn_topic_0225568942_p32502353"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row51031407"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p39903265"><a name="zh-cn_topic_0225568942_p39903265"></a><a name="zh-cn_topic_0225568942_p39903265"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p10939048"><a name="zh-cn_topic_0225568942_p10939048"></a><a name="zh-cn_topic_0225568942_p10939048"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p13647724"><a name="zh-cn_topic_0225568942_p13647724"></a><a name="zh-cn_topic_0225568942_p13647724"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row61320148"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p876124"><a name="zh-cn_topic_0225568942_p876124"></a><a name="zh-cn_topic_0225568942_p876124"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p3857204"><a name="zh-cn_topic_0225568942_p3857204"></a><a name="zh-cn_topic_0225568942_p3857204"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p43998084"><a name="zh-cn_topic_0225568942_p43998084"></a><a name="zh-cn_topic_0225568942_p43998084"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row40388913"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p50276488"><a name="zh-cn_topic_0225568942_p50276488"></a><a name="zh-cn_topic_0225568942_p50276488"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p45863748"><a name="zh-cn_topic_0225568942_p45863748"></a><a name="zh-cn_topic_0225568942_p45863748"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p23976141"><a name="zh-cn_topic_0225568942_p23976141"></a><a name="zh-cn_topic_0225568942_p23976141"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row14458682"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p30302560"><a name="zh-cn_topic_0225568942_p30302560"></a><a name="zh-cn_topic_0225568942_p30302560"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p38588295"><a name="zh-cn_topic_0225568942_p38588295"></a><a name="zh-cn_topic_0225568942_p38588295"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p38644182"><a name="zh-cn_topic_0225568942_p38644182"></a><a name="zh-cn_topic_0225568942_p38644182"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row12253325"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p52995244"><a name="zh-cn_topic_0225568942_p52995244"></a><a name="zh-cn_topic_0225568942_p52995244"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p64756360"><a name="zh-cn_topic_0225568942_p64756360"></a><a name="zh-cn_topic_0225568942_p64756360"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p10773768"><a name="zh-cn_topic_0225568942_p10773768"></a><a name="zh-cn_topic_0225568942_p10773768"></a>发布的环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row29855049"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p2339899"><a name="zh-cn_topic_0225568942_p2339899"></a><a name="zh-cn_topic_0225568942_p2339899"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p55314117"><a name="zh-cn_topic_0225568942_p55314117"></a><a name="zh-cn_topic_0225568942_p55314117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p51258512"><a name="zh-cn_topic_0225568942_p51258512"></a><a name="zh-cn_topic_0225568942_p51258512"></a>发布的环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row58673429"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p54927332"><a name="zh-cn_topic_0225568942_p54927332"></a><a name="zh-cn_topic_0225568942_p54927332"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p19928903"><a name="zh-cn_topic_0225568942_p19928903"></a><a name="zh-cn_topic_0225568942_p19928903"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p3628455"><a name="zh-cn_topic_0225568942_p3628455"></a><a name="zh-cn_topic_0225568942_p3628455"></a>API的发布记录编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row8616217"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p26824986"><a name="zh-cn_topic_0225568942_p26824986"></a><a name="zh-cn_topic_0225568942_p26824986"></a>signature_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p25340259"><a name="zh-cn_topic_0225568942_p25340259"></a><a name="zh-cn_topic_0225568942_p25340259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p39295133"><a name="zh-cn_topic_0225568942_p39295133"></a><a name="zh-cn_topic_0225568942_p39295133"></a>已绑定的签名密钥名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row194436159307"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p124441715143014"><a name="zh-cn_topic_0225568942_p124441715143014"></a><a name="zh-cn_topic_0225568942_p124441715143014"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p1644461519309"><a name="zh-cn_topic_0225568942_p1644461519309"></a><a name="zh-cn_topic_0225568942_p1644461519309"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p18444315103014"><a name="zh-cn_topic_0225568942_p18444315103014"></a><a name="zh-cn_topic_0225568942_p18444315103014"></a>API的认证方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row62593129319"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568942_p1925910128315"><a name="zh-cn_topic_0225568942_p1925910128315"></a><a name="zh-cn_topic_0225568942_p1925910128315"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568942_p15259161219319"><a name="zh-cn_topic_0225568942_p15259161219319"></a><a name="zh-cn_topic_0225568942_p15259161219319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568942_p1226051212318"><a name="zh-cn_topic_0225568942_p1226051212318"></a><a name="zh-cn_topic_0225568942_p1226051212318"></a>API的访问地址</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"apis": [{
		"name": "bbb",
		"type": 1,
		"group_id": "7ccc0b94-eb5a-48e6-8554-6d0105a540e2",
		"id": "3c6769c6-ec61-4b45-b478-c60310dbaa1b",
		"group_name": "asd",
		"run_env_name": "das",
		"run_env_id": "1fdcb2e4-f90a-4159-817d-98c9b8e8b215",
		"publish_id": "6dff16c4-813f-486a-bba4-fdad45a55a70",
		"auth_type": "NONE",
		"req_uri": "/test"
	},
	{
		"name": "aaa",
		"type": 1,
		"group_id": "7ccc0b94-eb5a-48e6-8554-6d0105a540e2",
		"id": "d85c502a-f916-47e8-bba0-50537a2d1af2",
		"group_name": "asd",
		"run_env_name": "das",
		"run_env_id": "1fdcb2e4-f90a-4159-817d-98c9b8e8b215",
		"publish_id": "dec83400-a0c6-4ea6-abfd-5bf237292f4d",
		"auth_type": "NONE",
		"req_uri": "/test"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568942_section17268672"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568942_table59741839"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568942_row51360638"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568942_p66570984"><a name="zh-cn_topic_0225568942_p66570984"></a><a name="zh-cn_topic_0225568942_p66570984"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568942_p10538870"><a name="zh-cn_topic_0225568942_p10538870"></a><a name="zh-cn_topic_0225568942_p10538870"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568942_row32426065"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568942_p9265629"><a name="zh-cn_topic_0225568942_p9265629"></a><a name="zh-cn_topic_0225568942_p9265629"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568942_p12318518"><a name="zh-cn_topic_0225568942_p12318518"></a><a name="zh-cn_topic_0225568942_p12318518"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row43757803"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568942_p54721121"><a name="zh-cn_topic_0225568942_p54721121"></a><a name="zh-cn_topic_0225568942_p54721121"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568942_p3225816"><a name="zh-cn_topic_0225568942_p3225816"></a><a name="zh-cn_topic_0225568942_p3225816"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row29032347"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568942_p2809910"><a name="zh-cn_topic_0225568942_p2809910"></a><a name="zh-cn_topic_0225568942_p2809910"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568942_p26276133"><a name="zh-cn_topic_0225568942_p26276133"></a><a name="zh-cn_topic_0225568942_p26276133"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row35158608"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568942_p29274969"><a name="zh-cn_topic_0225568942_p29274969"></a><a name="zh-cn_topic_0225568942_p29274969"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568942_p22462250"><a name="zh-cn_topic_0225568942_p22462250"></a><a name="zh-cn_topic_0225568942_p22462250"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row833661"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568942_p417742"><a name="zh-cn_topic_0225568942_p417742"></a><a name="zh-cn_topic_0225568942_p417742"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568942_p15296380"><a name="zh-cn_topic_0225568942_p15296380"></a><a name="zh-cn_topic_0225568942_p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568942_row36099169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568942_p38351589"><a name="zh-cn_topic_0225568942_p38351589"></a><a name="zh-cn_topic_0225568942_p38351589"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568942_p6744143"><a name="zh-cn_topic_0225568942_p6744143"></a><a name="zh-cn_topic_0225568942_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

