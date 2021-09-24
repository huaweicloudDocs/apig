# 修改自定义认证<a name="ZH-CN_TOPIC_0000001081976233"></a>

## 功能介绍<a name="zh-cn_topic_0225569041_section66524352"></a>

修改自定义认证

## URI<a name="zh-cn_topic_0225569041_section61848258"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225569041_table27084002"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569041_row40355780"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569041_p47592766"><a name="zh-cn_topic_0225569041_p47592766"></a><a name="zh-cn_topic_0225569041_p47592766"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569041_p29808828"><a name="zh-cn_topic_0225569041_p29808828"></a><a name="zh-cn_topic_0225569041_p29808828"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569041_row65704871"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569041_p20494310"><a name="zh-cn_topic_0225569041_p20494310"></a><a name="zh-cn_topic_0225569041_p20494310"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569041_p49426402"><a name="zh-cn_topic_0225569041_p49426402"></a><a name="zh-cn_topic_0225569041_p49426402"></a>/v1/{project_id}/apigw/instances/{instance_id}/authorizers/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225569041_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569041_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569041_p23103637"><a name="zh-cn_topic_0225569041_p23103637"></a><a name="zh-cn_topic_0225569041_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569041_p59455291"><a name="zh-cn_topic_0225569041_p59455291"></a><a name="zh-cn_topic_0225569041_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569041_p51149303"><a name="zh-cn_topic_0225569041_p51149303"></a><a name="zh-cn_topic_0225569041_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569041_p49452846"><a name="zh-cn_topic_0225569041_p49452846"></a><a name="zh-cn_topic_0225569041_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569041_row104409110920"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p45981727916"><a name="zh-cn_topic_0225569041_p45981727916"></a><a name="zh-cn_topic_0225569041_p45981727916"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p1559882399"><a name="zh-cn_topic_0225569041_p1559882399"></a><a name="zh-cn_topic_0225569041_p1559882399"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p0598822910"><a name="zh-cn_topic_0225569041_p0598822910"></a><a name="zh-cn_topic_0225569041_p0598822910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p14598228919"><a name="zh-cn_topic_0225569041_p14598228919"></a><a name="zh-cn_topic_0225569041_p14598228919"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row69041409916"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p1780913159538"><a name="zh-cn_topic_0225569041_p1780913159538"></a><a name="zh-cn_topic_0225569041_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p9809215115310"><a name="zh-cn_topic_0225569041_p9809215115310"></a><a name="zh-cn_topic_0225569041_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p1280914152538"><a name="zh-cn_topic_0225569041_p1280914152538"></a><a name="zh-cn_topic_0225569041_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p1880914157537"><a name="zh-cn_topic_0225569041_p1880914157537"></a><a name="zh-cn_topic_0225569041_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p55878963"><a name="zh-cn_topic_0225569041_p55878963"></a><a name="zh-cn_topic_0225569041_p55878963"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p29902160"><a name="zh-cn_topic_0225569041_p29902160"></a><a name="zh-cn_topic_0225569041_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p6155914"><a name="zh-cn_topic_0225569041_p6155914"></a><a name="zh-cn_topic_0225569041_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p28867016"><a name="zh-cn_topic_0225569041_p28867016"></a><a name="zh-cn_topic_0225569041_p28867016"></a>自定义认证的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225569041_section19763417"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225569041_table44115586"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569041_row63561487"><th class="cellrowborder" valign="top" width="15.17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569041_p48206846"><a name="zh-cn_topic_0225569041_p48206846"></a><a name="zh-cn_topic_0225569041_p48206846"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.12%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569041_p12440449"><a name="zh-cn_topic_0225569041_p12440449"></a><a name="zh-cn_topic_0225569041_p12440449"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569041_p1043457"><a name="zh-cn_topic_0225569041_p1043457"></a><a name="zh-cn_topic_0225569041_p1043457"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569041_p17411173"><a name="zh-cn_topic_0225569041_p17411173"></a><a name="zh-cn_topic_0225569041_p17411173"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569041_row1018902"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p15422203"><a name="zh-cn_topic_0225569041_p15422203"></a><a name="zh-cn_topic_0225569041_p15422203"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p41238908"><a name="zh-cn_topic_0225569041_p41238908"></a><a name="zh-cn_topic_0225569041_p41238908"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p52017283"><a name="zh-cn_topic_0225569041_p52017283"></a><a name="zh-cn_topic_0225569041_p52017283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p52650357"><a name="zh-cn_topic_0225569041_p52650357"></a><a name="zh-cn_topic_0225569041_p52650357"></a>自定义认证的名称。</p>
<p id="zh-cn_topic_0225569041_p62949411"><a name="zh-cn_topic_0225569041_p62949411"></a><a name="zh-cn_topic_0225569041_p62949411"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以英文或中文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row25118534"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p21335372"><a name="zh-cn_topic_0225569041_p21335372"></a><a name="zh-cn_topic_0225569041_p21335372"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p335614714610"><a name="zh-cn_topic_0225569041_p335614714610"></a><a name="zh-cn_topic_0225569041_p335614714610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p59395084"><a name="zh-cn_topic_0225569041_p59395084"></a><a name="zh-cn_topic_0225569041_p59395084"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p46272536"><a name="zh-cn_topic_0225569041_p46272536"></a><a name="zh-cn_topic_0225569041_p46272536"></a>自定义认证类型：</p>
<a name="zh-cn_topic_0225569041_ul184514919444"></a><a name="zh-cn_topic_0225569041_ul184514919444"></a><ul id="zh-cn_topic_0225569041_ul184514919444"><li>FRONTEND：前端</li><li>BACKEND：后端</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row57551867452"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p6755263454"><a name="zh-cn_topic_0225569041_p6755263454"></a><a name="zh-cn_topic_0225569041_p6755263454"></a>authorizer_type</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p167581072468"><a name="zh-cn_topic_0225569041_p167581072468"></a><a name="zh-cn_topic_0225569041_p167581072468"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p15525410194617"><a name="zh-cn_topic_0225569041_p15525410194617"></a><a name="zh-cn_topic_0225569041_p15525410194617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p177550674512"><a name="zh-cn_topic_0225569041_p177550674512"></a><a name="zh-cn_topic_0225569041_p177550674512"></a>只能为：FUNC</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row8176415184514"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p21761515154518"><a name="zh-cn_topic_0225569041_p21761515154518"></a><a name="zh-cn_topic_0225569041_p21761515154518"></a>authorizer_uri</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p12270104464914"><a name="zh-cn_topic_0225569041_p12270104464914"></a><a name="zh-cn_topic_0225569041_p12270104464914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p1924219460498"><a name="zh-cn_topic_0225569041_p1924219460498"></a><a name="zh-cn_topic_0225569041_p1924219460498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p10176161584511"><a name="zh-cn_topic_0225569041_p10176161584511"></a><a name="zh-cn_topic_0225569041_p10176161584511"></a>函数urn</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row143721441454"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p837219434519"><a name="zh-cn_topic_0225569041_p837219434519"></a><a name="zh-cn_topic_0225569041_p837219434519"></a>identities</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p276710171500"><a name="zh-cn_topic_0225569041_p276710171500"></a><a name="zh-cn_topic_0225569041_p276710171500"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p143721548454"><a name="zh-cn_topic_0225569041_p143721548454"></a><a name="zh-cn_topic_0225569041_p143721548454"></a>List</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p7372104124510"><a name="zh-cn_topic_0225569041_p7372104124510"></a><a name="zh-cn_topic_0225569041_p7372104124510"></a>认证来源</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row16161657164410"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p2161175774411"><a name="zh-cn_topic_0225569041_p2161175774411"></a><a name="zh-cn_topic_0225569041_p2161175774411"></a>ttl</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p2848315204816"><a name="zh-cn_topic_0225569041_p2848315204816"></a><a name="zh-cn_topic_0225569041_p2848315204816"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p9162195715445"><a name="zh-cn_topic_0225569041_p9162195715445"></a><a name="zh-cn_topic_0225569041_p9162195715445"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p1116215578449"><a name="zh-cn_topic_0225569041_p1116215578449"></a><a name="zh-cn_topic_0225569041_p1116215578449"></a>缓存时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row193245015451"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p33241209456"><a name="zh-cn_topic_0225569041_p33241209456"></a><a name="zh-cn_topic_0225569041_p33241209456"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p15324209458"><a name="zh-cn_topic_0225569041_p15324209458"></a><a name="zh-cn_topic_0225569041_p15324209458"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p119995794713"><a name="zh-cn_topic_0225569041_p119995794713"></a><a name="zh-cn_topic_0225569041_p119995794713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p63241708451"><a name="zh-cn_topic_0225569041_p63241708451"></a><a name="zh-cn_topic_0225569041_p63241708451"></a>用户数据</p>
</td>
</tr>
</tbody>
</table>

**表 4**  identities参数说明

<a name="zh-cn_topic_0225569041_table751518476529"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569041_row15515104765219"><th class="cellrowborder" valign="top" width="15.17%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569041_p051534710522"><a name="zh-cn_topic_0225569041_p051534710522"></a><a name="zh-cn_topic_0225569041_p051534710522"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.12%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569041_p7515247185217"><a name="zh-cn_topic_0225569041_p7515247185217"></a><a name="zh-cn_topic_0225569041_p7515247185217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569041_p1851554745210"><a name="zh-cn_topic_0225569041_p1851554745210"></a><a name="zh-cn_topic_0225569041_p1851554745210"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569041_p1251518475521"><a name="zh-cn_topic_0225569041_p1251518475521"></a><a name="zh-cn_topic_0225569041_p1251518475521"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569041_row115151247115218"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p851544715212"><a name="zh-cn_topic_0225569041_p851544715212"></a><a name="zh-cn_topic_0225569041_p851544715212"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p135159470525"><a name="zh-cn_topic_0225569041_p135159470525"></a><a name="zh-cn_topic_0225569041_p135159470525"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p05151147195213"><a name="zh-cn_topic_0225569041_p05151147195213"></a><a name="zh-cn_topic_0225569041_p05151147195213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p15515247185210"><a name="zh-cn_topic_0225569041_p15515247185210"></a><a name="zh-cn_topic_0225569041_p15515247185210"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row20515847185220"><td class="cellrowborder" valign="top" width="15.17%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569041_p138669785419"><a name="zh-cn_topic_0225569041_p138669785419"></a><a name="zh-cn_topic_0225569041_p138669785419"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="14.12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569041_p551613475524"><a name="zh-cn_topic_0225569041_p551613475524"></a><a name="zh-cn_topic_0225569041_p551613475524"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569041_p151684735216"><a name="zh-cn_topic_0225569041_p151684735216"></a><a name="zh-cn_topic_0225569041_p151684735216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569041_p164741530135518"><a name="zh-cn_topic_0225569041_p164741530135518"></a><a name="zh-cn_topic_0225569041_p164741530135518"></a>参数位置：</p>
<a name="zh-cn_topic_0225569041_ul20474173014554"></a><a name="zh-cn_topic_0225569041_ul20474173014554"></a><ul id="zh-cn_topic_0225569041_ul20474173014554"><li>HEADER：头</li><li>QUERY：query</li></ul>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
    "name":"Authorizer_9dlh",
    "type":"FRONTEND",
    "authorizer_type":"FUNC",
    "authorizer_uri":"urn:fss:regionexample:dbb5762c88f045c6a1427a952bcae284:function:default:test111",
    "ttl":10,
    "user_data":"aaaa",
    "identities":[
        {
            "name":"Authorization",
            "location":"HEADER"
        }
    ]
}
```

## 响应消息<a name="zh-cn_topic_0225569041_section57332943"></a>

**表 5**  参数说明

<a name="zh-cn_topic_0225569041_table2803298"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569041_row9258659"><th class="cellrowborder" valign="top" width="20.02%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225569041_p11753897"><a name="zh-cn_topic_0225569041_p11753897"></a><a name="zh-cn_topic_0225569041_p11753897"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.98%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225569041_p12541637"><a name="zh-cn_topic_0225569041_p12541637"></a><a name="zh-cn_topic_0225569041_p12541637"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225569041_p9239644"><a name="zh-cn_topic_0225569041_p9239644"></a><a name="zh-cn_topic_0225569041_p9239644"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569041_row10213720"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p22005025"><a name="zh-cn_topic_0225569041_p22005025"></a><a name="zh-cn_topic_0225569041_p22005025"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p37576606"><a name="zh-cn_topic_0225569041_p37576606"></a><a name="zh-cn_topic_0225569041_p37576606"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p23806264"><a name="zh-cn_topic_0225569041_p23806264"></a><a name="zh-cn_topic_0225569041_p23806264"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row12929787"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p40679818"><a name="zh-cn_topic_0225569041_p40679818"></a><a name="zh-cn_topic_0225569041_p40679818"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p6730986"><a name="zh-cn_topic_0225569041_p6730986"></a><a name="zh-cn_topic_0225569041_p6730986"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p4183116625"><a name="zh-cn_topic_0225569041_p4183116625"></a><a name="zh-cn_topic_0225569041_p4183116625"></a>自定义认证的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row7942236"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p078091916016"><a name="zh-cn_topic_0225569041_p078091916016"></a><a name="zh-cn_topic_0225569041_p078091916016"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p43191612927"><a name="zh-cn_topic_0225569041_p43191612927"></a><a name="zh-cn_topic_0225569041_p43191612927"></a></p>
<p id="zh-cn_topic_0225569041_p1131817121824"><a name="zh-cn_topic_0225569041_p1131817121824"></a><a name="zh-cn_topic_0225569041_p1131817121824"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p174157561811"><a name="zh-cn_topic_0225569041_p174157561811"></a><a name="zh-cn_topic_0225569041_p174157561811"></a>自定义认证类型：</p>
<a name="zh-cn_topic_0225569041_ul04151356316"></a><a name="zh-cn_topic_0225569041_ul04151356316"></a><ul id="zh-cn_topic_0225569041_ul04151356316"><li>FRONTEND：前端</li><li>BACKEND：后端</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row26358777"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p14730142317016"><a name="zh-cn_topic_0225569041_p14730142317016"></a><a name="zh-cn_topic_0225569041_p14730142317016"></a>authorizer_type</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p398200"><a name="zh-cn_topic_0225569041_p398200"></a><a name="zh-cn_topic_0225569041_p398200"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p10821651114"><a name="zh-cn_topic_0225569041_p10821651114"></a><a name="zh-cn_topic_0225569041_p10821651114"></a>只能为：FUNC</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row21852379"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p1530418271701"><a name="zh-cn_topic_0225569041_p1530418271701"></a><a name="zh-cn_topic_0225569041_p1530418271701"></a>authorizer_uri</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p36223141827"><a name="zh-cn_topic_0225569041_p36223141827"></a><a name="zh-cn_topic_0225569041_p36223141827"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p13462546519"><a name="zh-cn_topic_0225569041_p13462546519"></a><a name="zh-cn_topic_0225569041_p13462546519"></a>函数urn</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row17074768"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p1404467010"><a name="zh-cn_topic_0225569041_p1404467010"></a><a name="zh-cn_topic_0225569041_p1404467010"></a>identities</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p1289301726"><a name="zh-cn_topic_0225569041_p1289301726"></a><a name="zh-cn_topic_0225569041_p1289301726"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p3687421212"><a name="zh-cn_topic_0225569041_p3687421212"></a><a name="zh-cn_topic_0225569041_p3687421212"></a>认证来源</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row23864751"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p176566481901"><a name="zh-cn_topic_0225569041_p176566481901"></a><a name="zh-cn_topic_0225569041_p176566481901"></a>ttl</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p2566123613220"><a name="zh-cn_topic_0225569041_p2566123613220"></a><a name="zh-cn_topic_0225569041_p2566123613220"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p11732173710119"><a name="zh-cn_topic_0225569041_p11732173710119"></a><a name="zh-cn_topic_0225569041_p11732173710119"></a>缓存时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row19473624"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p13273951706"><a name="zh-cn_topic_0225569041_p13273951706"></a><a name="zh-cn_topic_0225569041_p13273951706"></a>user_data</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p2062812416220"><a name="zh-cn_topic_0225569041_p2062812416220"></a><a name="zh-cn_topic_0225569041_p2062812416220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p112028271314"><a name="zh-cn_topic_0225569041_p112028271314"></a><a name="zh-cn_topic_0225569041_p112028271314"></a>用户数据</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row168471214124017"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p19764828113"><a name="zh-cn_topic_0225569041_p19764828113"></a><a name="zh-cn_topic_0225569041_p19764828113"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p64189201"><a name="zh-cn_topic_0225569041_p64189201"></a><a name="zh-cn_topic_0225569041_p64189201"></a>Time</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p31942831"><a name="zh-cn_topic_0225569041_p31942831"></a><a name="zh-cn_topic_0225569041_p31942831"></a>创建时间</p>
</td>
</tr>
</tbody>
</table>

**表 6**  identities参数说明

<a name="zh-cn_topic_0225569041_table19554526582"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569041_row65535215818"><th class="cellrowborder" valign="top" width="20.02%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225569041_p1555145245815"><a name="zh-cn_topic_0225569041_p1555145245815"></a><a name="zh-cn_topic_0225569041_p1555145245815"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.98%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225569041_p135555214586"><a name="zh-cn_topic_0225569041_p135555214586"></a><a name="zh-cn_topic_0225569041_p135555214586"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225569041_p135535214586"><a name="zh-cn_topic_0225569041_p135535214586"></a><a name="zh-cn_topic_0225569041_p135535214586"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569041_row25525218586"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p146251519115919"><a name="zh-cn_topic_0225569041_p146251519115919"></a><a name="zh-cn_topic_0225569041_p146251519115919"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p165525265811"><a name="zh-cn_topic_0225569041_p165525265811"></a><a name="zh-cn_topic_0225569041_p165525265811"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p1097423515913"><a name="zh-cn_topic_0225569041_p1097423515913"></a><a name="zh-cn_topic_0225569041_p1097423515913"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row125565225812"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225569041_p10536132655914"><a name="zh-cn_topic_0225569041_p10536132655914"></a><a name="zh-cn_topic_0225569041_p10536132655914"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225569041_p655452205813"><a name="zh-cn_topic_0225569041_p655452205813"></a><a name="zh-cn_topic_0225569041_p655452205813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225569041_p692424514593"><a name="zh-cn_topic_0225569041_p692424514593"></a><a name="zh-cn_topic_0225569041_p692424514593"></a>参数位置：</p>
<a name="zh-cn_topic_0225569041_ul5924194585913"></a><a name="zh-cn_topic_0225569041_ul5924194585913"></a><ul id="zh-cn_topic_0225569041_ul5924194585913"><li>HEADER：头</li><li>QUERY：query</li></ul>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
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
    "create_time":"2020-01-19T11:48:56.576611862Z"
}
```

## 状态码<a name="zh-cn_topic_0225569041_section43653029"></a>

**表 7**  返回消息说明

<a name="zh-cn_topic_0225569041_table61067539"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569041_row16541512"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569041_p64794090"><a name="zh-cn_topic_0225569041_p64794090"></a><a name="zh-cn_topic_0225569041_p64794090"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569041_p13829924"><a name="zh-cn_topic_0225569041_p13829924"></a><a name="zh-cn_topic_0225569041_p13829924"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569041_row46482079"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569041_p6952067"><a name="zh-cn_topic_0225569041_p6952067"></a><a name="zh-cn_topic_0225569041_p6952067"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569041_p73578115452"><a name="zh-cn_topic_0225569041_p73578115452"></a><a name="zh-cn_topic_0225569041_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row34892078"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569041_p7686078"><a name="zh-cn_topic_0225569041_p7686078"></a><a name="zh-cn_topic_0225569041_p7686078"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569041_p48128109554"><a name="zh-cn_topic_0225569041_p48128109554"></a><a name="zh-cn_topic_0225569041_p48128109554"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row33115333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569041_p65096331"><a name="zh-cn_topic_0225569041_p65096331"></a><a name="zh-cn_topic_0225569041_p65096331"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569041_p9203142078"><a name="zh-cn_topic_0225569041_p9203142078"></a><a name="zh-cn_topic_0225569041_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row9258873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569041_p11771280"><a name="zh-cn_topic_0225569041_p11771280"></a><a name="zh-cn_topic_0225569041_p11771280"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569041_p13949586"><a name="zh-cn_topic_0225569041_p13949586"></a><a name="zh-cn_topic_0225569041_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569041_row58437416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569041_p35810232"><a name="zh-cn_topic_0225569041_p35810232"></a><a name="zh-cn_topic_0225569041_p35810232"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569041_p14947689"><a name="zh-cn_topic_0225569041_p14947689"></a><a name="zh-cn_topic_0225569041_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

