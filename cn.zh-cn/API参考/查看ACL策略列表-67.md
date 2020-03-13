# 查看ACL策略列表<a name="apig-phapi-180713090"></a>

## 功能介绍<a name="section54506040"></a>

查询所有的ACL策略列表。

## URI<a name="section20792320"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table49710652"></a>
<table><thead align="left"><tr id="row2321837"><th class="cellrowborder" valign="top" width="34%" id="mcps1.2.3.1.1"><p id="p53851113"><a name="p53851113"></a><a name="p53851113"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="66%" id="mcps1.2.3.1.2"><p id="p66972893"><a name="p66972893"></a><a name="p66972893"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row56095282"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.3.1.1 "><p id="p47424016"><a name="p47424016"></a><a name="p47424016"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.3.1.2 "><p id="p16140062"><a name="p16140062"></a><a name="p16140062"></a><span id="ph835492834418"><a name="ph835492834418"></a><a name="ph835492834418"></a>/v1/{project_id}/apigw/instances/{instance_id}</span>/acls[?page_size, page_no, id, name, acl_type, entity_type, project_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：id、name、acl\_type、entity\_type、project\_id、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table41548102"></a>
<table><thead align="left"><tr id="row34623372"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p53029720"><a name="p53029720"></a><a name="p53029720"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p440089"><a name="p440089"></a><a name="p440089"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p35647287"><a name="p35647287"></a><a name="p35647287"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p1749145"><a name="p1749145"></a><a name="p1749145"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row458174371913"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
<div class="note" id="note2872111254811"><a name="note2872111254811"></a><a name="note2872111254811"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p0872912174810"><a name="p0872912174810"></a><a name="p0872912174810"></a>本字段为请求Path中的project_id。</p>
</div></div>
</td>
</tr>
<tr id="row139752420199"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row7463080"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p529739"><a name="p529739"></a><a name="p529739"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p42908907"><a name="p42908907"></a><a name="p42908907"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p53069423"><a name="p53069423"></a><a name="p53069423"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p3656000"><a name="p3656000"></a><a name="p3656000"></a>编号</p>
</td>
</tr>
<tr id="row32904000"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p47978350"><a name="p47978350"></a><a name="p47978350"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p61041181"><a name="p61041181"></a><a name="p61041181"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p45388661"><a name="p45388661"></a><a name="p45388661"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p52602909"><a name="p52602909"></a><a name="p52602909"></a>名称</p>
</td>
</tr>
<tr id="row3664134"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p28359466"><a name="p28359466"></a><a name="p28359466"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p15415410"><a name="p15415410"></a><a name="p15415410"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p40688711"><a name="p40688711"></a><a name="p40688711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p7451280"><a name="p7451280"></a><a name="p7451280"></a>类型：PERMIT或DENY</p>
</td>
</tr>
<tr id="row67061524"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p63274343"><a name="p63274343"></a><a name="p63274343"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p24948130"><a name="p24948130"></a><a name="p24948130"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p7532654"><a name="p7532654"></a><a name="p7532654"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p6165234"><a name="p6165234"></a><a name="p6165234"></a>作用的对象类型：IP或DOMAIN</p>
</td>
</tr>
<tr id="row11754417143714"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p13754617133710"><a name="p13754617133710"></a><a name="p13754617133710"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p14754111763712"><a name="p14754111763712"></a><a name="p14754111763712"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p57541173377"><a name="p57541173377"></a><a name="p57541173377"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p117547176376"><a name="p117547176376"></a><a name="p117547176376"></a>创建者的项目ID，仅当管理员查询时有效</p>
<div class="note" id="note317714454617"><a name="note317714454617"></a><a name="note317714454617"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p7326104620"><a name="p7326104620"></a><a name="p7326104620"></a>本字段为查询参数中的project_id。</p>
</div></div>
</td>
</tr>
<tr id="row45249232"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p41309167"><a name="p41309167"></a><a name="p41309167"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p57708255"><a name="p57708255"></a><a name="p57708255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p43857096"><a name="p43857096"></a><a name="p43857096"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p62763857"><a name="p62763857"></a><a name="p62763857"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row28003801"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p53715381"><a name="p53715381"></a><a name="p53715381"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p55978630"><a name="p55978630"></a><a name="p55978630"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p37975220"><a name="p37975220"></a><a name="p37975220"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p56093990"><a name="p56093990"></a><a name="p56093990"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="row114619568504"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p814795675016"><a name="p814795675016"></a><a name="p814795675016"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p18147185612502"><a name="p18147185612502"></a><a name="p18147185612502"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p3147135625016"><a name="p3147135625016"></a><a name="p3147135625016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p014785645017"><a name="p014785645017"></a><a name="p014785645017"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section52913152"></a>

无。

## 响应消息<a name="section58106904"></a>

**表 3**  参数说明

<a name="table62046156"></a>
<table><thead align="left"><tr id="row49550150"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p54139234"><a name="p54139234"></a><a name="p54139234"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p23201867"><a name="p23201867"></a><a name="p23201867"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p303080"><a name="p303080"></a><a name="p303080"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row24549538"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p42355552"><a name="p42355552"></a><a name="p42355552"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8247691"><a name="p8247691"></a><a name="p8247691"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p64083210"><a name="p64083210"></a><a name="p64083210"></a>当前页返回的ACL策略个数</p>
</td>
</tr>
<tr id="row39877981"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8890998"><a name="p8890998"></a><a name="p8890998"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p49082199"><a name="p49082199"></a><a name="p49082199"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16235177"><a name="p16235177"></a><a name="p16235177"></a>ACL策略总个数</p>
</td>
</tr>
<tr id="row11898867"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24284209"><a name="p24284209"></a><a name="p24284209"></a>acls</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20863923"><a name="p20863923"></a><a name="p20863923"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12256226"><a name="p12256226"></a><a name="p12256226"></a>本次查询返回的ACL策略列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  acls参数说明

<a name="table43197173"></a>
<table><thead align="left"><tr id="row67072250"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p64143135"><a name="p64143135"></a><a name="p64143135"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p28211424"><a name="p28211424"></a><a name="p28211424"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p3424039"><a name="p3424039"></a><a name="p3424039"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8911705"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50759520"><a name="p50759520"></a><a name="p50759520"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17880484"><a name="p17880484"></a><a name="p17880484"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p39033100"><a name="p39033100"></a><a name="p39033100"></a>编号</p>
</td>
</tr>
<tr id="row15753585"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p972043"><a name="p972043"></a><a name="p972043"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11626686"><a name="p11626686"></a><a name="p11626686"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2237489"><a name="p2237489"></a><a name="p2237489"></a>名称</p>
</td>
</tr>
<tr id="row20137402"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20516848"><a name="p20516848"></a><a name="p20516848"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51252028"><a name="p51252028"></a><a name="p51252028"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57773571"><a name="p57773571"></a><a name="p57773571"></a>类型</p>
<a name="ul50200097"></a><a name="ul50200097"></a><ul id="ul50200097"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="row21540392"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p67050197"><a name="p67050197"></a><a name="p67050197"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62356895"><a name="p62356895"></a><a name="p62356895"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p101249161544"><a name="p101249161544"></a><a name="p101249161544"></a>ACL策略的值</p>
</td>
</tr>
<tr id="row25475801"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50274025"><a name="p50274025"></a><a name="p50274025"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p45664242"><a name="p45664242"></a><a name="p45664242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7816091"><a name="p7816091"></a><a name="p7816091"></a>对象类型：</p>
<a name="ul3235955"></a><a name="ul3235955"></a><ul id="ul3235955"><li>IP</li><li>DOMAIN</li><li>ADMIN</li></ul>
</td>
</tr>
<tr id="row10201070"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20980328"><a name="p20980328"></a><a name="p20980328"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p21685027"><a name="p21685027"></a><a name="p21685027"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11656775"><a name="p11656775"></a><a name="p11656775"></a>更新时间</p>
</td>
</tr>
<tr id="row37491016615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52361752033"><a name="p52361752033"></a><a name="p52361752033"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12236185032"><a name="p12236185032"></a><a name="p12236185032"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17236557312"><a name="p17236557312"></a><a name="p17236557312"></a>绑定的API数量</p>
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

## 状态码<a name="section6456322"></a>

**表 5**  返回消息说明

<a name="table7663352"></a>
<table><thead align="left"><tr id="row65346335"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p58561797"><a name="p58561797"></a><a name="p58561797"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p45885123"><a name="p45885123"></a><a name="p45885123"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row25707522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1934570"><a name="p1934570"></a><a name="p1934570"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p22482466"><a name="p22482466"></a><a name="p22482466"></a>OK</p>
</td>
</tr>
<tr id="row1015603"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p15155047"><a name="p15155047"></a><a name="p15155047"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p19599295"><a name="p19599295"></a><a name="p19599295"></a>Bad Request</p>
</td>
</tr>
<tr id="row42175932"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p60807366"><a name="p60807366"></a><a name="p60807366"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

