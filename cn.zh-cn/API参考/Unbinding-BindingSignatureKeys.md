# 解除绑定<a name="ZH-CN_TOPIC_0000001082135139"></a>

## 功能介绍<a name="zh-cn_topic_0118924557_section14755569"></a>

解除API与签名密钥的绑定关系。

## URI<a name="zh-cn_topic_0118924557_section65691257"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924557_table19817972"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924557_row17991642"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924557_p48036934"><a name="zh-cn_topic_0118924557_p48036934"></a><a name="zh-cn_topic_0118924557_p48036934"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924557_p65786413"><a name="zh-cn_topic_0118924557_p65786413"></a><a name="zh-cn_topic_0118924557_p65786413"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924557_row27099257"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924557_p47556242"><a name="zh-cn_topic_0118924557_p47556242"></a><a name="zh-cn_topic_0118924557_p47556242"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924557_p26850399"><a name="zh-cn_topic_0118924557_p26850399"></a><a name="zh-cn_topic_0118924557_p26850399"></a>/v1.0/apigw/sign-bindings/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924557_table45261972"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924557_row64352789"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924557_p45193382"><a name="zh-cn_topic_0118924557_p45193382"></a><a name="zh-cn_topic_0118924557_p45193382"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.36816318368163%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924557_p36785320"><a name="zh-cn_topic_0118924557_p36785320"></a><a name="zh-cn_topic_0118924557_p36785320"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924557_p26820930"><a name="zh-cn_topic_0118924557_p26820930"></a><a name="zh-cn_topic_0118924557_p26820930"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.815918408159185%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924557_p25011741"><a name="zh-cn_topic_0118924557_p25011741"></a><a name="zh-cn_topic_0118924557_p25011741"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924557_row12685153"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924557_p20864436"><a name="zh-cn_topic_0118924557_p20864436"></a><a name="zh-cn_topic_0118924557_p20864436"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.36816318368163%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924557_p12297793"><a name="zh-cn_topic_0118924557_p12297793"></a><a name="zh-cn_topic_0118924557_p12297793"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924557_p56597166"><a name="zh-cn_topic_0118924557_p56597166"></a><a name="zh-cn_topic_0118924557_p56597166"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.815918408159185%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924557_p20967715"><a name="zh-cn_topic_0118924557_p20967715"></a><a name="zh-cn_topic_0118924557_p20967715"></a>API与签名密钥的绑定关系编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924557_section54350403"></a>

无

## 响应消息<a name="zh-cn_topic_0118924557_section40306538"></a>

无

## 状态码<a name="zh-cn_topic_0118924557_section19391585"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924557_table31210887"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924557_row28095078"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924557_p61108822"><a name="zh-cn_topic_0118924557_p61108822"></a><a name="zh-cn_topic_0118924557_p61108822"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924557_p55154851"><a name="zh-cn_topic_0118924557_p55154851"></a><a name="zh-cn_topic_0118924557_p55154851"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924557_row9677322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924557_p45665645"><a name="zh-cn_topic_0118924557_p45665645"></a><a name="zh-cn_topic_0118924557_p45665645"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924557_p7929744"><a name="zh-cn_topic_0118924557_p7929744"></a><a name="zh-cn_topic_0118924557_p7929744"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924557_row4258833"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924557_p9421175"><a name="zh-cn_topic_0118924557_p9421175"></a><a name="zh-cn_topic_0118924557_p9421175"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924557_p24917747"><a name="zh-cn_topic_0118924557_p24917747"></a><a name="zh-cn_topic_0118924557_p24917747"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924557_row22933131"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924557_p45644352"><a name="zh-cn_topic_0118924557_p45644352"></a><a name="zh-cn_topic_0118924557_p45644352"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924557_p6205054"><a name="zh-cn_topic_0118924557_p6205054"></a><a name="zh-cn_topic_0118924557_p6205054"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924557_row55845487"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924557_p27190604"><a name="zh-cn_topic_0118924557_p27190604"></a><a name="zh-cn_topic_0118924557_p27190604"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924557_p15296380"><a name="zh-cn_topic_0118924557_p15296380"></a><a name="zh-cn_topic_0118924557_p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924557_row24835961"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924557_p65555816"><a name="zh-cn_topic_0118924557_p65555816"></a><a name="zh-cn_topic_0118924557_p65555816"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924557_p8420904"><a name="zh-cn_topic_0118924557_p8420904"></a><a name="zh-cn_topic_0118924557_p8420904"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

