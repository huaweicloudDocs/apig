# 修改特殊设置<a name="ZH-CN_TOPIC_0000001082135193"></a>

## 功能介绍<a name="zh-cn_topic_0225568878_section27881611"></a>

修改某个流控策略下的某个特殊设置。

## URI<a name="zh-cn_topic_0225568878_section49607908"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568878_table56305912"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568878_row32051164"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568878_p46007462"><a name="zh-cn_topic_0225568878_p46007462"></a><a name="zh-cn_topic_0225568878_p46007462"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568878_p35616924"><a name="zh-cn_topic_0225568878_p35616924"></a><a name="zh-cn_topic_0225568878_p35616924"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568878_row66398632"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568878_p9580079"><a name="zh-cn_topic_0225568878_p9580079"></a><a name="zh-cn_topic_0225568878_p9580079"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568878_p37788955"><a name="zh-cn_topic_0225568878_p37788955"></a><a name="zh-cn_topic_0225568878_p37788955"></a>/v1/{project_id}/apigw/instances/{instance_id}/throttle-specials/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568878_table41006548"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568878_row54982740"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568878_p24416931"><a name="zh-cn_topic_0225568878_p24416931"></a><a name="zh-cn_topic_0225568878_p24416931"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568878_p31614383"><a name="zh-cn_topic_0225568878_p31614383"></a><a name="zh-cn_topic_0225568878_p31614383"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568878_p10628191"><a name="zh-cn_topic_0225568878_p10628191"></a><a name="zh-cn_topic_0225568878_p10628191"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568878_p55577115"><a name="zh-cn_topic_0225568878_p55577115"></a><a name="zh-cn_topic_0225568878_p55577115"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568878_row6729201914178"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568878_p55878963"><a name="zh-cn_topic_0225568878_p55878963"></a><a name="zh-cn_topic_0225568878_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568878_p29902160"><a name="zh-cn_topic_0225568878_p29902160"></a><a name="zh-cn_topic_0225568878_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568878_p6155914"><a name="zh-cn_topic_0225568878_p6155914"></a><a name="zh-cn_topic_0225568878_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568878_p28867016"><a name="zh-cn_topic_0225568878_p28867016"></a><a name="zh-cn_topic_0225568878_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row153171931718"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568878_p1780913159538"><a name="zh-cn_topic_0225568878_p1780913159538"></a><a name="zh-cn_topic_0225568878_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568878_p9809215115310"><a name="zh-cn_topic_0225568878_p9809215115310"></a><a name="zh-cn_topic_0225568878_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568878_p1280914152538"><a name="zh-cn_topic_0225568878_p1280914152538"></a><a name="zh-cn_topic_0225568878_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568878_p1880914157537"><a name="zh-cn_topic_0225568878_p1880914157537"></a><a name="zh-cn_topic_0225568878_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row5452492"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568878_p38998746"><a name="zh-cn_topic_0225568878_p38998746"></a><a name="zh-cn_topic_0225568878_p38998746"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568878_p4781868"><a name="zh-cn_topic_0225568878_p4781868"></a><a name="zh-cn_topic_0225568878_p4781868"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568878_p51787051"><a name="zh-cn_topic_0225568878_p51787051"></a><a name="zh-cn_topic_0225568878_p51787051"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568878_p34001598"><a name="zh-cn_topic_0225568878_p34001598"></a><a name="zh-cn_topic_0225568878_p34001598"></a>特殊配置的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568878_section43817996"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568878_table2666062"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568878_row20791817"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568878_p6415648"><a name="zh-cn_topic_0225568878_p6415648"></a><a name="zh-cn_topic_0225568878_p6415648"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568878_p49905442"><a name="zh-cn_topic_0225568878_p49905442"></a><a name="zh-cn_topic_0225568878_p49905442"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568878_p15809017"><a name="zh-cn_topic_0225568878_p15809017"></a><a name="zh-cn_topic_0225568878_p15809017"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568878_p5462029"><a name="zh-cn_topic_0225568878_p5462029"></a><a name="zh-cn_topic_0225568878_p5462029"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568878_row39771205"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568878_p242186"><a name="zh-cn_topic_0225568878_p242186"></a><a name="zh-cn_topic_0225568878_p242186"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568878_p19617091"><a name="zh-cn_topic_0225568878_p19617091"></a><a name="zh-cn_topic_0225568878_p19617091"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568878_p45480537"><a name="zh-cn_topic_0225568878_p45480537"></a><a name="zh-cn_topic_0225568878_p45480537"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568878_p60044851"><a name="zh-cn_topic_0225568878_p60044851"></a><a name="zh-cn_topic_0225568878_p60044851"></a>特殊对象在流控时间内能够调用API的最大次数限制</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"call_limits": 180
}
```

## 响应消息<a name="zh-cn_topic_0225568878_section59596819"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568878_table22899263"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568878_row37572135"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568878_p23444129"><a name="zh-cn_topic_0225568878_p23444129"></a><a name="zh-cn_topic_0225568878_p23444129"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568878_p19926324"><a name="zh-cn_topic_0225568878_p19926324"></a><a name="zh-cn_topic_0225568878_p19926324"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568878_p3419527"><a name="zh-cn_topic_0225568878_p3419527"></a><a name="zh-cn_topic_0225568878_p3419527"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568878_row8546242"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p21157006"><a name="zh-cn_topic_0225568878_p21157006"></a><a name="zh-cn_topic_0225568878_p21157006"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p35995922"><a name="zh-cn_topic_0225568878_p35995922"></a><a name="zh-cn_topic_0225568878_p35995922"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p29988599"><a name="zh-cn_topic_0225568878_p29988599"></a><a name="zh-cn_topic_0225568878_p29988599"></a>特殊配置的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row1461941"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p51308430"><a name="zh-cn_topic_0225568878_p51308430"></a><a name="zh-cn_topic_0225568878_p51308430"></a>strategy_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p62342171"><a name="zh-cn_topic_0225568878_p62342171"></a><a name="zh-cn_topic_0225568878_p62342171"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p16551109"><a name="zh-cn_topic_0225568878_p16551109"></a><a name="zh-cn_topic_0225568878_p16551109"></a>流控策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row14742256"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p53272079"><a name="zh-cn_topic_0225568878_p53272079"></a><a name="zh-cn_topic_0225568878_p53272079"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p20071167"><a name="zh-cn_topic_0225568878_p20071167"></a><a name="zh-cn_topic_0225568878_p20071167"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p15151848"><a name="zh-cn_topic_0225568878_p15151848"></a><a name="zh-cn_topic_0225568878_p15151848"></a>特殊对象的身份标识</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row1259734165413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p160910449544"><a name="zh-cn_topic_0225568878_p160910449544"></a><a name="zh-cn_topic_0225568878_p160910449544"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p126101442541"><a name="zh-cn_topic_0225568878_p126101442541"></a><a name="zh-cn_topic_0225568878_p126101442541"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p461364413545"><a name="zh-cn_topic_0225568878_p461364413545"></a><a name="zh-cn_topic_0225568878_p461364413545"></a>作用的APP或租户的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row2148905"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p39843577"><a name="zh-cn_topic_0225568878_p39843577"></a><a name="zh-cn_topic_0225568878_p39843577"></a>instance_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p6104277"><a name="zh-cn_topic_0225568878_p6104277"></a><a name="zh-cn_topic_0225568878_p6104277"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p24684454"><a name="zh-cn_topic_0225568878_p24684454"></a><a name="zh-cn_topic_0225568878_p24684454"></a>特殊对象的类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row20833502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p9792121"><a name="zh-cn_topic_0225568878_p9792121"></a><a name="zh-cn_topic_0225568878_p9792121"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p54964349"><a name="zh-cn_topic_0225568878_p54964349"></a><a name="zh-cn_topic_0225568878_p54964349"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p22927248"><a name="zh-cn_topic_0225568878_p22927248"></a><a name="zh-cn_topic_0225568878_p22927248"></a>特殊对象在流控时间内能够访问API的最大次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row5018648"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p3857352"><a name="zh-cn_topic_0225568878_p3857352"></a><a name="zh-cn_topic_0225568878_p3857352"></a>apply_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p44010076"><a name="zh-cn_topic_0225568878_p44010076"></a><a name="zh-cn_topic_0225568878_p44010076"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p8046397"><a name="zh-cn_topic_0225568878_p8046397"></a><a name="zh-cn_topic_0225568878_p8046397"></a>设置时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row2848658175313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p10212179195415"><a name="zh-cn_topic_0225568878_p10212179195415"></a><a name="zh-cn_topic_0225568878_p10212179195415"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p92151898547"><a name="zh-cn_topic_0225568878_p92151898547"></a><a name="zh-cn_topic_0225568878_p92151898547"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p152168918547"><a name="zh-cn_topic_0225568878_p152168918547"></a><a name="zh-cn_topic_0225568878_p152168918547"></a>作用的APP编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row5308709"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568878_p27352291"><a name="zh-cn_topic_0225568878_p27352291"></a><a name="zh-cn_topic_0225568878_p27352291"></a>app_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568878_p943138"><a name="zh-cn_topic_0225568878_p943138"></a><a name="zh-cn_topic_0225568878_p943138"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568878_p9285386"><a name="zh-cn_topic_0225568878_p9285386"></a><a name="zh-cn_topic_0225568878_p9285386"></a>作用的APP名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "778879b8-df10-495b-a087-874859fdea6d",
	"strategy_id": "a3106cfe-801f-4919-b0d7-d785dc5b47f9",
	"instance_id": "98efd77d-10b5-4eca-8170-ed30a4a286a4",
	"instance_name": "app_002",
	"instance_type": "APP",
	"call_limits": 180,
	"apply_time": "2017-12-29T03:11:18Z",
	"app_id": "98efd77d-10b5-4eca-8170-ed30a4a286a4",
	"app_name": "app_002"
}
```

## 状态码<a name="zh-cn_topic_0225568878_section58817651"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568878_table26254568"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568878_row24172196"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568878_p11790859"><a name="zh-cn_topic_0225568878_p11790859"></a><a name="zh-cn_topic_0225568878_p11790859"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568878_p15535514"><a name="zh-cn_topic_0225568878_p15535514"></a><a name="zh-cn_topic_0225568878_p15535514"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568878_row50417146"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568878_p57257043"><a name="zh-cn_topic_0225568878_p57257043"></a><a name="zh-cn_topic_0225568878_p57257043"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568878_p7308876"><a name="zh-cn_topic_0225568878_p7308876"></a><a name="zh-cn_topic_0225568878_p7308876"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row65779884"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568878_p26570360"><a name="zh-cn_topic_0225568878_p26570360"></a><a name="zh-cn_topic_0225568878_p26570360"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568878_p4715577"><a name="zh-cn_topic_0225568878_p4715577"></a><a name="zh-cn_topic_0225568878_p4715577"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row42440201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568878_p15104276"><a name="zh-cn_topic_0225568878_p15104276"></a><a name="zh-cn_topic_0225568878_p15104276"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568878_p15486856"><a name="zh-cn_topic_0225568878_p15486856"></a><a name="zh-cn_topic_0225568878_p15486856"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row5163976"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568878_p15628907"><a name="zh-cn_topic_0225568878_p15628907"></a><a name="zh-cn_topic_0225568878_p15628907"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568878_p57981963"><a name="zh-cn_topic_0225568878_p57981963"></a><a name="zh-cn_topic_0225568878_p57981963"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row52075621"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568878_p57375754"><a name="zh-cn_topic_0225568878_p57375754"></a><a name="zh-cn_topic_0225568878_p57375754"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568878_p16924512"><a name="zh-cn_topic_0225568878_p16924512"></a><a name="zh-cn_topic_0225568878_p16924512"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568878_row18102885"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568878_p57047558"><a name="zh-cn_topic_0225568878_p57047558"></a><a name="zh-cn_topic_0225568878_p57047558"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568878_p57449517"><a name="zh-cn_topic_0225568878_p57449517"></a><a name="zh-cn_topic_0225568878_p57449517"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

