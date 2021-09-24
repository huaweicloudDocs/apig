# 查询APP概况<a name="ZH-CN_TOPIC_0000001082221217"></a>

## 功能介绍<a name="zh-cn_topic_0118924544_section46313469"></a>

查询租户名下的APP概况：已进行API访问授权的APP个数，未进行API访问授权的APP个数。

## URI<a name="zh-cn_topic_0118924544_section14168045"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924544_table53146607"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924544_row44635631"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924544_p58716368"><a name="zh-cn_topic_0118924544_p58716368"></a><a name="zh-cn_topic_0118924544_p58716368"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924544_p58405369"><a name="zh-cn_topic_0118924544_p58405369"></a><a name="zh-cn_topic_0118924544_p58405369"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924544_row33214483"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924544_p6018630"><a name="zh-cn_topic_0118924544_p6018630"></a><a name="zh-cn_topic_0118924544_p6018630"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924544_p17747001"><a name="zh-cn_topic_0118924544_p17747001"></a><a name="zh-cn_topic_0118924544_p17747001"></a>/v1.0/apigw/resources/outline/apps</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924544_section60403546"></a>

无

## 响应消息<a name="zh-cn_topic_0118924544_section60849047"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118924544_table20164232"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924544_row243552"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924544_p19727751"><a name="zh-cn_topic_0118924544_p19727751"></a><a name="zh-cn_topic_0118924544_p19727751"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924544_p54443990"><a name="zh-cn_topic_0118924544_p54443990"></a><a name="zh-cn_topic_0118924544_p54443990"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924544_p47887094"><a name="zh-cn_topic_0118924544_p47887094"></a><a name="zh-cn_topic_0118924544_p47887094"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924544_row53649423"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924544_p50635976"><a name="zh-cn_topic_0118924544_p50635976"></a><a name="zh-cn_topic_0118924544_p50635976"></a>authed_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924544_p7873353"><a name="zh-cn_topic_0118924544_p7873353"></a><a name="zh-cn_topic_0118924544_p7873353"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924544_p33761851"><a name="zh-cn_topic_0118924544_p33761851"></a><a name="zh-cn_topic_0118924544_p33761851"></a>已进行API访问授权的APP个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924544_row35421205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924544_p50545395"><a name="zh-cn_topic_0118924544_p50545395"></a><a name="zh-cn_topic_0118924544_p50545395"></a>unauthed_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924544_p536341"><a name="zh-cn_topic_0118924544_p536341"></a><a name="zh-cn_topic_0118924544_p536341"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924544_p43443684"><a name="zh-cn_topic_0118924544_p43443684"></a><a name="zh-cn_topic_0118924544_p43443684"></a>未进行API访问授权的APP个数</p>
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

## 状态码<a name="zh-cn_topic_0118924544_section6761005"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924544_table65080456"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924544_row13904495"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924544_p52522300"><a name="zh-cn_topic_0118924544_p52522300"></a><a name="zh-cn_topic_0118924544_p52522300"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924544_p26447889"><a name="zh-cn_topic_0118924544_p26447889"></a><a name="zh-cn_topic_0118924544_p26447889"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924544_row61904279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924544_p48190709"><a name="zh-cn_topic_0118924544_p48190709"></a><a name="zh-cn_topic_0118924544_p48190709"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924544_p50988816"><a name="zh-cn_topic_0118924544_p50988816"></a><a name="zh-cn_topic_0118924544_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924544_row33091708"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924544_p63182654"><a name="zh-cn_topic_0118924544_p63182654"></a><a name="zh-cn_topic_0118924544_p63182654"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924544_p17521365"><a name="zh-cn_topic_0118924544_p17521365"></a><a name="zh-cn_topic_0118924544_p17521365"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924544_row23474564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924544_p22391541"><a name="zh-cn_topic_0118924544_p22391541"></a><a name="zh-cn_topic_0118924544_p22391541"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924544_p1775534"><a name="zh-cn_topic_0118924544_p1775534"></a><a name="zh-cn_topic_0118924544_p1775534"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924544_row15979814"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924544_p19296543"><a name="zh-cn_topic_0118924544_p19296543"></a><a name="zh-cn_topic_0118924544_p19296543"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924544_p13949586"><a name="zh-cn_topic_0118924544_p13949586"></a><a name="zh-cn_topic_0118924544_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924544_row41427614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924544_p193545"><a name="zh-cn_topic_0118924544_p193545"></a><a name="zh-cn_topic_0118924544_p193545"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924544_p6744143"><a name="zh-cn_topic_0118924544_p6744143"></a><a name="zh-cn_topic_0118924544_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

