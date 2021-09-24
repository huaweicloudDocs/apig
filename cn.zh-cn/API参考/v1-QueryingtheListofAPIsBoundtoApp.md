# 查看APP已绑定的API列表<a name="ZH-CN_TOPIC_0000001082221261"></a>

## 功能介绍<a name="zh-cn_topic_0225568844_section45617990"></a>

查询APP已经绑定的API列表。

>![](public_sys-resources/icon-note.gif) **说明：** 
>将API发布到相应的授权的环境后，才能查询到结果。

## URI<a name="zh-cn_topic_0225568844_section7908727"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568844_table40887806"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568844_row9298403"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568844_p14973182"><a name="zh-cn_topic_0225568844_p14973182"></a><a name="zh-cn_topic_0225568844_p14973182"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568844_p4868205"><a name="zh-cn_topic_0225568844_p4868205"></a><a name="zh-cn_topic_0225568844_p4868205"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568844_row58780313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568844_p63584873"><a name="zh-cn_topic_0225568844_p63584873"></a><a name="zh-cn_topic_0225568844_p63584873"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568844_p50101061"><a name="zh-cn_topic_0225568844_p50101061"></a><a name="zh-cn_topic_0225568844_p50101061"></a>/v1/{project_id}/apigw/instances/{instance_id}/app-auths/binded-apis[?page_size, page_no, app_id, api_id, api_name,group_id,group_name,env_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：app\_id、 api\_id 、 api\_name、group\_id、group\_name、env\_id、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568844_table48164278"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568844_row10528204"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568844_p47478189"><a name="zh-cn_topic_0225568844_p47478189"></a><a name="zh-cn_topic_0225568844_p47478189"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568844_p20528066"><a name="zh-cn_topic_0225568844_p20528066"></a><a name="zh-cn_topic_0225568844_p20528066"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568844_p52160627"><a name="zh-cn_topic_0225568844_p52160627"></a><a name="zh-cn_topic_0225568844_p52160627"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568844_p64261290"><a name="zh-cn_topic_0225568844_p64261290"></a><a name="zh-cn_topic_0225568844_p64261290"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568844_row913074913466"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p55878963"><a name="zh-cn_topic_0225568844_p55878963"></a><a name="zh-cn_topic_0225568844_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p29902160"><a name="zh-cn_topic_0225568844_p29902160"></a><a name="zh-cn_topic_0225568844_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p6155914"><a name="zh-cn_topic_0225568844_p6155914"></a><a name="zh-cn_topic_0225568844_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p28867016"><a name="zh-cn_topic_0225568844_p28867016"></a><a name="zh-cn_topic_0225568844_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row20960204813463"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p1780913159538"><a name="zh-cn_topic_0225568844_p1780913159538"></a><a name="zh-cn_topic_0225568844_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p9809215115310"><a name="zh-cn_topic_0225568844_p9809215115310"></a><a name="zh-cn_topic_0225568844_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p1280914152538"><a name="zh-cn_topic_0225568844_p1280914152538"></a><a name="zh-cn_topic_0225568844_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p1880914157537"><a name="zh-cn_topic_0225568844_p1880914157537"></a><a name="zh-cn_topic_0225568844_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row37781964"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p40440259"><a name="zh-cn_topic_0225568844_p40440259"></a><a name="zh-cn_topic_0225568844_p40440259"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p54435575"><a name="zh-cn_topic_0225568844_p54435575"></a><a name="zh-cn_topic_0225568844_p54435575"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p47205455"><a name="zh-cn_topic_0225568844_p47205455"></a><a name="zh-cn_topic_0225568844_p47205455"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p65545524"><a name="zh-cn_topic_0225568844_p65545524"></a><a name="zh-cn_topic_0225568844_p65545524"></a>应用编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row53038806"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p1176057"><a name="zh-cn_topic_0225568844_p1176057"></a><a name="zh-cn_topic_0225568844_p1176057"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p28151772"><a name="zh-cn_topic_0225568844_p28151772"></a><a name="zh-cn_topic_0225568844_p28151772"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p65701031"><a name="zh-cn_topic_0225568844_p65701031"></a><a name="zh-cn_topic_0225568844_p65701031"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p20183299"><a name="zh-cn_topic_0225568844_p20183299"></a><a name="zh-cn_topic_0225568844_p20183299"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row47431967"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p16784086"><a name="zh-cn_topic_0225568844_p16784086"></a><a name="zh-cn_topic_0225568844_p16784086"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p17333746"><a name="zh-cn_topic_0225568844_p17333746"></a><a name="zh-cn_topic_0225568844_p17333746"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p61856219"><a name="zh-cn_topic_0225568844_p61856219"></a><a name="zh-cn_topic_0225568844_p61856219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p44297848"><a name="zh-cn_topic_0225568844_p44297848"></a><a name="zh-cn_topic_0225568844_p44297848"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row63136318"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p13768133"><a name="zh-cn_topic_0225568844_p13768133"></a><a name="zh-cn_topic_0225568844_p13768133"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p41476980"><a name="zh-cn_topic_0225568844_p41476980"></a><a name="zh-cn_topic_0225568844_p41476980"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p4192244"><a name="zh-cn_topic_0225568844_p4192244"></a><a name="zh-cn_topic_0225568844_p4192244"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p4027501"><a name="zh-cn_topic_0225568844_p4027501"></a><a name="zh-cn_topic_0225568844_p4027501"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row36247510"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p50367158"><a name="zh-cn_topic_0225568844_p50367158"></a><a name="zh-cn_topic_0225568844_p50367158"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p53207970"><a name="zh-cn_topic_0225568844_p53207970"></a><a name="zh-cn_topic_0225568844_p53207970"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p14878339"><a name="zh-cn_topic_0225568844_p14878339"></a><a name="zh-cn_topic_0225568844_p14878339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p64294849"><a name="zh-cn_topic_0225568844_p64294849"></a><a name="zh-cn_topic_0225568844_p64294849"></a>API分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row41782734"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p28958306"><a name="zh-cn_topic_0225568844_p28958306"></a><a name="zh-cn_topic_0225568844_p28958306"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p63921413"><a name="zh-cn_topic_0225568844_p63921413"></a><a name="zh-cn_topic_0225568844_p63921413"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p10252002"><a name="zh-cn_topic_0225568844_p10252002"></a><a name="zh-cn_topic_0225568844_p10252002"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p25105823"><a name="zh-cn_topic_0225568844_p25105823"></a><a name="zh-cn_topic_0225568844_p25105823"></a>授权的环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row24625817"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p48534154"><a name="zh-cn_topic_0225568844_p48534154"></a><a name="zh-cn_topic_0225568844_p48534154"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p38952367"><a name="zh-cn_topic_0225568844_p38952367"></a><a name="zh-cn_topic_0225568844_p38952367"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p1025136"><a name="zh-cn_topic_0225568844_p1025136"></a><a name="zh-cn_topic_0225568844_p1025136"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p15927223"><a name="zh-cn_topic_0225568844_p15927223"></a><a name="zh-cn_topic_0225568844_p15927223"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row9127279"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568844_p1112119"><a name="zh-cn_topic_0225568844_p1112119"></a><a name="zh-cn_topic_0225568844_p1112119"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568844_p22972791"><a name="zh-cn_topic_0225568844_p22972791"></a><a name="zh-cn_topic_0225568844_p22972791"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568844_p48856792"><a name="zh-cn_topic_0225568844_p48856792"></a><a name="zh-cn_topic_0225568844_p48856792"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568844_p65086081"><a name="zh-cn_topic_0225568844_p65086081"></a><a name="zh-cn_topic_0225568844_p65086081"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568844_section4069680"></a>

无

## 响应消息<a name="zh-cn_topic_0225568844_section61208646"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568844_table43505476"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568844_row17298029"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568844_p58963140"><a name="zh-cn_topic_0225568844_p58963140"></a><a name="zh-cn_topic_0225568844_p58963140"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568844_p11284998"><a name="zh-cn_topic_0225568844_p11284998"></a><a name="zh-cn_topic_0225568844_p11284998"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568844_p41669661"><a name="zh-cn_topic_0225568844_p41669661"></a><a name="zh-cn_topic_0225568844_p41669661"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568844_row19799409"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p60248297"><a name="zh-cn_topic_0225568844_p60248297"></a><a name="zh-cn_topic_0225568844_p60248297"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p48273902"><a name="zh-cn_topic_0225568844_p48273902"></a><a name="zh-cn_topic_0225568844_p48273902"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p17871975"><a name="zh-cn_topic_0225568844_p17871975"></a><a name="zh-cn_topic_0225568844_p17871975"></a>符合条件的API总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row26630051"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p9550502"><a name="zh-cn_topic_0225568844_p9550502"></a><a name="zh-cn_topic_0225568844_p9550502"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p35393169"><a name="zh-cn_topic_0225568844_p35393169"></a><a name="zh-cn_topic_0225568844_p35393169"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p48274445"><a name="zh-cn_topic_0225568844_p48274445"></a><a name="zh-cn_topic_0225568844_p48274445"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row31816825"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p27026000"><a name="zh-cn_topic_0225568844_p27026000"></a><a name="zh-cn_topic_0225568844_p27026000"></a>auths</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p41622412"><a name="zh-cn_topic_0225568844_p41622412"></a><a name="zh-cn_topic_0225568844_p41622412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p15972245"><a name="zh-cn_topic_0225568844_p15972245"></a><a name="zh-cn_topic_0225568844_p15972245"></a>本次返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  auths参数说明

<a name="zh-cn_topic_0225568844_table9532482"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568844_row5407061"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568844_p35318772"><a name="zh-cn_topic_0225568844_p35318772"></a><a name="zh-cn_topic_0225568844_p35318772"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568844_p42248272"><a name="zh-cn_topic_0225568844_p42248272"></a><a name="zh-cn_topic_0225568844_p42248272"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568844_p66666832"><a name="zh-cn_topic_0225568844_p66666832"></a><a name="zh-cn_topic_0225568844_p66666832"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568844_row31304284"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p52619101"><a name="zh-cn_topic_0225568844_p52619101"></a><a name="zh-cn_topic_0225568844_p52619101"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p34288827"><a name="zh-cn_topic_0225568844_p34288827"></a><a name="zh-cn_topic_0225568844_p34288827"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p25931613"><a name="zh-cn_topic_0225568844_p25931613"></a><a name="zh-cn_topic_0225568844_p25931613"></a>授权关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row32057932"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p46555663"><a name="zh-cn_topic_0225568844_p46555663"></a><a name="zh-cn_topic_0225568844_p46555663"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p12912396"><a name="zh-cn_topic_0225568844_p12912396"></a><a name="zh-cn_topic_0225568844_p12912396"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p39271145"><a name="zh-cn_topic_0225568844_p39271145"></a><a name="zh-cn_topic_0225568844_p39271145"></a>API的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row17895987"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p40288836"><a name="zh-cn_topic_0225568844_p40288836"></a><a name="zh-cn_topic_0225568844_p40288836"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p42170249"><a name="zh-cn_topic_0225568844_p42170249"></a><a name="zh-cn_topic_0225568844_p42170249"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p60346986"><a name="zh-cn_topic_0225568844_p60346986"></a><a name="zh-cn_topic_0225568844_p60346986"></a>API的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row6251969"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p36647513"><a name="zh-cn_topic_0225568844_p36647513"></a><a name="zh-cn_topic_0225568844_p36647513"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p15658561"><a name="zh-cn_topic_0225568844_p15658561"></a><a name="zh-cn_topic_0225568844_p15658561"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p60383905"><a name="zh-cn_topic_0225568844_p60383905"></a><a name="zh-cn_topic_0225568844_p60383905"></a>API绑定的分组</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row6584238"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p63561270"><a name="zh-cn_topic_0225568844_p63561270"></a><a name="zh-cn_topic_0225568844_p63561270"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p48189259"><a name="zh-cn_topic_0225568844_p48189259"></a><a name="zh-cn_topic_0225568844_p48189259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p11015892"><a name="zh-cn_topic_0225568844_p11015892"></a><a name="zh-cn_topic_0225568844_p11015892"></a>API的描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row32034168"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p44630795"><a name="zh-cn_topic_0225568844_p44630795"></a><a name="zh-cn_topic_0225568844_p44630795"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p58324614"><a name="zh-cn_topic_0225568844_p58324614"></a><a name="zh-cn_topic_0225568844_p58324614"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p26673298"><a name="zh-cn_topic_0225568844_p26673298"></a><a name="zh-cn_topic_0225568844_p26673298"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row38733094"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p50372877"><a name="zh-cn_topic_0225568844_p50372877"></a><a name="zh-cn_topic_0225568844_p50372877"></a>envname</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p53671257"><a name="zh-cn_topic_0225568844_p53671257"></a><a name="zh-cn_topic_0225568844_p53671257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p52404594"><a name="zh-cn_topic_0225568844_p52404594"></a><a name="zh-cn_topic_0225568844_p52404594"></a>API授权绑定的环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row15974184212283"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p697416426280"><a name="zh-cn_topic_0225568844_p697416426280"></a><a name="zh-cn_topic_0225568844_p697416426280"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p9974742132816"><a name="zh-cn_topic_0225568844_p9974742132816"></a><a name="zh-cn_topic_0225568844_p9974742132816"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p1974542152815"><a name="zh-cn_topic_0225568844_p1974542152815"></a><a name="zh-cn_topic_0225568844_p1974542152815"></a>API授权绑定的环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row1879303"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p18005821"><a name="zh-cn_topic_0225568844_p18005821"></a><a name="zh-cn_topic_0225568844_p18005821"></a>auth_role</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p49185396"><a name="zh-cn_topic_0225568844_p49185396"></a><a name="zh-cn_topic_0225568844_p49185396"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p24594131"><a name="zh-cn_topic_0225568844_p24594131"></a><a name="zh-cn_topic_0225568844_p24594131"></a>授权者</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row20020594"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p11055393"><a name="zh-cn_topic_0225568844_p11055393"></a><a name="zh-cn_topic_0225568844_p11055393"></a>auth_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p23071629"><a name="zh-cn_topic_0225568844_p23071629"></a><a name="zh-cn_topic_0225568844_p23071629"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p56862621"><a name="zh-cn_topic_0225568844_p56862621"></a><a name="zh-cn_topic_0225568844_p56862621"></a>授权创建的时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row42001542"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p46681736"><a name="zh-cn_topic_0225568844_p46681736"></a><a name="zh-cn_topic_0225568844_p46681736"></a>appid</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p23124258"><a name="zh-cn_topic_0225568844_p23124258"></a><a name="zh-cn_topic_0225568844_p23124258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p61125629"><a name="zh-cn_topic_0225568844_p61125629"></a><a name="zh-cn_topic_0225568844_p61125629"></a>APP的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row13259754"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p298313"><a name="zh-cn_topic_0225568844_p298313"></a><a name="zh-cn_topic_0225568844_p298313"></a>app_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p24163388"><a name="zh-cn_topic_0225568844_p24163388"></a><a name="zh-cn_topic_0225568844_p24163388"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p11077420"><a name="zh-cn_topic_0225568844_p11077420"></a><a name="zh-cn_topic_0225568844_p11077420"></a>APP的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row32587918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p22375683"><a name="zh-cn_topic_0225568844_p22375683"></a><a name="zh-cn_topic_0225568844_p22375683"></a>app_creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p491049"><a name="zh-cn_topic_0225568844_p491049"></a><a name="zh-cn_topic_0225568844_p491049"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p39775015"><a name="zh-cn_topic_0225568844_p39775015"></a><a name="zh-cn_topic_0225568844_p39775015"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0225568844_ul22430823"></a><a name="zh-cn_topic_0225568844_ul22430823"></a><ul id="zh-cn_topic_0225568844_ul22430823"><li>USER：租户自己创建</li><li>MARKET：API市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row970995142615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p1871015142618"><a name="zh-cn_topic_0225568844_p1871015142618"></a><a name="zh-cn_topic_0225568844_p1871015142618"></a>app_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p1571011542618"><a name="zh-cn_topic_0225568844_p1571011542618"></a><a name="zh-cn_topic_0225568844_p1571011542618"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p20710175172620"><a name="zh-cn_topic_0225568844_p20710175172620"></a><a name="zh-cn_topic_0225568844_p20710175172620"></a>APP的描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row11885110132717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p2088541012274"><a name="zh-cn_topic_0225568844_p2088541012274"></a><a name="zh-cn_topic_0225568844_p2088541012274"></a>app_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p1588531017277"><a name="zh-cn_topic_0225568844_p1588531017277"></a><a name="zh-cn_topic_0225568844_p1588531017277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p588513106271"><a name="zh-cn_topic_0225568844_p588513106271"></a><a name="zh-cn_topic_0225568844_p588513106271"></a>APP的类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row124635369285"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568844_p1046343617283"><a name="zh-cn_topic_0225568844_p1046343617283"></a><a name="zh-cn_topic_0225568844_p1046343617283"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568844_p154631136102815"><a name="zh-cn_topic_0225568844_p154631136102815"></a><a name="zh-cn_topic_0225568844_p154631136102815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568844_p184638366284"><a name="zh-cn_topic_0225568844_p184638366284"></a><a name="zh-cn_topic_0225568844_p184638366284"></a>API的发布编号</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 1,
	"size": 1,
	"auths": [{
		"id": "cfa688d8-094b-445a-b270-6aeb0b70a84a",
		"api_id": "6632a062-9dcf-4f18-9646-3cabb925a290",
		"api_name": "查询API列表",
		"group_name": "api_group_001",
		"api_type": 1,
		"api_remark": "查询API列表",
		"envname": "RELEASE",
		"auth_role": "PROVIDER",
		"auth_time": "2017-12-28T12:46:43Z",
		"appid": "14b399ac-967f-4115-bb62-c0346b4537e9",
		"app_name": "app_001",
		"app_creator": "USER",
		"env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"app_remark": "APP的描述信息",
		"app_type": "apig",
		"publish_id": "f500ba7e369b4b1ebae99aa9d114a17a"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568844_section36627122"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568844_table16081870"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568844_row27929984"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568844_p47736268"><a name="zh-cn_topic_0225568844_p47736268"></a><a name="zh-cn_topic_0225568844_p47736268"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568844_p41432467"><a name="zh-cn_topic_0225568844_p41432467"></a><a name="zh-cn_topic_0225568844_p41432467"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568844_row586687"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568844_p47521720"><a name="zh-cn_topic_0225568844_p47521720"></a><a name="zh-cn_topic_0225568844_p47521720"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568844_p24054117"><a name="zh-cn_topic_0225568844_p24054117"></a><a name="zh-cn_topic_0225568844_p24054117"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row15160467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568844_p20038314"><a name="zh-cn_topic_0225568844_p20038314"></a><a name="zh-cn_topic_0225568844_p20038314"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568844_p12490729"><a name="zh-cn_topic_0225568844_p12490729"></a><a name="zh-cn_topic_0225568844_p12490729"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row45307704"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568844_p46045383"><a name="zh-cn_topic_0225568844_p46045383"></a><a name="zh-cn_topic_0225568844_p46045383"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568844_p164181330094"><a name="zh-cn_topic_0225568844_p164181330094"></a><a name="zh-cn_topic_0225568844_p164181330094"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row12652459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568844_p18216220"><a name="zh-cn_topic_0225568844_p18216220"></a><a name="zh-cn_topic_0225568844_p18216220"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568844_p66227710"><a name="zh-cn_topic_0225568844_p66227710"></a><a name="zh-cn_topic_0225568844_p66227710"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row59178480"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568844_p28727614"><a name="zh-cn_topic_0225568844_p28727614"></a><a name="zh-cn_topic_0225568844_p28727614"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568844_p45235408"><a name="zh-cn_topic_0225568844_p45235408"></a><a name="zh-cn_topic_0225568844_p45235408"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568844_row4465495"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568844_p26160778"><a name="zh-cn_topic_0225568844_p26160778"></a><a name="zh-cn_topic_0225568844_p26160778"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568844_p14947689"><a name="zh-cn_topic_0225568844_p14947689"></a><a name="zh-cn_topic_0225568844_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

