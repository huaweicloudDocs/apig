# 批量删除API<a name="apig-phapi-181219253"></a>

## 功能介绍<a name="section24863152"></a>

批量删除指定的多个API，以及指定分组下的所有API。

删除API时，同时删除该API所有相关的资源信息或绑定关系，如API的发布记录、绑定的后端服务和对APP的授权信息等。

## URI<a name="section22441780"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table47776868"></a>
<table><thead align="left"><tr id="row14972112"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p4781565"><a name="p4781565"></a><a name="p4781565"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p51762503"><a name="p51762503"></a><a name="p51762503"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row32013205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p42932816"><a name="p42932816"></a><a name="p42932816"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p55006047"><a name="p55006047"></a><a name="p55006047"></a>/v1/{project_id}/apigw/instances/{instance_id}/apis[?action]</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table26304811"></a>
<table><thead align="left"><tr id="row11931990"><th class="cellrowborder" valign="top" width="21.19%" id="mcps1.2.5.1.1"><p id="p26967144"><a name="p26967144"></a><a name="p26967144"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.98%" id="mcps1.2.5.1.2"><p id="p36855079"><a name="p36855079"></a><a name="p36855079"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.83%" id="mcps1.2.5.1.3"><p id="p32471418"><a name="p32471418"></a><a name="p32471418"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41%" id="mcps1.2.5.1.4"><p id="p12939210"><a name="p12939210"></a><a name="p12939210"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row14240731151718"><td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.83%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row1217143117173"><td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.83%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row41443070"><td class="cellrowborder" valign="top" width="21.19%" headers="mcps1.2.5.1.1 "><p id="p1445503"><a name="p1445503"></a><a name="p1445503"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="18.98%" headers="mcps1.2.5.1.2 "><p id="p49976884"><a name="p49976884"></a><a name="p49976884"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.83%" headers="mcps1.2.5.1.3 "><p id="p21595781"><a name="p21595781"></a><a name="p21595781"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41%" headers="mcps1.2.5.1.4 "><p id="p4427868"><a name="p4427868"></a><a name="p4427868"></a>必须为delete</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section649433"></a>

**表 3**  参数说明

<a name="table11428152"></a>
<table><thead align="left"><tr id="row63593960"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p50837158"><a name="p50837158"></a><a name="p50837158"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p24169108"><a name="p24169108"></a><a name="p24169108"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p11540698"><a name="p11540698"></a><a name="p11540698"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p62381345"><a name="p62381345"></a><a name="p62381345"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19724176"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p111152374516"><a name="p111152374516"></a><a name="p111152374516"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p24434185"><a name="p24434185"></a><a name="p24434185"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p33011938"><a name="p33011938"></a><a name="p33011938"></a>String Array</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p56721283"><a name="p56721283"></a><a name="p56721283"></a>需要删除的API ID列表</p>
</td>
</tr>
<tr id="row10755391"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p65880381"><a name="p65880381"></a><a name="p65880381"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p34710655"><a name="p34710655"></a><a name="p34710655"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p60099694"><a name="p60099694"></a><a name="p60099694"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p36237041"><a name="p36237041"></a><a name="p36237041"></a>分组ID，将删除对应分组下所有API</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"apis": ["81efcfd94b8747a0b21e8c04144a4e8c","7addcd00cfab433984b1d8bf2fe08aaa"],
	"group_id": "7efb2b91155a4f6a9f45c5c95a6e4950"
}
```

## 响应消息<a name="section52604147"></a>

**表 4**  参数说明

<a name="table2981672313"></a>
<table><thead align="left"><tr id="row898177103111"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="p109837183116"><a name="p109837183116"></a><a name="p109837183116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="p1098474319"><a name="p1098474319"></a><a name="p1098474319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="p1398197193117"><a name="p1398197193117"></a><a name="p1398197193117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49812719314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p782812469154"><a name="p782812469154"></a><a name="p782812469154"></a>success_count</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p209815717318"><a name="p209815717318"></a><a name="p209815717318"></a>Number</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p8980773120"><a name="p8980773120"></a><a name="p8980773120"></a>删除成功的API数量</p>
</td>
</tr>
<tr id="row119827123112"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p159814710314"><a name="p159814710314"></a><a name="p159814710314"></a>failure</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p1698871311"><a name="p1698871311"></a><a name="p1698871311"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p109897153112"><a name="p109897153112"></a><a name="p109897153112"></a>删除失败的API及错误信息</p>
</td>
</tr>
</tbody>
</table>

**表 5**  failure参数说明

<a name="table15660564193"></a>
<table><thead align="left"><tr id="row137265631919"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="p173165641915"><a name="p173165641915"></a><a name="p173165641915"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="p187385616195"><a name="p187385616195"></a><a name="p187385616195"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="p1876256171919"><a name="p1876256171919"></a><a name="p1876256171919"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row57665621920"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p477175615191"><a name="p477175615191"></a><a name="p477175615191"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p179185671915"><a name="p179185671915"></a><a name="p179185671915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p1379115621913"><a name="p1379115621913"></a><a name="p1379115621913"></a>删除失败的API ID</p>
</td>
</tr>
<tr id="row1217813206516"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p10180620115120"><a name="p10180620115120"></a><a name="p10180620115120"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p91801620165120"><a name="p91801620165120"></a><a name="p91801620165120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p61801320105112"><a name="p61801320105112"></a><a name="p61801320105112"></a>删除失败的API名称</p>
</td>
</tr>
<tr id="row138175661920"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p11458112915203"><a name="p11458112915203"></a><a name="p11458112915203"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p38145613190"><a name="p38145613190"></a><a name="p38145613190"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p1882175612193"><a name="p1882175612193"></a><a name="p1882175612193"></a>删除失败的错误码</p>
</td>
</tr>
<tr id="row18262135516207"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p142627557208"><a name="p142627557208"></a><a name="p142627557208"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p1426220553205"><a name="p1426220553205"></a><a name="p1426220553205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p32621855152010"><a name="p32621855152010"></a><a name="p32621855152010"></a>删除失败的错误信息</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"failure": [{
		"api_id": "81efcfd94b8747a0b21e8c04144a4e8c",
		"error_code": "APIG.3002",
		"error_msg": "api with id 81efcfd94b8747a0b21e8c04144a4e8c not found"
	}],
	"success_count": 3
}
```

## 状态码<a name="section5844905"></a>

**表 6**  返回消息说明

<a name="table15714732"></a>
<table><thead align="left"><tr id="row24997277"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p11513591"><a name="p11513591"></a><a name="p11513591"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p60185706"><a name="p60185706"></a><a name="p60185706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row43203997"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9862840"><a name="p9862840"></a><a name="p9862840"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p73578115452"><a name="p73578115452"></a><a name="p73578115452"></a>Created</p>
</td>
</tr>
<tr id="row9362312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20149775"><a name="p20149775"></a><a name="p20149775"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p21519099"><a name="p21519099"></a><a name="p21519099"></a>Bad Request</p>
</td>
</tr>
<tr id="row59454171"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p51058521"><a name="p51058521"></a><a name="p51058521"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row43351211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p21787193"><a name="p21787193"></a><a name="p21787193"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row45172181"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p35068062"><a name="p35068062"></a><a name="p35068062"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p21940743"><a name="p21940743"></a><a name="p21940743"></a>Not Found</p>
</td>
</tr>
<tr id="row63248959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22892027"><a name="p22892027"></a><a name="p22892027"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

<a name="table60212917"></a>
<table><thead align="left"></thead>
<tbody></tbody>
</table>

