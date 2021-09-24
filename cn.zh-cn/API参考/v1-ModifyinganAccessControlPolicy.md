# 修改ACL策略<a name="ZH-CN_TOPIC_0000001081837367"></a>

## 功能介绍<a name="zh-cn_topic_0225568884_section27236044"></a>

修改指定的ACL策略，其中可修改的属性为：acl\_name、acl\_type、acl\_value，其它属性不可修改。

## URI<a name="zh-cn_topic_0225568884_section43797810"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568884_table40682065"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568884_row57344652"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568884_p14405208"><a name="zh-cn_topic_0225568884_p14405208"></a><a name="zh-cn_topic_0225568884_p14405208"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568884_p25971225"><a name="zh-cn_topic_0225568884_p25971225"></a><a name="zh-cn_topic_0225568884_p25971225"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568884_row23294519"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568884_p7807897"><a name="zh-cn_topic_0225568884_p7807897"></a><a name="zh-cn_topic_0225568884_p7807897"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568884_p28459944"><a name="zh-cn_topic_0225568884_p28459944"></a><a name="zh-cn_topic_0225568884_p28459944"></a>/v1/{project_id}/apigw/instances/{instance_id}/acls/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568884_table23554123"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568884_row26198085"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568884_p41670118"><a name="zh-cn_topic_0225568884_p41670118"></a><a name="zh-cn_topic_0225568884_p41670118"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568884_p19836429"><a name="zh-cn_topic_0225568884_p19836429"></a><a name="zh-cn_topic_0225568884_p19836429"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568884_p63246879"><a name="zh-cn_topic_0225568884_p63246879"></a><a name="zh-cn_topic_0225568884_p63246879"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568884_p22723590"><a name="zh-cn_topic_0225568884_p22723590"></a><a name="zh-cn_topic_0225568884_p22723590"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568884_row7767111219186"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568884_p55878963"><a name="zh-cn_topic_0225568884_p55878963"></a><a name="zh-cn_topic_0225568884_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568884_p29902160"><a name="zh-cn_topic_0225568884_p29902160"></a><a name="zh-cn_topic_0225568884_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568884_p6155914"><a name="zh-cn_topic_0225568884_p6155914"></a><a name="zh-cn_topic_0225568884_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568884_p28867016"><a name="zh-cn_topic_0225568884_p28867016"></a><a name="zh-cn_topic_0225568884_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row85581612121817"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568884_p1780913159538"><a name="zh-cn_topic_0225568884_p1780913159538"></a><a name="zh-cn_topic_0225568884_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568884_p9809215115310"><a name="zh-cn_topic_0225568884_p9809215115310"></a><a name="zh-cn_topic_0225568884_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568884_p1280914152538"><a name="zh-cn_topic_0225568884_p1280914152538"></a><a name="zh-cn_topic_0225568884_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568884_p1880914157537"><a name="zh-cn_topic_0225568884_p1880914157537"></a><a name="zh-cn_topic_0225568884_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row28671530"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568884_p40692594"><a name="zh-cn_topic_0225568884_p40692594"></a><a name="zh-cn_topic_0225568884_p40692594"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568884_p7765831"><a name="zh-cn_topic_0225568884_p7765831"></a><a name="zh-cn_topic_0225568884_p7765831"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568884_p25052560"><a name="zh-cn_topic_0225568884_p25052560"></a><a name="zh-cn_topic_0225568884_p25052560"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568884_p15991478"><a name="zh-cn_topic_0225568884_p15991478"></a><a name="zh-cn_topic_0225568884_p15991478"></a>ACL策略的编号。可通过查询ACL信息获取该ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568884_section58635976"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568884_table20241312"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568884_row40262103"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568884_p40004933"><a name="zh-cn_topic_0225568884_p40004933"></a><a name="zh-cn_topic_0225568884_p40004933"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568884_p19174115"><a name="zh-cn_topic_0225568884_p19174115"></a><a name="zh-cn_topic_0225568884_p19174115"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568884_p9599449"><a name="zh-cn_topic_0225568884_p9599449"></a><a name="zh-cn_topic_0225568884_p9599449"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568884_row39357904"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p33873647"><a name="zh-cn_topic_0225568884_p33873647"></a><a name="zh-cn_topic_0225568884_p33873647"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p59410911"><a name="zh-cn_topic_0225568884_p59410911"></a><a name="zh-cn_topic_0225568884_p59410911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p64172706"><a name="zh-cn_topic_0225568884_p64172706"></a><a name="zh-cn_topic_0225568884_p64172706"></a>ACL策略名称。</p>
<p id="zh-cn_topic_0225568884_p7024991"><a name="zh-cn_topic_0225568884_p7024991"></a><a name="zh-cn_topic_0225568884_p7024991"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0225568884_note1155910113419"><a name="zh-cn_topic_0225568884_note1155910113419"></a><a name="zh-cn_topic_0225568884_note1155910113419"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568884_p1559011141"><a name="zh-cn_topic_0225568884_p1559011141"></a><a name="zh-cn_topic_0225568884_p1559011141"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row25337353"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p39059673"><a name="zh-cn_topic_0225568884_p39059673"></a><a name="zh-cn_topic_0225568884_p39059673"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p9716917"><a name="zh-cn_topic_0225568884_p9716917"></a><a name="zh-cn_topic_0225568884_p9716917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p48872838"><a name="zh-cn_topic_0225568884_p48872838"></a><a name="zh-cn_topic_0225568884_p48872838"></a>类型</p>
<a name="zh-cn_topic_0225568884_ul10284551"></a><a name="zh-cn_topic_0225568884_ul10284551"></a><ul id="zh-cn_topic_0225568884_ul10284551"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row8544294"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p20999237"><a name="zh-cn_topic_0225568884_p20999237"></a><a name="zh-cn_topic_0225568884_p20999237"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p23216632"><a name="zh-cn_topic_0225568884_p23216632"></a><a name="zh-cn_topic_0225568884_p23216632"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p31195995"><a name="zh-cn_topic_0225568884_p31195995"></a><a name="zh-cn_topic_0225568884_p31195995"></a>ACL策略值，支持一个或多个值，使用英文半角逗号分隔</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row1575736142216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p4576036102211"><a name="zh-cn_topic_0225568884_p4576036102211"></a><a name="zh-cn_topic_0225568884_p4576036102211"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p257613620225"><a name="zh-cn_topic_0225568884_p257613620225"></a><a name="zh-cn_topic_0225568884_p257613620225"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p2576153692220"><a name="zh-cn_topic_0225568884_p2576153692220"></a><a name="zh-cn_topic_0225568884_p2576153692220"></a>ACL策略约束对象。取值范围：</p>
<a name="zh-cn_topic_0225568884_ul931411563148"></a><a name="zh-cn_topic_0225568884_ul931411563148"></a><ul id="zh-cn_topic_0225568884_ul931411563148"><li>IP</li><li>DOMAIN （租户名称）</li></ul>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
"acl_name": "string",
	"acl_type": "PERMIT",
	"acl_value": "19asdfaf-adfadf",
	"entity_type": "IP"
}
```

## 响应消息<a name="zh-cn_topic_0225568884_section51893649"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568884_table43596375"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568884_row53923507"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568884_p5727970"><a name="zh-cn_topic_0225568884_p5727970"></a><a name="zh-cn_topic_0225568884_p5727970"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568884_p61312421"><a name="zh-cn_topic_0225568884_p61312421"></a><a name="zh-cn_topic_0225568884_p61312421"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568884_p250213"><a name="zh-cn_topic_0225568884_p250213"></a><a name="zh-cn_topic_0225568884_p250213"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568884_row20267273"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p31036410"><a name="zh-cn_topic_0225568884_p31036410"></a><a name="zh-cn_topic_0225568884_p31036410"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p30921247"><a name="zh-cn_topic_0225568884_p30921247"></a><a name="zh-cn_topic_0225568884_p30921247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p21593056"><a name="zh-cn_topic_0225568884_p21593056"></a><a name="zh-cn_topic_0225568884_p21593056"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row60119783"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p37864287"><a name="zh-cn_topic_0225568884_p37864287"></a><a name="zh-cn_topic_0225568884_p37864287"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p47108391"><a name="zh-cn_topic_0225568884_p47108391"></a><a name="zh-cn_topic_0225568884_p47108391"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p57683303"><a name="zh-cn_topic_0225568884_p57683303"></a><a name="zh-cn_topic_0225568884_p57683303"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row18181035182511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p88568448256"><a name="zh-cn_topic_0225568884_p88568448256"></a><a name="zh-cn_topic_0225568884_p88568448256"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p1285617444259"><a name="zh-cn_topic_0225568884_p1285617444259"></a><a name="zh-cn_topic_0225568884_p1285617444259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p1856194414258"><a name="zh-cn_topic_0225568884_p1856194414258"></a><a name="zh-cn_topic_0225568884_p1856194414258"></a>ACL策略约束对象。取值范围：</p>
<a name="zh-cn_topic_0225568884_ul17856174411259"></a><a name="zh-cn_topic_0225568884_ul17856174411259"></a><ul id="zh-cn_topic_0225568884_ul17856174411259"><li>IP</li><li>DOMAIN （租户名称）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row49387684"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p40979468"><a name="zh-cn_topic_0225568884_p40979468"></a><a name="zh-cn_topic_0225568884_p40979468"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p31002625"><a name="zh-cn_topic_0225568884_p31002625"></a><a name="zh-cn_topic_0225568884_p31002625"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p28184682"><a name="zh-cn_topic_0225568884_p28184682"></a><a name="zh-cn_topic_0225568884_p28184682"></a>类型</p>
<a name="zh-cn_topic_0225568884_ul649664181710"></a><a name="zh-cn_topic_0225568884_ul649664181710"></a><ul id="zh-cn_topic_0225568884_ul649664181710"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row11321137"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p44596876"><a name="zh-cn_topic_0225568884_p44596876"></a><a name="zh-cn_topic_0225568884_p44596876"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p55577208"><a name="zh-cn_topic_0225568884_p55577208"></a><a name="zh-cn_topic_0225568884_p55577208"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p5459996"><a name="zh-cn_topic_0225568884_p5459996"></a><a name="zh-cn_topic_0225568884_p5459996"></a>ACL策略的值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row47547802"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568884_p26166745"><a name="zh-cn_topic_0225568884_p26166745"></a><a name="zh-cn_topic_0225568884_p26166745"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568884_p39131625"><a name="zh-cn_topic_0225568884_p39131625"></a><a name="zh-cn_topic_0225568884_p39131625"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568884_p15545074"><a name="zh-cn_topic_0225568884_p15545074"></a><a name="zh-cn_topic_0225568884_p15545074"></a>更新时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "d402b35e-1054-4280-b1c5-0d741a28c995",
	"acl_name": "goodone",
	"entity_type": "IP",
	"acl_type": "PERMIT",
	"acl_value": "19asdfaf-adfadf",
	"update_time": "2017-11-18T14:27:36.918578+08:00"
}
```

## 状态码<a name="zh-cn_topic_0225568884_section57961744"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568884_table64018620"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568884_row60346675"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568884_p56242477"><a name="zh-cn_topic_0225568884_p56242477"></a><a name="zh-cn_topic_0225568884_p56242477"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568884_p59346771"><a name="zh-cn_topic_0225568884_p59346771"></a><a name="zh-cn_topic_0225568884_p59346771"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568884_row42359183"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568884_p8541766"><a name="zh-cn_topic_0225568884_p8541766"></a><a name="zh-cn_topic_0225568884_p8541766"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568884_p20794466"><a name="zh-cn_topic_0225568884_p20794466"></a><a name="zh-cn_topic_0225568884_p20794466"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row52932474"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568884_p59671976"><a name="zh-cn_topic_0225568884_p59671976"></a><a name="zh-cn_topic_0225568884_p59671976"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568884_p1591854"><a name="zh-cn_topic_0225568884_p1591854"></a><a name="zh-cn_topic_0225568884_p1591854"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row14326690"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568884_p19611232"><a name="zh-cn_topic_0225568884_p19611232"></a><a name="zh-cn_topic_0225568884_p19611232"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568884_p45005963"><a name="zh-cn_topic_0225568884_p45005963"></a><a name="zh-cn_topic_0225568884_p45005963"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568884_row2400484"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568884_p60221533"><a name="zh-cn_topic_0225568884_p60221533"></a><a name="zh-cn_topic_0225568884_p60221533"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568884_p46105974"><a name="zh-cn_topic_0225568884_p46105974"></a><a name="zh-cn_topic_0225568884_p46105974"></a>Not Found</p>
</td>
</tr>
</tbody>
</table>

