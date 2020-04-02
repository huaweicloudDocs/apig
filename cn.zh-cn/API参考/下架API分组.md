# 下架API分组<a name="apig-phapi-180713104"></a>

## 功能介绍<a name="section24818239"></a>

将某个已上架的API分组从云市场下架。下架后，其他用户将无法再次购买，但已购买的用户依然能够调用这个分组下的API，直至购买的次数用完为止。API分组下架后，可以重新上架。

## URI<a name="section22037565"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table2932438"></a>
<table><thead align="left"><tr id="row15810818"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p5607849"><a name="p5607849"></a><a name="p5607849"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p51582645"><a name="p51582645"></a><a name="p51582645"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row17444750"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p3738651"><a name="p3738651"></a><a name="p3738651"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p157114075518"><a name="p157114075518"></a><a name="p157114075518"></a>/v1/{project_id}/apigw/instances/{instance_id}/market/api-groups/onsell/{group_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  Head参数信息

<a name="table1077685961811"></a>
<table><thead align="left"><tr id="row6776145921810"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p87761159141817"><a name="p87761159141817"></a><a name="p87761159141817"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p4776175919185"><a name="p4776175919185"></a><a name="p4776175919185"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p677610599186"><a name="p677610599186"></a><a name="p677610599186"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p1177635911817"><a name="p1177635911817"></a><a name="p1177635911817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row177635917187"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p18981357121915"><a name="p18981357121915"></a><a name="p18981357121915"></a>X-Domain-Id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1877615911184"><a name="p1877615911184"></a><a name="p1877615911184"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p11776115931813"><a name="p11776115931813"></a><a name="p11776115931813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p877695917180"><a name="p877695917180"></a><a name="p877695917180"></a>租户的DomainId</p>
</td>
</tr>
</tbody>
</table>

**表 3**  参数说明

<a name="table34558579"></a>
<table><thead align="left"><tr id="row3194617"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p57437397"><a name="p57437397"></a><a name="p57437397"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.24%" id="mcps1.2.5.1.2"><p id="p21917606"><a name="p21917606"></a><a name="p21917606"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.55%" id="mcps1.2.5.1.3"><p id="p30495700"><a name="p30495700"></a><a name="p30495700"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.21%" id="mcps1.2.5.1.4"><p id="p54232646"><a name="p54232646"></a><a name="p54232646"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row11483346222"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.55%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.21%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row14616163313221"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.55%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.21%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row30768229"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p9198616"><a name="p9198616"></a><a name="p9198616"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.2.5.1.2 "><p id="p6890440"><a name="p6890440"></a><a name="p6890440"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.55%" headers="mcps1.2.5.1.3 "><p id="p21254748"><a name="p21254748"></a><a name="p21254748"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.21%" headers="mcps1.2.5.1.4 "><p id="p43913021"><a name="p43913021"></a><a name="p43913021"></a>API分组编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section64120358"></a>

无

## 响应消息<a name="section26366538"></a>

无

## 状态码<a name="section40212317"></a>

**表 4**  返回消息说明

<a name="table14978051"></a>
<table><thead align="left"><tr id="row11266626"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p40181490"><a name="p40181490"></a><a name="p40181490"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p33475267"><a name="p33475267"></a><a name="p33475267"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row27142108"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p51027174"><a name="p51027174"></a><a name="p51027174"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p39560457"><a name="p39560457"></a><a name="p39560457"></a>No Content</p>
</td>
</tr>
<tr id="row20499795"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p49870669"><a name="p49870669"></a><a name="p49870669"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p12992371"><a name="p12992371"></a><a name="p12992371"></a>Unauthorized</p>
</td>
</tr>
<tr id="row49822483"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9089319"><a name="p9089319"></a><a name="p9089319"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p65146268"><a name="p65146268"></a><a name="p65146268"></a>Forbidden</p>
</td>
</tr>
<tr id="row49445506"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p45663083"><a name="p45663083"></a><a name="p45663083"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p7722248"><a name="p7722248"></a><a name="p7722248"></a>Not Found</p>
</td>
</tr>
<tr id="row2391374"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p59483605"><a name="p59483605"></a><a name="p59483605"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

