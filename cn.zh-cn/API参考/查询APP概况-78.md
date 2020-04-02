# 查询APP概况<a name="apig-phapi-180713132"></a>

## 功能介绍<a name="section46313469"></a>

查询租户名下的APP概况：已进行API访问授权的APP个数，未进行API访问授权的APP个数。

## URI<a name="section14168045"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table53146607"></a>
<table><thead align="left"><tr id="row44635631"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p58716368"><a name="p58716368"></a><a name="p58716368"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p58405369"><a name="p58405369"></a><a name="p58405369"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row33214483"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6018630"><a name="p6018630"></a><a name="p6018630"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p17747001"><a name="p17747001"></a><a name="p17747001"></a>/v1/{project_id}/apigw/instances/{instance_id}/resources/outline/apps</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table38510415"></a>
<table><thead align="left"><tr id="row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="p23103637"><a name="p23103637"></a><a name="p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p59455291"><a name="p59455291"></a><a name="p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="p51149303"><a name="p51149303"></a><a name="p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="p49452846"><a name="p49452846"></a><a name="p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section60403546"></a>

无

## 响应消息<a name="section60849047"></a>

**表 3**  参数说明

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

**表 4**  返回消息说明

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

