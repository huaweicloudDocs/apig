# 解除授权<a name="ZH-CN_TOPIC_0000001081837275"></a>

## 功能介绍<a name="zh-cn_topic_0118922241_section59173016"></a>

解除API对APP的授权关系。解除授权后，APP将不再能够调用该API。

## URI<a name="zh-cn_topic_0118922241_section62795097"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922241_table9779415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922241_row3539980"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922241_p18302929"><a name="zh-cn_topic_0118922241_p18302929"></a><a name="zh-cn_topic_0118922241_p18302929"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922241_p6142258"><a name="zh-cn_topic_0118922241_p6142258"></a><a name="zh-cn_topic_0118922241_p6142258"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922241_row27760921"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922241_p34042091"><a name="zh-cn_topic_0118922241_p34042091"></a><a name="zh-cn_topic_0118922241_p34042091"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922241_p5946002"><a name="zh-cn_topic_0118922241_p5946002"></a><a name="zh-cn_topic_0118922241_p5946002"></a>/v1.0/apigw/app-auths/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922241_table11864182"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922241_row62649346"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922241_p41432236"><a name="zh-cn_topic_0118922241_p41432236"></a><a name="zh-cn_topic_0118922241_p41432236"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.36816318368163%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922241_p567938"><a name="zh-cn_topic_0118922241_p567938"></a><a name="zh-cn_topic_0118922241_p567938"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922241_p46003054"><a name="zh-cn_topic_0118922241_p46003054"></a><a name="zh-cn_topic_0118922241_p46003054"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.815918408159185%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922241_p35259861"><a name="zh-cn_topic_0118922241_p35259861"></a><a name="zh-cn_topic_0118922241_p35259861"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922241_row37476513"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922241_p15698746"><a name="zh-cn_topic_0118922241_p15698746"></a><a name="zh-cn_topic_0118922241_p15698746"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.36816318368163%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922241_p63638919"><a name="zh-cn_topic_0118922241_p63638919"></a><a name="zh-cn_topic_0118922241_p63638919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922241_p54478833"><a name="zh-cn_topic_0118922241_p54478833"></a><a name="zh-cn_topic_0118922241_p54478833"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.815918408159185%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922241_p50709343"><a name="zh-cn_topic_0118922241_p50709343"></a><a name="zh-cn_topic_0118922241_p50709343"></a>授权关系的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922241_section28284964"></a>

无

## 响应消息<a name="zh-cn_topic_0118922241_section9380773"></a>

无

## 状态码<a name="zh-cn_topic_0118922241_section53238091"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118922241_table45364073"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922241_row52860430"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922241_p53836432"><a name="zh-cn_topic_0118922241_p53836432"></a><a name="zh-cn_topic_0118922241_p53836432"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922241_p65783722"><a name="zh-cn_topic_0118922241_p65783722"></a><a name="zh-cn_topic_0118922241_p65783722"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922241_row26881285"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922241_p29900489"><a name="zh-cn_topic_0118922241_p29900489"></a><a name="zh-cn_topic_0118922241_p29900489"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922241_p6020508"><a name="zh-cn_topic_0118922241_p6020508"></a><a name="zh-cn_topic_0118922241_p6020508"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922241_row54184580"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922241_p26874868"><a name="zh-cn_topic_0118922241_p26874868"></a><a name="zh-cn_topic_0118922241_p26874868"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922241_p29380680"><a name="zh-cn_topic_0118922241_p29380680"></a><a name="zh-cn_topic_0118922241_p29380680"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922241_row63099531"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922241_p10788401"><a name="zh-cn_topic_0118922241_p10788401"></a><a name="zh-cn_topic_0118922241_p10788401"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922241_p1445295"><a name="zh-cn_topic_0118922241_p1445295"></a><a name="zh-cn_topic_0118922241_p1445295"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922241_row13007663"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922241_p46987814"><a name="zh-cn_topic_0118922241_p46987814"></a><a name="zh-cn_topic_0118922241_p46987814"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922241_p47916552"><a name="zh-cn_topic_0118922241_p47916552"></a><a name="zh-cn_topic_0118922241_p47916552"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922241_row28595790"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922241_p34557630"><a name="zh-cn_topic_0118922241_p34557630"></a><a name="zh-cn_topic_0118922241_p34557630"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922241_p47704655"><a name="zh-cn_topic_0118922241_p47704655"></a><a name="zh-cn_topic_0118922241_p47704655"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922241_row26688715"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922241_p14302320"><a name="zh-cn_topic_0118922241_p14302320"></a><a name="zh-cn_topic_0118922241_p14302320"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922241_p14947689"><a name="zh-cn_topic_0118922241_p14947689"></a><a name="zh-cn_topic_0118922241_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

