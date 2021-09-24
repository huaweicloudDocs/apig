# 查询API分组概况<a name="ZH-CN_TOPIC_0000001081837305"></a>

## 功能介绍<a name="zh-cn_topic_0118924542_section3399625"></a>

查询租户名下的API分组概况：上架的API分组个数，未上架的API分组个数。

## URI<a name="zh-cn_topic_0118924542_section30596633"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924542_table53951889"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924542_row50990633"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924542_p36600634"><a name="zh-cn_topic_0118924542_p36600634"></a><a name="zh-cn_topic_0118924542_p36600634"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924542_p11861416"><a name="zh-cn_topic_0118924542_p11861416"></a><a name="zh-cn_topic_0118924542_p11861416"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924542_row21250650"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924542_p43581113"><a name="zh-cn_topic_0118924542_p43581113"></a><a name="zh-cn_topic_0118924542_p43581113"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924542_p40409260"><a name="zh-cn_topic_0118924542_p40409260"></a><a name="zh-cn_topic_0118924542_p40409260"></a>/v1.0/apigw/resources/outline/groups</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924542_section6934242"></a>

无

## 响应消息<a name="zh-cn_topic_0118924542_section24802735"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118924542_table25113310"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924542_row43584205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924542_p40659732"><a name="zh-cn_topic_0118924542_p40659732"></a><a name="zh-cn_topic_0118924542_p40659732"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924542_p5104024"><a name="zh-cn_topic_0118924542_p5104024"></a><a name="zh-cn_topic_0118924542_p5104024"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924542_p10772800"><a name="zh-cn_topic_0118924542_p10772800"></a><a name="zh-cn_topic_0118924542_p10772800"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924542_row181621"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924542_p14711326"><a name="zh-cn_topic_0118924542_p14711326"></a><a name="zh-cn_topic_0118924542_p14711326"></a>offsell_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924542_p50766756"><a name="zh-cn_topic_0118924542_p50766756"></a><a name="zh-cn_topic_0118924542_p50766756"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924542_p18466542"><a name="zh-cn_topic_0118924542_p18466542"></a><a name="zh-cn_topic_0118924542_p18466542"></a>未上架的API分组个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924542_row31981152"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924542_p40336524"><a name="zh-cn_topic_0118924542_p40336524"></a><a name="zh-cn_topic_0118924542_p40336524"></a>onsell_nums</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924542_p46033008"><a name="zh-cn_topic_0118924542_p46033008"></a><a name="zh-cn_topic_0118924542_p46033008"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924542_p37686197"><a name="zh-cn_topic_0118924542_p37686197"></a><a name="zh-cn_topic_0118924542_p37686197"></a>已上架的API分组个数</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"offsell_nums": 1,
	"onsell_nums": 2
}
```

## 状态码<a name="zh-cn_topic_0118924542_section62408183"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924542_table56899163"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924542_row33450687"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924542_p25151132"><a name="zh-cn_topic_0118924542_p25151132"></a><a name="zh-cn_topic_0118924542_p25151132"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924542_p23975830"><a name="zh-cn_topic_0118924542_p23975830"></a><a name="zh-cn_topic_0118924542_p23975830"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924542_row62994068"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924542_p2245887"><a name="zh-cn_topic_0118924542_p2245887"></a><a name="zh-cn_topic_0118924542_p2245887"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924542_p50988816"><a name="zh-cn_topic_0118924542_p50988816"></a><a name="zh-cn_topic_0118924542_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924542_row26639025"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924542_p10277386"><a name="zh-cn_topic_0118924542_p10277386"></a><a name="zh-cn_topic_0118924542_p10277386"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924542_p27161899"><a name="zh-cn_topic_0118924542_p27161899"></a><a name="zh-cn_topic_0118924542_p27161899"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924542_row43130502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924542_p3909799"><a name="zh-cn_topic_0118924542_p3909799"></a><a name="zh-cn_topic_0118924542_p3909799"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924542_p48258341"><a name="zh-cn_topic_0118924542_p48258341"></a><a name="zh-cn_topic_0118924542_p48258341"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924542_row31671890"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924542_p15286310"><a name="zh-cn_topic_0118924542_p15286310"></a><a name="zh-cn_topic_0118924542_p15286310"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924542_p13949586"><a name="zh-cn_topic_0118924542_p13949586"></a><a name="zh-cn_topic_0118924542_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924542_row3648601"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924542_p27101273"><a name="zh-cn_topic_0118924542_p27101273"></a><a name="zh-cn_topic_0118924542_p27101273"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924542_p6744143"><a name="zh-cn_topic_0118924542_p6744143"></a><a name="zh-cn_topic_0118924542_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

