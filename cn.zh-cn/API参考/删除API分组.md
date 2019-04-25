# 删除API分组<a name="apig-zh-api-180713018"></a>

## 功能介绍<a name="section39839947"></a>

删除指定的API分组。

删除时，会一并删除直接或间接关联到该分组下的所有资源，包括API、独立域名、SSL证书、上架信息、分组下所有API的授权信息、编排信息、白名单配置、认证增强信息等等。并会将外部域名与子域名的绑定关系进行解除（取决于域名cname方式）。

## URI<a name="section23015206"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table33561337"></a>
<table><thead align="left"><tr id="row12491901"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p5211088"><a name="p5211088"></a><a name="p5211088"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p19444963"><a name="p19444963"></a><a name="p19444963"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row31538142"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p4452714"><a name="p4452714"></a><a name="p4452714"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p25125550"><a name="p25125550"></a><a name="p25125550"></a>/v1.0/apigw/api-groups/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table21903699"></a>
<table><thead align="left"><tr id="row27881548"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="p43812907"><a name="p43812907"></a><a name="p43812907"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.36816318368163%" id="mcps1.2.5.1.2"><p id="p59184603"><a name="p59184603"></a><a name="p59184603"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="p29223556"><a name="p29223556"></a><a name="p29223556"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.815918408159185%" id="mcps1.2.5.1.4"><p id="p18297805"><a name="p18297805"></a><a name="p18297805"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5727198"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p61249888"><a name="p61249888"></a><a name="p61249888"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.36816318368163%" headers="mcps1.2.5.1.2 "><p id="p62293882"><a name="p62293882"></a><a name="p62293882"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p12639701"><a name="p12639701"></a><a name="p12639701"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.815918408159185%" headers="mcps1.2.5.1.4 "><p id="p17182873"><a name="p17182873"></a><a name="p17182873"></a>分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section5810268"></a>

无

## 响应消息<a name="section869665"></a>

无

## 状态码<a name="section52292412"></a>

**表 3**  返回消息说明

<a name="table61047417"></a>
<table><thead align="left"><tr id="row36318009"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p56077582"><a name="p56077582"></a><a name="p56077582"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p45990271"><a name="p45990271"></a><a name="p45990271"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34224502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20721240"><a name="p20721240"></a><a name="p20721240"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13445195614478"><a name="p13445195614478"></a><a name="p13445195614478"></a>No Content</p>
</td>
</tr>
<tr id="row6290062"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p39733023"><a name="p39733023"></a><a name="p39733023"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p64258296"><a name="p64258296"></a><a name="p64258296"></a>Unauthorized</p>
</td>
</tr>
<tr id="row41453760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p2311385"><a name="p2311385"></a><a name="p2311385"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row7278408"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p52680147"><a name="p52680147"></a><a name="p52680147"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p39233519"><a name="p39233519"></a><a name="p39233519"></a>Not Found</p>
</td>
</tr>
<tr id="row17557355"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p12859618"><a name="p12859618"></a><a name="p12859618"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p34996158"><a name="p34996158"></a><a name="p34996158"></a>Conflict</p>
</td>
</tr>
<tr id="row46529974"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p10831524"><a name="p10831524"></a><a name="p10831524"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p4938218"><a name="p4938218"></a><a name="p4938218"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

