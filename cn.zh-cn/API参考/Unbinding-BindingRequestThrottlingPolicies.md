# 解除绑定<a name="ZH-CN_TOPIC_0000001082135115"></a>

## 功能介绍<a name="zh-cn_topic_0118922267_section40370977"></a>

解除API与流控策略的绑定关系。

## URI<a name="zh-cn_topic_0118922267_section27794473"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922267_table38359531"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922267_row33945921"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922267_p65265079"><a name="zh-cn_topic_0118922267_p65265079"></a><a name="zh-cn_topic_0118922267_p65265079"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922267_p51980017"><a name="zh-cn_topic_0118922267_p51980017"></a><a name="zh-cn_topic_0118922267_p51980017"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922267_row49631831"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922267_p60755411"><a name="zh-cn_topic_0118922267_p60755411"></a><a name="zh-cn_topic_0118922267_p60755411"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922267_p22241226"><a name="zh-cn_topic_0118922267_p22241226"></a><a name="zh-cn_topic_0118922267_p22241226"></a>/v1.0/apigw/throttle-bindings/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922267_table56708902"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922267_row14847524"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922267_p61798799"><a name="zh-cn_topic_0118922267_p61798799"></a><a name="zh-cn_topic_0118922267_p61798799"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.36816318368163%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922267_p39646798"><a name="zh-cn_topic_0118922267_p39646798"></a><a name="zh-cn_topic_0118922267_p39646798"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922267_p57274058"><a name="zh-cn_topic_0118922267_p57274058"></a><a name="zh-cn_topic_0118922267_p57274058"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.815918408159185%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922267_p8687082"><a name="zh-cn_topic_0118922267_p8687082"></a><a name="zh-cn_topic_0118922267_p8687082"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922267_row32565014"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922267_p20520503"><a name="zh-cn_topic_0118922267_p20520503"></a><a name="zh-cn_topic_0118922267_p20520503"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.36816318368163%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922267_p51548085"><a name="zh-cn_topic_0118922267_p51548085"></a><a name="zh-cn_topic_0118922267_p51548085"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922267_p14645367"><a name="zh-cn_topic_0118922267_p14645367"></a><a name="zh-cn_topic_0118922267_p14645367"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.815918408159185%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922267_p45424102"><a name="zh-cn_topic_0118922267_p45424102"></a><a name="zh-cn_topic_0118922267_p45424102"></a>API与流控策略的绑定关系编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922267_section48823670"></a>

无

## 响应消息<a name="zh-cn_topic_0118922267_section62403175"></a>

无

## 状态码<a name="zh-cn_topic_0118922267_section36759847"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118922267_table64179945"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922267_row56928238"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922267_p47784572"><a name="zh-cn_topic_0118922267_p47784572"></a><a name="zh-cn_topic_0118922267_p47784572"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922267_p45345163"><a name="zh-cn_topic_0118922267_p45345163"></a><a name="zh-cn_topic_0118922267_p45345163"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922267_row49079619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922267_p16026187"><a name="zh-cn_topic_0118922267_p16026187"></a><a name="zh-cn_topic_0118922267_p16026187"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922267_p23052747"><a name="zh-cn_topic_0118922267_p23052747"></a><a name="zh-cn_topic_0118922267_p23052747"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922267_row6148136"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922267_p28237008"><a name="zh-cn_topic_0118922267_p28237008"></a><a name="zh-cn_topic_0118922267_p28237008"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922267_p5496325"><a name="zh-cn_topic_0118922267_p5496325"></a><a name="zh-cn_topic_0118922267_p5496325"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922267_row49466927"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922267_p47398178"><a name="zh-cn_topic_0118922267_p47398178"></a><a name="zh-cn_topic_0118922267_p47398178"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922267_p14047189"><a name="zh-cn_topic_0118922267_p14047189"></a><a name="zh-cn_topic_0118922267_p14047189"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922267_row59315838"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922267_p39853556"><a name="zh-cn_topic_0118922267_p39853556"></a><a name="zh-cn_topic_0118922267_p39853556"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922267_p19914534527"><a name="zh-cn_topic_0118922267_p19914534527"></a><a name="zh-cn_topic_0118922267_p19914534527"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922267_row62213760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922267_p6149829"><a name="zh-cn_topic_0118922267_p6149829"></a><a name="zh-cn_topic_0118922267_p6149829"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922267_p28374163"><a name="zh-cn_topic_0118922267_p28374163"></a><a name="zh-cn_topic_0118922267_p28374163"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

