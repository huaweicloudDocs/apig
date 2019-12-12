# 校验APP<a name="apig-zh-api-180713040"></a>

## 功能介绍<a name="section1576982"></a>

校验APP是否存在，非APP所有者可以调用该接口校验APP是否真实存在。这个接口只展示app的基本信息id 、name、 remark，其他信息不显示。

## URI<a name="section14192838"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table54237251"></a>
<table><thead align="left"><tr id="row37958205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p54715780"><a name="p54715780"></a><a name="p54715780"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p2793224"><a name="p2793224"></a><a name="p2793224"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row24924592"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p5626085"><a name="p5626085"></a><a name="p5626085"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p53059726"><a name="p53059726"></a><a name="p53059726"></a>/v1.0/apigw/apps/validation/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table2870548"></a>
<table><thead align="left"><tr id="row65945959"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p40022483"><a name="p40022483"></a><a name="p40022483"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p20595724"><a name="p20595724"></a><a name="p20595724"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p57640953"><a name="p57640953"></a><a name="p57640953"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p38405635"><a name="p38405635"></a><a name="p38405635"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row23848721"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p52698252"><a name="p52698252"></a><a name="p52698252"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p40699995"><a name="p40699995"></a><a name="p40699995"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p8365287"><a name="p8365287"></a><a name="p8365287"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p6499607"><a name="p6499607"></a><a name="p6499607"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section60626681"></a>

无

## 响应消息<a name="section158712613416"></a>

**表 3**  参数说明

<a name="table10643028"></a>
<table><thead align="left"><tr id="row49499761"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p50057741"><a name="p50057741"></a><a name="p50057741"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p28145188"><a name="p28145188"></a><a name="p28145188"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p65167776"><a name="p65167776"></a><a name="p65167776"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row44098537"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15211750"><a name="p15211750"></a><a name="p15211750"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24192256"><a name="p24192256"></a><a name="p24192256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13415710"><a name="p13415710"></a><a name="p13415710"></a>编号</p>
</td>
</tr>
<tr id="row53632530"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p49267698"><a name="p49267698"></a><a name="p49267698"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31260619"><a name="p31260619"></a><a name="p31260619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p49082180"><a name="p49082180"></a><a name="p49082180"></a>名称</p>
</td>
</tr>
<tr id="row39086436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11884720"><a name="p11884720"></a><a name="p11884720"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23138289"><a name="p23138289"></a><a name="p23138289"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p62262159"><a name="p62262159"></a><a name="p62262159"></a>描述</p>
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

## 状态码<a name="section8769225"></a>

**表 4**  返回消息说明

<a name="table29793924"></a>
<table><thead align="left"><tr id="row42605835"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p28520574"><a name="p28520574"></a><a name="p28520574"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p28465195"><a name="p28465195"></a><a name="p28465195"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row23979448"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p63287117"><a name="p63287117"></a><a name="p63287117"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row32519216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p16810817"><a name="p16810817"></a><a name="p16810817"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p19498968"><a name="p19498968"></a><a name="p19498968"></a>Unauthorized</p>
</td>
</tr>
<tr id="row41272984"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p54777392"><a name="p54777392"></a><a name="p54777392"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p7783744"><a name="p7783744"></a><a name="p7783744"></a>Not Found</p>
</td>
</tr>
<tr id="row2944837"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p37205245"><a name="p37205245"></a><a name="p37205245"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p60834882"><a name="p60834882"></a><a name="p60834882"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

