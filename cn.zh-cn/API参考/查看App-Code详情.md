# 查看App Code详情<a name="apig-phapi-200226003"></a>

## 功能介绍<a name="zh-cn_topic_0118921764_section48433431"></a>

查看App Code详细信息。

## URI<a name="zh-cn_topic_0118921763_section37593697"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921763_table15644193"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row49821820"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921763_p9035630"><a name="zh-cn_topic_0118921763_p9035630"></a><a name="zh-cn_topic_0118921763_p9035630"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921763_p60797453"><a name="zh-cn_topic_0118921763_p60797453"></a><a name="zh-cn_topic_0118921763_p60797453"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921763_row25646656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p64113264"><a name="zh-cn_topic_0118921763_p64113264"></a><a name="zh-cn_topic_0118921763_p64113264"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p25791876"><a name="zh-cn_topic_0118921763_p25791876"></a><a name="zh-cn_topic_0118921763_p25791876"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps/{app_id}/app-codes/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921763_table8767205"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row50080004"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921763_p29948539"><a name="zh-cn_topic_0118921763_p29948539"></a><a name="zh-cn_topic_0118921763_p29948539"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921763_p9912623"><a name="zh-cn_topic_0118921763_p9912623"></a><a name="zh-cn_topic_0118921763_p9912623"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921763_p64724999"><a name="zh-cn_topic_0118921763_p64724999"></a><a name="zh-cn_topic_0118921763_p64724999"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921763_p8233580"><a name="zh-cn_topic_0118921763_p8233580"></a><a name="zh-cn_topic_0118921763_p8233580"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12521928162"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row159727301665"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row62940229"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921763_p64993787"><a name="zh-cn_topic_0118921763_p64993787"></a><a name="zh-cn_topic_0118921763_p64993787"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921763_p30005365"><a name="zh-cn_topic_0118921763_p30005365"></a><a name="zh-cn_topic_0118921763_p30005365"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921763_p14515483"><a name="zh-cn_topic_0118921763_p14515483"></a><a name="zh-cn_topic_0118921763_p14515483"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921763_p34903511"><a name="zh-cn_topic_0118921763_p34903511"></a><a name="zh-cn_topic_0118921763_p34903511"></a>App Code的编号</p>
</td>
</tr>
<tr id="row943312981910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p24341599197"><a name="p24341599197"></a><a name="p24341599197"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p5434290195"><a name="p5434290195"></a><a name="p5434290195"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p543529161911"><a name="p543529161911"></a><a name="p543529161911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p19435996196"><a name="p19435996196"></a><a name="p19435996196"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921763_section2798957"></a>

无

## 响应消息<a name="zh-cn_topic_0118921763_section25388955"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921758_table20910139"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921758_row9919741"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921758_p65301594"><a name="zh-cn_topic_0118921758_p65301594"></a><a name="zh-cn_topic_0118921758_p65301594"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921758_p54937751"><a name="zh-cn_topic_0118921758_p54937751"></a><a name="zh-cn_topic_0118921758_p54937751"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921758_p20772828"><a name="zh-cn_topic_0118921758_p20772828"></a><a name="zh-cn_topic_0118921758_p20772828"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921758_row4877522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p59535008"><a name="zh-cn_topic_0118921758_p59535008"></a><a name="zh-cn_topic_0118921758_p59535008"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p57606383"><a name="zh-cn_topic_0118921758_p57606383"></a><a name="zh-cn_topic_0118921758_p57606383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p35605479"><a name="zh-cn_topic_0118921758_p35605479"></a><a name="zh-cn_topic_0118921758_p35605479"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row52013857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p52372904"><a name="zh-cn_topic_0118921758_p52372904"></a><a name="zh-cn_topic_0118921758_p52372904"></a>app_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p14346860"><a name="zh-cn_topic_0118921758_p14346860"></a><a name="zh-cn_topic_0118921758_p14346860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p21245012"><a name="zh-cn_topic_0118921758_p21245012"></a><a name="zh-cn_topic_0118921758_p21245012"></a>App Code值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row56987385"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p52575507"><a name="zh-cn_topic_0118921758_p52575507"></a><a name="zh-cn_topic_0118921758_p52575507"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p30757702"><a name="zh-cn_topic_0118921758_p30757702"></a><a name="zh-cn_topic_0118921758_p30757702"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1284315287524"><a name="p1284315287524"></a><a name="p1284315287524"></a>APP的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row8004354"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p44372920"><a name="zh-cn_topic_0118921758_p44372920"></a><a name="zh-cn_topic_0118921758_p44372920"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p37436804"><a name="zh-cn_topic_0118921758_p37436804"></a><a name="zh-cn_topic_0118921758_p37436804"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p12482251"><a name="zh-cn_topic_0118921758_p12482251"></a><a name="zh-cn_topic_0118921758_p12482251"></a>创建时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
    "app_code": "GjOD3g80AABuuFeEJpVQADBlAjBh3UzC7W+gr4VJBB5BtJ4fdVOQoSvoji3gFxUDb5pWBz9wUcw9+8/bFZ1B/4pq29wCMQC0pQWX6zTndljDEl99As1pw+WntAU9xcq+ffagoH6zDpKUvdxV6Ezj8LcCcPZN6BU=",
    "id": "2fb07c4391d0401696ed345dd1229158",
    "app_id": "db246f3f2ecd45f29ecb0f305e821fdc",
    "create_time": "2019-06-05T04:57:14.470987604Z"
}
```

## 状态码<a name="zh-cn_topic_0118921763_section25190616"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118921763_table26492330"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row38027958"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921763_p60365757"><a name="zh-cn_topic_0118921763_p60365757"></a><a name="zh-cn_topic_0118921763_p60365757"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921763_p57788140"><a name="zh-cn_topic_0118921763_p57788140"></a><a name="zh-cn_topic_0118921763_p57788140"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921763_row50327788"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p50019045"><a name="zh-cn_topic_0118921763_p50019045"></a><a name="zh-cn_topic_0118921763_p50019045"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p25010814"><a name="zh-cn_topic_0118921763_p25010814"></a><a name="zh-cn_topic_0118921763_p25010814"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row23770734"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p46381274"><a name="zh-cn_topic_0118921763_p46381274"></a><a name="zh-cn_topic_0118921763_p46381274"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p65895739"><a name="zh-cn_topic_0118921763_p65895739"></a><a name="zh-cn_topic_0118921763_p65895739"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row56190747"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p55156678"><a name="zh-cn_topic_0118921763_p55156678"></a><a name="zh-cn_topic_0118921763_p55156678"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p38505946"><a name="zh-cn_topic_0118921763_p38505946"></a><a name="zh-cn_topic_0118921763_p38505946"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row11009194"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p19329517"><a name="zh-cn_topic_0118921763_p19329517"></a><a name="zh-cn_topic_0118921763_p19329517"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p22187053"><a name="zh-cn_topic_0118921763_p22187053"></a><a name="zh-cn_topic_0118921763_p22187053"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row65465751"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p1125596"><a name="zh-cn_topic_0118921763_p1125596"></a><a name="zh-cn_topic_0118921763_p1125596"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p24064466"><a name="zh-cn_topic_0118921763_p24064466"></a><a name="zh-cn_topic_0118921763_p24064466"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

