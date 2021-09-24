# 查看变量详情<a name="ZH-CN_TOPIC_0000001081976115"></a>

## 功能介绍<a name="zh-cn_topic_0118922252_section33434708"></a>

查看指定的环境变量的详情。

## URI<a name="zh-cn_topic_0118922252_section32476923"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922252_table33084576"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922252_row45012170"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922252_p22107169"><a name="zh-cn_topic_0118922252_p22107169"></a><a name="zh-cn_topic_0118922252_p22107169"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922252_p45850293"><a name="zh-cn_topic_0118922252_p45850293"></a><a name="zh-cn_topic_0118922252_p45850293"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922252_row22886253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922252_p41847218"><a name="zh-cn_topic_0118922252_p41847218"></a><a name="zh-cn_topic_0118922252_p41847218"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922252_p34181483"><a name="zh-cn_topic_0118922252_p34181483"></a><a name="zh-cn_topic_0118922252_p34181483"></a>/v1.0/apigw/env-variables/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922252_table17236737"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922252_row19987860"><th class="cellrowborder" valign="top" width="25.772577257725775%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922252_p8403984"><a name="zh-cn_topic_0118922252_p8403984"></a><a name="zh-cn_topic_0118922252_p8403984"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25.772577257725775%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922252_p9634137"><a name="zh-cn_topic_0118922252_p9634137"></a><a name="zh-cn_topic_0118922252_p9634137"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25.772577257725775%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922252_p42167638"><a name="zh-cn_topic_0118922252_p42167638"></a><a name="zh-cn_topic_0118922252_p42167638"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="22.682268226822686%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922252_p60135536"><a name="zh-cn_topic_0118922252_p60135536"></a><a name="zh-cn_topic_0118922252_p60135536"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922252_row39140238"><td class="cellrowborder" valign="top" width="25.772577257725775%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922252_p16242713"><a name="zh-cn_topic_0118922252_p16242713"></a><a name="zh-cn_topic_0118922252_p16242713"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25.772577257725775%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922252_p40591352"><a name="zh-cn_topic_0118922252_p40591352"></a><a name="zh-cn_topic_0118922252_p40591352"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25.772577257725775%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922252_p66674068"><a name="zh-cn_topic_0118922252_p66674068"></a><a name="zh-cn_topic_0118922252_p66674068"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="22.682268226822686%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922252_p31890388"><a name="zh-cn_topic_0118922252_p31890388"></a><a name="zh-cn_topic_0118922252_p31890388"></a>环境变量的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922252_section23856851"></a>

无

## 响应消息<a name="zh-cn_topic_0118922252_section53356774"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118922252_table36414545"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922252_row62584417"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922252_p36173016"><a name="zh-cn_topic_0118922252_p36173016"></a><a name="zh-cn_topic_0118922252_p36173016"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922252_p44333175"><a name="zh-cn_topic_0118922252_p44333175"></a><a name="zh-cn_topic_0118922252_p44333175"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922252_p34217447"><a name="zh-cn_topic_0118922252_p34217447"></a><a name="zh-cn_topic_0118922252_p34217447"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922252_row20149840"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922252_p21524313"><a name="zh-cn_topic_0118922252_p21524313"></a><a name="zh-cn_topic_0118922252_p21524313"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922252_p65747754"><a name="zh-cn_topic_0118922252_p65747754"></a><a name="zh-cn_topic_0118922252_p65747754"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922252_p23967852"><a name="zh-cn_topic_0118922252_p23967852"></a><a name="zh-cn_topic_0118922252_p23967852"></a>环境变量的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row14384078"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922252_p24259708"><a name="zh-cn_topic_0118922252_p24259708"></a><a name="zh-cn_topic_0118922252_p24259708"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922252_p18879342"><a name="zh-cn_topic_0118922252_p18879342"></a><a name="zh-cn_topic_0118922252_p18879342"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922252_p52831757"><a name="zh-cn_topic_0118922252_p52831757"></a><a name="zh-cn_topic_0118922252_p52831757"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row5723768"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922252_p60972101"><a name="zh-cn_topic_0118922252_p60972101"></a><a name="zh-cn_topic_0118922252_p60972101"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922252_p39793138"><a name="zh-cn_topic_0118922252_p39793138"></a><a name="zh-cn_topic_0118922252_p39793138"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922252_p2018727"><a name="zh-cn_topic_0118922252_p2018727"></a><a name="zh-cn_topic_0118922252_p2018727"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row18168549"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922252_p62366330"><a name="zh-cn_topic_0118922252_p62366330"></a><a name="zh-cn_topic_0118922252_p62366330"></a>variable_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922252_p18507947"><a name="zh-cn_topic_0118922252_p18507947"></a><a name="zh-cn_topic_0118922252_p18507947"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922252_p22748770"><a name="zh-cn_topic_0118922252_p22748770"></a><a name="zh-cn_topic_0118922252_p22748770"></a>变量名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row3412338"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922252_p7963946"><a name="zh-cn_topic_0118922252_p7963946"></a><a name="zh-cn_topic_0118922252_p7963946"></a>variable_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922252_p41099866"><a name="zh-cn_topic_0118922252_p41099866"></a><a name="zh-cn_topic_0118922252_p41099866"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922252_p40754859"><a name="zh-cn_topic_0118922252_p40754859"></a><a name="zh-cn_topic_0118922252_p40754859"></a>变量值</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "104185e5-3e8f-4c63-a7e5-ef4117bf870c",
	"env_id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
	"group_id": "73c58022-f20d-495a-a188-85d718647f09",
	"variable_name": "address",
	"variable_value": "192.168.1.5"
}
```

## 状态码<a name="zh-cn_topic_0118922252_section13385070"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118922252_table54507617"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922252_row12107248"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922252_p41162995"><a name="zh-cn_topic_0118922252_p41162995"></a><a name="zh-cn_topic_0118922252_p41162995"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922252_p45868336"><a name="zh-cn_topic_0118922252_p45868336"></a><a name="zh-cn_topic_0118922252_p45868336"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922252_row24347725"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922252_p26008690"><a name="zh-cn_topic_0118922252_p26008690"></a><a name="zh-cn_topic_0118922252_p26008690"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922252_p26329160"><a name="zh-cn_topic_0118922252_p26329160"></a><a name="zh-cn_topic_0118922252_p26329160"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row35635853"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922252_p822958"><a name="zh-cn_topic_0118922252_p822958"></a><a name="zh-cn_topic_0118922252_p822958"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922252_p66659669"><a name="zh-cn_topic_0118922252_p66659669"></a><a name="zh-cn_topic_0118922252_p66659669"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row63066109"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922252_p8081189"><a name="zh-cn_topic_0118922252_p8081189"></a><a name="zh-cn_topic_0118922252_p8081189"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922252_p50596549"><a name="zh-cn_topic_0118922252_p50596549"></a><a name="zh-cn_topic_0118922252_p50596549"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row52715762"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922252_p42118330"><a name="zh-cn_topic_0118922252_p42118330"></a><a name="zh-cn_topic_0118922252_p42118330"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922252_p56141583"><a name="zh-cn_topic_0118922252_p56141583"></a><a name="zh-cn_topic_0118922252_p56141583"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row35512201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922252_p57916060"><a name="zh-cn_topic_0118922252_p57916060"></a><a name="zh-cn_topic_0118922252_p57916060"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922252_p60689263"><a name="zh-cn_topic_0118922252_p60689263"></a><a name="zh-cn_topic_0118922252_p60689263"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922252_row9332456"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922252_p17731454"><a name="zh-cn_topic_0118922252_p17731454"></a><a name="zh-cn_topic_0118922252_p17731454"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922252_p14947689"><a name="zh-cn_topic_0118922252_p14947689"></a><a name="zh-cn_topic_0118922252_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

