# 删除环境<a name="ZH-CN_TOPIC_0000001082221265"></a>

## 功能介绍<a name="zh-cn_topic_0225568851_section46666531"></a>

删除指定的环境。

该操作将导致此API在指定的环境无法被访问，可能会影响相当一部分应用和用户。请确保已经告知用户，或者确认需要强制下线。

## URI<a name="zh-cn_topic_0225568851_section17345600"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568851_table34653453"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568851_row50089110"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568851_p30686111"><a name="zh-cn_topic_0225568851_p30686111"></a><a name="zh-cn_topic_0225568851_p30686111"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568851_p2547097"><a name="zh-cn_topic_0225568851_p2547097"></a><a name="zh-cn_topic_0225568851_p2547097"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568851_row4988332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568851_p1401727"><a name="zh-cn_topic_0225568851_p1401727"></a><a name="zh-cn_topic_0225568851_p1401727"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568851_p46431034"><a name="zh-cn_topic_0225568851_p46431034"></a><a name="zh-cn_topic_0225568851_p46431034"></a>/v1/{project_id}/apigw/instances/{instance_id}/envs/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568851_table2817414"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568851_row39899899"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568851_p10666353"><a name="zh-cn_topic_0225568851_p10666353"></a><a name="zh-cn_topic_0225568851_p10666353"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.580000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568851_p58668264"><a name="zh-cn_topic_0225568851_p58668264"></a><a name="zh-cn_topic_0225568851_p58668264"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.72%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568851_p54508935"><a name="zh-cn_topic_0225568851_p54508935"></a><a name="zh-cn_topic_0225568851_p54508935"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.7%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568851_p53147639"><a name="zh-cn_topic_0225568851_p53147639"></a><a name="zh-cn_topic_0225568851_p53147639"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568851_row182051320104820"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568851_p55878963"><a name="zh-cn_topic_0225568851_p55878963"></a><a name="zh-cn_topic_0225568851_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568851_p29902160"><a name="zh-cn_topic_0225568851_p29902160"></a><a name="zh-cn_topic_0225568851_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568851_p6155914"><a name="zh-cn_topic_0225568851_p6155914"></a><a name="zh-cn_topic_0225568851_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.7%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568851_p28867016"><a name="zh-cn_topic_0225568851_p28867016"></a><a name="zh-cn_topic_0225568851_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568851_row1074518196489"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568851_p1780913159538"><a name="zh-cn_topic_0225568851_p1780913159538"></a><a name="zh-cn_topic_0225568851_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568851_p9809215115310"><a name="zh-cn_topic_0225568851_p9809215115310"></a><a name="zh-cn_topic_0225568851_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568851_p1280914152538"><a name="zh-cn_topic_0225568851_p1280914152538"></a><a name="zh-cn_topic_0225568851_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.7%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568851_p1880914157537"><a name="zh-cn_topic_0225568851_p1880914157537"></a><a name="zh-cn_topic_0225568851_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568851_row9991520"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568851_p4006761"><a name="zh-cn_topic_0225568851_p4006761"></a><a name="zh-cn_topic_0225568851_p4006761"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568851_p56112186"><a name="zh-cn_topic_0225568851_p56112186"></a><a name="zh-cn_topic_0225568851_p56112186"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568851_p48793212"><a name="zh-cn_topic_0225568851_p48793212"></a><a name="zh-cn_topic_0225568851_p48793212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.7%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568851_p59936086"><a name="zh-cn_topic_0225568851_p59936086"></a><a name="zh-cn_topic_0225568851_p59936086"></a>环境的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568851_section21892675"></a>

无

## 响应消息<a name="zh-cn_topic_0225568851_section28476231"></a>

无

## 状态码<a name="zh-cn_topic_0225568851_section62816349"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568851_table49830901"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568851_row9625088"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568851_p41434644"><a name="zh-cn_topic_0225568851_p41434644"></a><a name="zh-cn_topic_0225568851_p41434644"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568851_p762997"><a name="zh-cn_topic_0225568851_p762997"></a><a name="zh-cn_topic_0225568851_p762997"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568851_row61802762"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568851_p39967803"><a name="zh-cn_topic_0225568851_p39967803"></a><a name="zh-cn_topic_0225568851_p39967803"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568851_p16166642"><a name="zh-cn_topic_0225568851_p16166642"></a><a name="zh-cn_topic_0225568851_p16166642"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568851_row11282050"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568851_p41430842"><a name="zh-cn_topic_0225568851_p41430842"></a><a name="zh-cn_topic_0225568851_p41430842"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568851_p455018"><a name="zh-cn_topic_0225568851_p455018"></a><a name="zh-cn_topic_0225568851_p455018"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568851_row4095167"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568851_p63273111"><a name="zh-cn_topic_0225568851_p63273111"></a><a name="zh-cn_topic_0225568851_p63273111"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568851_p24848380"><a name="zh-cn_topic_0225568851_p24848380"></a><a name="zh-cn_topic_0225568851_p24848380"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568851_row22308830"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568851_p62184833"><a name="zh-cn_topic_0225568851_p62184833"></a><a name="zh-cn_topic_0225568851_p62184833"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568851_p3806692"><a name="zh-cn_topic_0225568851_p3806692"></a><a name="zh-cn_topic_0225568851_p3806692"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568851_row34260229"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568851_p23615147"><a name="zh-cn_topic_0225568851_p23615147"></a><a name="zh-cn_topic_0225568851_p23615147"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568851_p33778791"><a name="zh-cn_topic_0225568851_p33778791"></a><a name="zh-cn_topic_0225568851_p33778791"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568851_row35573663"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568851_p62894484"><a name="zh-cn_topic_0225568851_p62894484"></a><a name="zh-cn_topic_0225568851_p62894484"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568851_p14947689"><a name="zh-cn_topic_0225568851_p14947689"></a><a name="zh-cn_topic_0225568851_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

