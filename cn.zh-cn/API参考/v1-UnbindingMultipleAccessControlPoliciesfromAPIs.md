# 批量解除API与ACL策略的绑定<a name="ZH-CN_TOPIC_0000001082221287"></a>

## 功能介绍<a name="zh-cn_topic_0225568898_section24863152"></a>

批量解除API与ACL策略的绑定关系。

## URI<a name="zh-cn_topic_0225568898_section22441780"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568898_table47776868"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568898_row14972112"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568898_p4781565"><a name="zh-cn_topic_0225568898_p4781565"></a><a name="zh-cn_topic_0225568898_p4781565"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568898_p51762503"><a name="zh-cn_topic_0225568898_p51762503"></a><a name="zh-cn_topic_0225568898_p51762503"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568898_row32013205"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568898_p42932816"><a name="zh-cn_topic_0225568898_p42932816"></a><a name="zh-cn_topic_0225568898_p42932816"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568898_p55006047"><a name="zh-cn_topic_0225568898_p55006047"></a><a name="zh-cn_topic_0225568898_p55006047"></a>/v1/{project_id}/apigw/instances/{instance_id}/acl-bindings[?action]</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568898_table26304811"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568898_row11931990"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568898_p26967144"><a name="zh-cn_topic_0225568898_p26967144"></a><a name="zh-cn_topic_0225568898_p26967144"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.02%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568898_p36855079"><a name="zh-cn_topic_0225568898_p36855079"></a><a name="zh-cn_topic_0225568898_p36855079"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.68%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568898_p32471418"><a name="zh-cn_topic_0225568898_p32471418"></a><a name="zh-cn_topic_0225568898_p32471418"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="37.3%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568898_p12939210"><a name="zh-cn_topic_0225568898_p12939210"></a><a name="zh-cn_topic_0225568898_p12939210"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568898_row14221165132113"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568898_p55878963"><a name="zh-cn_topic_0225568898_p55878963"></a><a name="zh-cn_topic_0225568898_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.02%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568898_p29902160"><a name="zh-cn_topic_0225568898_p29902160"></a><a name="zh-cn_topic_0225568898_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568898_p6155914"><a name="zh-cn_topic_0225568898_p6155914"></a><a name="zh-cn_topic_0225568898_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.3%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568898_p28867016"><a name="zh-cn_topic_0225568898_p28867016"></a><a name="zh-cn_topic_0225568898_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row17799194182118"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568898_p1780913159538"><a name="zh-cn_topic_0225568898_p1780913159538"></a><a name="zh-cn_topic_0225568898_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.02%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568898_p9809215115310"><a name="zh-cn_topic_0225568898_p9809215115310"></a><a name="zh-cn_topic_0225568898_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568898_p1280914152538"><a name="zh-cn_topic_0225568898_p1280914152538"></a><a name="zh-cn_topic_0225568898_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.3%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568898_p1880914157537"><a name="zh-cn_topic_0225568898_p1880914157537"></a><a name="zh-cn_topic_0225568898_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row41443070"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568898_p1445503"><a name="zh-cn_topic_0225568898_p1445503"></a><a name="zh-cn_topic_0225568898_p1445503"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="18.02%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568898_p49976884"><a name="zh-cn_topic_0225568898_p49976884"></a><a name="zh-cn_topic_0225568898_p49976884"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.68%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568898_p21595781"><a name="zh-cn_topic_0225568898_p21595781"></a><a name="zh-cn_topic_0225568898_p21595781"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.3%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568898_p4427868"><a name="zh-cn_topic_0225568898_p4427868"></a><a name="zh-cn_topic_0225568898_p4427868"></a>必须为delete</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568898_section649433"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568898_table11428152"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568898_row63593960"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568898_p50837158"><a name="zh-cn_topic_0225568898_p50837158"></a><a name="zh-cn_topic_0225568898_p50837158"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568898_p24169108"><a name="zh-cn_topic_0225568898_p24169108"></a><a name="zh-cn_topic_0225568898_p24169108"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568898_p11540698"><a name="zh-cn_topic_0225568898_p11540698"></a><a name="zh-cn_topic_0225568898_p11540698"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568898_p62381345"><a name="zh-cn_topic_0225568898_p62381345"></a><a name="zh-cn_topic_0225568898_p62381345"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568898_row19724176"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568898_p111152374516"><a name="zh-cn_topic_0225568898_p111152374516"></a><a name="zh-cn_topic_0225568898_p111152374516"></a>acl_bindings</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568898_p24434185"><a name="zh-cn_topic_0225568898_p24434185"></a><a name="zh-cn_topic_0225568898_p24434185"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568898_p33011938"><a name="zh-cn_topic_0225568898_p33011938"></a><a name="zh-cn_topic_0225568898_p33011938"></a>String Array</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568898_p56721283"><a name="zh-cn_topic_0225568898_p56721283"></a><a name="zh-cn_topic_0225568898_p56721283"></a>需要解除绑定的ACL策略ID列表</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
    "acl_bindings": ["81efcfd94b8747a0b21e8c04144a4e8c","7addcd00cfab433984b1d8bf2fe08aaa"]
}
```

## 响应消息<a name="zh-cn_topic_0225568898_section52604147"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568898_table2981672313"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568898_row898177103111"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568898_p109837183116"><a name="zh-cn_topic_0225568898_p109837183116"></a><a name="zh-cn_topic_0225568898_p109837183116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568898_p1098474319"><a name="zh-cn_topic_0225568898_p1098474319"></a><a name="zh-cn_topic_0225568898_p1098474319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568898_p1398197193117"><a name="zh-cn_topic_0225568898_p1398197193117"></a><a name="zh-cn_topic_0225568898_p1398197193117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568898_row49812719314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568898_p782812469154"><a name="zh-cn_topic_0225568898_p782812469154"></a><a name="zh-cn_topic_0225568898_p782812469154"></a>success_count</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568898_p209815717318"><a name="zh-cn_topic_0225568898_p209815717318"></a><a name="zh-cn_topic_0225568898_p209815717318"></a>Number</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568898_p8980773120"><a name="zh-cn_topic_0225568898_p8980773120"></a><a name="zh-cn_topic_0225568898_p8980773120"></a>成功解除绑定的ACL策略数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row119827123112"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568898_p159814710314"><a name="zh-cn_topic_0225568898_p159814710314"></a><a name="zh-cn_topic_0225568898_p159814710314"></a>failure</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568898_p1698871311"><a name="zh-cn_topic_0225568898_p1698871311"></a><a name="zh-cn_topic_0225568898_p1698871311"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568898_p109897153112"><a name="zh-cn_topic_0225568898_p109897153112"></a><a name="zh-cn_topic_0225568898_p109897153112"></a>解除绑定失败的ACL策略及错误信息</p>
</td>
</tr>
</tbody>
</table>

**表 5**  failure参数说明

<a name="zh-cn_topic_0225568898_table15660564193"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568898_row137265631919"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568898_p173165641915"><a name="zh-cn_topic_0225568898_p173165641915"></a><a name="zh-cn_topic_0225568898_p173165641915"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568898_p187385616195"><a name="zh-cn_topic_0225568898_p187385616195"></a><a name="zh-cn_topic_0225568898_p187385616195"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568898_p1876256171919"><a name="zh-cn_topic_0225568898_p1876256171919"></a><a name="zh-cn_topic_0225568898_p1876256171919"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568898_row57665621920"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568898_p477175615191"><a name="zh-cn_topic_0225568898_p477175615191"></a><a name="zh-cn_topic_0225568898_p477175615191"></a>bind_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568898_p179185671915"><a name="zh-cn_topic_0225568898_p179185671915"></a><a name="zh-cn_topic_0225568898_p179185671915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568898_p1379115621913"><a name="zh-cn_topic_0225568898_p1379115621913"></a><a name="zh-cn_topic_0225568898_p1379115621913"></a>解除绑定失败的ACL策略ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row138175661920"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568898_p11458112915203"><a name="zh-cn_topic_0225568898_p11458112915203"></a><a name="zh-cn_topic_0225568898_p11458112915203"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568898_p38145613190"><a name="zh-cn_topic_0225568898_p38145613190"></a><a name="zh-cn_topic_0225568898_p38145613190"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568898_p1882175612193"><a name="zh-cn_topic_0225568898_p1882175612193"></a><a name="zh-cn_topic_0225568898_p1882175612193"></a>解除绑定失败的错误码</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row18262135516207"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568898_p142627557208"><a name="zh-cn_topic_0225568898_p142627557208"></a><a name="zh-cn_topic_0225568898_p142627557208"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568898_p1426220553205"><a name="zh-cn_topic_0225568898_p1426220553205"></a><a name="zh-cn_topic_0225568898_p1426220553205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568898_p32621855152010"><a name="zh-cn_topic_0225568898_p32621855152010"></a><a name="zh-cn_topic_0225568898_p32621855152010"></a>解除绑定失败的错误信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row1512815719557"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568898_p121281785513"><a name="zh-cn_topic_0225568898_p121281785513"></a><a name="zh-cn_topic_0225568898_p121281785513"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568898_p7128876552"><a name="zh-cn_topic_0225568898_p7128876552"></a><a name="zh-cn_topic_0225568898_p7128876552"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568898_p612813765512"><a name="zh-cn_topic_0225568898_p612813765512"></a><a name="zh-cn_topic_0225568898_p612813765512"></a>解除绑定失败的API的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row12281493556"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568898_p922889135517"><a name="zh-cn_topic_0225568898_p922889135517"></a><a name="zh-cn_topic_0225568898_p922889135517"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568898_p1022817905512"><a name="zh-cn_topic_0225568898_p1022817905512"></a><a name="zh-cn_topic_0225568898_p1022817905512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568898_p182281895557"><a name="zh-cn_topic_0225568898_p182281895557"></a><a name="zh-cn_topic_0225568898_p182281895557"></a>解除绑定失败的API的名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"failure": [{
		"bind_id": "81efcfd94b8747a0b21e8c04144a4e8c",
		"error_code": "APIG.3010",
		"error_msg": "Access control policy binding record not found",
                "api_id": "81efcfd94b8747a0b21e8c04144a4e8c",
		"api_name": "api01"
	}],
	"success_count": 3
}
```

## 状态码<a name="zh-cn_topic_0225568898_section5844905"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0225568898_table15714732"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568898_row24997277"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568898_p11513591"><a name="zh-cn_topic_0225568898_p11513591"></a><a name="zh-cn_topic_0225568898_p11513591"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568898_p60185706"><a name="zh-cn_topic_0225568898_p60185706"></a><a name="zh-cn_topic_0225568898_p60185706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568898_row43203997"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568898_p9862840"><a name="zh-cn_topic_0225568898_p9862840"></a><a name="zh-cn_topic_0225568898_p9862840"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568898_p73578115452"><a name="zh-cn_topic_0225568898_p73578115452"></a><a name="zh-cn_topic_0225568898_p73578115452"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row9362312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568898_p20149775"><a name="zh-cn_topic_0225568898_p20149775"></a><a name="zh-cn_topic_0225568898_p20149775"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568898_p21519099"><a name="zh-cn_topic_0225568898_p21519099"></a><a name="zh-cn_topic_0225568898_p21519099"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row59454171"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568898_p51058521"><a name="zh-cn_topic_0225568898_p51058521"></a><a name="zh-cn_topic_0225568898_p51058521"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568898_p9203142078"><a name="zh-cn_topic_0225568898_p9203142078"></a><a name="zh-cn_topic_0225568898_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row43351211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568898_p21787193"><a name="zh-cn_topic_0225568898_p21787193"></a><a name="zh-cn_topic_0225568898_p21787193"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568898_p13949586"><a name="zh-cn_topic_0225568898_p13949586"></a><a name="zh-cn_topic_0225568898_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row45172181"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568898_p35068062"><a name="zh-cn_topic_0225568898_p35068062"></a><a name="zh-cn_topic_0225568898_p35068062"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568898_p21940743"><a name="zh-cn_topic_0225568898_p21940743"></a><a name="zh-cn_topic_0225568898_p21940743"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568898_row63248959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568898_p22892027"><a name="zh-cn_topic_0225568898_p22892027"></a><a name="zh-cn_topic_0225568898_p22892027"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568898_p14947689"><a name="zh-cn_topic_0225568898_p14947689"></a><a name="zh-cn_topic_0225568898_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

