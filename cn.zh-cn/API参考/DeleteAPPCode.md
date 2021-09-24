# 删除App Code<a name="ZH-CN_TOPIC_0000001081976105"></a>

## 功能介绍<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921764_section48433431"></a>

删除App Code，App Code删除后，将无法再通过简易认证访问对应的API。

## URI<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_section4658588"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_table12448204"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row28819405"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p52670492"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p52670492"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p52670492"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p38451455"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p38451455"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p38451455"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row27560159"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p17780387"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p17780387"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p17780387"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p30925236"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p30925236"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p30925236"></a>/v1.0/apigw/apps/{app_id}/app-codes/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_table8767205"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_row50080004"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p29948539"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p29948539"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p29948539"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p9912623"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p9912623"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p9912623"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p64724999"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p64724999"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p64724999"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p8233580"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p8233580"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p8233580"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_row62940229"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p64993787"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p64993787"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p64993787"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p30005365"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p30005365"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p30005365"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p14515483"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p14515483"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p14515483"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p34903511"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p34903511"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921763_p34903511"></a>App Code的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0226740193_row943312981910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0226740193_p24341599197"><a name="zh-cn_topic_0226740193_p24341599197"></a><a name="zh-cn_topic_0226740193_p24341599197"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0226740193_p5434290195"><a name="zh-cn_topic_0226740193_p5434290195"></a><a name="zh-cn_topic_0226740193_p5434290195"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0226740193_p543529161911"><a name="zh-cn_topic_0226740193_p543529161911"></a><a name="zh-cn_topic_0226740193_p543529161911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0226740193_p19435996196"><a name="zh-cn_topic_0226740193_p19435996196"></a><a name="zh-cn_topic_0226740193_p19435996196"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_section41927295"></a>

无

## 响应消息<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_section40667726"></a>

无

## 状态码<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_section41801338"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_table65433826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row9180004"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p5382851"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p5382851"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p5382851"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p33357811"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p33357811"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p33357811"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row17628188"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p18597093"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p18597093"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p18597093"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p29969526"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p29969526"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p29969526"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row1290281"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p37403962"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p37403962"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p37403962"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p9822120"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p9822120"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p9822120"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row21290221"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p46786353"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p46786353"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p46786353"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p31598212"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p31598212"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p31598212"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row15948460"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p16756892"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p16756892"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p16756892"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p1169465911116"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p1169465911116"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p1169465911116"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row1961203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p24639769"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p24639769"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p24639769"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p49664279"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p49664279"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p49664279"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row44325335"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p33582414"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p33582414"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p33582414"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p35820976"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p35820976"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p35820976"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_row53953334"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p8143910"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p8143910"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p8143910"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p55676983"><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p55676983"></a><a name="zh-cn_topic_0226740193_zh-cn_topic_0118921761_p55676983"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

