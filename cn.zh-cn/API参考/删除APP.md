# 删除APP<a name="apig-zh-api-180713039"></a>

## 功能介绍<a name="section60169944"></a>

删除指定的APP。

APP删除后，将无法再调用任何API；其中，云市场自动创建的APP无法被删除。

## URI<a name="section4658588"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table12448204"></a>
<table><thead align="left"><tr id="row28819405"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p52670492"><a name="p52670492"></a><a name="p52670492"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p38451455"><a name="p38451455"></a><a name="p38451455"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row27560159"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p17780387"><a name="p17780387"></a><a name="p17780387"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p30925236"><a name="p30925236"></a><a name="p30925236"></a>/v1.0/apigw/apps/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table21916153"></a>
<table><thead align="left"><tr id="row42598074"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p27891998"><a name="p27891998"></a><a name="p27891998"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p44659366"><a name="p44659366"></a><a name="p44659366"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p60638907"><a name="p60638907"></a><a name="p60638907"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p12804420"><a name="p12804420"></a><a name="p12804420"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row30525098"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p56613844"><a name="p56613844"></a><a name="p56613844"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p22318634"><a name="p22318634"></a><a name="p22318634"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p62978966"><a name="p62978966"></a><a name="p62978966"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1022589"><a name="p1022589"></a><a name="p1022589"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section41927295"></a>

无

## 响应消息<a name="section40667726"></a>

无

## 状态码<a name="section41801338"></a>

**表 3**  返回消息说明

<a name="table65433826"></a>
<table><thead align="left"><tr id="row9180004"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p5382851"><a name="p5382851"></a><a name="p5382851"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p33357811"><a name="p33357811"></a><a name="p33357811"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17628188"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p18597093"><a name="p18597093"></a><a name="p18597093"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p29969526"><a name="p29969526"></a><a name="p29969526"></a>No Content</p>
</td>
</tr>
<tr id="row1290281"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p37403962"><a name="p37403962"></a><a name="p37403962"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9822120"><a name="p9822120"></a><a name="p9822120"></a>Bad Request</p>
</td>
</tr>
<tr id="row21290221"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p46786353"><a name="p46786353"></a><a name="p46786353"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p31598212"><a name="p31598212"></a><a name="p31598212"></a>Unauthorized</p>
</td>
</tr>
<tr id="row15948460"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p16756892"><a name="p16756892"></a><a name="p16756892"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1169465911116"><a name="p1169465911116"></a><a name="p1169465911116"></a>Forbidden</p>
</td>
</tr>
<tr id="row1961203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p24639769"><a name="p24639769"></a><a name="p24639769"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p49664279"><a name="p49664279"></a><a name="p49664279"></a>Not Found</p>
</td>
</tr>
<tr id="row44325335"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p33582414"><a name="p33582414"></a><a name="p33582414"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p35820976"><a name="p35820976"></a><a name="p35820976"></a>Conflict</p>
</td>
</tr>
<tr id="row53953334"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p8143910"><a name="p8143910"></a><a name="p8143910"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p55676983"><a name="p55676983"></a><a name="p55676983"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

