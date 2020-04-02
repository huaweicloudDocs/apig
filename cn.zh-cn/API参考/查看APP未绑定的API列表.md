# 查看APP未绑定的API列表<a name="apig-zh-api-180713045"></a>

## 功能简介<a name="section57945658"></a>

查询指定环境上某个APP未绑定的API列表，包括自有API和从云市场购买的API。

## URI<a name="section51748875"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table65264697"></a>
<table><thead align="left"><tr id="row59320654"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p40243635"><a name="p40243635"></a><a name="p40243635"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p38508980"><a name="p38508980"></a><a name="p38508980"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row32219707"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p59659437"><a name="p59659437"></a><a name="p59659437"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p576244"><a name="p576244"></a><a name="p576244"></a>/v1.0/apigw/app-auths/unbinded-apis[?page_size, page_no, app_id, env_id, api_id, api_name, group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：app\_id、api\_id、api\_name、group\_id、env\_id、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table22390613"></a>
<table><thead align="left"><tr id="row15100740"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p15200464"><a name="p15200464"></a><a name="p15200464"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p23278039"><a name="p23278039"></a><a name="p23278039"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p6473027"><a name="p6473027"></a><a name="p6473027"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p54553212"><a name="p54553212"></a><a name="p54553212"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row56734057"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p32055923"><a name="p32055923"></a><a name="p32055923"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p46392961"><a name="p46392961"></a><a name="p46392961"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p66842364"><a name="p66842364"></a><a name="p66842364"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p45522379"><a name="p45522379"></a><a name="p45522379"></a>应用id</p>
</td>
</tr>
<tr id="row7048230"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p34035727"><a name="p34035727"></a><a name="p34035727"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p5430464"><a name="p5430464"></a><a name="p5430464"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p37214434"><a name="p37214434"></a><a name="p37214434"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p61579164"><a name="p61579164"></a><a name="p61579164"></a>环境id</p>
</td>
</tr>
<tr id="row17341570"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p62489940"><a name="p62489940"></a><a name="p62489940"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p28520403"><a name="p28520403"></a><a name="p28520403"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p28451302"><a name="p28451302"></a><a name="p28451302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p22854134"><a name="p22854134"></a><a name="p22854134"></a>API分组编号</p>
</td>
</tr>
<tr id="row4360616"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p17665597"><a name="p17665597"></a><a name="p17665597"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p21627267"><a name="p21627267"></a><a name="p21627267"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6978209"><a name="p6978209"></a><a name="p6978209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p28364096"><a name="p28364096"></a><a name="p28364096"></a>API编号</p>
</td>
</tr>
<tr id="row53950280"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p7896522"><a name="p7896522"></a><a name="p7896522"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p35638561"><a name="p35638561"></a><a name="p35638561"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1042357"><a name="p1042357"></a><a name="p1042357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p17322093"><a name="p17322093"></a><a name="p17322093"></a>API名称</p>
</td>
</tr>
<tr id="row21681114"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p11339844"><a name="p11339844"></a><a name="p11339844"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p46112199"><a name="p46112199"></a><a name="p46112199"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p44100618"><a name="p44100618"></a><a name="p44100618"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p15380277"><a name="p15380277"></a><a name="p15380277"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row4204769"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p5042045"><a name="p5042045"></a><a name="p5042045"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p5752468"><a name="p5752468"></a><a name="p5752468"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p63296784"><a name="p63296784"></a><a name="p63296784"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p26765913"><a name="p26765913"></a><a name="p26765913"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section63086694"></a>

无

## 响应消息<a name="section9748615"></a>

**表 3**  参数说明

<a name="table35112378"></a>
<table><thead align="left"><tr id="row10083439"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p11452202"><a name="p11452202"></a><a name="p11452202"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p55213174"><a name="p55213174"></a><a name="p55213174"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p43082106"><a name="p43082106"></a><a name="p43082106"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row67098591"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p66276813"><a name="p66276813"></a><a name="p66276813"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66821611"><a name="p66821611"></a><a name="p66821611"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p43841377"><a name="p43841377"></a><a name="p43841377"></a>符合条件的API的总数</p>
</td>
</tr>
<tr id="row59028077"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16544923"><a name="p16544923"></a><a name="p16544923"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p65070390"><a name="p65070390"></a><a name="p65070390"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36210213"><a name="p36210213"></a><a name="p36210213"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="row57456464"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p23461977"><a name="p23461977"></a><a name="p23461977"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p21371946"><a name="p21371946"></a><a name="p21371946"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53406060"><a name="p53406060"></a><a name="p53406060"></a>本次返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table10892494"></a>
<table><thead align="left"><tr id="row42715000"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p37363013"><a name="p37363013"></a><a name="p37363013"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p6505202"><a name="p6505202"></a><a name="p6505202"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p57159335"><a name="p57159335"></a><a name="p57159335"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row66503437"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18069323"><a name="p18069323"></a><a name="p18069323"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p54329098"><a name="p54329098"></a><a name="p54329098"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38580850"><a name="p38580850"></a><a name="p38580850"></a>API编号</p>
</td>
</tr>
<tr id="row11683332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6825851"><a name="p6825851"></a><a name="p6825851"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16023087"><a name="p16023087"></a><a name="p16023087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p22801671"><a name="p22801671"></a><a name="p22801671"></a>API名称</p>
</td>
</tr>
<tr id="row3888452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p46529230"><a name="p46529230"></a><a name="p46529230"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10771313"><a name="p10771313"></a><a name="p10771313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61140"><a name="p61140"></a><a name="p61140"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row550261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44571163"><a name="p44571163"></a><a name="p44571163"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p53494487"><a name="p53494487"></a><a name="p53494487"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38086158"><a name="p38086158"></a><a name="p38086158"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row43301387"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17751458"><a name="p17751458"></a><a name="p17751458"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p28581985"><a name="p28581985"></a><a name="p28581985"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p33439473"><a name="p33439473"></a><a name="p33439473"></a>API描述</p>
</td>
</tr>
<tr id="row63537654"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p46276336"><a name="p46276336"></a><a name="p46276336"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57395755"><a name="p57395755"></a><a name="p57395755"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18544591"><a name="p18544591"></a><a name="p18544591"></a>发布的环境名</p>
</td>
</tr>
<tr id="row32683591"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p30125210"><a name="p30125210"></a><a name="p30125210"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24222954"><a name="p24222954"></a><a name="p24222954"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15902238"><a name="p15902238"></a><a name="p15902238"></a>发布的环境id</p>
</td>
</tr>
<tr id="row8902417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p50007191"><a name="p50007191"></a><a name="p50007191"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24050677"><a name="p24050677"></a><a name="p24050677"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1947860"><a name="p1947860"></a><a name="p1947860"></a>发布记录的编号</p>
</td>
</tr>
<tr id="row18713323316"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p587733133318"><a name="p587733133318"></a><a name="p587733133318"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1588163353318"><a name="p1588163353318"></a><a name="p1588163353318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p188133343318"><a name="p188133343318"></a><a name="p188133343318"></a>API的认证方式</p>
</td>
</tr>
<tr id="row1130901133416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12309171103416"><a name="p12309171103416"></a><a name="p12309171103416"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p133092011193413"><a name="p133092011193413"></a><a name="p133092011193413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p113092118346"><a name="p113092118346"></a><a name="p113092118346"></a>API的访问地址</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 1,
	"size": 1,
	"apis": [{
		"id": "5bbc47e2-95b0-4a56-904e-a3cdc422f8e9",
		"name": "查询分组列表",
		"remark": "查询分组列表",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"group_name": "api_group_001",
		"run_env_name": "RELEASE",
		"run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"publish_id": "65e6fe53-1ac3-4481-ba36-9f0bc6f22057",
		"auth_type": "APP",
		"req_uri": "/test"
	}]
}
```

## 状态码<a name="section30909341"></a>

**表 5**  返回消息说明

<a name="table54370672"></a>
<table><thead align="left"><tr id="row45779426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p17146043"><a name="p17146043"></a><a name="p17146043"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p46652212"><a name="p46652212"></a><a name="p46652212"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20732789"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1634343"><a name="p1634343"></a><a name="p1634343"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p65272945"><a name="p65272945"></a><a name="p65272945"></a>OK</p>
</td>
</tr>
<tr id="row50585599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3792865"><a name="p3792865"></a><a name="p3792865"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p38786672"><a name="p38786672"></a><a name="p38786672"></a>Bad Request</p>
</td>
</tr>
<tr id="row13535731"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22652464"><a name="p22652464"></a><a name="p22652464"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p22910285"><a name="p22910285"></a><a name="p22910285"></a>Unauthorized</p>
</td>
</tr>
<tr id="row4865975"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p58599688"><a name="p58599688"></a><a name="p58599688"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p48954253"><a name="p48954253"></a><a name="p48954253"></a>Forbidden</p>
</td>
</tr>
<tr id="row37935094"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p52843813"><a name="p52843813"></a><a name="p52843813"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p52490493"><a name="p52490493"></a><a name="p52490493"></a>Not Found</p>
</td>
</tr>
<tr id="row2652391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p13517134"><a name="p13517134"></a><a name="p13517134"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

