# 删除API<a name="ZH-CN_TOPIC_0000001081976165"></a>

## 功能介绍<a name="zh-cn_topic_0225568817_section24863152"></a>

删除指定的API。

删除API时，会删除该API所有相关的资源信息或绑定关系，如API的发布记录，绑定的后端服务，对APP的授权信息等。

## URI<a name="zh-cn_topic_0225568817_section22441780"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568817_table47776868"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568817_row14972112"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568817_p4781565"><a name="zh-cn_topic_0225568817_p4781565"></a><a name="zh-cn_topic_0225568817_p4781565"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568817_p51762503"><a name="zh-cn_topic_0225568817_p51762503"></a><a name="zh-cn_topic_0225568817_p51762503"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568817_row32013205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568817_p42932816"><a name="zh-cn_topic_0225568817_p42932816"></a><a name="zh-cn_topic_0225568817_p42932816"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568817_p55006047"><a name="zh-cn_topic_0225568817_p55006047"></a><a name="zh-cn_topic_0225568817_p55006047"></a>/v1/{project_id}/apigw/instances/{instance_id}/apis/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568817_table26304811"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568817_row11931990"><th class="cellrowborder" valign="top" width="20.72%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568817_p26967144"><a name="zh-cn_topic_0225568817_p26967144"></a><a name="zh-cn_topic_0225568817_p26967144"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.53%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568817_p36855079"><a name="zh-cn_topic_0225568817_p36855079"></a><a name="zh-cn_topic_0225568817_p36855079"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.509999999999998%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568817_p32471418"><a name="zh-cn_topic_0225568817_p32471418"></a><a name="zh-cn_topic_0225568817_p32471418"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.24%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568817_p12939210"><a name="zh-cn_topic_0225568817_p12939210"></a><a name="zh-cn_topic_0225568817_p12939210"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568817_row820361316176"><td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568817_p55878963"><a name="zh-cn_topic_0225568817_p55878963"></a><a name="zh-cn_topic_0225568817_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568817_p29902160"><a name="zh-cn_topic_0225568817_p29902160"></a><a name="zh-cn_topic_0225568817_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568817_p6155914"><a name="zh-cn_topic_0225568817_p6155914"></a><a name="zh-cn_topic_0225568817_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.24%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568817_p28867016"><a name="zh-cn_topic_0225568817_p28867016"></a><a name="zh-cn_topic_0225568817_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568817_row118121381717"><td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568817_p1780913159538"><a name="zh-cn_topic_0225568817_p1780913159538"></a><a name="zh-cn_topic_0225568817_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568817_p9809215115310"><a name="zh-cn_topic_0225568817_p9809215115310"></a><a name="zh-cn_topic_0225568817_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568817_p1280914152538"><a name="zh-cn_topic_0225568817_p1280914152538"></a><a name="zh-cn_topic_0225568817_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.24%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568817_p1880914157537"><a name="zh-cn_topic_0225568817_p1880914157537"></a><a name="zh-cn_topic_0225568817_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568817_row41443070"><td class="cellrowborder" valign="top" width="20.72%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568817_p1445503"><a name="zh-cn_topic_0225568817_p1445503"></a><a name="zh-cn_topic_0225568817_p1445503"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568817_p49976884"><a name="zh-cn_topic_0225568817_p49976884"></a><a name="zh-cn_topic_0225568817_p49976884"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.509999999999998%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568817_p21595781"><a name="zh-cn_topic_0225568817_p21595781"></a><a name="zh-cn_topic_0225568817_p21595781"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.24%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568817_p4427868"><a name="zh-cn_topic_0225568817_p4427868"></a><a name="zh-cn_topic_0225568817_p4427868"></a>API的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568817_section649433"></a>

无

## 响应消息<a name="zh-cn_topic_0225568817_section52604147"></a>

无

## 状态码<a name="zh-cn_topic_0225568817_section5844905"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568817_table60212917"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568817_row17862286"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568817_p37559096"><a name="zh-cn_topic_0225568817_p37559096"></a><a name="zh-cn_topic_0225568817_p37559096"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568817_p22387963"><a name="zh-cn_topic_0225568817_p22387963"></a><a name="zh-cn_topic_0225568817_p22387963"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568817_row1485694"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568817_p53232361"><a name="zh-cn_topic_0225568817_p53232361"></a><a name="zh-cn_topic_0225568817_p53232361"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568817_p13445195614478"><a name="zh-cn_topic_0225568817_p13445195614478"></a><a name="zh-cn_topic_0225568817_p13445195614478"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568817_row17468177"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568817_p5636200"><a name="zh-cn_topic_0225568817_p5636200"></a><a name="zh-cn_topic_0225568817_p5636200"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568817_p53879076"><a name="zh-cn_topic_0225568817_p53879076"></a><a name="zh-cn_topic_0225568817_p53879076"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568817_row15149644"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568817_p19161626"><a name="zh-cn_topic_0225568817_p19161626"></a><a name="zh-cn_topic_0225568817_p19161626"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568817_p13949586"><a name="zh-cn_topic_0225568817_p13949586"></a><a name="zh-cn_topic_0225568817_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568817_row10181700"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568817_p19411362"><a name="zh-cn_topic_0225568817_p19411362"></a><a name="zh-cn_topic_0225568817_p19411362"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568817_p28816493"><a name="zh-cn_topic_0225568817_p28816493"></a><a name="zh-cn_topic_0225568817_p28816493"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568817_row58021846"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568817_p2149103"><a name="zh-cn_topic_0225568817_p2149103"></a><a name="zh-cn_topic_0225568817_p2149103"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568817_p39859624"><a name="zh-cn_topic_0225568817_p39859624"></a><a name="zh-cn_topic_0225568817_p39859624"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568817_row23192296"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568817_p66636660"><a name="zh-cn_topic_0225568817_p66636660"></a><a name="zh-cn_topic_0225568817_p66636660"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568817_p14947689"><a name="zh-cn_topic_0225568817_p14947689"></a><a name="zh-cn_topic_0225568817_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

