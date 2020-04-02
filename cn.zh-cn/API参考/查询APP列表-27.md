# 查询APP列表<a name="apig-phapi-180713042"></a>

## 功能介绍<a name="section48433431"></a>

查询APP列表。

## URI<a name="section33247697"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table33538507"></a>
<table><thead align="left"><tr id="row26439774"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p61246963"><a name="p61246963"></a><a name="p61246963"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p62056956"><a name="p62056956"></a><a name="p62056956"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row60557538"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6213516"><a name="p6213516"></a><a name="p6213516"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p33532770"><a name="p33532770"></a><a name="p33532770"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps[?page_size, page_no, id, name, app_key, creator]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：id、name、app\_key、creator、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table29558883"></a>
<table><thead align="left"><tr id="row37253980"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p64782395"><a name="p64782395"></a><a name="p64782395"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.32%" id="mcps1.2.5.1.2"><p id="p12882667"><a name="p12882667"></a><a name="p12882667"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.86%" id="mcps1.2.5.1.3"><p id="p36863124"><a name="p36863124"></a><a name="p36863124"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.82%" id="mcps1.2.5.1.4"><p id="p33123037"><a name="p33123037"></a><a name="p33123037"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2037411811464"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row1215121874618"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row65720302"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p21744240"><a name="p21744240"></a><a name="p21744240"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p16453002"><a name="p16453002"></a><a name="p16453002"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p57624805"><a name="p57624805"></a><a name="p57624805"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p37097641"><a name="p37097641"></a><a name="p37097641"></a>编号</p>
</td>
</tr>
<tr id="row65443313"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p66416996"><a name="p66416996"></a><a name="p66416996"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p11067604"><a name="p11067604"></a><a name="p11067604"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p24060712"><a name="p24060712"></a><a name="p24060712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p2760649"><a name="p2760649"></a><a name="p2760649"></a>名称</p>
</td>
</tr>
<tr id="row1007519"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p14500243"><a name="p14500243"></a><a name="p14500243"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p33669035"><a name="p33669035"></a><a name="p33669035"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p42837328"><a name="p42837328"></a><a name="p42837328"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p47271529"><a name="p47271529"></a><a name="p47271529"></a>状态</p>
</td>
</tr>
<tr id="row22790581"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p34097752"><a name="p34097752"></a><a name="p34097752"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p10454499"><a name="p10454499"></a><a name="p10454499"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p41508095"><a name="p41508095"></a><a name="p41508095"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p6712531"><a name="p6712531"></a><a name="p6712531"></a>APP的KEY</p>
</td>
</tr>
<tr id="row2838323152510"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p148381123152516"><a name="p148381123152516"></a><a name="p148381123152516"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p10838223112516"><a name="p10838223112516"></a><a name="p10838223112516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p128381023202515"><a name="p128381023202515"></a><a name="p128381023202515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p78385238252"><a name="p78385238252"></a><a name="p78385238252"></a>APP的创建者，取值如下：</p>
<a name="ul1126756132511"></a><a name="ul1126756132511"></a><ul id="ul1126756132511"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="row60412786"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p61597518"><a name="p61597518"></a><a name="p61597518"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p23343095"><a name="p23343095"></a><a name="p23343095"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p11742548"><a name="p11742548"></a><a name="p11742548"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p11622350"><a name="p11622350"></a><a name="p11622350"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row37492289"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p16976560"><a name="p16976560"></a><a name="p16976560"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p32924144"><a name="p32924144"></a><a name="p32924144"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p49610025"><a name="p49610025"></a><a name="p49610025"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p58989058"><a name="p58989058"></a><a name="p58989058"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="row1797011282498"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p297092819498"><a name="p297092819498"></a><a name="p297092819498"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="p397092812491"><a name="p397092812491"></a><a name="p397092812491"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="p49701728194913"><a name="p49701728194913"></a><a name="p49701728194913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="p19970928194911"><a name="p19970928194911"></a><a name="p19970928194911"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section30793819"></a>

无

## 响应消息<a name="section11271404"></a>

**表 3**  参数说明

<a name="table23954455"></a>
<table><thead align="left"><tr id="row66752668"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p38257064"><a name="p38257064"></a><a name="p38257064"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p11814447"><a name="p11814447"></a><a name="p11814447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p17446171"><a name="p17446171"></a><a name="p17446171"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3853780"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p43720769"><a name="p43720769"></a><a name="p43720769"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51721419"><a name="p51721419"></a><a name="p51721419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p28685401"><a name="p28685401"></a><a name="p28685401"></a>符合条件的APP总数</p>
</td>
</tr>
<tr id="row56842021"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40801013"><a name="p40801013"></a><a name="p40801013"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16547774"><a name="p16547774"></a><a name="p16547774"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65301287"><a name="p65301287"></a><a name="p65301287"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="row50840671"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24453659"><a name="p24453659"></a><a name="p24453659"></a>apps</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34589388"><a name="p34589388"></a><a name="p34589388"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p50277082"><a name="p50277082"></a><a name="p50277082"></a>APP列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apps参数说明

<a name="table49840559"></a>
<table><thead align="left"><tr id="row181838"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p14728898"><a name="p14728898"></a><a name="p14728898"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p52190083"><a name="p52190083"></a><a name="p52190083"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p66647160"><a name="p66647160"></a><a name="p66647160"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row29710857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57769248"><a name="p57769248"></a><a name="p57769248"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48797474"><a name="p48797474"></a><a name="p48797474"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60281337"><a name="p60281337"></a><a name="p60281337"></a>编号</p>
</td>
</tr>
<tr id="row5661128"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55898233"><a name="p55898233"></a><a name="p55898233"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31463026"><a name="p31463026"></a><a name="p31463026"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65477212"><a name="p65477212"></a><a name="p65477212"></a>名称</p>
</td>
</tr>
<tr id="row52424003"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18485849"><a name="p18485849"></a><a name="p18485849"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20958771"><a name="p20958771"></a><a name="p20958771"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19938873"><a name="p19938873"></a><a name="p19938873"></a>状态</p>
</td>
</tr>
<tr id="row45232137"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39924477"><a name="p39924477"></a><a name="p39924477"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12657234"><a name="p12657234"></a><a name="p12657234"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18603056"><a name="p18603056"></a><a name="p18603056"></a>APP的key</p>
</td>
</tr>
<tr id="row33209777"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5637422"><a name="p5637422"></a><a name="p5637422"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p53978056"><a name="p53978056"></a><a name="p53978056"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10146406"><a name="p10146406"></a><a name="p10146406"></a>密钥</p>
</td>
</tr>
<tr id="row24208794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14755322"><a name="p14755322"></a><a name="p14755322"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p54330451"><a name="p54330451"></a><a name="p54330451"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38690380"><a name="p38690380"></a><a name="p38690380"></a>注册时间</p>
</td>
</tr>
<tr id="row12669100"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19564152"><a name="p19564152"></a><a name="p19564152"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p41192505"><a name="p41192505"></a><a name="p41192505"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48258647"><a name="p48258647"></a><a name="p48258647"></a>描述</p>
</td>
</tr>
<tr id="row31674644"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15509384"><a name="p15509384"></a><a name="p15509384"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48300555"><a name="p48300555"></a><a name="p48300555"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20030920"><a name="p20030920"></a><a name="p20030920"></a>更新时间</p>
</td>
</tr>
<tr id="row81831714928"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p111407484101"><a name="p111407484101"></a><a name="p111407484101"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p214013484105"><a name="p214013484105"></a><a name="p214013484105"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p214004841017"><a name="p214004841017"></a><a name="p214004841017"></a>APP的创建者，取值如下：</p>
<a name="ul101401948201015"></a><a name="ul101401948201015"></a><ul id="ul101401948201015"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="row16235953312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52361752033"><a name="p52361752033"></a><a name="p52361752033"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12236185032"><a name="p12236185032"></a><a name="p12236185032"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17236557312"><a name="p17236557312"></a><a name="p17236557312"></a>绑定的API数量</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"apps": [{
		"id": "98efd77d-10b5-4eca-8170-ed30a4a286a4",
		"name": "app_002",
		"status": 1,
		"app_key": "f627fbaa-2c8b-4f58-a690-f478f54d3fe2",
		"app_secret": "******",
		"remark": "第二个APP",
		"register_time": "2017-12-28T12:32:50Z",
		"update_time": "2017-12-28T12:32:50Z",
		"creator": "MARKET",
                "bind_num": 2
	},
	{
		"id": "14b399ac-967f-4115-bb62-c0346b4537e9",
		"name": "app_001",
		"status": 1,
		"app_key": "d49b1cbf-cc81-4a5f-b2a0-61b568e376eb",
		"app_secret": "******",
		"remark": "第一个APP",
		"register_time": "2017-12-28T12:26:54Z",
		"update_time": "2017-12-28T12:29:35.571Z",
		"creator": "USER",
                "bind_num": 2
	}]
}
```

## 状态码<a name="section8708918"></a>

**表 5**  返回消息说明

<a name="table10390965"></a>
<table><thead align="left"><tr id="row66877087"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p48334990"><a name="p48334990"></a><a name="p48334990"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p22820113"><a name="p22820113"></a><a name="p22820113"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row36489873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p2889717"><a name="p2889717"></a><a name="p2889717"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p32740518"><a name="p32740518"></a><a name="p32740518"></a>OK</p>
</td>
</tr>
<tr id="row26229206"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p44190948"><a name="p44190948"></a><a name="p44190948"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p22697075"><a name="p22697075"></a><a name="p22697075"></a>Bad Request</p>
</td>
</tr>
<tr id="row2947091"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p37387781"><a name="p37387781"></a><a name="p37387781"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p8511436"><a name="p8511436"></a><a name="p8511436"></a>Unauthorized</p>
</td>
</tr>
<tr id="row9494067"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p30821972"><a name="p30821972"></a><a name="p30821972"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13551805"><a name="p13551805"></a><a name="p13551805"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

