# 删除流控策略<a name="ZH-CN_TOPIC_0000001082221195"></a>

## 功能介绍<a name="zh-cn_topic_0118922258_section13937026"></a>

删除指定的流控策略，以及该流控策略与API的所有绑定关系。

## URI<a name="zh-cn_topic_0118922258_section58324371"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922258_table59484814"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922258_row32208838"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922258_p58779092"><a name="zh-cn_topic_0118922258_p58779092"></a><a name="zh-cn_topic_0118922258_p58779092"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922258_p63486051"><a name="zh-cn_topic_0118922258_p63486051"></a><a name="zh-cn_topic_0118922258_p63486051"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922258_row42096539"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922258_p54376483"><a name="zh-cn_topic_0118922258_p54376483"></a><a name="zh-cn_topic_0118922258_p54376483"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922258_p42418979"><a name="zh-cn_topic_0118922258_p42418979"></a><a name="zh-cn_topic_0118922258_p42418979"></a>/v1.0/apigw/throttles/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922258_table13385284"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922258_row62579373"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922258_p35764424"><a name="zh-cn_topic_0118922258_p35764424"></a><a name="zh-cn_topic_0118922258_p35764424"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922258_p11237236"><a name="zh-cn_topic_0118922258_p11237236"></a><a name="zh-cn_topic_0118922258_p11237236"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922258_p37800920"><a name="zh-cn_topic_0118922258_p37800920"></a><a name="zh-cn_topic_0118922258_p37800920"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922258_p41975709"><a name="zh-cn_topic_0118922258_p41975709"></a><a name="zh-cn_topic_0118922258_p41975709"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922258_row44589291"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922258_p54962793"><a name="zh-cn_topic_0118922258_p54962793"></a><a name="zh-cn_topic_0118922258_p54962793"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922258_p22801215"><a name="zh-cn_topic_0118922258_p22801215"></a><a name="zh-cn_topic_0118922258_p22801215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922258_p34959126"><a name="zh-cn_topic_0118922258_p34959126"></a><a name="zh-cn_topic_0118922258_p34959126"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922258_p13116949"><a name="zh-cn_topic_0118922258_p13116949"></a><a name="zh-cn_topic_0118922258_p13116949"></a>流控策略的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922258_section55157294"></a>

无

## 响应消息<a name="zh-cn_topic_0118922258_section38555855"></a>

无

## 状态码<a name="zh-cn_topic_0118922258_section26653605"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118922258_table26743982"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922258_row66720907"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922258_p35684412"><a name="zh-cn_topic_0118922258_p35684412"></a><a name="zh-cn_topic_0118922258_p35684412"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922258_p4756298"><a name="zh-cn_topic_0118922258_p4756298"></a><a name="zh-cn_topic_0118922258_p4756298"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922258_row49715868"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922258_p453531"><a name="zh-cn_topic_0118922258_p453531"></a><a name="zh-cn_topic_0118922258_p453531"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922258_p36736046"><a name="zh-cn_topic_0118922258_p36736046"></a><a name="zh-cn_topic_0118922258_p36736046"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922258_row62188963"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922258_p4141232"><a name="zh-cn_topic_0118922258_p4141232"></a><a name="zh-cn_topic_0118922258_p4141232"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922258_p67004357"><a name="zh-cn_topic_0118922258_p67004357"></a><a name="zh-cn_topic_0118922258_p67004357"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922258_row66168307"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922258_p58032616"><a name="zh-cn_topic_0118922258_p58032616"></a><a name="zh-cn_topic_0118922258_p58032616"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922258_p3021433"><a name="zh-cn_topic_0118922258_p3021433"></a><a name="zh-cn_topic_0118922258_p3021433"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922258_row27192904"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922258_p55141648"><a name="zh-cn_topic_0118922258_p55141648"></a><a name="zh-cn_topic_0118922258_p55141648"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922258_p37288488"><a name="zh-cn_topic_0118922258_p37288488"></a><a name="zh-cn_topic_0118922258_p37288488"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922258_row52073"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922258_p4217981"><a name="zh-cn_topic_0118922258_p4217981"></a><a name="zh-cn_topic_0118922258_p4217981"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922258_p6112181"><a name="zh-cn_topic_0118922258_p6112181"></a><a name="zh-cn_topic_0118922258_p6112181"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922258_row55009634"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922258_p26595404"><a name="zh-cn_topic_0118922258_p26595404"></a><a name="zh-cn_topic_0118922258_p26595404"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922258_p6744143"><a name="zh-cn_topic_0118922258_p6744143"></a><a name="zh-cn_topic_0118922258_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

