# 查看ACL策略列表<a name="ZH-CN_TOPIC_0000001081976129"></a>

## 功能介绍<a name="zh-cn_topic_0118924502_section54506040"></a>

查询所有的ACL策略列表。

## URI<a name="zh-cn_topic_0118924502_section20792320"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924502_table49710652"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924502_row2321837"><th class="cellrowborder" valign="top" width="34%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924502_p53851113"><a name="zh-cn_topic_0118924502_p53851113"></a><a name="zh-cn_topic_0118924502_p53851113"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924502_p66972893"><a name="zh-cn_topic_0118924502_p66972893"></a><a name="zh-cn_topic_0118924502_p66972893"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924502_row56095282"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924502_p47424016"><a name="zh-cn_topic_0118924502_p47424016"></a><a name="zh-cn_topic_0118924502_p47424016"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924502_p16140062"><a name="zh-cn_topic_0118924502_p16140062"></a><a name="zh-cn_topic_0118924502_p16140062"></a>/v1.0/apigw/acls[?page_size, page_no, id, name, acl_type, entity_type]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、name、acl\_type、entity\_type、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924502_table41548102"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924502_row34623372"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924502_p53029720"><a name="zh-cn_topic_0118924502_p53029720"></a><a name="zh-cn_topic_0118924502_p53029720"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924502_p440089"><a name="zh-cn_topic_0118924502_p440089"></a><a name="zh-cn_topic_0118924502_p440089"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924502_p35647287"><a name="zh-cn_topic_0118924502_p35647287"></a><a name="zh-cn_topic_0118924502_p35647287"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924502_p1749145"><a name="zh-cn_topic_0118924502_p1749145"></a><a name="zh-cn_topic_0118924502_p1749145"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924502_row7463080"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924502_p529739"><a name="zh-cn_topic_0118924502_p529739"></a><a name="zh-cn_topic_0118924502_p529739"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924502_p42908907"><a name="zh-cn_topic_0118924502_p42908907"></a><a name="zh-cn_topic_0118924502_p42908907"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924502_p53069423"><a name="zh-cn_topic_0118924502_p53069423"></a><a name="zh-cn_topic_0118924502_p53069423"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924502_p3656000"><a name="zh-cn_topic_0118924502_p3656000"></a><a name="zh-cn_topic_0118924502_p3656000"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row32904000"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924502_p47978350"><a name="zh-cn_topic_0118924502_p47978350"></a><a name="zh-cn_topic_0118924502_p47978350"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924502_p61041181"><a name="zh-cn_topic_0118924502_p61041181"></a><a name="zh-cn_topic_0118924502_p61041181"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924502_p45388661"><a name="zh-cn_topic_0118924502_p45388661"></a><a name="zh-cn_topic_0118924502_p45388661"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924502_p52602909"><a name="zh-cn_topic_0118924502_p52602909"></a><a name="zh-cn_topic_0118924502_p52602909"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row3664134"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924502_p28359466"><a name="zh-cn_topic_0118924502_p28359466"></a><a name="zh-cn_topic_0118924502_p28359466"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924502_p15415410"><a name="zh-cn_topic_0118924502_p15415410"></a><a name="zh-cn_topic_0118924502_p15415410"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924502_p40688711"><a name="zh-cn_topic_0118924502_p40688711"></a><a name="zh-cn_topic_0118924502_p40688711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924502_p7451280"><a name="zh-cn_topic_0118924502_p7451280"></a><a name="zh-cn_topic_0118924502_p7451280"></a>类型：PERMIT或DENY</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row67061524"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924502_p63274343"><a name="zh-cn_topic_0118924502_p63274343"></a><a name="zh-cn_topic_0118924502_p63274343"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924502_p24948130"><a name="zh-cn_topic_0118924502_p24948130"></a><a name="zh-cn_topic_0118924502_p24948130"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924502_p7532654"><a name="zh-cn_topic_0118924502_p7532654"></a><a name="zh-cn_topic_0118924502_p7532654"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924502_p6165234"><a name="zh-cn_topic_0118924502_p6165234"></a><a name="zh-cn_topic_0118924502_p6165234"></a>作用的对象类型：IP或DOMAIN</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row45249232"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924502_p41309167"><a name="zh-cn_topic_0118924502_p41309167"></a><a name="zh-cn_topic_0118924502_p41309167"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924502_p57708255"><a name="zh-cn_topic_0118924502_p57708255"></a><a name="zh-cn_topic_0118924502_p57708255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924502_p43857096"><a name="zh-cn_topic_0118924502_p43857096"></a><a name="zh-cn_topic_0118924502_p43857096"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924502_p62763857"><a name="zh-cn_topic_0118924502_p62763857"></a><a name="zh-cn_topic_0118924502_p62763857"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row28003801"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924502_p53715381"><a name="zh-cn_topic_0118924502_p53715381"></a><a name="zh-cn_topic_0118924502_p53715381"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924502_p55978630"><a name="zh-cn_topic_0118924502_p55978630"></a><a name="zh-cn_topic_0118924502_p55978630"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924502_p37975220"><a name="zh-cn_topic_0118924502_p37975220"></a><a name="zh-cn_topic_0118924502_p37975220"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924502_p56093990"><a name="zh-cn_topic_0118924502_p56093990"></a><a name="zh-cn_topic_0118924502_p56093990"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row114619568504"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924502_p814795675016"><a name="zh-cn_topic_0118924502_p814795675016"></a><a name="zh-cn_topic_0118924502_p814795675016"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924502_p18147185612502"><a name="zh-cn_topic_0118924502_p18147185612502"></a><a name="zh-cn_topic_0118924502_p18147185612502"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924502_p3147135625016"><a name="zh-cn_topic_0118924502_p3147135625016"></a><a name="zh-cn_topic_0118924502_p3147135625016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924502_p014785645017"><a name="zh-cn_topic_0118924502_p014785645017"></a><a name="zh-cn_topic_0118924502_p014785645017"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924502_section52913152"></a>

无。

## 响应消息<a name="zh-cn_topic_0118924502_section58106904"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924502_table62046156"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924502_row49550150"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924502_p54139234"><a name="zh-cn_topic_0118924502_p54139234"></a><a name="zh-cn_topic_0118924502_p54139234"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924502_p23201867"><a name="zh-cn_topic_0118924502_p23201867"></a><a name="zh-cn_topic_0118924502_p23201867"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924502_p303080"><a name="zh-cn_topic_0118924502_p303080"></a><a name="zh-cn_topic_0118924502_p303080"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924502_row24549538"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p42355552"><a name="zh-cn_topic_0118924502_p42355552"></a><a name="zh-cn_topic_0118924502_p42355552"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p8247691"><a name="zh-cn_topic_0118924502_p8247691"></a><a name="zh-cn_topic_0118924502_p8247691"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p64083210"><a name="zh-cn_topic_0118924502_p64083210"></a><a name="zh-cn_topic_0118924502_p64083210"></a>当前页返回的ACL策略个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row39877981"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p8890998"><a name="zh-cn_topic_0118924502_p8890998"></a><a name="zh-cn_topic_0118924502_p8890998"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p49082199"><a name="zh-cn_topic_0118924502_p49082199"></a><a name="zh-cn_topic_0118924502_p49082199"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p16235177"><a name="zh-cn_topic_0118924502_p16235177"></a><a name="zh-cn_topic_0118924502_p16235177"></a>ACL策略总个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row11898867"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p24284209"><a name="zh-cn_topic_0118924502_p24284209"></a><a name="zh-cn_topic_0118924502_p24284209"></a>acls</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p20863923"><a name="zh-cn_topic_0118924502_p20863923"></a><a name="zh-cn_topic_0118924502_p20863923"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p12256226"><a name="zh-cn_topic_0118924502_p12256226"></a><a name="zh-cn_topic_0118924502_p12256226"></a>本次查询返回的ACL策略列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  acls参数说明

<a name="zh-cn_topic_0118924502_table43197173"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924502_row67072250"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924502_p64143135"><a name="zh-cn_topic_0118924502_p64143135"></a><a name="zh-cn_topic_0118924502_p64143135"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924502_p28211424"><a name="zh-cn_topic_0118924502_p28211424"></a><a name="zh-cn_topic_0118924502_p28211424"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924502_p3424039"><a name="zh-cn_topic_0118924502_p3424039"></a><a name="zh-cn_topic_0118924502_p3424039"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924502_row8911705"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p50759520"><a name="zh-cn_topic_0118924502_p50759520"></a><a name="zh-cn_topic_0118924502_p50759520"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p17880484"><a name="zh-cn_topic_0118924502_p17880484"></a><a name="zh-cn_topic_0118924502_p17880484"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p39033100"><a name="zh-cn_topic_0118924502_p39033100"></a><a name="zh-cn_topic_0118924502_p39033100"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row15753585"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p972043"><a name="zh-cn_topic_0118924502_p972043"></a><a name="zh-cn_topic_0118924502_p972043"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p11626686"><a name="zh-cn_topic_0118924502_p11626686"></a><a name="zh-cn_topic_0118924502_p11626686"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p2237489"><a name="zh-cn_topic_0118924502_p2237489"></a><a name="zh-cn_topic_0118924502_p2237489"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row20137402"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p20516848"><a name="zh-cn_topic_0118924502_p20516848"></a><a name="zh-cn_topic_0118924502_p20516848"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p51252028"><a name="zh-cn_topic_0118924502_p51252028"></a><a name="zh-cn_topic_0118924502_p51252028"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p57773571"><a name="zh-cn_topic_0118924502_p57773571"></a><a name="zh-cn_topic_0118924502_p57773571"></a>类型</p>
<a name="zh-cn_topic_0118924502_ul50200097"></a><a name="zh-cn_topic_0118924502_ul50200097"></a><ul id="zh-cn_topic_0118924502_ul50200097"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row21540392"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p67050197"><a name="zh-cn_topic_0118924502_p67050197"></a><a name="zh-cn_topic_0118924502_p67050197"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p62356895"><a name="zh-cn_topic_0118924502_p62356895"></a><a name="zh-cn_topic_0118924502_p62356895"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p101249161544"><a name="zh-cn_topic_0118924502_p101249161544"></a><a name="zh-cn_topic_0118924502_p101249161544"></a>ACL策略的值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row25475801"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p50274025"><a name="zh-cn_topic_0118924502_p50274025"></a><a name="zh-cn_topic_0118924502_p50274025"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p45664242"><a name="zh-cn_topic_0118924502_p45664242"></a><a name="zh-cn_topic_0118924502_p45664242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p7816091"><a name="zh-cn_topic_0118924502_p7816091"></a><a name="zh-cn_topic_0118924502_p7816091"></a>对象类型：</p>
<a name="zh-cn_topic_0118924502_ul3235955"></a><a name="zh-cn_topic_0118924502_ul3235955"></a><ul id="zh-cn_topic_0118924502_ul3235955"><li>IP</li><li>DOMAIN</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row10201070"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p20980328"><a name="zh-cn_topic_0118924502_p20980328"></a><a name="zh-cn_topic_0118924502_p20980328"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p21685027"><a name="zh-cn_topic_0118924502_p21685027"></a><a name="zh-cn_topic_0118924502_p21685027"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p11656775"><a name="zh-cn_topic_0118924502_p11656775"></a><a name="zh-cn_topic_0118924502_p11656775"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row37491016615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924502_p52361752033"><a name="zh-cn_topic_0118924502_p52361752033"></a><a name="zh-cn_topic_0118924502_p52361752033"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924502_p12236185032"><a name="zh-cn_topic_0118924502_p12236185032"></a><a name="zh-cn_topic_0118924502_p12236185032"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924502_p17236557312"><a name="zh-cn_topic_0118924502_p17236557312"></a><a name="zh-cn_topic_0118924502_p17236557312"></a>绑定的API数量</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 1,
	"size": 1,
	"acls": [{
		"id": "d402b35e-1054-4280-b1c5-0d741a28c995",
		"acl_name": "goodone",
		"entity_type": "DOMAIN",
		"acl_type": "PERMIT",
		"acl_value": "19asdfaf-adfadf",
		"update_time": "2017-11-18T14:27:36.918578+08:00",
                "bind_num":1
	}]
}
```

## 状态码<a name="zh-cn_topic_0118924502_section6456322"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924502_table7663352"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924502_row65346335"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924502_p58561797"><a name="zh-cn_topic_0118924502_p58561797"></a><a name="zh-cn_topic_0118924502_p58561797"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924502_p45885123"><a name="zh-cn_topic_0118924502_p45885123"></a><a name="zh-cn_topic_0118924502_p45885123"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924502_row25707522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924502_p1934570"><a name="zh-cn_topic_0118924502_p1934570"></a><a name="zh-cn_topic_0118924502_p1934570"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924502_p22482466"><a name="zh-cn_topic_0118924502_p22482466"></a><a name="zh-cn_topic_0118924502_p22482466"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row1015603"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924502_p15155047"><a name="zh-cn_topic_0118924502_p15155047"></a><a name="zh-cn_topic_0118924502_p15155047"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924502_p19599295"><a name="zh-cn_topic_0118924502_p19599295"></a><a name="zh-cn_topic_0118924502_p19599295"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924502_row42175932"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924502_p60807366"><a name="zh-cn_topic_0118924502_p60807366"></a><a name="zh-cn_topic_0118924502_p60807366"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924502_p6744143"><a name="zh-cn_topic_0118924502_p6744143"></a><a name="zh-cn_topic_0118924502_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

