# 删除变量<a name="ZH-CN_TOPIC_0000001081837281"></a>

## 功能介绍<a name="zh-cn_topic_0118922251_section55943762"></a>

删除指定的环境变量。

## URI<a name="zh-cn_topic_0118922251_section33731811"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922251_table19729176"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922251_row5771036"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922251_p64800780"><a name="zh-cn_topic_0118922251_p64800780"></a><a name="zh-cn_topic_0118922251_p64800780"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922251_p14371808"><a name="zh-cn_topic_0118922251_p14371808"></a><a name="zh-cn_topic_0118922251_p14371808"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922251_row23265793"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922251_p5481046"><a name="zh-cn_topic_0118922251_p5481046"></a><a name="zh-cn_topic_0118922251_p5481046"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922251_p41311559"><a name="zh-cn_topic_0118922251_p41311559"></a><a name="zh-cn_topic_0118922251_p41311559"></a>/v1.0/apigw/env-variables/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922251_table57902014"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922251_row49206371"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922251_p26293128"><a name="zh-cn_topic_0118922251_p26293128"></a><a name="zh-cn_topic_0118922251_p26293128"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922251_p49368609"><a name="zh-cn_topic_0118922251_p49368609"></a><a name="zh-cn_topic_0118922251_p49368609"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922251_p39434391"><a name="zh-cn_topic_0118922251_p39434391"></a><a name="zh-cn_topic_0118922251_p39434391"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922251_p40069073"><a name="zh-cn_topic_0118922251_p40069073"></a><a name="zh-cn_topic_0118922251_p40069073"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922251_row24369463"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922251_p27769523"><a name="zh-cn_topic_0118922251_p27769523"></a><a name="zh-cn_topic_0118922251_p27769523"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922251_p34738858"><a name="zh-cn_topic_0118922251_p34738858"></a><a name="zh-cn_topic_0118922251_p34738858"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922251_p62384134"><a name="zh-cn_topic_0118922251_p62384134"></a><a name="zh-cn_topic_0118922251_p62384134"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922251_p19950127"><a name="zh-cn_topic_0118922251_p19950127"></a><a name="zh-cn_topic_0118922251_p19950127"></a>环境变量的ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922251_section35150849"></a>

无

## 响应消息<a name="zh-cn_topic_0118922251_section28646509"></a>

无

## 状态码<a name="zh-cn_topic_0118922251_section47922188"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118922251_table30502150"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922251_row53785576"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922251_p61664417"><a name="zh-cn_topic_0118922251_p61664417"></a><a name="zh-cn_topic_0118922251_p61664417"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922251_p28761850"><a name="zh-cn_topic_0118922251_p28761850"></a><a name="zh-cn_topic_0118922251_p28761850"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922251_row48008475"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922251_p63481261"><a name="zh-cn_topic_0118922251_p63481261"></a><a name="zh-cn_topic_0118922251_p63481261"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922251_p41708503"><a name="zh-cn_topic_0118922251_p41708503"></a><a name="zh-cn_topic_0118922251_p41708503"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922251_row39832213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922251_p5183831"><a name="zh-cn_topic_0118922251_p5183831"></a><a name="zh-cn_topic_0118922251_p5183831"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922251_p19149641153911"><a name="zh-cn_topic_0118922251_p19149641153911"></a><a name="zh-cn_topic_0118922251_p19149641153911"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922251_row20916985"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922251_p16554262"><a name="zh-cn_topic_0118922251_p16554262"></a><a name="zh-cn_topic_0118922251_p16554262"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922251_p65826835"><a name="zh-cn_topic_0118922251_p65826835"></a><a name="zh-cn_topic_0118922251_p65826835"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922251_row55570605"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922251_p4925150"><a name="zh-cn_topic_0118922251_p4925150"></a><a name="zh-cn_topic_0118922251_p4925150"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922251_p63392835"><a name="zh-cn_topic_0118922251_p63392835"></a><a name="zh-cn_topic_0118922251_p63392835"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922251_row33664604"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922251_p42478443"><a name="zh-cn_topic_0118922251_p42478443"></a><a name="zh-cn_topic_0118922251_p42478443"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922251_p18201891"><a name="zh-cn_topic_0118922251_p18201891"></a><a name="zh-cn_topic_0118922251_p18201891"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922251_row29599293"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922251_p48732548"><a name="zh-cn_topic_0118922251_p48732548"></a><a name="zh-cn_topic_0118922251_p48732548"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922251_p14947689"><a name="zh-cn_topic_0118922251_p14947689"></a><a name="zh-cn_topic_0118922251_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

