# 查询已购买的API列表<a name="apig-zh-api-180713112"></a>

## 功能介绍<a name="section29753322"></a>

租户查询已购买的API列表。

## URI<a name="section66453312"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table48425505"></a>
<table><thead align="left"><tr id="row56159133"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p52595892"><a name="p52595892"></a><a name="p52595892"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p32408880"><a name="p32408880"></a><a name="p32408880"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row7873657"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p33786486"><a name="p33786486"></a><a name="p33786486"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p52350864"><a name="p52350864"></a><a name="p52350864"></a>/v1.0/apigw/purchases/apis[?page_size, page_no, api_id, api_name, group_id, group_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：api\_id、api\_name、group\_id 、group\_name 、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table30588162"></a>
<table><thead align="left"><tr id="row36555591"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p8212881"><a name="p8212881"></a><a name="p8212881"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p61263644"><a name="p61263644"></a><a name="p61263644"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p63408144"><a name="p63408144"></a><a name="p63408144"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p35786003"><a name="p35786003"></a><a name="p35786003"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12985168"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p45165677"><a name="p45165677"></a><a name="p45165677"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p34541202"><a name="p34541202"></a><a name="p34541202"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p46373992"><a name="p46373992"></a><a name="p46373992"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p65305878"><a name="p65305878"></a><a name="p65305878"></a>API编号</p>
</td>
</tr>
<tr id="row50881998"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p27801205"><a name="p27801205"></a><a name="p27801205"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p37305095"><a name="p37305095"></a><a name="p37305095"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p1813870"><a name="p1813870"></a><a name="p1813870"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p12705810"><a name="p12705810"></a><a name="p12705810"></a>API名称</p>
</td>
</tr>
<tr id="row47243430"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1512623"><a name="p1512623"></a><a name="p1512623"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p55413673"><a name="p55413673"></a><a name="p55413673"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p59322556"><a name="p59322556"></a><a name="p59322556"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p40397711"><a name="p40397711"></a><a name="p40397711"></a>API分组编号</p>
</td>
</tr>
<tr id="row28035080"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p56248990"><a name="p56248990"></a><a name="p56248990"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p59874378"><a name="p59874378"></a><a name="p59874378"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p17986417"><a name="p17986417"></a><a name="p17986417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p47613693"><a name="p47613693"></a><a name="p47613693"></a>API分组名称</p>
</td>
</tr>
<tr id="row16992086"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p34181701"><a name="p34181701"></a><a name="p34181701"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p17254385"><a name="p17254385"></a><a name="p17254385"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p55427905"><a name="p55427905"></a><a name="p55427905"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p60475293"><a name="p60475293"></a><a name="p60475293"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row7406732"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p63074406"><a name="p63074406"></a><a name="p63074406"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p8753281"><a name="p8753281"></a><a name="p8753281"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p37927173"><a name="p37927173"></a><a name="p37927173"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p52202136"><a name="p52202136"></a><a name="p52202136"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section61208897"></a>

无

## 响应消息<a name="section58973653"></a>

**表 3**  参数说明

<a name="table52022692"></a>
<table><thead align="left"><tr id="row36307850"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p55254728"><a name="p55254728"></a><a name="p55254728"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p46447987"><a name="p46447987"></a><a name="p46447987"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p4190578"><a name="p4190578"></a><a name="p4190578"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3892526"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p46859150"><a name="p46859150"></a><a name="p46859150"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p37494778"><a name="p37494778"></a><a name="p37494778"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17178203"><a name="p17178203"></a><a name="p17178203"></a>满足查询条件的API总数</p>
</td>
</tr>
<tr id="row20386107"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40661990"><a name="p40661990"></a><a name="p40661990"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5286906"><a name="p5286906"></a><a name="p5286906"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p25586205"><a name="p25586205"></a><a name="p25586205"></a>本次查询返回的API个数</p>
</td>
</tr>
<tr id="row28949261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63188813"><a name="p63188813"></a><a name="p63188813"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18020209"><a name="p18020209"></a><a name="p18020209"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p50350818"><a name="p50350818"></a><a name="p50350818"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table50504178"></a>
<table><thead align="left"><tr id="row21047105"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p27093960"><a name="p27093960"></a><a name="p27093960"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p47127180"><a name="p47127180"></a><a name="p47127180"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p59205236"><a name="p59205236"></a><a name="p59205236"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row30894825"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19452882"><a name="p19452882"></a><a name="p19452882"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p32179608"><a name="p32179608"></a><a name="p32179608"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56411426"><a name="p56411426"></a><a name="p56411426"></a>API编号</p>
</td>
</tr>
<tr id="row37940788"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53304992"><a name="p53304992"></a><a name="p53304992"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22737092"><a name="p22737092"></a><a name="p22737092"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p29765193"><a name="p29765193"></a><a name="p29765193"></a>API名称</p>
</td>
</tr>
<tr id="row14028463"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p62563701"><a name="p62563701"></a><a name="p62563701"></a>purchase_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34495057"><a name="p34495057"></a><a name="p34495057"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p42636200"><a name="p42636200"></a><a name="p42636200"></a>订购关系编号</p>
</td>
</tr>
<tr id="row48181486"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10386316"><a name="p10386316"></a><a name="p10386316"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35985242"><a name="p35985242"></a><a name="p35985242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p29123456"><a name="p29123456"></a><a name="p29123456"></a>API描述</p>
</td>
</tr>
<tr id="row60784516"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24598754"><a name="p24598754"></a><a name="p24598754"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p46342061"><a name="p46342061"></a><a name="p46342061"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p62719436"><a name="p62719436"></a><a name="p62719436"></a>API的访问地址</p>
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

## 状态码<a name="section14009168"></a>

**表 5**  返回消息说明

<a name="table41687570"></a>
<table><thead align="left"><tr id="row56205210"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p56328139"><a name="p56328139"></a><a name="p56328139"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p66285442"><a name="p66285442"></a><a name="p66285442"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row411684"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p33346459"><a name="p33346459"></a><a name="p33346459"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p16708687"><a name="p16708687"></a><a name="p16708687"></a>OK</p>
</td>
</tr>
<tr id="row16160459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p33928804"><a name="p33928804"></a><a name="p33928804"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p63878638"><a name="p63878638"></a><a name="p63878638"></a>Bad Request</p>
</td>
</tr>
<tr id="row38036837"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p61084955"><a name="p61084955"></a><a name="p61084955"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p48934293"><a name="p48934293"></a><a name="p48934293"></a>Unauthorized</p>
</td>
</tr>
<tr id="row37755455"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p38293019"><a name="p38293019"></a><a name="p38293019"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

