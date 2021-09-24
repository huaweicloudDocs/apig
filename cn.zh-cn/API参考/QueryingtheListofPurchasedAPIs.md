# 查询已购买的API列表<a name="ZH-CN_TOPIC_0000001082135129"></a>

## 功能介绍<a name="zh-cn_topic_0118924524_section29753322"></a>

租户查询已购买的API列表。

## URI<a name="zh-cn_topic_0118924524_section66453312"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924524_table48425505"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924524_row56159133"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924524_p52595892"><a name="zh-cn_topic_0118924524_p52595892"></a><a name="zh-cn_topic_0118924524_p52595892"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924524_p32408880"><a name="zh-cn_topic_0118924524_p32408880"></a><a name="zh-cn_topic_0118924524_p32408880"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924524_row7873657"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924524_p33786486"><a name="zh-cn_topic_0118924524_p33786486"></a><a name="zh-cn_topic_0118924524_p33786486"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924524_p52350864"><a name="zh-cn_topic_0118924524_p52350864"></a><a name="zh-cn_topic_0118924524_p52350864"></a>/v1.0/apigw/purchases/apis[?page_size, page_no, api_id, api_name, group_id, group_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：api\_id、api\_name、group\_id 、group\_name 、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924524_table30588162"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924524_row36555591"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924524_p8212881"><a name="zh-cn_topic_0118924524_p8212881"></a><a name="zh-cn_topic_0118924524_p8212881"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924524_p61263644"><a name="zh-cn_topic_0118924524_p61263644"></a><a name="zh-cn_topic_0118924524_p61263644"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924524_p63408144"><a name="zh-cn_topic_0118924524_p63408144"></a><a name="zh-cn_topic_0118924524_p63408144"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924524_p35786003"><a name="zh-cn_topic_0118924524_p35786003"></a><a name="zh-cn_topic_0118924524_p35786003"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924524_row12985168"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924524_p45165677"><a name="zh-cn_topic_0118924524_p45165677"></a><a name="zh-cn_topic_0118924524_p45165677"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924524_p34541202"><a name="zh-cn_topic_0118924524_p34541202"></a><a name="zh-cn_topic_0118924524_p34541202"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924524_p46373992"><a name="zh-cn_topic_0118924524_p46373992"></a><a name="zh-cn_topic_0118924524_p46373992"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924524_p65305878"><a name="zh-cn_topic_0118924524_p65305878"></a><a name="zh-cn_topic_0118924524_p65305878"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row50881998"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924524_p27801205"><a name="zh-cn_topic_0118924524_p27801205"></a><a name="zh-cn_topic_0118924524_p27801205"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924524_p37305095"><a name="zh-cn_topic_0118924524_p37305095"></a><a name="zh-cn_topic_0118924524_p37305095"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924524_p1813870"><a name="zh-cn_topic_0118924524_p1813870"></a><a name="zh-cn_topic_0118924524_p1813870"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924524_p12705810"><a name="zh-cn_topic_0118924524_p12705810"></a><a name="zh-cn_topic_0118924524_p12705810"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row47243430"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924524_p1512623"><a name="zh-cn_topic_0118924524_p1512623"></a><a name="zh-cn_topic_0118924524_p1512623"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924524_p55413673"><a name="zh-cn_topic_0118924524_p55413673"></a><a name="zh-cn_topic_0118924524_p55413673"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924524_p59322556"><a name="zh-cn_topic_0118924524_p59322556"></a><a name="zh-cn_topic_0118924524_p59322556"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924524_p40397711"><a name="zh-cn_topic_0118924524_p40397711"></a><a name="zh-cn_topic_0118924524_p40397711"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row28035080"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924524_p56248990"><a name="zh-cn_topic_0118924524_p56248990"></a><a name="zh-cn_topic_0118924524_p56248990"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924524_p59874378"><a name="zh-cn_topic_0118924524_p59874378"></a><a name="zh-cn_topic_0118924524_p59874378"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924524_p17986417"><a name="zh-cn_topic_0118924524_p17986417"></a><a name="zh-cn_topic_0118924524_p17986417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924524_p47613693"><a name="zh-cn_topic_0118924524_p47613693"></a><a name="zh-cn_topic_0118924524_p47613693"></a>API分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row16992086"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924524_p34181701"><a name="zh-cn_topic_0118924524_p34181701"></a><a name="zh-cn_topic_0118924524_p34181701"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924524_p17254385"><a name="zh-cn_topic_0118924524_p17254385"></a><a name="zh-cn_topic_0118924524_p17254385"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924524_p55427905"><a name="zh-cn_topic_0118924524_p55427905"></a><a name="zh-cn_topic_0118924524_p55427905"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924524_p60475293"><a name="zh-cn_topic_0118924524_p60475293"></a><a name="zh-cn_topic_0118924524_p60475293"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row7406732"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924524_p63074406"><a name="zh-cn_topic_0118924524_p63074406"></a><a name="zh-cn_topic_0118924524_p63074406"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924524_p8753281"><a name="zh-cn_topic_0118924524_p8753281"></a><a name="zh-cn_topic_0118924524_p8753281"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924524_p37927173"><a name="zh-cn_topic_0118924524_p37927173"></a><a name="zh-cn_topic_0118924524_p37927173"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924524_p52202136"><a name="zh-cn_topic_0118924524_p52202136"></a><a name="zh-cn_topic_0118924524_p52202136"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924524_section61208897"></a>

无

## 响应消息<a name="zh-cn_topic_0118924524_section58973653"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924524_table52022692"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924524_row36307850"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924524_p55254728"><a name="zh-cn_topic_0118924524_p55254728"></a><a name="zh-cn_topic_0118924524_p55254728"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924524_p46447987"><a name="zh-cn_topic_0118924524_p46447987"></a><a name="zh-cn_topic_0118924524_p46447987"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924524_p4190578"><a name="zh-cn_topic_0118924524_p4190578"></a><a name="zh-cn_topic_0118924524_p4190578"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924524_row3892526"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p46859150"><a name="zh-cn_topic_0118924524_p46859150"></a><a name="zh-cn_topic_0118924524_p46859150"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p37494778"><a name="zh-cn_topic_0118924524_p37494778"></a><a name="zh-cn_topic_0118924524_p37494778"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p17178203"><a name="zh-cn_topic_0118924524_p17178203"></a><a name="zh-cn_topic_0118924524_p17178203"></a>满足查询条件的API总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row20386107"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p40661990"><a name="zh-cn_topic_0118924524_p40661990"></a><a name="zh-cn_topic_0118924524_p40661990"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p5286906"><a name="zh-cn_topic_0118924524_p5286906"></a><a name="zh-cn_topic_0118924524_p5286906"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p25586205"><a name="zh-cn_topic_0118924524_p25586205"></a><a name="zh-cn_topic_0118924524_p25586205"></a>本次查询返回的API个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row28949261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p63188813"><a name="zh-cn_topic_0118924524_p63188813"></a><a name="zh-cn_topic_0118924524_p63188813"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p18020209"><a name="zh-cn_topic_0118924524_p18020209"></a><a name="zh-cn_topic_0118924524_p18020209"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p50350818"><a name="zh-cn_topic_0118924524_p50350818"></a><a name="zh-cn_topic_0118924524_p50350818"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="zh-cn_topic_0118924524_table50504178"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924524_row21047105"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924524_p27093960"><a name="zh-cn_topic_0118924524_p27093960"></a><a name="zh-cn_topic_0118924524_p27093960"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924524_p47127180"><a name="zh-cn_topic_0118924524_p47127180"></a><a name="zh-cn_topic_0118924524_p47127180"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924524_p59205236"><a name="zh-cn_topic_0118924524_p59205236"></a><a name="zh-cn_topic_0118924524_p59205236"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924524_row30894825"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p19452882"><a name="zh-cn_topic_0118924524_p19452882"></a><a name="zh-cn_topic_0118924524_p19452882"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p32179608"><a name="zh-cn_topic_0118924524_p32179608"></a><a name="zh-cn_topic_0118924524_p32179608"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p56411426"><a name="zh-cn_topic_0118924524_p56411426"></a><a name="zh-cn_topic_0118924524_p56411426"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row37940788"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p53304992"><a name="zh-cn_topic_0118924524_p53304992"></a><a name="zh-cn_topic_0118924524_p53304992"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p22737092"><a name="zh-cn_topic_0118924524_p22737092"></a><a name="zh-cn_topic_0118924524_p22737092"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p29765193"><a name="zh-cn_topic_0118924524_p29765193"></a><a name="zh-cn_topic_0118924524_p29765193"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row14028463"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p62563701"><a name="zh-cn_topic_0118924524_p62563701"></a><a name="zh-cn_topic_0118924524_p62563701"></a>purchase_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p34495057"><a name="zh-cn_topic_0118924524_p34495057"></a><a name="zh-cn_topic_0118924524_p34495057"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p42636200"><a name="zh-cn_topic_0118924524_p42636200"></a><a name="zh-cn_topic_0118924524_p42636200"></a>订购关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row48181486"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p10386316"><a name="zh-cn_topic_0118924524_p10386316"></a><a name="zh-cn_topic_0118924524_p10386316"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p35985242"><a name="zh-cn_topic_0118924524_p35985242"></a><a name="zh-cn_topic_0118924524_p35985242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p29123456"><a name="zh-cn_topic_0118924524_p29123456"></a><a name="zh-cn_topic_0118924524_p29123456"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row60784516"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924524_p24598754"><a name="zh-cn_topic_0118924524_p24598754"></a><a name="zh-cn_topic_0118924524_p24598754"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924524_p46342061"><a name="zh-cn_topic_0118924524_p46342061"></a><a name="zh-cn_topic_0118924524_p46342061"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924524_p62719436"><a name="zh-cn_topic_0118924524_p62719436"></a><a name="zh-cn_topic_0118924524_p62719436"></a>API的访问地址</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 3,
	"size": 3,
	"apis": [{
		"id": "cb498965-8acf-4c98-bd08-4033ef1fcfb4",
		"name": "查询环境列表",
		"purchase_id": "730f8a84-c8db-45ba-a6a5-2669ceb08574",
		"remark": "查询环境列表",
		"req_uri": "/envs"
	},
	{
		"id": "5bbc47e2-95b0-4a56-904e-a3cdc422f8e9",
		"name": "查询分组列表",
		"purchase_id": "2ae11f50-3938-4560-8b76-58e89bb3f825",
		"remark": "查询分组列表",
		"req_uri": "/groups"
	},
	{
		"id": "6632a062-9dcf-4f18-9646-3cabb925a290",
		"name": "查询API列表",
		"purchase_id": "2ae11f50-3938-4560-8b76-58e89bb3f825",
		"remark": "查询API列表",
		"req_uri": "/apis"
	}]
}
```

## 状态码<a name="zh-cn_topic_0118924524_section14009168"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924524_table41687570"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924524_row56205210"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924524_p56328139"><a name="zh-cn_topic_0118924524_p56328139"></a><a name="zh-cn_topic_0118924524_p56328139"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924524_p66285442"><a name="zh-cn_topic_0118924524_p66285442"></a><a name="zh-cn_topic_0118924524_p66285442"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924524_row411684"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924524_p33346459"><a name="zh-cn_topic_0118924524_p33346459"></a><a name="zh-cn_topic_0118924524_p33346459"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924524_p16708687"><a name="zh-cn_topic_0118924524_p16708687"></a><a name="zh-cn_topic_0118924524_p16708687"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row16160459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924524_p33928804"><a name="zh-cn_topic_0118924524_p33928804"></a><a name="zh-cn_topic_0118924524_p33928804"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924524_p63878638"><a name="zh-cn_topic_0118924524_p63878638"></a><a name="zh-cn_topic_0118924524_p63878638"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row38036837"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924524_p61084955"><a name="zh-cn_topic_0118924524_p61084955"></a><a name="zh-cn_topic_0118924524_p61084955"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924524_p48934293"><a name="zh-cn_topic_0118924524_p48934293"></a><a name="zh-cn_topic_0118924524_p48934293"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924524_row37755455"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924524_p38293019"><a name="zh-cn_topic_0118924524_p38293019"></a><a name="zh-cn_topic_0118924524_p38293019"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924524_p6744143"><a name="zh-cn_topic_0118924524_p6744143"></a><a name="zh-cn_topic_0118924524_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

