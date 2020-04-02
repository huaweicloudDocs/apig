# 刷新API资源至ETCD<a name="apig-phapi-181031240"></a>

## 功能介绍<a name="section142594180538"></a>

提供给op\_svc\_apig角色的管理员的接口。

刷新API资源至ETCD。

## URI<a name="section142591518145311"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table2068511412554"></a>
<table><thead align="left"><tr id="row20685341185519"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p3384161845312"><a name="p3384161845312"></a><a name="p3384161845312"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p1384111865313"><a name="p1384111865313"></a><a name="p1384111865313"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row8685164116555"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p838411184539"><a name="p838411184539"></a><a name="p838411184539"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p19384151865310"><a name="p19384151865310"></a><a name="p19384151865310"></a>/v1/{project_id}/apigw/instances/{instance_id}/op-operations/router/apis</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table38510415"></a>
<table><thead align="left"><tr id="row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="p23103637"><a name="p23103637"></a><a name="p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p59455291"><a name="p59455291"></a><a name="p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="p51149303"><a name="p51149303"></a><a name="p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="p49452846"><a name="p49452846"></a><a name="p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求参数<a name="section1027541812532"></a>

无

## 响应消息<a name="section172751818145312"></a>

无

## 状态码<a name="section7275818155314"></a>

**表 3**  返回消息说明

<a name="table102754180538"></a>
<table><thead align="left"><tr id="row18384818135317"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p15384181811535"><a name="p15384181811535"></a><a name="p15384181811535"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p538421813536"><a name="p538421813536"></a><a name="p538421813536"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row73841218185318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p03841018135311"><a name="p03841018135311"></a><a name="p03841018135311"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p203846181534"><a name="p203846181534"></a><a name="p203846181534"></a>OK</p>
</td>
</tr>
<tr id="row14384718155310"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1938441812532"><a name="p1938441812532"></a><a name="p1938441812532"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p153841218155313"><a name="p153841218155313"></a><a name="p153841218155313"></a>Unauthorized</p>
</td>
</tr>
<tr id="row438421818535"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1638491825318"><a name="p1638491825318"></a><a name="p1638491825318"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p33841218175316"><a name="p33841218175316"></a><a name="p33841218175316"></a>Forbidden</p>
</td>
</tr>
<tr id="row10384111816533"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p138411819539"><a name="p138411819539"></a><a name="p138411819539"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

