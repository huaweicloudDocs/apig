# 查询已经上架的API分组列表<a name="apig-phapi-180713103"></a>

## 功能介绍<a name="section46998241"></a>

查询已经在云市场上架的API分组。

## URI<a name="section20330987"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table40505145"></a>
<table><thead align="left"><tr id="row54329699"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p38629533"><a name="p38629533"></a><a name="p38629533"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p41984496"><a name="p41984496"></a><a name="p41984496"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row45300995"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p45501950"><a name="p45501950"></a><a name="p45501950"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p61779338"><a name="p61779338"></a><a name="p61779338"></a>/v1/{project_id}/apigw/instances/{instance_id}/market/api-groups/onsell[?page_size, page_no, name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：name、page\_size、page\_no。  

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
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1877615911184"><a name="p1877615911184"></a><a name="p1877615911184"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p11776115931813"><a name="p11776115931813"></a><a name="p11776115931813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p877695917180"><a name="p877695917180"></a><a name="p877695917180"></a>租户的DomainId</p>
</td>
</tr>
</tbody>
</table>

**表 3**  参数信息

<a name="table1220001"></a>
<table><thead align="left"><tr id="row1993291"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p27238907"><a name="p27238907"></a><a name="p27238907"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.15%" id="mcps1.2.5.1.2"><p id="p58867876"><a name="p58867876"></a><a name="p58867876"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.7%" id="mcps1.2.5.1.3"><p id="p3568621"><a name="p3568621"></a><a name="p3568621"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.15%" id="mcps1.2.5.1.4"><p id="p20622846"><a name="p20622846"></a><a name="p20622846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19132198112216"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.15%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row7600177172216"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.15%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row59837824"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p15025562"><a name="p15025562"></a><a name="p15025562"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.5.1.2 "><p id="p9111029"><a name="p9111029"></a><a name="p9111029"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.5.1.3 "><p id="p66904761"><a name="p66904761"></a><a name="p66904761"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.15%" headers="mcps1.2.5.1.4 "><p id="p50576524"><a name="p50576524"></a><a name="p50576524"></a>API分组名称</p>
</td>
</tr>
<tr id="row52535540"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p27520356"><a name="p27520356"></a><a name="p27520356"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.5.1.2 "><p id="p14556344"><a name="p14556344"></a><a name="p14556344"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.5.1.3 "><p id="p38213209"><a name="p38213209"></a><a name="p38213209"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="38.15%" headers="mcps1.2.5.1.4 "><p id="p8262190"><a name="p8262190"></a><a name="p8262190"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row7250847"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p50447774"><a name="p50447774"></a><a name="p50447774"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="19.15%" headers="mcps1.2.5.1.2 "><p id="p59737926"><a name="p59737926"></a><a name="p59737926"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.7%" headers="mcps1.2.5.1.3 "><p id="p6933822"><a name="p6933822"></a><a name="p6933822"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="38.15%" headers="mcps1.2.5.1.4 "><p id="p24768686"><a name="p24768686"></a><a name="p24768686"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section48761158"></a>

无

## 响应消息<a name="section57339740"></a>

**表 4**  消息参数

<a name="table38779059"></a>
<table><thead align="left"><tr id="row3980335"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p53971742"><a name="p53971742"></a><a name="p53971742"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p9634977"><a name="p9634977"></a><a name="p9634977"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p42235681"><a name="p42235681"></a><a name="p42235681"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row65646981"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15805238"><a name="p15805238"></a><a name="p15805238"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5155867"><a name="p5155867"></a><a name="p5155867"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14972060"><a name="p14972060"></a><a name="p14972060"></a>查询到的满足条件的API分组总数</p>
</td>
</tr>
<tr id="row530819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p42996411"><a name="p42996411"></a><a name="p42996411"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p60157251"><a name="p60157251"></a><a name="p60157251"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p40899139"><a name="p40899139"></a><a name="p40899139"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="row32547936"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19137160"><a name="p19137160"></a><a name="p19137160"></a>groups</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6606141"><a name="p6606141"></a><a name="p6606141"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65335398"><a name="p65335398"></a><a name="p65335398"></a>本次查询返回的API分组列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  groups参数说明

<a name="table51147674"></a>
<table><thead align="left"><tr id="row26992952"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p38945471"><a name="p38945471"></a><a name="p38945471"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p466603"><a name="p466603"></a><a name="p466603"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p37794916"><a name="p37794916"></a><a name="p37794916"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row41489361"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5195099"><a name="p5195099"></a><a name="p5195099"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18149865"><a name="p18149865"></a><a name="p18149865"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60852964"><a name="p60852964"></a><a name="p60852964"></a>API分组编号</p>
</td>
</tr>
<tr id="row10805765"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2851790"><a name="p2851790"></a><a name="p2851790"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p29668407"><a name="p29668407"></a><a name="p29668407"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54330728"><a name="p54330728"></a><a name="p54330728"></a>API分组名称</p>
</td>
</tr>
<tr id="row19214507"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12871260"><a name="p12871260"></a><a name="p12871260"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35939178"><a name="p35939178"></a><a name="p35939178"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p25392316"><a name="p25392316"></a><a name="p25392316"></a>API分组描述</p>
</td>
</tr>
<tr id="row27204259"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p56061334"><a name="p56061334"></a><a name="p56061334"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44674243"><a name="p44674243"></a><a name="p44674243"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61843920"><a name="p61843920"></a><a name="p61843920"></a>API分组最后更新时间</p>
</td>
</tr>
<tr id="row19724370"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p54170131"><a name="p54170131"></a><a name="p54170131"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p25704456"><a name="p25704456"></a><a name="p25704456"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1686169"><a name="p1686169"></a><a name="p1686169"></a>云市场分配给该API分组的访问域名</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 3,
	"size": 3,
	"groups": [{
		"id": "f0585333-5722-4878-b7fa-31ae00b6ae3a",
		"name": "api_group_003",
		"remark": "分组003",
		"update_time": "2017-12-29T03:38:32Z",
		"url_domain": "test03.market.example.com"
	},
	{
		"id": "02a8ab3c-b278-4de5-a096-852829671ae7",
		"name": "api_group_002",
		"remark": "分组002",
		"update_time": "2017-12-28T11:57:35Z",
		"url_domain": "test02.market.example.com"
	},
	{
		"id": "73c58022-f20d-495a-a188-85d718647f09",
		"name": "api_group_001",
		"remark": "分组001",
		"update_time": "2017-12-28T11:57:27Z",
		"url_domain": "test.market.example.com"
	}]
}
```

## 状态码<a name="section36197244"></a>

**表 6**  返回消息说明

<a name="table36793112"></a>
<table><thead align="left"><tr id="row14161903"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p6263465"><a name="p6263465"></a><a name="p6263465"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p37578639"><a name="p37578639"></a><a name="p37578639"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row23970955"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p62599170"><a name="p62599170"></a><a name="p62599170"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p37368030"><a name="p37368030"></a><a name="p37368030"></a>OK</p>
</td>
</tr>
<tr id="row767958"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p62204612"><a name="p62204612"></a><a name="p62204612"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p5408778"><a name="p5408778"></a><a name="p5408778"></a>Bad Request</p>
</td>
</tr>
<tr id="row48679006"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p50685404"><a name="p50685404"></a><a name="p50685404"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p11877063"><a name="p11877063"></a><a name="p11877063"></a>Unauthorized</p>
</td>
</tr>
<tr id="row39784704"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1335609"><a name="p1335609"></a><a name="p1335609"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

