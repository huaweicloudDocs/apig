# 查看签名密钥未绑定的API列表<a name="apig-zh-api-180713141"></a>

## 功能介绍<a name="section51759191"></a>

查询所有未绑定到该签名密钥上的API列表。需要API已经发布，未发布的API不予展示。

## URI<a name="section63179535"></a>

HTTP/HTTPS请求方法以及URI如表3-73所示。

**表 1**  HTTP/HTTPS请求方法以及

<a name="table42511059"></a>
<table><thead align="left"><tr id="row55091690"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p33241899"><a name="p33241899"></a><a name="p33241899"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p8239264"><a name="p8239264"></a><a name="p8239264"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row63400625"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p35177032"><a name="p35177032"></a><a name="p35177032"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p30767306"><a name="p30767306"></a><a name="p30767306"></a>/v1.0/apigw/sign-bindings/unbinded-apis[?page_size, page_no, sign_id ,env_id, api_id, api_name, group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：sign\_id、env\_id、api\_id、api\_name、group\_id、page\_size、page\_no。  

## 请求消息<a name="section31744903"></a>

**表 2**  参数说明

<a name="table5666522"></a>
<table><thead align="left"><tr id="row16340827"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p48538593"><a name="p48538593"></a><a name="p48538593"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p39311997"><a name="p39311997"></a><a name="p39311997"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p30155156"><a name="p30155156"></a><a name="p30155156"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p26648592"><a name="p26648592"></a><a name="p26648592"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row11052377"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p22827350"><a name="p22827350"></a><a name="p22827350"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p37076080"><a name="p37076080"></a><a name="p37076080"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p50372494"><a name="p50372494"></a><a name="p50372494"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p53640217"><a name="p53640217"></a><a name="p53640217"></a>安全密钥编号</p>
</td>
</tr>
<tr id="row12999906"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p46359483"><a name="p46359483"></a><a name="p46359483"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p64130612"><a name="p64130612"></a><a name="p64130612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p27197045"><a name="p27197045"></a><a name="p27197045"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p55477031"><a name="p55477031"></a><a name="p55477031"></a>环境编号</p>
</td>
</tr>
<tr id="row29531233"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p43219711"><a name="p43219711"></a><a name="p43219711"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p11135713"><a name="p11135713"></a><a name="p11135713"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p29577584"><a name="p29577584"></a><a name="p29577584"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p46974099"><a name="p46974099"></a><a name="p46974099"></a>API编号</p>
</td>
</tr>
<tr id="row20113712"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p18597965"><a name="p18597965"></a><a name="p18597965"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p30040178"><a name="p30040178"></a><a name="p30040178"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p17335368"><a name="p17335368"></a><a name="p17335368"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p61987574"><a name="p61987574"></a><a name="p61987574"></a>API名称</p>
</td>
</tr>
<tr id="row21017262"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p24676693"><a name="p24676693"></a><a name="p24676693"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p52655079"><a name="p52655079"></a><a name="p52655079"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p37203022"><a name="p37203022"></a><a name="p37203022"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p60654834"><a name="p60654834"></a><a name="p60654834"></a>API分组编号</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section21200323"></a>

**表 3**  参数说明

<a name="table34366064"></a>
<table><thead align="left"><tr id="row59541114"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p58100907"><a name="p58100907"></a><a name="p58100907"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="p8553058"><a name="p8553058"></a><a name="p8553058"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p21709060"><a name="p21709060"></a><a name="p21709060"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13603451"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p28137775"><a name="p28137775"></a><a name="p28137775"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p64567303"><a name="p64567303"></a><a name="p64567303"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p62569068"><a name="p62569068"></a><a name="p62569068"></a>满足查询条件的API的总个数</p>
</td>
</tr>
<tr id="row26250702"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p45932145"><a name="p45932145"></a><a name="p45932145"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p29516244"><a name="p29516244"></a><a name="p29516244"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p42005535"><a name="p42005535"></a><a name="p42005535"></a>本次查询返回的API列表长度</p>
</td>
</tr>
<tr id="row42505499"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p20393431"><a name="p20393431"></a><a name="p20393431"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p41255182"><a name="p41255182"></a><a name="p41255182"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p53335466"><a name="p53335466"></a><a name="p53335466"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table10257154"></a>
<table><thead align="left"><tr id="row50958760"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p34018899"><a name="p34018899"></a><a name="p34018899"></a><strong id="b37734636"><a name="b37734636"></a><a name="b37734636"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="p36606693"><a name="p36606693"></a><a name="p36606693"></a><strong id="b61024782"><a name="b61024782"></a><a name="b61024782"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p44060270"><a name="p44060270"></a><a name="p44060270"></a><strong id="b60998111"><a name="b60998111"></a><a name="b60998111"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row41899953"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p38453019"><a name="p38453019"></a><a name="p38453019"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p27686854"><a name="p27686854"></a><a name="p27686854"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p28042714"><a name="p28042714"></a><a name="p28042714"></a>API编号</p>
</td>
</tr>
<tr id="row51057834"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p42043885"><a name="p42043885"></a><a name="p42043885"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p50111533"><a name="p50111533"></a><a name="p50111533"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p32502353"><a name="p32502353"></a><a name="p32502353"></a>API名称</p>
</td>
</tr>
<tr id="row51031407"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p39903265"><a name="p39903265"></a><a name="p39903265"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p10939048"><a name="p10939048"></a><a name="p10939048"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p13647724"><a name="p13647724"></a><a name="p13647724"></a>API类型</p>
</td>
</tr>
<tr id="row61320148"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p876124"><a name="p876124"></a><a name="p876124"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p3857204"><a name="p3857204"></a><a name="p3857204"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p43998084"><a name="p43998084"></a><a name="p43998084"></a>API描述</p>
</td>
</tr>
<tr id="row40388913"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p50276488"><a name="p50276488"></a><a name="p50276488"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p45863748"><a name="p45863748"></a><a name="p45863748"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p23976141"><a name="p23976141"></a><a name="p23976141"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row14458682"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p30302560"><a name="p30302560"></a><a name="p30302560"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p38588295"><a name="p38588295"></a><a name="p38588295"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p38644182"><a name="p38644182"></a><a name="p38644182"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row12253325"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p52995244"><a name="p52995244"></a><a name="p52995244"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p64756360"><a name="p64756360"></a><a name="p64756360"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p10773768"><a name="p10773768"></a><a name="p10773768"></a>发布的环境名</p>
</td>
</tr>
<tr id="row29855049"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p2339899"><a name="p2339899"></a><a name="p2339899"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p55314117"><a name="p55314117"></a><a name="p55314117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p51258512"><a name="p51258512"></a><a name="p51258512"></a>发布的环境id</p>
</td>
</tr>
<tr id="row58673429"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p54927332"><a name="p54927332"></a><a name="p54927332"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p19928903"><a name="p19928903"></a><a name="p19928903"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p3628455"><a name="p3628455"></a><a name="p3628455"></a>API的发布记录编号</p>
</td>
</tr>
<tr id="row8616217"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p26824986"><a name="p26824986"></a><a name="p26824986"></a>signature_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p25340259"><a name="p25340259"></a><a name="p25340259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p39295133"><a name="p39295133"></a><a name="p39295133"></a>已绑定的签名密钥名称</p>
</td>
</tr>
<tr id="row194436159307"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p124441715143014"><a name="p124441715143014"></a><a name="p124441715143014"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p1644461519309"><a name="p1644461519309"></a><a name="p1644461519309"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p18444315103014"><a name="p18444315103014"></a><a name="p18444315103014"></a>API的认证方式</p>
</td>
</tr>
<tr id="row62593129319"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1925910128315"><a name="p1925910128315"></a><a name="p1925910128315"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p15259161219319"><a name="p15259161219319"></a><a name="p15259161219319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p1226051212318"><a name="p1226051212318"></a><a name="p1226051212318"></a>API的访问地址</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"apis": [{
		"name": "bbb",
		"type": 1,
		"group_id": "7ccc0b94-eb5a-48e6-8554-6d0105a540e2",
		"id": "3c6769c6-ec61-4b45-b478-c60310dbaa1b",
		"group_name": "asd",
		"run_env_name": "das",
		"run_env_id": "1fdcb2e4-f90a-4159-817d-98c9b8e8b215",
		"publish_id": "6dff16c4-813f-486a-bba4-fdad45a55a70",
		"auth_type": "NONE",
		"req_uri": "/test"
	},
	{
		"name": "aaa",
		"type": 1,
		"group_id": "7ccc0b94-eb5a-48e6-8554-6d0105a540e2",
		"id": "d85c502a-f916-47e8-bba0-50537a2d1af2",
		"group_name": "asd",
		"run_env_name": "das",
		"run_env_id": "1fdcb2e4-f90a-4159-817d-98c9b8e8b215",
		"publish_id": "dec83400-a0c6-4ea6-abfd-5bf237292f4d",
		"auth_type": "NONE",
		"req_uri": "/test"
	}]
}
```

## 状态码<a name="section17268672"></a>

**表 5**  返回消息说明

<a name="table59741839"></a>
<table><thead align="left"><tr id="row51360638"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p66570984"><a name="p66570984"></a><a name="p66570984"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p10538870"><a name="p10538870"></a><a name="p10538870"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row32426065"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9265629"><a name="p9265629"></a><a name="p9265629"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p12318518"><a name="p12318518"></a><a name="p12318518"></a>OK</p>
</td>
</tr>
<tr id="row43757803"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p54721121"><a name="p54721121"></a><a name="p54721121"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p3225816"><a name="p3225816"></a><a name="p3225816"></a>Bad Request</p>
</td>
</tr>
<tr id="row29032347"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p2809910"><a name="p2809910"></a><a name="p2809910"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p26276133"><a name="p26276133"></a><a name="p26276133"></a>Unauthorized</p>
</td>
</tr>
<tr id="row35158608"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p29274969"><a name="p29274969"></a><a name="p29274969"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p22462250"><a name="p22462250"></a><a name="p22462250"></a>Forbidden</p>
</td>
</tr>
<tr id="row833661"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p417742"><a name="p417742"></a><a name="p417742"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p15296380"><a name="p15296380"></a><a name="p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="row36099169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p38351589"><a name="p38351589"></a><a name="p38351589"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

