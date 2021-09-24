# 删除签名密钥<a name="ZH-CN_TOPIC_0000001082221295"></a>

## 功能介绍<a name="zh-cn_topic_0225568938_section60931416"></a>

删除指定的签名密钥。

删除签名密钥时，其配置的绑定关系会一并删除，相应的签名密钥会失效。

## URI<a name="zh-cn_topic_0225568938_section11511833"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568938_table57268308"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568938_row52124471"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568938_p61332598"><a name="zh-cn_topic_0225568938_p61332598"></a><a name="zh-cn_topic_0225568938_p61332598"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568938_p1884530"><a name="zh-cn_topic_0225568938_p1884530"></a><a name="zh-cn_topic_0225568938_p1884530"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568938_row18429202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568938_p16370366"><a name="zh-cn_topic_0225568938_p16370366"></a><a name="zh-cn_topic_0225568938_p16370366"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568938_p50931295"><a name="zh-cn_topic_0225568938_p50931295"></a><a name="zh-cn_topic_0225568938_p50931295"></a>/v1/{project_id}/apigw/instances/{instance_id}/signs/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568938_table17712970"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568938_row29708827"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568938_p57604768"><a name="zh-cn_topic_0225568938_p57604768"></a><a name="zh-cn_topic_0225568938_p57604768"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.919999999999998%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568938_p35474646"><a name="zh-cn_topic_0225568938_p35474646"></a><a name="zh-cn_topic_0225568938_p35474646"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="21.310000000000002%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568938_p54874084"><a name="zh-cn_topic_0225568938_p54874084"></a><a name="zh-cn_topic_0225568938_p54874084"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.769999999999996%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568938_p15615859"><a name="zh-cn_topic_0225568938_p15615859"></a><a name="zh-cn_topic_0225568938_p15615859"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568938_row762104210502"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568938_p55878963"><a name="zh-cn_topic_0225568938_p55878963"></a><a name="zh-cn_topic_0225568938_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568938_p29902160"><a name="zh-cn_topic_0225568938_p29902160"></a><a name="zh-cn_topic_0225568938_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.310000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568938_p6155914"><a name="zh-cn_topic_0225568938_p6155914"></a><a name="zh-cn_topic_0225568938_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568938_p28867016"><a name="zh-cn_topic_0225568938_p28867016"></a><a name="zh-cn_topic_0225568938_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568938_row1536241145013"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568938_p1780913159538"><a name="zh-cn_topic_0225568938_p1780913159538"></a><a name="zh-cn_topic_0225568938_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568938_p9809215115310"><a name="zh-cn_topic_0225568938_p9809215115310"></a><a name="zh-cn_topic_0225568938_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.310000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568938_p1280914152538"><a name="zh-cn_topic_0225568938_p1280914152538"></a><a name="zh-cn_topic_0225568938_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568938_p1880914157537"><a name="zh-cn_topic_0225568938_p1880914157537"></a><a name="zh-cn_topic_0225568938_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568938_row56925099"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568938_p47530291"><a name="zh-cn_topic_0225568938_p47530291"></a><a name="zh-cn_topic_0225568938_p47530291"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.919999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568938_p24748339"><a name="zh-cn_topic_0225568938_p24748339"></a><a name="zh-cn_topic_0225568938_p24748339"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.310000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568938_p58458452"><a name="zh-cn_topic_0225568938_p58458452"></a><a name="zh-cn_topic_0225568938_p58458452"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.769999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568938_p37514173"><a name="zh-cn_topic_0225568938_p37514173"></a><a name="zh-cn_topic_0225568938_p37514173"></a>签名密钥的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568938_section36497635"></a>

无

## 响应消息<a name="zh-cn_topic_0225568938_section3518463"></a>

无

## 状态码<a name="zh-cn_topic_0225568938_section60043263"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568938_table45073116"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568938_row51996804"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568938_p50991592"><a name="zh-cn_topic_0225568938_p50991592"></a><a name="zh-cn_topic_0225568938_p50991592"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568938_p61669403"><a name="zh-cn_topic_0225568938_p61669403"></a><a name="zh-cn_topic_0225568938_p61669403"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568938_row61165433"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568938_p55453007"><a name="zh-cn_topic_0225568938_p55453007"></a><a name="zh-cn_topic_0225568938_p55453007"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568938_p62508582"><a name="zh-cn_topic_0225568938_p62508582"></a><a name="zh-cn_topic_0225568938_p62508582"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568938_row25706329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568938_p1837908"><a name="zh-cn_topic_0225568938_p1837908"></a><a name="zh-cn_topic_0225568938_p1837908"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568938_p14652835"><a name="zh-cn_topic_0225568938_p14652835"></a><a name="zh-cn_topic_0225568938_p14652835"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568938_row64766654"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568938_p11607591"><a name="zh-cn_topic_0225568938_p11607591"></a><a name="zh-cn_topic_0225568938_p11607591"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568938_p690776"><a name="zh-cn_topic_0225568938_p690776"></a><a name="zh-cn_topic_0225568938_p690776"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568938_row6216987"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568938_p33813964"><a name="zh-cn_topic_0225568938_p33813964"></a><a name="zh-cn_topic_0225568938_p33813964"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568938_p54576602"><a name="zh-cn_topic_0225568938_p54576602"></a><a name="zh-cn_topic_0225568938_p54576602"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568938_row21427375"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568938_p57895827"><a name="zh-cn_topic_0225568938_p57895827"></a><a name="zh-cn_topic_0225568938_p57895827"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568938_p15296380"><a name="zh-cn_topic_0225568938_p15296380"></a><a name="zh-cn_topic_0225568938_p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568938_row61691326"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568938_p30941518"><a name="zh-cn_topic_0225568938_p30941518"></a><a name="zh-cn_topic_0225568938_p30941518"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568938_p6744143"><a name="zh-cn_topic_0225568938_p6744143"></a><a name="zh-cn_topic_0225568938_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

