# 删除自定义认证<a name="ZH-CN_TOPIC_0000001082221311"></a>

## 功能介绍<a name="zh-cn_topic_0225569042_section66524352"></a>

删除自定义认证

## URI<a name="zh-cn_topic_0225569042_section61848258"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225569042_table27084002"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569042_row40355780"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569042_p47592766"><a name="zh-cn_topic_0225569042_p47592766"></a><a name="zh-cn_topic_0225569042_p47592766"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569042_p29808828"><a name="zh-cn_topic_0225569042_p29808828"></a><a name="zh-cn_topic_0225569042_p29808828"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569042_row65704871"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569042_p20494310"><a name="zh-cn_topic_0225569042_p20494310"></a><a name="zh-cn_topic_0225569042_p20494310"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569042_p49426402"><a name="zh-cn_topic_0225569042_p49426402"></a><a name="zh-cn_topic_0225569042_p49426402"></a>/v1/{project_id}/apigw/instances/{instance_id}/authorizers/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225569042_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569042_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569042_p23103637"><a name="zh-cn_topic_0225569042_p23103637"></a><a name="zh-cn_topic_0225569042_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569042_p59455291"><a name="zh-cn_topic_0225569042_p59455291"></a><a name="zh-cn_topic_0225569042_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569042_p51149303"><a name="zh-cn_topic_0225569042_p51149303"></a><a name="zh-cn_topic_0225569042_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569042_p49452846"><a name="zh-cn_topic_0225569042_p49452846"></a><a name="zh-cn_topic_0225569042_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569042_row5785398914"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569042_p118581710090"><a name="zh-cn_topic_0225569042_p118581710090"></a><a name="zh-cn_topic_0225569042_p118581710090"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569042_p98581110496"><a name="zh-cn_topic_0225569042_p98581110496"></a><a name="zh-cn_topic_0225569042_p98581110496"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569042_p1785871017910"><a name="zh-cn_topic_0225569042_p1785871017910"></a><a name="zh-cn_topic_0225569042_p1785871017910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569042_p198580106913"><a name="zh-cn_topic_0225569042_p198580106913"></a><a name="zh-cn_topic_0225569042_p198580106913"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569042_row192658915910"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569042_p1780913159538"><a name="zh-cn_topic_0225569042_p1780913159538"></a><a name="zh-cn_topic_0225569042_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569042_p9809215115310"><a name="zh-cn_topic_0225569042_p9809215115310"></a><a name="zh-cn_topic_0225569042_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569042_p1280914152538"><a name="zh-cn_topic_0225569042_p1280914152538"></a><a name="zh-cn_topic_0225569042_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569042_p1880914157537"><a name="zh-cn_topic_0225569042_p1880914157537"></a><a name="zh-cn_topic_0225569042_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569042_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569042_p55878963"><a name="zh-cn_topic_0225569042_p55878963"></a><a name="zh-cn_topic_0225569042_p55878963"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569042_p29902160"><a name="zh-cn_topic_0225569042_p29902160"></a><a name="zh-cn_topic_0225569042_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569042_p6155914"><a name="zh-cn_topic_0225569042_p6155914"></a><a name="zh-cn_topic_0225569042_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569042_p28867016"><a name="zh-cn_topic_0225569042_p28867016"></a><a name="zh-cn_topic_0225569042_p28867016"></a>自定义认证的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225569042_section19763417"></a>

无

## 响应消息<a name="zh-cn_topic_0225569042_section57332943"></a>

无

## 状态码<a name="zh-cn_topic_0225569042_section43653029"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225569042_table61047417"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569042_row36318009"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569042_p56077582"><a name="zh-cn_topic_0225569042_p56077582"></a><a name="zh-cn_topic_0225569042_p56077582"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569042_p45990271"><a name="zh-cn_topic_0225569042_p45990271"></a><a name="zh-cn_topic_0225569042_p45990271"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569042_row34224502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569042_p20721240"><a name="zh-cn_topic_0225569042_p20721240"></a><a name="zh-cn_topic_0225569042_p20721240"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569042_p13445195614478"><a name="zh-cn_topic_0225569042_p13445195614478"></a><a name="zh-cn_topic_0225569042_p13445195614478"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569042_row6290062"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569042_p39733023"><a name="zh-cn_topic_0225569042_p39733023"></a><a name="zh-cn_topic_0225569042_p39733023"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569042_p64258296"><a name="zh-cn_topic_0225569042_p64258296"></a><a name="zh-cn_topic_0225569042_p64258296"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569042_row41453760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569042_p2311385"><a name="zh-cn_topic_0225569042_p2311385"></a><a name="zh-cn_topic_0225569042_p2311385"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569042_p13949586"><a name="zh-cn_topic_0225569042_p13949586"></a><a name="zh-cn_topic_0225569042_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569042_row7278408"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569042_p52680147"><a name="zh-cn_topic_0225569042_p52680147"></a><a name="zh-cn_topic_0225569042_p52680147"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569042_p39233519"><a name="zh-cn_topic_0225569042_p39233519"></a><a name="zh-cn_topic_0225569042_p39233519"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569042_row17557355"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569042_p12859618"><a name="zh-cn_topic_0225569042_p12859618"></a><a name="zh-cn_topic_0225569042_p12859618"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569042_p34996158"><a name="zh-cn_topic_0225569042_p34996158"></a><a name="zh-cn_topic_0225569042_p34996158"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569042_row46529974"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569042_p10831524"><a name="zh-cn_topic_0225569042_p10831524"></a><a name="zh-cn_topic_0225569042_p10831524"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569042_p4938218"><a name="zh-cn_topic_0225569042_p4938218"></a><a name="zh-cn_topic_0225569042_p4938218"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

