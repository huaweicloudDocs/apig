# 查询可上架的API分组列表<a name="apig-phapi-180713100"></a>

## 功能介绍<a name="section47153539"></a>

查询租户名下有哪些API分组可以上架到云市场。

满足要求的API分组应具备以下特性：分组下有已发布到RELEASE环境且认证方式为APP认证的公有API。

## URI<a name="section21728667"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table810618"></a>
<table><thead align="left"><tr id="row24350089"><th class="cellrowborder" valign="top" width="40.129999999999995%" id="mcps1.2.3.1.1"><p id="p26200207"><a name="p26200207"></a><a name="p26200207"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="59.870000000000005%" id="mcps1.2.3.1.2"><p id="p41842029"><a name="p41842029"></a><a name="p41842029"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row33761228"><td class="cellrowborder" valign="top" width="40.129999999999995%" headers="mcps1.2.3.1.1 "><p id="p50304980"><a name="p50304980"></a><a name="p50304980"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="59.870000000000005%" headers="mcps1.2.3.1.2 "><p id="p48171564"><a name="p48171564"></a><a name="p48171564"></a>/v1/{project_id}/apigw/instances/{instance_id}/market/api-groups/tosell[?page_size, page_no, name]</p>
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

<a name="table57467174"></a>
<table><thead align="left"><tr id="row58385281"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p31587325"><a name="p31587325"></a><a name="p31587325"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p8436529"><a name="p8436529"></a><a name="p8436529"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p12270278"><a name="p12270278"></a><a name="p12270278"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p54368484"><a name="p54368484"></a><a name="p54368484"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46891632142116"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row915173210210"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row41771058"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p28012504"><a name="p28012504"></a><a name="p28012504"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p54420351"><a name="p54420351"></a><a name="p54420351"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p45972302"><a name="p45972302"></a><a name="p45972302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p32769006"><a name="p32769006"></a><a name="p32769006"></a>API分组的名称</p>
</td>
</tr>
<tr id="row26485604"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p64959168"><a name="p64959168"></a><a name="p64959168"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p27201216"><a name="p27201216"></a><a name="p27201216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p55814860"><a name="p55814860"></a><a name="p55814860"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p24709837"><a name="p24709837"></a><a name="p24709837"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row21061949"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p28296328"><a name="p28296328"></a><a name="p28296328"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p10301244"><a name="p10301244"></a><a name="p10301244"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p29094399"><a name="p29094399"></a><a name="p29094399"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p7836156"><a name="p7836156"></a><a name="p7836156"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section61340275"></a>

无

## 响应消息<a name="section2506351"></a>

**表 4**  参数说明

<a name="table33988889"></a>
<table><thead align="left"><tr id="row2774919"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p23441890"><a name="p23441890"></a><a name="p23441890"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p19744913"><a name="p19744913"></a><a name="p19744913"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p55834109"><a name="p55834109"></a><a name="p55834109"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26268941"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47409449"><a name="p47409449"></a><a name="p47409449"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14960186"><a name="p14960186"></a><a name="p14960186"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3815592"><a name="p3815592"></a><a name="p3815592"></a>满足查询条件的API分组总数</p>
</td>
</tr>
<tr id="row34340333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p30103601"><a name="p30103601"></a><a name="p30103601"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22472580"><a name="p22472580"></a><a name="p22472580"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8339729"><a name="p8339729"></a><a name="p8339729"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="row7948700"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39864944"><a name="p39864944"></a><a name="p39864944"></a>groups</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7835025"><a name="p7835025"></a><a name="p7835025"></a>字典数据类型：待上架的API分组列表</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30657254"><a name="p30657254"></a><a name="p30657254"></a>本次查询返回的API分组列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  groups参数说明

<a name="table7479831"></a>
<table><thead align="left"><tr id="row2008551"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p28474971"><a name="p28474971"></a><a name="p28474971"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p24771315"><a name="p24771315"></a><a name="p24771315"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p60319512"><a name="p60319512"></a><a name="p60319512"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row54042289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15349287"><a name="p15349287"></a><a name="p15349287"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35332705"><a name="p35332705"></a><a name="p35332705"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p43376839"><a name="p43376839"></a><a name="p43376839"></a>API分组编号</p>
</td>
</tr>
<tr id="row13441371"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15009296"><a name="p15009296"></a><a name="p15009296"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7793486"><a name="p7793486"></a><a name="p7793486"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27292604"><a name="p27292604"></a><a name="p27292604"></a>API分组名称</p>
</td>
</tr>
<tr id="row32084630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48718228"><a name="p48718228"></a><a name="p48718228"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p53862399"><a name="p53862399"></a><a name="p53862399"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p778174"><a name="p778174"></a><a name="p778174"></a>API分组描述</p>
</td>
</tr>
<tr id="row30418186"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47953963"><a name="p47953963"></a><a name="p47953963"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p59065789"><a name="p59065789"></a><a name="p59065789"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19599591"><a name="p19599591"></a><a name="p19599591"></a>API分组最后更新时间</p>
</td>
</tr>
<tr id="row61023207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p43932758"><a name="p43932758"></a><a name="p43932758"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1783641"><a name="p1783641"></a><a name="p1783641"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10257241"><a name="p10257241"></a><a name="p10257241"></a>API分组绑定的子域名</p>
</td>
</tr>
<tr id="row28444968"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p22341086"><a name="p22341086"></a><a name="p22341086"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64797548"><a name="p64797548"></a><a name="p64797548"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14110075"><a name="p14110075"></a><a name="p14110075"></a>云市场为API分组分配的访问域名，当该分组是二次上架时，该字段有返回值。</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 4,
	"size": 4,
	"groups": [{
		"id": "4faf6453-13a8-4780-ba52-a8488db01dea",
		"name": "api_group_004",
		"remark": "分组004",
		"sl_domain": "xxxxxxxxxxxxxxxxx",
		"url_domain": "yyyyyyyyyyyyyyyy",
		"update_time": "2017-12-29T03:38:37Z"
	},
	{
		"id": "f0585333-5722-4878-b7fa-31ae00b6ae3a",
		"name": "api_group_003",
		"remark": "分组003",
		"sl_domain": "xxxxxxxxxxxxxxxxx",
		"url_domain": "",
		"update_time": "2017-12-29T03:38:32Z"
	},
	{
		"id": "02a8ab3c-b278-4de5-a096-852829671ae7",
		"name": "api_group_002",
		"remark": "分组002",
		"sl_domain": "xxxxxxxxxxxxxxxxx",
		"url_domain": "",
		"update_time": "2017-12-28T11:57:35Z"
	},
	{
		"id": "73c58022-f20d-495a-a188-85d718647f09",
		"name": "api_group_001",
		"remark": "分组001",
		"sl_domain": "xxxxxxxxxxxxxxxxx",
		"url_domain": "",
		"update_time": "2017-12-28T11:57:27Z"
	}]
}
```

## 状态码<a name="section15191564"></a>

**表 6**  返回消息说明

<a name="table7632062"></a>
<table><thead align="left"><tr id="row29647066"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p52602177"><a name="p52602177"></a><a name="p52602177"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p32917907"><a name="p32917907"></a><a name="p32917907"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49104826"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p18067998"><a name="p18067998"></a><a name="p18067998"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p54221734"><a name="p54221734"></a><a name="p54221734"></a>OK</p>
</td>
</tr>
<tr id="row18233563"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p523669"><a name="p523669"></a><a name="p523669"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p42417256"><a name="p42417256"></a><a name="p42417256"></a>Bad Request</p>
</td>
</tr>
<tr id="row46210986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p52102356"><a name="p52102356"></a><a name="p52102356"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p59541290"><a name="p59541290"></a><a name="p59541290"></a>Unauthorized</p>
</td>
</tr>
<tr id="row66109570"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p53274950"><a name="p53274950"></a><a name="p53274950"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

