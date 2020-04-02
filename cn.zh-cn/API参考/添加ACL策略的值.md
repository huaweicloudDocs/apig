# 添加ACL策略的值<a name="apig-phapi-180713087"></a>

## 功能介绍<a name="section8713456"></a>

为ACL策略添加一个或多个策略值， 如果acl\_type的类型是PERMIT则添加的就是白名单；如果acl\_type的类型是DENY则添加的就是黑名单。

根据entity\_type的类型可以添加的值可以为ip或者domain类型。

## URI<a name="section11312246"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table31287710"></a>
<table><thead align="left"><tr id="row8840550"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p44995975"><a name="p44995975"></a><a name="p44995975"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p20795397"><a name="p20795397"></a><a name="p20795397"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row6705607"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p6283318"><a name="p6283318"></a><a name="p6283318"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p39186745"><a name="p39186745"></a><a name="p39186745"></a>/v1/{project_id}/apigw/instances/{instance_id}/acls/aclvalue/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table20009785"></a>
<table><thead align="left"><tr id="row18906804"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p55056187"><a name="p55056187"></a><a name="p55056187"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p30366125"><a name="p30366125"></a><a name="p30366125"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p43737076"><a name="p43737076"></a><a name="p43737076"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p53042296"><a name="p53042296"></a><a name="p53042296"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1337910501181"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row108942049141816"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row1458720"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p51047509"><a name="p51047509"></a><a name="p51047509"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p41207550"><a name="p41207550"></a><a name="p41207550"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p49477252"><a name="p49477252"></a><a name="p49477252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p48234446"><a name="p48234446"></a><a name="p48234446"></a>ACL策略的编号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section34701358"></a>

输入要添加的黑名单或者白名单的值，支持多个值同时输入，使用英文半角逗号分隔。

```
{
	"acl_value": "a987945sdfg-adfa8788-dfa-adfadd423"
}
```

## 响应消息<a name="section59346588"></a>

**表 3**  参数说明

<a name="table13784744"></a>
<table><thead align="left"><tr id="row28652721"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p39169096"><a name="p39169096"></a><a name="p39169096"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p18580170"><a name="p18580170"></a><a name="p18580170"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p28598817"><a name="p28598817"></a><a name="p28598817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34802869"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p460141"><a name="p460141"></a><a name="p460141"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p37271474"><a name="p37271474"></a><a name="p37271474"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66199403"><a name="p66199403"></a><a name="p66199403"></a>编号</p>
</td>
</tr>
<tr id="row58923719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8091914"><a name="p8091914"></a><a name="p8091914"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51465269"><a name="p51465269"></a><a name="p51465269"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7937265"><a name="p7937265"></a><a name="p7937265"></a>名称</p>
</td>
</tr>
<tr id="row4326525"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14904212"><a name="p14904212"></a><a name="p14904212"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66390544"><a name="p66390544"></a><a name="p66390544"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8925017"><a name="p8925017"></a><a name="p8925017"></a>类型</p>
<a name="ul13216294"></a><a name="ul13216294"></a><ul id="ul13216294"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="row38110832"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p67078542"><a name="p67078542"></a><a name="p67078542"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64652825"><a name="p64652825"></a><a name="p64652825"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2387448"><a name="p2387448"></a><a name="p2387448"></a>ACL策略的值</p>
</td>
</tr>
<tr id="row21487035"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p62728244"><a name="p62728244"></a><a name="p62728244"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47822965"><a name="p47822965"></a><a name="p47822965"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48454951"><a name="p48454951"></a><a name="p48454951"></a>对象类型：</p>
<a name="ul33441377"></a><a name="ul33441377"></a><ul id="ul33441377"><li>IP</li><li>DOMAIN</li><li>ADMIN</li></ul>
</td>
</tr>
<tr id="row18246908"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1604592"><a name="p1604592"></a><a name="p1604592"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62863091"><a name="p62863091"></a><a name="p62863091"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p58745648"><a name="p58745648"></a><a name="p58745648"></a>更新时间</p>
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
        "acl_value": "19asdfaf-adfadf，a987945sdfg-adfa8788-dfa-adfadd423",
        "update_time": "2017-11-18T14: 27: 36.918578+08: 00"  
}
```

## 状态码<a name="section43876767"></a>

**表 4**  返回消息说明

<a name="table28544405"></a>
<table><thead align="left"><tr id="row12387945"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p63899507"><a name="p63899507"></a><a name="p63899507"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p8477569"><a name="p8477569"></a><a name="p8477569"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row15594492"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p55194315"><a name="p55194315"></a><a name="p55194315"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p41554519"><a name="p41554519"></a><a name="p41554519"></a>OK</p>
</td>
</tr>
<tr id="row38446351"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p27146688"><a name="p27146688"></a><a name="p27146688"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p51398114"><a name="p51398114"></a><a name="p51398114"></a>Bad Request</p>
</td>
</tr>
<tr id="row59929844"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22479234"><a name="p22479234"></a><a name="p22479234"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p8878676"><a name="p8878676"></a><a name="p8878676"></a>Forbidden</p>
</td>
</tr>
<tr id="row12799227"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p30104430"><a name="p30104430"></a><a name="p30104430"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p22539803"><a name="p22539803"></a><a name="p22539803"></a>Not Found</p>
</td>
</tr>
</tbody>
</table>

