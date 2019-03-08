# 查看APP已绑定的API列表<a name="apig-zh-api-180713047"></a>

## 功能介绍<a name="section45617990"></a>

查询APP已经绑定的API列表。

>![](public_sys-resources/icon-note.gif) **说明：**   
>将API发布到相应的授权的环境后，才能查询到结果。  

## URI<a name="section7908727"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table40887806"></a>
<table><thead align="left"><tr id="row9298403"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p14973182"><a name="p14973182"></a><a name="p14973182"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p4868205"><a name="p4868205"></a><a name="p4868205"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row58780313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p63584873"><a name="p63584873"></a><a name="p63584873"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50101061"><a name="p50101061"></a><a name="p50101061"></a>/v1.0/apigw/app-auths/binded-apis[?page_size, page_no, app_id, api_id, api_name,group_id,group_name,env_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：app\_id、 api\_id 、 api\_name、group\_id、group\_name、env\_id、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table48164278"></a>
<table><thead align="left"><tr id="row10528204"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p47478189"><a name="p47478189"></a><a name="p47478189"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p20528066"><a name="p20528066"></a><a name="p20528066"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p52160627"><a name="p52160627"></a><a name="p52160627"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p64261290"><a name="p64261290"></a><a name="p64261290"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row37781964"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p40440259"><a name="p40440259"></a><a name="p40440259"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p54435575"><a name="p54435575"></a><a name="p54435575"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p47205455"><a name="p47205455"></a><a name="p47205455"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p65545524"><a name="p65545524"></a><a name="p65545524"></a>应用编号</p>
</td>
</tr>
<tr id="row53038806"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1176057"><a name="p1176057"></a><a name="p1176057"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p28151772"><a name="p28151772"></a><a name="p28151772"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p65701031"><a name="p65701031"></a><a name="p65701031"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p20183299"><a name="p20183299"></a><a name="p20183299"></a>API编号</p>
</td>
</tr>
<tr id="row47431967"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p16784086"><a name="p16784086"></a><a name="p16784086"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p17333746"><a name="p17333746"></a><a name="p17333746"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p61856219"><a name="p61856219"></a><a name="p61856219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p44297848"><a name="p44297848"></a><a name="p44297848"></a>API名称</p>
</td>
</tr>
<tr id="row63136318"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p13768133"><a name="p13768133"></a><a name="p13768133"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p41476980"><a name="p41476980"></a><a name="p41476980"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p4192244"><a name="p4192244"></a><a name="p4192244"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p4027501"><a name="p4027501"></a><a name="p4027501"></a>API分组编号</p>
</td>
</tr>
<tr id="row36247510"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p50367158"><a name="p50367158"></a><a name="p50367158"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p53207970"><a name="p53207970"></a><a name="p53207970"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p14878339"><a name="p14878339"></a><a name="p14878339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p64294849"><a name="p64294849"></a><a name="p64294849"></a>API分组名称</p>
</td>
</tr>
<tr id="row41782734"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p28958306"><a name="p28958306"></a><a name="p28958306"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p63921413"><a name="p63921413"></a><a name="p63921413"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p10252002"><a name="p10252002"></a><a name="p10252002"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p25105823"><a name="p25105823"></a><a name="p25105823"></a>授权的环境编号</p>
</td>
</tr>
<tr id="row24625817"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p48534154"><a name="p48534154"></a><a name="p48534154"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p38952367"><a name="p38952367"></a><a name="p38952367"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1025136"><a name="p1025136"></a><a name="p1025136"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p15927223"><a name="p15927223"></a><a name="p15927223"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row9127279"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1112119"><a name="p1112119"></a><a name="p1112119"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p22972791"><a name="p22972791"></a><a name="p22972791"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p48856792"><a name="p48856792"></a><a name="p48856792"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p65086081"><a name="p65086081"></a><a name="p65086081"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section4069680"></a>

无

## 响应消息<a name="section61208646"></a>

**表 3**  参数说明

<a name="table43505476"></a>
<table><thead align="left"><tr id="row17298029"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p58963140"><a name="p58963140"></a><a name="p58963140"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11284998"><a name="p11284998"></a><a name="p11284998"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p41669661"><a name="p41669661"></a><a name="p41669661"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19799409"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p60248297"><a name="p60248297"></a><a name="p60248297"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48273902"><a name="p48273902"></a><a name="p48273902"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17871975"><a name="p17871975"></a><a name="p17871975"></a>符合条件的API总数</p>
</td>
</tr>
<tr id="row26630051"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9550502"><a name="p9550502"></a><a name="p9550502"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35393169"><a name="p35393169"></a><a name="p35393169"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48274445"><a name="p48274445"></a><a name="p48274445"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="row31816825"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p27026000"><a name="p27026000"></a><a name="p27026000"></a>auths</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p41622412"><a name="p41622412"></a><a name="p41622412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15972245"><a name="p15972245"></a><a name="p15972245"></a>本次返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  auths参数说明

<a name="table9532482"></a>
<table><thead align="left"><tr id="row5407061"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p35318772"><a name="p35318772"></a><a name="p35318772"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p42248272"><a name="p42248272"></a><a name="p42248272"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p66666832"><a name="p66666832"></a><a name="p66666832"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row31304284"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52619101"><a name="p52619101"></a><a name="p52619101"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34288827"><a name="p34288827"></a><a name="p34288827"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p25931613"><a name="p25931613"></a><a name="p25931613"></a>授权关系编号</p>
</td>
</tr>
<tr id="row32057932"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p46555663"><a name="p46555663"></a><a name="p46555663"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12912396"><a name="p12912396"></a><a name="p12912396"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p39271145"><a name="p39271145"></a><a name="p39271145"></a>API的编号</p>
</td>
</tr>
<tr id="row17895987"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40288836"><a name="p40288836"></a><a name="p40288836"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42170249"><a name="p42170249"></a><a name="p42170249"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60346986"><a name="p60346986"></a><a name="p60346986"></a>API的名称</p>
</td>
</tr>
<tr id="row6251969"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p36647513"><a name="p36647513"></a><a name="p36647513"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15658561"><a name="p15658561"></a><a name="p15658561"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60383905"><a name="p60383905"></a><a name="p60383905"></a>API绑定的分组</p>
</td>
</tr>
<tr id="row6584238"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63561270"><a name="p63561270"></a><a name="p63561270"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48189259"><a name="p48189259"></a><a name="p48189259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11015892"><a name="p11015892"></a><a name="p11015892"></a>API的描述信息</p>
</td>
</tr>
<tr id="row32034168"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44630795"><a name="p44630795"></a><a name="p44630795"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p58324614"><a name="p58324614"></a><a name="p58324614"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p26673298"><a name="p26673298"></a><a name="p26673298"></a>API类型</p>
</td>
</tr>
<tr id="row38733094"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50372877"><a name="p50372877"></a><a name="p50372877"></a>envname</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p53671257"><a name="p53671257"></a><a name="p53671257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52404594"><a name="p52404594"></a><a name="p52404594"></a>api授权绑定的环境</p>
</td>
</tr>
<tr id="row1879303"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18005821"><a name="p18005821"></a><a name="p18005821"></a>auth_role</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p49185396"><a name="p49185396"></a><a name="p49185396"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p24594131"><a name="p24594131"></a><a name="p24594131"></a>授权者</p>
</td>
</tr>
<tr id="row20020594"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11055393"><a name="p11055393"></a><a name="p11055393"></a>auth_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23071629"><a name="p23071629"></a><a name="p23071629"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56862621"><a name="p56862621"></a><a name="p56862621"></a>授权创建的时间</p>
</td>
</tr>
<tr id="row42001542"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p46681736"><a name="p46681736"></a><a name="p46681736"></a>appid</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23124258"><a name="p23124258"></a><a name="p23124258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61125629"><a name="p61125629"></a><a name="p61125629"></a>APP的编号</p>
</td>
</tr>
<tr id="row13259754"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p298313"><a name="p298313"></a><a name="p298313"></a>app_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24163388"><a name="p24163388"></a><a name="p24163388"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11077420"><a name="p11077420"></a><a name="p11077420"></a>APP的名称</p>
</td>
</tr>
<tr id="row32587918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p22375683"><a name="p22375683"></a><a name="p22375683"></a>app_creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p491049"><a name="p491049"></a><a name="p491049"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p39775015"><a name="p39775015"></a><a name="p39775015"></a>APP的创建者，取值如下：</p>
<a name="ul22430823"></a><a name="ul22430823"></a><ul id="ul22430823"><li>USER：租户自己创建</li><li>MARKET：API市场分配</li></ul>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"auths": [{
		"id": "cfa688d8-094b-445a-b270-6aeb0b70a84a",
		"api_id": "6632a062-9dcf-4f18-9646-3cabb925a290",
		"api_name": "查询API列表",
		"group_name": "api_group_001",
		"api_type": 1,
		"api_remark": "查询API列表",
		"envname": "RELEASE",
		"auth_role": "PROVIDER",
		"auth_time": "2017-12-28T12:46:43Z",
		"appid": "14b399ac-967f-4115-bb62-c0346b4537e9",
		"app_name": "app_001",
		"app_creator": "USER"
	},
	{
		"id": "c3fec803-dcdc-4fdf-9278-4872ebdc2a2e",
		"api_id": "5bbc47e2-95b0-4a56-904e-a3cdc422f8e9",
		"api_name": "查询分组列表",
		"group_name": "api_group_001",
		"api_type": 1,
		"api_remark": "查询分组列表",
		"envname": "RELEASE",
		"auth_role": "PROVIDER",
		"auth_time": "2017-12-28T12:46:43Z",
		"appid": "14b399ac-967f-4115-bb62-c0346b4537e9",
		"app_name": "app_001",
		"app_creator": "USER"
	}]
}
```

## 状态码<a name="section36627122"></a>

**表 5**  返回消息说明

<a name="table16081870"></a>
<table><thead align="left"><tr id="row27929984"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p47736268"><a name="p47736268"></a><a name="p47736268"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p41432467"><a name="p41432467"></a><a name="p41432467"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row586687"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p47521720"><a name="p47521720"></a><a name="p47521720"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p24054117"><a name="p24054117"></a><a name="p24054117"></a>OK</p>
</td>
</tr>
<tr id="row15160467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20038314"><a name="p20038314"></a><a name="p20038314"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p12490729"><a name="p12490729"></a><a name="p12490729"></a>Bad Request</p>
</td>
</tr>
<tr id="row45307704"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p46045383"><a name="p46045383"></a><a name="p46045383"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p164181330094"><a name="p164181330094"></a><a name="p164181330094"></a>Unauthorized</p>
</td>
</tr>
<tr id="row12652459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p18216220"><a name="p18216220"></a><a name="p18216220"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p66227710"><a name="p66227710"></a><a name="p66227710"></a>Forbidden</p>
</td>
</tr>
<tr id="row59178480"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p28727614"><a name="p28727614"></a><a name="p28727614"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p45235408"><a name="p45235408"></a><a name="p45235408"></a>Not Found</p>
</td>
</tr>
<tr id="row4465495"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p26160778"><a name="p26160778"></a><a name="p26160778"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

