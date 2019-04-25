# 查询API分组概况<a name="apig-zh-api-180713130"></a>

## 功能介绍<a name="section3399625"></a>

查询租户名下的API分组概况：上架的API分组个数，未上架的API分组个数。

## URI<a name="section30596633"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table53951889"></a>
<table><thead align="left"><tr id="row50990633"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p36600634"><a name="p36600634"></a><a name="p36600634"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p11861416"><a name="p11861416"></a><a name="p11861416"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row21250650"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p43581113"><a name="p43581113"></a><a name="p43581113"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p40409260"><a name="p40409260"></a><a name="p40409260"></a>/v1.0/apigw/resources/outline/groups</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section6934242"></a>

无

## 响应消息<a name="section24802735"></a>

**表 2**  参数说明

<a name="table25113310"></a>
<table><thead align="left"><tr id="row43584205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p40659732"><a name="p40659732"></a><a name="p40659732"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p5104024"><a name="p5104024"></a><a name="p5104024"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p10772800"><a name="p10772800"></a><a name="p10772800"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row181621"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14711326"><a name="p14711326"></a><a name="p14711326"></a>offsell_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p50766756"><a name="p50766756"></a><a name="p50766756"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18466542"><a name="p18466542"></a><a name="p18466542"></a>未上架的API分组个数</p>
</td>
</tr>
<tr id="row31981152"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40336524"><a name="p40336524"></a><a name="p40336524"></a>onsell_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p46033008"><a name="p46033008"></a><a name="p46033008"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p37686197"><a name="p37686197"></a><a name="p37686197"></a>已上架的API分组个数</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"offsell_nums": 1,
	"onsell_nums": 2
}
```

## 状态码<a name="section62408183"></a>

**表 3**  返回消息说明

<a name="table56899163"></a>
<table><thead align="left"><tr id="row33450687"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p25151132"><a name="p25151132"></a><a name="p25151132"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p23975830"><a name="p23975830"></a><a name="p23975830"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row62994068"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p2245887"><a name="p2245887"></a><a name="p2245887"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row26639025"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p10277386"><a name="p10277386"></a><a name="p10277386"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p27161899"><a name="p27161899"></a><a name="p27161899"></a>Bad Request</p>
</td>
</tr>
<tr id="row43130502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3909799"><a name="p3909799"></a><a name="p3909799"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p48258341"><a name="p48258341"></a><a name="p48258341"></a>Unauthorized</p>
</td>
</tr>
<tr id="row31671890"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p15286310"><a name="p15286310"></a><a name="p15286310"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row3648601"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p27101273"><a name="p27101273"></a><a name="p27101273"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

