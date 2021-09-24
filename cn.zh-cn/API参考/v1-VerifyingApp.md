# 校验APP<a name="ZH-CN_TOPIC_0000001082221255"></a>

## 功能介绍<a name="zh-cn_topic_0225568837_section1576982"></a>

校验APP是否存在，非APP所有者可以调用该接口校验APP是否真实存在。这个接口只展示app的基本信息id 、name、 remark，其他信息不显示。

## URI<a name="zh-cn_topic_0225568837_section14192838"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568837_table54237251"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568837_row37958205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568837_p54715780"><a name="zh-cn_topic_0225568837_p54715780"></a><a name="zh-cn_topic_0225568837_p54715780"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568837_p2793224"><a name="zh-cn_topic_0225568837_p2793224"></a><a name="zh-cn_topic_0225568837_p2793224"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568837_row24924592"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568837_p5626085"><a name="zh-cn_topic_0225568837_p5626085"></a><a name="zh-cn_topic_0225568837_p5626085"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568837_p53059726"><a name="zh-cn_topic_0225568837_p53059726"></a><a name="zh-cn_topic_0225568837_p53059726"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps/validation/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568837_table2870548"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568837_row65945959"><th class="cellrowborder" valign="top" width="25.000000000000007%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568837_p40022483"><a name="zh-cn_topic_0225568837_p40022483"></a><a name="zh-cn_topic_0225568837_p40022483"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.09%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568837_p20595724"><a name="zh-cn_topic_0225568837_p20595724"></a><a name="zh-cn_topic_0225568837_p20595724"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.69%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568837_p57640953"><a name="zh-cn_topic_0225568837_p57640953"></a><a name="zh-cn_topic_0225568837_p57640953"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.220000000000006%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568837_p38405635"><a name="zh-cn_topic_0225568837_p38405635"></a><a name="zh-cn_topic_0225568837_p38405635"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568837_row1811515773914"><td class="cellrowborder" valign="top" width="25.000000000000007%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568837_p55878963"><a name="zh-cn_topic_0225568837_p55878963"></a><a name="zh-cn_topic_0225568837_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568837_p29902160"><a name="zh-cn_topic_0225568837_p29902160"></a><a name="zh-cn_topic_0225568837_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.69%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568837_p6155914"><a name="zh-cn_topic_0225568837_p6155914"></a><a name="zh-cn_topic_0225568837_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.220000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568837_p28867016"><a name="zh-cn_topic_0225568837_p28867016"></a><a name="zh-cn_topic_0225568837_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568837_row1494216683917"><td class="cellrowborder" valign="top" width="25.000000000000007%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568837_p1780913159538"><a name="zh-cn_topic_0225568837_p1780913159538"></a><a name="zh-cn_topic_0225568837_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568837_p9809215115310"><a name="zh-cn_topic_0225568837_p9809215115310"></a><a name="zh-cn_topic_0225568837_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.69%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568837_p1280914152538"><a name="zh-cn_topic_0225568837_p1280914152538"></a><a name="zh-cn_topic_0225568837_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.220000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568837_p1880914157537"><a name="zh-cn_topic_0225568837_p1880914157537"></a><a name="zh-cn_topic_0225568837_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568837_row23848721"><td class="cellrowborder" valign="top" width="25.000000000000007%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568837_p52698252"><a name="zh-cn_topic_0225568837_p52698252"></a><a name="zh-cn_topic_0225568837_p52698252"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568837_p40699995"><a name="zh-cn_topic_0225568837_p40699995"></a><a name="zh-cn_topic_0225568837_p40699995"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.69%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568837_p8365287"><a name="zh-cn_topic_0225568837_p8365287"></a><a name="zh-cn_topic_0225568837_p8365287"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.220000000000006%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568837_p6499607"><a name="zh-cn_topic_0225568837_p6499607"></a><a name="zh-cn_topic_0225568837_p6499607"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568837_section60626681"></a>

无

## 响应消息<a name="zh-cn_topic_0225568837_section158712613416"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568837_table10643028"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568837_row49499761"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568837_p50057741"><a name="zh-cn_topic_0225568837_p50057741"></a><a name="zh-cn_topic_0225568837_p50057741"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568837_p28145188"><a name="zh-cn_topic_0225568837_p28145188"></a><a name="zh-cn_topic_0225568837_p28145188"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568837_p65167776"><a name="zh-cn_topic_0225568837_p65167776"></a><a name="zh-cn_topic_0225568837_p65167776"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568837_row44098537"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568837_p15211750"><a name="zh-cn_topic_0225568837_p15211750"></a><a name="zh-cn_topic_0225568837_p15211750"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568837_p24192256"><a name="zh-cn_topic_0225568837_p24192256"></a><a name="zh-cn_topic_0225568837_p24192256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568837_p13415710"><a name="zh-cn_topic_0225568837_p13415710"></a><a name="zh-cn_topic_0225568837_p13415710"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568837_row53632530"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568837_p49267698"><a name="zh-cn_topic_0225568837_p49267698"></a><a name="zh-cn_topic_0225568837_p49267698"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568837_p31260619"><a name="zh-cn_topic_0225568837_p31260619"></a><a name="zh-cn_topic_0225568837_p31260619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568837_p49082180"><a name="zh-cn_topic_0225568837_p49082180"></a><a name="zh-cn_topic_0225568837_p49082180"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568837_row39086436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568837_p11884720"><a name="zh-cn_topic_0225568837_p11884720"></a><a name="zh-cn_topic_0225568837_p11884720"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568837_p23138289"><a name="zh-cn_topic_0225568837_p23138289"></a><a name="zh-cn_topic_0225568837_p23138289"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568837_p62262159"><a name="zh-cn_topic_0225568837_p62262159"></a><a name="zh-cn_topic_0225568837_p62262159"></a>描述</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "14b399ac-967f-4115-bb62-c0346b4537e9",
	"name": "app_001",
	"remark": "第一个APP"
}
```

## 状态码<a name="zh-cn_topic_0225568837_section8769225"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0225568837_table29793924"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568837_row42605835"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568837_p28520574"><a name="zh-cn_topic_0225568837_p28520574"></a><a name="zh-cn_topic_0225568837_p28520574"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568837_p28465195"><a name="zh-cn_topic_0225568837_p28465195"></a><a name="zh-cn_topic_0225568837_p28465195"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568837_row23979448"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568837_p63287117"><a name="zh-cn_topic_0225568837_p63287117"></a><a name="zh-cn_topic_0225568837_p63287117"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568837_p50988816"><a name="zh-cn_topic_0225568837_p50988816"></a><a name="zh-cn_topic_0225568837_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568837_row32519216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568837_p16810817"><a name="zh-cn_topic_0225568837_p16810817"></a><a name="zh-cn_topic_0225568837_p16810817"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568837_p19498968"><a name="zh-cn_topic_0225568837_p19498968"></a><a name="zh-cn_topic_0225568837_p19498968"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568837_row41272984"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568837_p54777392"><a name="zh-cn_topic_0225568837_p54777392"></a><a name="zh-cn_topic_0225568837_p54777392"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568837_p7783744"><a name="zh-cn_topic_0225568837_p7783744"></a><a name="zh-cn_topic_0225568837_p7783744"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568837_row2944837"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568837_p37205245"><a name="zh-cn_topic_0225568837_p37205245"></a><a name="zh-cn_topic_0225568837_p37205245"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568837_p60834882"><a name="zh-cn_topic_0225568837_p60834882"></a><a name="zh-cn_topic_0225568837_p60834882"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

