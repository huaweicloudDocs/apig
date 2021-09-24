# 删除API分组<a name="ZH-CN_TOPIC_0000001082221243"></a>

## 功能介绍<a name="zh-cn_topic_0225568808_section39839947"></a>

删除指定的API分组。

删除时，会一并删除直接或间接关联到该分组下的所有资源，包括API、独立域名、SSL证书、上架信息、分组下所有API的授权信息、编排信息、白名单配置、认证增强信息等等。并会将外部域名与子域名的绑定关系进行解除（取决于域名cname方式）。

## URI<a name="zh-cn_topic_0225568808_section23015206"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568808_table33561337"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568808_row12491901"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568808_p5211088"><a name="zh-cn_topic_0225568808_p5211088"></a><a name="zh-cn_topic_0225568808_p5211088"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568808_p19444963"><a name="zh-cn_topic_0225568808_p19444963"></a><a name="zh-cn_topic_0225568808_p19444963"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568808_row31538142"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568808_p4452714"><a name="zh-cn_topic_0225568808_p4452714"></a><a name="zh-cn_topic_0225568808_p4452714"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568808_p25125550"><a name="zh-cn_topic_0225568808_p25125550"></a><a name="zh-cn_topic_0225568808_p25125550"></a>/v1/{project_id}/apigw/instances/{instance_id}/api-groups/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568808_table21903699"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568808_row27881548"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568808_p43812907"><a name="zh-cn_topic_0225568808_p43812907"></a><a name="zh-cn_topic_0225568808_p43812907"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.36816318368163%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568808_p59184603"><a name="zh-cn_topic_0225568808_p59184603"></a><a name="zh-cn_topic_0225568808_p59184603"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568808_p29223556"><a name="zh-cn_topic_0225568808_p29223556"></a><a name="zh-cn_topic_0225568808_p29223556"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.815918408159185%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568808_p18297805"><a name="zh-cn_topic_0225568808_p18297805"></a><a name="zh-cn_topic_0225568808_p18297805"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568808_row2366928201320"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568808_p55878963"><a name="zh-cn_topic_0225568808_p55878963"></a><a name="zh-cn_topic_0225568808_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.36816318368163%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568808_p29902160"><a name="zh-cn_topic_0225568808_p29902160"></a><a name="zh-cn_topic_0225568808_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568808_p6155914"><a name="zh-cn_topic_0225568808_p6155914"></a><a name="zh-cn_topic_0225568808_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.815918408159185%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568808_p28867016"><a name="zh-cn_topic_0225568808_p28867016"></a><a name="zh-cn_topic_0225568808_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568808_row1318614283137"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568808_p1780913159538"><a name="zh-cn_topic_0225568808_p1780913159538"></a><a name="zh-cn_topic_0225568808_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.36816318368163%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568808_p9809215115310"><a name="zh-cn_topic_0225568808_p9809215115310"></a><a name="zh-cn_topic_0225568808_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568808_p1280914152538"><a name="zh-cn_topic_0225568808_p1280914152538"></a><a name="zh-cn_topic_0225568808_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.815918408159185%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568808_p1880914157537"><a name="zh-cn_topic_0225568808_p1880914157537"></a><a name="zh-cn_topic_0225568808_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568808_row5727198"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568808_p61249888"><a name="zh-cn_topic_0225568808_p61249888"></a><a name="zh-cn_topic_0225568808_p61249888"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.36816318368163%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568808_p62293882"><a name="zh-cn_topic_0225568808_p62293882"></a><a name="zh-cn_topic_0225568808_p62293882"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568808_p12639701"><a name="zh-cn_topic_0225568808_p12639701"></a><a name="zh-cn_topic_0225568808_p12639701"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.815918408159185%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568808_p17182873"><a name="zh-cn_topic_0225568808_p17182873"></a><a name="zh-cn_topic_0225568808_p17182873"></a>分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568808_section5810268"></a>

无

## 响应消息<a name="zh-cn_topic_0225568808_section869665"></a>

无

## 状态码<a name="zh-cn_topic_0225568808_section52292412"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568808_table61047417"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568808_row36318009"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568808_p56077582"><a name="zh-cn_topic_0225568808_p56077582"></a><a name="zh-cn_topic_0225568808_p56077582"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568808_p45990271"><a name="zh-cn_topic_0225568808_p45990271"></a><a name="zh-cn_topic_0225568808_p45990271"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568808_row34224502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568808_p20721240"><a name="zh-cn_topic_0225568808_p20721240"></a><a name="zh-cn_topic_0225568808_p20721240"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568808_p13445195614478"><a name="zh-cn_topic_0225568808_p13445195614478"></a><a name="zh-cn_topic_0225568808_p13445195614478"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568808_row6290062"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568808_p39733023"><a name="zh-cn_topic_0225568808_p39733023"></a><a name="zh-cn_topic_0225568808_p39733023"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568808_p64258296"><a name="zh-cn_topic_0225568808_p64258296"></a><a name="zh-cn_topic_0225568808_p64258296"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568808_row41453760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568808_p2311385"><a name="zh-cn_topic_0225568808_p2311385"></a><a name="zh-cn_topic_0225568808_p2311385"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568808_p13949586"><a name="zh-cn_topic_0225568808_p13949586"></a><a name="zh-cn_topic_0225568808_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568808_row7278408"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568808_p52680147"><a name="zh-cn_topic_0225568808_p52680147"></a><a name="zh-cn_topic_0225568808_p52680147"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568808_p39233519"><a name="zh-cn_topic_0225568808_p39233519"></a><a name="zh-cn_topic_0225568808_p39233519"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568808_row17557355"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568808_p12859618"><a name="zh-cn_topic_0225568808_p12859618"></a><a name="zh-cn_topic_0225568808_p12859618"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568808_p34996158"><a name="zh-cn_topic_0225568808_p34996158"></a><a name="zh-cn_topic_0225568808_p34996158"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568808_row46529974"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568808_p10831524"><a name="zh-cn_topic_0225568808_p10831524"></a><a name="zh-cn_topic_0225568808_p10831524"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568808_p4938218"><a name="zh-cn_topic_0225568808_p4938218"></a><a name="zh-cn_topic_0225568808_p4938218"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

