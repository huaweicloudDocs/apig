# 解除API与ACL策略的绑定<a name="apig-phapi-180713097"></a>

## 功能介绍<a name="section56668631"></a>

解除某条API与ACL策略的绑定关系

## URI<a name="section40255631"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table52942781"></a>
<table><thead align="left"><tr id="row36583141"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p10444414"><a name="p10444414"></a><a name="p10444414"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p40691167"><a name="p40691167"></a><a name="p40691167"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row7650225"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p15688475"><a name="p15688475"></a><a name="p15688475"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p62806982"><a name="p62806982"></a><a name="p62806982"></a><span id="ph157201233164419"><a name="ph157201233164419"></a><a name="ph157201233164419"></a>/v1/{project_id}/apigw/instances/{instance_id}</span>/acl-bindings/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table54200794"></a>
<table><thead align="left"><tr id="row33794268"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p52981202"><a name="p52981202"></a><a name="p52981202"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.669999999999998%" id="mcps1.2.5.1.2"><p id="p63618976"><a name="p63618976"></a><a name="p63618976"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.53%" id="mcps1.2.5.1.3"><p id="p52863471"><a name="p52863471"></a><a name="p52863471"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.8%" id="mcps1.2.5.1.4"><p id="p54082791"><a name="p54082791"></a><a name="p54082791"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13634185016206"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.669999999999998%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.8%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row7344250182011"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.669999999999998%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.8%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row18629935"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p32629743"><a name="p32629743"></a><a name="p32629743"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.669999999999998%" headers="mcps1.2.5.1.2 "><p id="p25763536"><a name="p25763536"></a><a name="p25763536"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.53%" headers="mcps1.2.5.1.3 "><p id="p6471673"><a name="p6471673"></a><a name="p6471673"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.8%" headers="mcps1.2.5.1.4 "><p id="p54443539"><a name="p54443539"></a><a name="p54443539"></a>绑定关系编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section26756366"></a>

无

## 响应消息<a name="section5160633122513"></a>

无

## 状态码<a name="section39480708"></a>

**表 3**  返回消息说明

<a name="table50690617"></a>
<table><thead align="left"><tr id="row40699524"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p8327115"><a name="p8327115"></a><a name="p8327115"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p3407735"><a name="p3407735"></a><a name="p3407735"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7591152"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p10903581"><a name="p10903581"></a><a name="p10903581"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p10774887"><a name="p10774887"></a><a name="p10774887"></a>No Content</p>
</td>
</tr>
<tr id="row29865122"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3155809"><a name="p3155809"></a><a name="p3155809"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p54294001"><a name="p54294001"></a><a name="p54294001"></a>Forbidden</p>
</td>
</tr>
<tr id="row18883967"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p53206347"><a name="p53206347"></a><a name="p53206347"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14746811"><a name="p14746811"></a><a name="p14746811"></a>Not Found</p>
</td>
</tr>
<tr id="row65612436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p13007094"><a name="p13007094"></a><a name="p13007094"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

