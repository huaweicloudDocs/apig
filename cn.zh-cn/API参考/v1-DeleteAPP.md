# 删除APP<a name="ZH-CN_TOPIC_0000001081976173"></a>

## 功能介绍<a name="zh-cn_topic_0225568836_section60169944"></a>

删除指定的APP。

APP删除后，将无法再调用任何API；其中，云市场自动创建的APP无法被删除。

## URI<a name="zh-cn_topic_0225568836_section4658588"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568836_table12448204"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568836_row28819405"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568836_p52670492"><a name="zh-cn_topic_0225568836_p52670492"></a><a name="zh-cn_topic_0225568836_p52670492"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568836_p38451455"><a name="zh-cn_topic_0225568836_p38451455"></a><a name="zh-cn_topic_0225568836_p38451455"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568836_row27560159"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p17780387"><a name="zh-cn_topic_0225568836_p17780387"></a><a name="zh-cn_topic_0225568836_p17780387"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p30925236"><a name="zh-cn_topic_0225568836_p30925236"></a><a name="zh-cn_topic_0225568836_p30925236"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568836_table21916153"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568836_row42598074"><th class="cellrowborder" valign="top" width="22.470000000000002%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568836_p27891998"><a name="zh-cn_topic_0225568836_p27891998"></a><a name="zh-cn_topic_0225568836_p27891998"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.2%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568836_p44659366"><a name="zh-cn_topic_0225568836_p44659366"></a><a name="zh-cn_topic_0225568836_p44659366"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.72%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568836_p60638907"><a name="zh-cn_topic_0225568836_p60638907"></a><a name="zh-cn_topic_0225568836_p60638907"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.61%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568836_p12804420"><a name="zh-cn_topic_0225568836_p12804420"></a><a name="zh-cn_topic_0225568836_p12804420"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568836_row15940503383"><td class="cellrowborder" valign="top" width="22.470000000000002%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568836_p55878963"><a name="zh-cn_topic_0225568836_p55878963"></a><a name="zh-cn_topic_0225568836_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.2%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568836_p29902160"><a name="zh-cn_topic_0225568836_p29902160"></a><a name="zh-cn_topic_0225568836_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568836_p6155914"><a name="zh-cn_topic_0225568836_p6155914"></a><a name="zh-cn_topic_0225568836_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.61%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568836_p28867016"><a name="zh-cn_topic_0225568836_p28867016"></a><a name="zh-cn_topic_0225568836_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row1441975093817"><td class="cellrowborder" valign="top" width="22.470000000000002%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568836_p1780913159538"><a name="zh-cn_topic_0225568836_p1780913159538"></a><a name="zh-cn_topic_0225568836_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.2%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568836_p9809215115310"><a name="zh-cn_topic_0225568836_p9809215115310"></a><a name="zh-cn_topic_0225568836_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568836_p1280914152538"><a name="zh-cn_topic_0225568836_p1280914152538"></a><a name="zh-cn_topic_0225568836_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.61%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568836_p1880914157537"><a name="zh-cn_topic_0225568836_p1880914157537"></a><a name="zh-cn_topic_0225568836_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row30525098"><td class="cellrowborder" valign="top" width="22.470000000000002%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568836_p56613844"><a name="zh-cn_topic_0225568836_p56613844"></a><a name="zh-cn_topic_0225568836_p56613844"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.2%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568836_p22318634"><a name="zh-cn_topic_0225568836_p22318634"></a><a name="zh-cn_topic_0225568836_p22318634"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568836_p62978966"><a name="zh-cn_topic_0225568836_p62978966"></a><a name="zh-cn_topic_0225568836_p62978966"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.61%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568836_p1022589"><a name="zh-cn_topic_0225568836_p1022589"></a><a name="zh-cn_topic_0225568836_p1022589"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568836_section41927295"></a>

无

## 响应消息<a name="zh-cn_topic_0225568836_section40667726"></a>

无

## 状态码<a name="zh-cn_topic_0225568836_section41801338"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568836_table65433826"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568836_row9180004"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568836_p5382851"><a name="zh-cn_topic_0225568836_p5382851"></a><a name="zh-cn_topic_0225568836_p5382851"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568836_p33357811"><a name="zh-cn_topic_0225568836_p33357811"></a><a name="zh-cn_topic_0225568836_p33357811"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568836_row17628188"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p18597093"><a name="zh-cn_topic_0225568836_p18597093"></a><a name="zh-cn_topic_0225568836_p18597093"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p29969526"><a name="zh-cn_topic_0225568836_p29969526"></a><a name="zh-cn_topic_0225568836_p29969526"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row1290281"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p37403962"><a name="zh-cn_topic_0225568836_p37403962"></a><a name="zh-cn_topic_0225568836_p37403962"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p9822120"><a name="zh-cn_topic_0225568836_p9822120"></a><a name="zh-cn_topic_0225568836_p9822120"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row21290221"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p46786353"><a name="zh-cn_topic_0225568836_p46786353"></a><a name="zh-cn_topic_0225568836_p46786353"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p31598212"><a name="zh-cn_topic_0225568836_p31598212"></a><a name="zh-cn_topic_0225568836_p31598212"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row15948460"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p16756892"><a name="zh-cn_topic_0225568836_p16756892"></a><a name="zh-cn_topic_0225568836_p16756892"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p1169465911116"><a name="zh-cn_topic_0225568836_p1169465911116"></a><a name="zh-cn_topic_0225568836_p1169465911116"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row1961203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p24639769"><a name="zh-cn_topic_0225568836_p24639769"></a><a name="zh-cn_topic_0225568836_p24639769"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p49664279"><a name="zh-cn_topic_0225568836_p49664279"></a><a name="zh-cn_topic_0225568836_p49664279"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row44325335"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p33582414"><a name="zh-cn_topic_0225568836_p33582414"></a><a name="zh-cn_topic_0225568836_p33582414"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p35820976"><a name="zh-cn_topic_0225568836_p35820976"></a><a name="zh-cn_topic_0225568836_p35820976"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568836_row53953334"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568836_p8143910"><a name="zh-cn_topic_0225568836_p8143910"></a><a name="zh-cn_topic_0225568836_p8143910"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568836_p55676983"><a name="zh-cn_topic_0225568836_p55676983"></a><a name="zh-cn_topic_0225568836_p55676983"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

