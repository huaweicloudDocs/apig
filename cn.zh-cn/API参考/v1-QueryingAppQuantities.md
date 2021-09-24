# 查询APP概况<a name="ZH-CN_TOPIC_0000001081976211"></a>

## 功能介绍<a name="zh-cn_topic_0225568933_section46313469"></a>

查询租户名下的APP概况：已进行API访问授权的APP个数，未进行API访问授权的APP个数。

## URI<a name="zh-cn_topic_0225568933_section14168045"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568933_table53146607"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568933_row44635631"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568933_p58716368"><a name="zh-cn_topic_0225568933_p58716368"></a><a name="zh-cn_topic_0225568933_p58716368"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568933_p58405369"><a name="zh-cn_topic_0225568933_p58405369"></a><a name="zh-cn_topic_0225568933_p58405369"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568933_row33214483"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568933_p6018630"><a name="zh-cn_topic_0225568933_p6018630"></a><a name="zh-cn_topic_0225568933_p6018630"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568933_p17747001"><a name="zh-cn_topic_0225568933_p17747001"></a><a name="zh-cn_topic_0225568933_p17747001"></a>/v1/{project_id}/apigw/instances/{instance_id}/resources/outline/apps</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568933_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568933_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568933_p23103637"><a name="zh-cn_topic_0225568933_p23103637"></a><a name="zh-cn_topic_0225568933_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568933_p59455291"><a name="zh-cn_topic_0225568933_p59455291"></a><a name="zh-cn_topic_0225568933_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568933_p51149303"><a name="zh-cn_topic_0225568933_p51149303"></a><a name="zh-cn_topic_0225568933_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568933_p49452846"><a name="zh-cn_topic_0225568933_p49452846"></a><a name="zh-cn_topic_0225568933_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568933_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568933_p55878963"><a name="zh-cn_topic_0225568933_p55878963"></a><a name="zh-cn_topic_0225568933_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568933_p29902160"><a name="zh-cn_topic_0225568933_p29902160"></a><a name="zh-cn_topic_0225568933_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568933_p6155914"><a name="zh-cn_topic_0225568933_p6155914"></a><a name="zh-cn_topic_0225568933_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568933_p28867016"><a name="zh-cn_topic_0225568933_p28867016"></a><a name="zh-cn_topic_0225568933_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568933_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568933_p1780913159538"><a name="zh-cn_topic_0225568933_p1780913159538"></a><a name="zh-cn_topic_0225568933_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568933_p9809215115310"><a name="zh-cn_topic_0225568933_p9809215115310"></a><a name="zh-cn_topic_0225568933_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568933_p1280914152538"><a name="zh-cn_topic_0225568933_p1280914152538"></a><a name="zh-cn_topic_0225568933_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568933_p1880914157537"><a name="zh-cn_topic_0225568933_p1880914157537"></a><a name="zh-cn_topic_0225568933_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568933_section60403546"></a>

无

## 响应消息<a name="zh-cn_topic_0225568933_section60849047"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568933_table20164232"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568933_row243552"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568933_p19727751"><a name="zh-cn_topic_0225568933_p19727751"></a><a name="zh-cn_topic_0225568933_p19727751"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568933_p54443990"><a name="zh-cn_topic_0225568933_p54443990"></a><a name="zh-cn_topic_0225568933_p54443990"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568933_p47887094"><a name="zh-cn_topic_0225568933_p47887094"></a><a name="zh-cn_topic_0225568933_p47887094"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568933_row53649423"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568933_p50635976"><a name="zh-cn_topic_0225568933_p50635976"></a><a name="zh-cn_topic_0225568933_p50635976"></a>authed_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568933_p7873353"><a name="zh-cn_topic_0225568933_p7873353"></a><a name="zh-cn_topic_0225568933_p7873353"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568933_p33761851"><a name="zh-cn_topic_0225568933_p33761851"></a><a name="zh-cn_topic_0225568933_p33761851"></a>已进行API访问授权的APP个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568933_row35421205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568933_p50545395"><a name="zh-cn_topic_0225568933_p50545395"></a><a name="zh-cn_topic_0225568933_p50545395"></a>unauthed_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568933_p536341"><a name="zh-cn_topic_0225568933_p536341"></a><a name="zh-cn_topic_0225568933_p536341"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568933_p43443684"><a name="zh-cn_topic_0225568933_p43443684"></a><a name="zh-cn_topic_0225568933_p43443684"></a>未进行API访问授权的APP个数</p>
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

## 状态码<a name="zh-cn_topic_0225568933_section6761005"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0225568933_table65080456"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568933_row13904495"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568933_p52522300"><a name="zh-cn_topic_0225568933_p52522300"></a><a name="zh-cn_topic_0225568933_p52522300"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568933_p26447889"><a name="zh-cn_topic_0225568933_p26447889"></a><a name="zh-cn_topic_0225568933_p26447889"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568933_row61904279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568933_p48190709"><a name="zh-cn_topic_0225568933_p48190709"></a><a name="zh-cn_topic_0225568933_p48190709"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568933_p50988816"><a name="zh-cn_topic_0225568933_p50988816"></a><a name="zh-cn_topic_0225568933_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568933_row33091708"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568933_p63182654"><a name="zh-cn_topic_0225568933_p63182654"></a><a name="zh-cn_topic_0225568933_p63182654"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568933_p17521365"><a name="zh-cn_topic_0225568933_p17521365"></a><a name="zh-cn_topic_0225568933_p17521365"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568933_row23474564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568933_p22391541"><a name="zh-cn_topic_0225568933_p22391541"></a><a name="zh-cn_topic_0225568933_p22391541"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568933_p1775534"><a name="zh-cn_topic_0225568933_p1775534"></a><a name="zh-cn_topic_0225568933_p1775534"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568933_row15979814"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568933_p19296543"><a name="zh-cn_topic_0225568933_p19296543"></a><a name="zh-cn_topic_0225568933_p19296543"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568933_p13949586"><a name="zh-cn_topic_0225568933_p13949586"></a><a name="zh-cn_topic_0225568933_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568933_row41427614"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568933_p193545"><a name="zh-cn_topic_0225568933_p193545"></a><a name="zh-cn_topic_0225568933_p193545"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568933_p6744143"><a name="zh-cn_topic_0225568933_p6744143"></a><a name="zh-cn_topic_0225568933_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

