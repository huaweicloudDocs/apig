# 查询APP概况<a name="apig-zh-api-180713132"></a>

## 功能介绍<a name="section46313469"></a>

查询租户名下的APP概况：已进行API访问授权的APP个数，未进行API访问授权的APP个数。

## URI<a name="section14168045"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table53146607"></a>
<table><thead align="left"><tr id="row44635631"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p58716368"><a name="p58716368"></a><a name="p58716368"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p58405369"><a name="p58405369"></a><a name="p58405369"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row33214483"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p6018630"><a name="p6018630"></a><a name="p6018630"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p17747001"><a name="p17747001"></a><a name="p17747001"></a>/v1.0/apigw/resources/outline/apps</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section60403546"></a>

无

## 响应消息<a name="section60849047"></a>

**表 2**  参数说明

<a name="table20164232"></a>
<table><thead align="left"><tr id="row243552"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p19727751"><a name="p19727751"></a><a name="p19727751"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p54443990"><a name="p54443990"></a><a name="p54443990"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p47887094"><a name="p47887094"></a><a name="p47887094"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row53649423"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50635976"><a name="p50635976"></a><a name="p50635976"></a>authed_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7873353"><a name="p7873353"></a><a name="p7873353"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p33761851"><a name="p33761851"></a><a name="p33761851"></a>已进行API访问授权的APP个数</p>
</td>
</tr>
<tr id="row35421205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50545395"><a name="p50545395"></a><a name="p50545395"></a>unauthed_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p536341"><a name="p536341"></a><a name="p536341"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p43443684"><a name="p43443684"></a><a name="p43443684"></a>未进行API访问授权的APP个数</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"authed_nums": 1,
	"unauthed_nums": 2
}
```

## 状态码<a name="section6761005"></a>

**表 3**  返回消息说明

<a name="table65080456"></a>
<table><thead align="left"><tr id="row13904495"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p52522300"><a name="p52522300"></a><a name="p52522300"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p26447889"><a name="p26447889"></a><a name="p26447889"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row61904279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p48190709"><a name="p48190709"></a><a name="p48190709"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row33091708"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p63182654"><a name="p63182654"></a><a name="p63182654"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p17521365"><a name="p17521365"></a><a name="p17521365"></a>Bad Request</p>
</td>
</tr>
<tr id="row23474564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22391541"><a name="p22391541"></a><a name="p22391541"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1775534"><a name="p1775534"></a><a name="p1775534"></a>Unauthorized</p>
</td>
</tr>
<tr id="row15979814"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p19296543"><a name="p19296543"></a><a name="p19296543"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row41427614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p193545"><a name="p193545"></a><a name="p193545"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

