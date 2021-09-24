# 解除API与ACL策略的绑定<a name="ZH-CN_TOPIC_0000001081837301"></a>

## 功能介绍<a name="zh-cn_topic_0118924509_section56668631"></a>

解除某条API与ACL策略的绑定关系

## URI<a name="zh-cn_topic_0118924509_section40255631"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924509_table52942781"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924509_row36583141"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924509_p10444414"><a name="zh-cn_topic_0118924509_p10444414"></a><a name="zh-cn_topic_0118924509_p10444414"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924509_p40691167"><a name="zh-cn_topic_0118924509_p40691167"></a><a name="zh-cn_topic_0118924509_p40691167"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924509_row7650225"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924509_p15688475"><a name="zh-cn_topic_0118924509_p15688475"></a><a name="zh-cn_topic_0118924509_p15688475"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924509_p62806982"><a name="zh-cn_topic_0118924509_p62806982"></a><a name="zh-cn_topic_0118924509_p62806982"></a>/v1.0/apigw/acl-bindings/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924509_table54200794"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924509_row33794268"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924509_p52981202"><a name="zh-cn_topic_0118924509_p52981202"></a><a name="zh-cn_topic_0118924509_p52981202"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924509_p63618976"><a name="zh-cn_topic_0118924509_p63618976"></a><a name="zh-cn_topic_0118924509_p63618976"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924509_p52863471"><a name="zh-cn_topic_0118924509_p52863471"></a><a name="zh-cn_topic_0118924509_p52863471"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924509_p54082791"><a name="zh-cn_topic_0118924509_p54082791"></a><a name="zh-cn_topic_0118924509_p54082791"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924509_row18629935"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924509_p32629743"><a name="zh-cn_topic_0118924509_p32629743"></a><a name="zh-cn_topic_0118924509_p32629743"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924509_p25763536"><a name="zh-cn_topic_0118924509_p25763536"></a><a name="zh-cn_topic_0118924509_p25763536"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924509_p6471673"><a name="zh-cn_topic_0118924509_p6471673"></a><a name="zh-cn_topic_0118924509_p6471673"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924509_p54443539"><a name="zh-cn_topic_0118924509_p54443539"></a><a name="zh-cn_topic_0118924509_p54443539"></a>绑定关系编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924509_section26756366"></a>

无

## 响应消息<a name="zh-cn_topic_0118924509_section5160633122513"></a>

无

## 状态码<a name="zh-cn_topic_0118924509_section39480708"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924509_table50690617"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924509_row40699524"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924509_p8327115"><a name="zh-cn_topic_0118924509_p8327115"></a><a name="zh-cn_topic_0118924509_p8327115"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924509_p3407735"><a name="zh-cn_topic_0118924509_p3407735"></a><a name="zh-cn_topic_0118924509_p3407735"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924509_row7591152"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924509_p10903581"><a name="zh-cn_topic_0118924509_p10903581"></a><a name="zh-cn_topic_0118924509_p10903581"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924509_p10774887"><a name="zh-cn_topic_0118924509_p10774887"></a><a name="zh-cn_topic_0118924509_p10774887"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924509_row29865122"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924509_p3155809"><a name="zh-cn_topic_0118924509_p3155809"></a><a name="zh-cn_topic_0118924509_p3155809"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924509_p54294001"><a name="zh-cn_topic_0118924509_p54294001"></a><a name="zh-cn_topic_0118924509_p54294001"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924509_row18883967"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924509_p53206347"><a name="zh-cn_topic_0118924509_p53206347"></a><a name="zh-cn_topic_0118924509_p53206347"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924509_p14746811"><a name="zh-cn_topic_0118924509_p14746811"></a><a name="zh-cn_topic_0118924509_p14746811"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924509_row65612436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924509_p13007094"><a name="zh-cn_topic_0118924509_p13007094"></a><a name="zh-cn_topic_0118924509_p13007094"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924509_p6744143"><a name="zh-cn_topic_0118924509_p6744143"></a><a name="zh-cn_topic_0118924509_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

