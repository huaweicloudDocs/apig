# 查看流控策略绑定的API列表<a name="apig-zh-api-180713073"></a>

## 功能介绍<a name="section55871885"></a>

查询某个流控策略上已经绑定的API列表。

## URI<a name="section33084918"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table15569850"></a>
<table><thead align="left"><tr id="row1181310"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p28577256"><a name="p28577256"></a><a name="p28577256"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p33056382"><a name="p33056382"></a><a name="p33056382"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row60321322"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p54188881"><a name="p54188881"></a><a name="p54188881"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p27223261"><a name="p27223261"></a><a name="p27223261"></a>/v1.0/apigw/throttle-bindings/binded-apis[?page_size, page_no, throttle_id, env_id, group_id, api_id,api_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：group\_id、env\_id、throttle\_id、api\_id、api\_name、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table47773025"></a>
<table><thead align="left"><tr id="row16397648"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p53141081"><a name="p53141081"></a><a name="p53141081"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p9460266"><a name="p9460266"></a><a name="p9460266"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p28084076"><a name="p28084076"></a><a name="p28084076"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p60217670"><a name="p60217670"></a><a name="p60217670"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row45793121"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p18255333"><a name="p18255333"></a><a name="p18255333"></a>throttle_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p2286968"><a name="p2286968"></a><a name="p2286968"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p51026757"><a name="p51026757"></a><a name="p51026757"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p39526642"><a name="p39526642"></a><a name="p39526642"></a>流控策略编号</p>
</td>
</tr>
<tr id="row20195460"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p25219557"><a name="p25219557"></a><a name="p25219557"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29518202"><a name="p29518202"></a><a name="p29518202"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p42164139"><a name="p42164139"></a><a name="p42164139"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p59852130"><a name="p59852130"></a><a name="p59852130"></a>环境的ID</p>
</td>
</tr>
<tr id="row1798258"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p11441194"><a name="p11441194"></a><a name="p11441194"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p54321498"><a name="p54321498"></a><a name="p54321498"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p37965227"><a name="p37965227"></a><a name="p37965227"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p55284548"><a name="p55284548"></a><a name="p55284548"></a>API分组编号</p>
</td>
</tr>
<tr id="row27798892"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p37117765"><a name="p37117765"></a><a name="p37117765"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p53748987"><a name="p53748987"></a><a name="p53748987"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p58700661"><a name="p58700661"></a><a name="p58700661"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p57133083"><a name="p57133083"></a><a name="p57133083"></a>API编号</p>
</td>
</tr>
<tr id="row44435707"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p42522511"><a name="p42522511"></a><a name="p42522511"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p21771396"><a name="p21771396"></a><a name="p21771396"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p18652674"><a name="p18652674"></a><a name="p18652674"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p34471600"><a name="p34471600"></a><a name="p34471600"></a>API名称</p>
</td>
</tr>
<tr id="row41808944"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p31081322"><a name="p31081322"></a><a name="p31081322"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p34559144"><a name="p34559144"></a><a name="p34559144"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p47827283"><a name="p47827283"></a><a name="p47827283"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p48804690"><a name="p48804690"></a><a name="p48804690"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row36589029"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p10921342"><a name="p10921342"></a><a name="p10921342"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p12213471"><a name="p12213471"></a><a name="p12213471"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p49767089"><a name="p49767089"></a><a name="p49767089"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p4602395"><a name="p4602395"></a><a name="p4602395"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section29328814"></a>

无

## 响应消息<a name="section26823765"></a>

**表 3**  参数说明

<a name="table19243893"></a>
<table><thead align="left"><tr id="row5561953"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p47865073"><a name="p47865073"></a><a name="p47865073"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p51865722"><a name="p51865722"></a><a name="p51865722"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p40373923"><a name="p40373923"></a><a name="p40373923"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49062292"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14622710"><a name="p14622710"></a><a name="p14622710"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p43588848"><a name="p43588848"></a><a name="p43588848"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p41035819"><a name="p41035819"></a><a name="p41035819"></a>满足条件的API总数</p>
</td>
</tr>
<tr id="row33778056"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51668039"><a name="p51668039"></a><a name="p51668039"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24361626"><a name="p24361626"></a><a name="p24361626"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27134698"><a name="p27134698"></a><a name="p27134698"></a>本次返回的API列表长度</p>
</td>
</tr>
<tr id="row42885692"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51189009"><a name="p51189009"></a><a name="p51189009"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p52669079"><a name="p52669079"></a><a name="p52669079"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38337013"><a name="p38337013"></a><a name="p38337013"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table9488805"></a>
<table><thead align="left"><tr id="row13375108"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p9641973"><a name="p9641973"></a><a name="p9641973"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p42802350"><a name="p42802350"></a><a name="p42802350"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p44438360"><a name="p44438360"></a><a name="p44438360"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row42737435"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39180190"><a name="p39180190"></a><a name="p39180190"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19478793"><a name="p19478793"></a><a name="p19478793"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p34278405"><a name="p34278405"></a><a name="p34278405"></a>API编号</p>
</td>
</tr>
<tr id="row40070193"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24460168"><a name="p24460168"></a><a name="p24460168"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35116612"><a name="p35116612"></a><a name="p35116612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p25873357"><a name="p25873357"></a><a name="p25873357"></a>API名称</p>
</td>
</tr>
<tr id="row31533626"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4086880"><a name="p4086880"></a><a name="p4086880"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62601863"><a name="p62601863"></a><a name="p62601863"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p37586134"><a name="p37586134"></a><a name="p37586134"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row2730893"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19875756"><a name="p19875756"></a><a name="p19875756"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66432392"><a name="p66432392"></a><a name="p66432392"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12314632"><a name="p12314632"></a><a name="p12314632"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row8162325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57168612"><a name="p57168612"></a><a name="p57168612"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p145991"><a name="p145991"></a><a name="p145991"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11825319"><a name="p11825319"></a><a name="p11825319"></a>API类型</p>
</td>
</tr>
<tr id="row32119029"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51504569"><a name="p51504569"></a><a name="p51504569"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11120524"><a name="p11120524"></a><a name="p11120524"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p28347289"><a name="p28347289"></a><a name="p28347289"></a>API描述</p>
</td>
</tr>
<tr id="row935583"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8673438"><a name="p8673438"></a><a name="p8673438"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31459910"><a name="p31459910"></a><a name="p31459910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65224766"><a name="p65224766"></a><a name="p65224766"></a>发布的环境名</p>
</td>
</tr>
<tr id="row50151983"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p35778851"><a name="p35778851"></a><a name="p35778851"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12405819"><a name="p12405819"></a><a name="p12405819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65347296"><a name="p65347296"></a><a name="p65347296"></a>发布的环境编号</p>
</td>
</tr>
<tr id="row51254754"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57994437"><a name="p57994437"></a><a name="p57994437"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p67037800"><a name="p67037800"></a><a name="p67037800"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61352691"><a name="p61352691"></a><a name="p61352691"></a>发布记录的编号</p>
</td>
</tr>
<tr id="row15303311"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p31608715"><a name="p31608715"></a><a name="p31608715"></a>throttle_apply_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10169090"><a name="p10169090"></a><a name="p10169090"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18389982"><a name="p18389982"></a><a name="p18389982"></a>与流控策略的绑定关系编号</p>
</td>
</tr>
<tr id="row31292118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51633604"><a name="p51633604"></a><a name="p51633604"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p21572362"><a name="p21572362"></a><a name="p21572362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2530897"><a name="p2530897"></a><a name="p2530897"></a>绑定的流控策略名称</p>
</td>
</tr>
<tr id="row128795"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10432412"><a name="p10432412"></a><a name="p10432412"></a>apply_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12994925195811"><a name="p12994925195811"></a><a name="p12994925195811"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p391693316585"><a name="p391693316585"></a><a name="p391693316585"></a>与已绑定的流控策略的绑定时间</p>
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
		"id": "5bbc47e2-95b0-4a56-904e-a3cdc422f8e9",
		"name": "查询分组列表",
		"type": 1,
		"remark": "查询分组列表",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"group_name": "api_group_001",
		"run_env_name": "RELEASE",
		"run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"publish_id": "65e6fe53-1ac3-4481-ba36-9f0bc6f22057",
		"throttle_apply_id": "90f05978-06a3-4096-8bea-b5e2fa12b843",
		"throttle_name": "throttle1",
		"apply_time": "2017-12-29T03:01:11.138456Z"
	},
	{
		"id": "6632a062-9dcf-4f18-9646-3cabb925a290",
		"name": "查询API列表",
		"type": 1,
		"remark": "查询API列表",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"group_name": "api_group_001",
		"run_env_name": "RELEASE",
		"run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"publish_id": "374a6d5a-20c7-4ea1-82e1-19fce4556956",
		"throttle_apply_id": "507c6a9f-8322-4dc2-8ba5-b4d74e3690d3",
		"throttle_name": "throttle1",
		"apply_time": "2017-12-29T03:01:11.138456Z"
	}]
}
```

## 状态码<a name="section62632741"></a>

**表 5**  返回消息说明

<a name="table64438490"></a>
<table><thead align="left"><tr id="row22918957"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p44496209"><a name="p44496209"></a><a name="p44496209"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p47423170"><a name="p47423170"></a><a name="p47423170"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16071527"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p26725288"><a name="p26725288"></a><a name="p26725288"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p17264751"><a name="p17264751"></a><a name="p17264751"></a>OK</p>
</td>
</tr>
<tr id="row21165031"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p36645935"><a name="p36645935"></a><a name="p36645935"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p15530735"><a name="p15530735"></a><a name="p15530735"></a>Bad Request</p>
</td>
</tr>
<tr id="row5558892"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p47617108"><a name="p47617108"></a><a name="p47617108"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p31780553"><a name="p31780553"></a><a name="p31780553"></a>Unauthorized</p>
</td>
</tr>
<tr id="row17589523"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p15465286"><a name="p15465286"></a><a name="p15465286"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p44728633"><a name="p44728633"></a><a name="p44728633"></a>Forbidden</p>
</td>
</tr>
<tr id="row67013378"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p59374520"><a name="p59374520"></a><a name="p59374520"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p44606852"><a name="p44606852"></a><a name="p44606852"></a>Not Found</p>
</td>
</tr>
<tr id="row65917348"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p37705001"><a name="p37705001"></a><a name="p37705001"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p34206263"><a name="p34206263"></a><a name="p34206263"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

