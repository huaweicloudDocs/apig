# 上架API分组<a name="apig-phapi-180713102"></a>

## 功能介绍<a name="section30801397"></a>

用户可以在API网关创建API，并将这些API开放到华为云市场上，供其他用户购买调用，产生经济价值和利益。只有公有且认证方式为APP认证，并且已经发布到RELEASE环境的API才可以在华为云市场上进行售卖，售卖的方式以API分组为单位，当用户购买了一个API分组之后，则该分组下的所有公有且认证方式为APP认证，并且已发布的API均可被该用户调用，直至购买的调用次数用尽为止。

当API分组通过云市场的上架审核流程后，云市场会调用API网关的上架接口通知API网关将该分组置于上架状态。当API分组完成上架后，其他租户便可在云市场上看见该分组并进行购买。

## URI<a name="section8777121"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table23079429"></a>
<table><thead align="left"><tr id="row2213484"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p45074490"><a name="p45074490"></a><a name="p45074490"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p27155040"><a name="p27155040"></a><a name="p27155040"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row52074631"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p57295574"><a name="p57295574"></a><a name="p57295574"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p10429942"><a name="p10429942"></a><a name="p10429942"></a>/v1/{project_id}/apigw/instances/{instance_id}/market/api-groups/onsell/{group_id}</p>
</td>
</tr>
</tbody>
</table>

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

<a name="table26760620"></a>
<table><thead align="left"><tr id="row21251861"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p43679219"><a name="p43679219"></a><a name="p43679219"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p48355861"><a name="p48355861"></a><a name="p48355861"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p24510692"><a name="p24510692"></a><a name="p24510692"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p39209031"><a name="p39209031"></a><a name="p39209031"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1196814550212"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row19599175410210"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row21814951"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p22180587"><a name="p22180587"></a><a name="p22180587"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p51797116"><a name="p51797116"></a><a name="p51797116"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p34816833"><a name="p34816833"></a><a name="p34816833"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p1591202"><a name="p1591202"></a><a name="p1591202"></a>将要上架到云市场的API分组编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section11885230"></a>

**表 4**  参数说明

<a name="table61778569"></a>
<table><thead align="left"><tr id="row62401262"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.5.1.1"><p id="p21337475"><a name="p21337475"></a><a name="p21337475"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.2"><p id="p50613900"><a name="p50613900"></a><a name="p50613900"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.3"><p id="p6085234"><a name="p6085234"></a><a name="p6085234"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.53%" id="mcps1.2.5.1.4"><p id="p23141916"><a name="p23141916"></a><a name="p23141916"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row62555890"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="p33862366"><a name="p33862366"></a><a name="p33862366"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.2 "><p id="p58497093"><a name="p58497093"></a><a name="p58497093"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.3 "><p id="p40644113"><a name="p40644113"></a><a name="p40644113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p3838890"><a name="p3838890"></a><a name="p3838890"></a>云市场给上架的API分组分配的访问域名</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"url_domain": "test.market.example.com"
}
```

## 响应消息<a name="section23179608"></a>

**表 5**  参数说明

<a name="table52907232"></a>
<table><thead align="left"><tr id="row17426675"><th class="cellrowborder" valign="top" width="20.200000000000003%" id="mcps1.2.4.1.1"><p id="p2274575"><a name="p2274575"></a><a name="p2274575"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="p50022883"><a name="p50022883"></a><a name="p50022883"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.62%" id="mcps1.2.4.1.3"><p id="p25321752"><a name="p25321752"></a><a name="p25321752"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row37796054"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p41581508"><a name="p41581508"></a><a name="p41581508"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p12658954"><a name="p12658954"></a><a name="p12658954"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p18742353"><a name="p18742353"></a><a name="p18742353"></a>API分组编号</p>
</td>
</tr>
<tr id="row40076231"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p24949254"><a name="p24949254"></a><a name="p24949254"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p7623682"><a name="p7623682"></a><a name="p7623682"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p13538466"><a name="p13538466"></a><a name="p13538466"></a>API分组名称</p>
</td>
</tr>
<tr id="row4538821"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p32100207"><a name="p32100207"></a><a name="p32100207"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p49979994"><a name="p49979994"></a><a name="p49979994"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p21847726"><a name="p21847726"></a><a name="p21847726"></a>API分组描述</p>
</td>
</tr>
<tr id="row22191521"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p52682785"><a name="p52682785"></a><a name="p52682785"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p39447173"><a name="p39447173"></a><a name="p39447173"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p41104438"><a name="p41104438"></a><a name="p41104438"></a>API分组最近更新时间</p>
</td>
</tr>
<tr id="row34582004"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p49678979"><a name="p49678979"></a><a name="p49678979"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p64574395"><a name="p64574395"></a><a name="p64574395"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p63143491"><a name="p63143491"></a><a name="p63143491"></a>云市场分配给该API分组的访问域名</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "73c58022-f20d-495a-a188-85d718647f09",
	"name": "api_group_001",
	"remark": "分组001",
	"update_time": "2017-12-28T11:57:27Z",
	"url_domain": "test.market.example.com"
}
```

## 状态码<a name="section39858214"></a>

**表 6**  返回消息说明

<a name="table34374863"></a>
<table><thead align="left"><tr id="row26616228"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p8430829"><a name="p8430829"></a><a name="p8430829"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p11808510"><a name="p11808510"></a><a name="p11808510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16965248"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p32007834"><a name="p32007834"></a><a name="p32007834"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p42497781"><a name="p42497781"></a><a name="p42497781"></a>Created</p>
</td>
</tr>
<tr id="row46935714"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p43696513"><a name="p43696513"></a><a name="p43696513"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p49756660"><a name="p49756660"></a><a name="p49756660"></a>Bad Request</p>
</td>
</tr>
<tr id="row45156761"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p33819014"><a name="p33819014"></a><a name="p33819014"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p54985595"><a name="p54985595"></a><a name="p54985595"></a>Unauthorized</p>
</td>
</tr>
<tr id="row25108313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20507438"><a name="p20507438"></a><a name="p20507438"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50489759"><a name="p50489759"></a><a name="p50489759"></a>Forbidden</p>
</td>
</tr>
<tr id="row51754654"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p31377478"><a name="p31377478"></a><a name="p31377478"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p58547774"><a name="p58547774"></a><a name="p58547774"></a>Not Found</p>
</td>
</tr>
<tr id="row57167919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p89891"><a name="p89891"></a><a name="p89891"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

