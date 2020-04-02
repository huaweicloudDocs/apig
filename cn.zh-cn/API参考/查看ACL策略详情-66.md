# 查看ACL策略详情<a name="apig-phapi-180713089"></a>

## 功能介绍<a name="section64324135"></a>

查询指定ACL策略的详情。

## URI<a name="section42046308"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table43616361"></a>
<table><thead align="left"><tr id="row53789382"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p61972686"><a name="p61972686"></a><a name="p61972686"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p53731683"><a name="p53731683"></a><a name="p53731683"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row57299052"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p10711634"><a name="p10711634"></a><a name="p10711634"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p62335996"><a name="p62335996"></a><a name="p62335996"></a>/v1/{project_id}/apigw/instances/{instance_id}/acls/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table16050898"></a>
<table><thead align="left"><tr id="row65998730"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p44296919"><a name="p44296919"></a><a name="p44296919"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.5%" id="mcps1.2.5.1.2"><p id="p31280705"><a name="p31280705"></a><a name="p31280705"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="22.939999999999998%" id="mcps1.2.5.1.3"><p id="p50709167"><a name="p50709167"></a><a name="p50709167"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.56%" id="mcps1.2.5.1.4"><p id="p13801866"><a name="p13801866"></a><a name="p13801866"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row6157202521917"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.5%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.56%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row569642419190"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.5%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.56%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row44209337"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p24186533"><a name="p24186533"></a><a name="p24186533"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.5%" headers="mcps1.2.5.1.2 "><p id="p12952117"><a name="p12952117"></a><a name="p12952117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="22.939999999999998%" headers="mcps1.2.5.1.3 "><p id="p42488529"><a name="p42488529"></a><a name="p42488529"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.56%" headers="mcps1.2.5.1.4 "><p id="p19018850"><a name="p19018850"></a><a name="p19018850"></a>ACL策略的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section42872455"></a>

无。

## 响应消息<a name="section50116811"></a>

**表 3**  参数说明

<a name="table5265801"></a>
<table><thead align="left"><tr id="row6311928"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p41504182"><a name="p41504182"></a><a name="p41504182"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p6395556"><a name="p6395556"></a><a name="p6395556"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p48277994"><a name="p48277994"></a><a name="p48277994"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18203441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p65192608"><a name="p65192608"></a><a name="p65192608"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p46109920"><a name="p46109920"></a><a name="p46109920"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p43916057"><a name="p43916057"></a><a name="p43916057"></a>编号</p>
</td>
</tr>
<tr id="row59700194"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3877506"><a name="p3877506"></a><a name="p3877506"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p45642542"><a name="p45642542"></a><a name="p45642542"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6058447"><a name="p6058447"></a><a name="p6058447"></a>名称</p>
</td>
</tr>
<tr id="row54526031"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p54532410"><a name="p54532410"></a><a name="p54532410"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p55049102"><a name="p55049102"></a><a name="p55049102"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p29792241"><a name="p29792241"></a><a name="p29792241"></a>类型</p>
<a name="ul66803585"></a><a name="ul66803585"></a><ul id="ul66803585"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="row45887499"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p25899920"><a name="p25899920"></a><a name="p25899920"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17518790"><a name="p17518790"></a><a name="p17518790"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9393147113"><a name="p9393147113"></a><a name="p9393147113"></a>ACL策略的值</p>
</td>
</tr>
<tr id="row20514172"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51035267"><a name="p51035267"></a><a name="p51035267"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p40215925"><a name="p40215925"></a><a name="p40215925"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36264508"><a name="p36264508"></a><a name="p36264508"></a>对象类型：</p>
<a name="ul57945123"></a><a name="ul57945123"></a><ul id="ul57945123"><li>IP</li><li>DOMAIN</li><li>ADMIN</li></ul>
</td>
</tr>
<tr id="row30519656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p56173085"><a name="p56173085"></a><a name="p56173085"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p53726022"><a name="p53726022"></a><a name="p53726022"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56840524"><a name="p56840524"></a><a name="p56840524"></a>更新时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "d402b35e-1054-4280-b1c5-0d741a28c995",
	"acl_name": "goodone",
	"entity_type": "DOMAIN",
	"acl_type": "PERMIT",
	"acl_value": "19asdfaf-adfadf",
	"update_time": "2017-11-18T14:27:36.918578+08:00"
}
```

## 状态码<a name="section50307777"></a>

**表 4**  返回消息说明

<a name="table27303042"></a>
<table><thead align="left"><tr id="row61133433"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p52861030"><a name="p52861030"></a><a name="p52861030"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p53885019"><a name="p53885019"></a><a name="p53885019"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2610433"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p10118527"><a name="p10118527"></a><a name="p10118527"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14294398"><a name="p14294398"></a><a name="p14294398"></a>OK</p>
</td>
</tr>
<tr id="row61540726"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p18742872"><a name="p18742872"></a><a name="p18742872"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p41777679"><a name="p41777679"></a><a name="p41777679"></a>Bad Request</p>
</td>
</tr>
<tr id="row40454798"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p55613215"><a name="p55613215"></a><a name="p55613215"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p8376568"><a name="p8376568"></a><a name="p8376568"></a>Forbidden</p>
</td>
</tr>
<tr id="row8280256"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p66720985"><a name="p66720985"></a><a name="p66720985"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p35690703"><a name="p35690703"></a><a name="p35690703"></a>Not Found</p>
</td>
</tr>
</tbody>
</table>

