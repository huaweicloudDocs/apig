# 查看APP详情<a name="ZH-CN_TOPIC_0000001082135097"></a>

## 功能介绍<a name="zh-cn_topic_0118921763_section41459779"></a>

查看指定APP的详细信息。

## URI<a name="zh-cn_topic_0118921763_section37593697"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921763_table15644193"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row49821820"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921763_p9035630"><a name="zh-cn_topic_0118921763_p9035630"></a><a name="zh-cn_topic_0118921763_p9035630"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921763_p60797453"><a name="zh-cn_topic_0118921763_p60797453"></a><a name="zh-cn_topic_0118921763_p60797453"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921763_row25646656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p64113264"><a name="zh-cn_topic_0118921763_p64113264"></a><a name="zh-cn_topic_0118921763_p64113264"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p25791876"><a name="zh-cn_topic_0118921763_p25791876"></a><a name="zh-cn_topic_0118921763_p25791876"></a>/v1.0/apigw/apps/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921763_table8767205"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row50080004"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921763_p29948539"><a name="zh-cn_topic_0118921763_p29948539"></a><a name="zh-cn_topic_0118921763_p29948539"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921763_p9912623"><a name="zh-cn_topic_0118921763_p9912623"></a><a name="zh-cn_topic_0118921763_p9912623"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921763_p64724999"><a name="zh-cn_topic_0118921763_p64724999"></a><a name="zh-cn_topic_0118921763_p64724999"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921763_p8233580"><a name="zh-cn_topic_0118921763_p8233580"></a><a name="zh-cn_topic_0118921763_p8233580"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921763_row62940229"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921763_p64993787"><a name="zh-cn_topic_0118921763_p64993787"></a><a name="zh-cn_topic_0118921763_p64993787"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921763_p30005365"><a name="zh-cn_topic_0118921763_p30005365"></a><a name="zh-cn_topic_0118921763_p30005365"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921763_p14515483"><a name="zh-cn_topic_0118921763_p14515483"></a><a name="zh-cn_topic_0118921763_p14515483"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921763_p34903511"><a name="zh-cn_topic_0118921763_p34903511"></a><a name="zh-cn_topic_0118921763_p34903511"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921763_section2798957"></a>

无

## 响应消息<a name="zh-cn_topic_0118921763_section25388955"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921763_table3064736"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row19944104"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921763_p4859756"><a name="zh-cn_topic_0118921763_p4859756"></a><a name="zh-cn_topic_0118921763_p4859756"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921763_p58095956"><a name="zh-cn_topic_0118921763_p58095956"></a><a name="zh-cn_topic_0118921763_p58095956"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921763_p8152009"><a name="zh-cn_topic_0118921763_p8152009"></a><a name="zh-cn_topic_0118921763_p8152009"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921763_row56332978"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p66677368"><a name="zh-cn_topic_0118921763_p66677368"></a><a name="zh-cn_topic_0118921763_p66677368"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p32157698"><a name="zh-cn_topic_0118921763_p32157698"></a><a name="zh-cn_topic_0118921763_p32157698"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p54636728"><a name="zh-cn_topic_0118921763_p54636728"></a><a name="zh-cn_topic_0118921763_p54636728"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row21968512"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p34619044"><a name="zh-cn_topic_0118921763_p34619044"></a><a name="zh-cn_topic_0118921763_p34619044"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p52679209"><a name="zh-cn_topic_0118921763_p52679209"></a><a name="zh-cn_topic_0118921763_p52679209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p39157559"><a name="zh-cn_topic_0118921763_p39157559"></a><a name="zh-cn_topic_0118921763_p39157559"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row16873712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p24593437"><a name="zh-cn_topic_0118921763_p24593437"></a><a name="zh-cn_topic_0118921763_p24593437"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p45911399"><a name="zh-cn_topic_0118921763_p45911399"></a><a name="zh-cn_topic_0118921763_p45911399"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p27835829"><a name="zh-cn_topic_0118921763_p27835829"></a><a name="zh-cn_topic_0118921763_p27835829"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row49195873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p25442801"><a name="zh-cn_topic_0118921763_p25442801"></a><a name="zh-cn_topic_0118921763_p25442801"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p47601018"><a name="zh-cn_topic_0118921763_p47601018"></a><a name="zh-cn_topic_0118921763_p47601018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p30477219"><a name="zh-cn_topic_0118921763_p30477219"></a><a name="zh-cn_topic_0118921763_p30477219"></a>APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row5859515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p4858679"><a name="zh-cn_topic_0118921763_p4858679"></a><a name="zh-cn_topic_0118921763_p4858679"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p58008744"><a name="zh-cn_topic_0118921763_p58008744"></a><a name="zh-cn_topic_0118921763_p58008744"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p1087862"><a name="zh-cn_topic_0118921763_p1087862"></a><a name="zh-cn_topic_0118921763_p1087862"></a>密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row261113332107"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p148381123152516"><a name="zh-cn_topic_0118921763_p148381123152516"></a><a name="zh-cn_topic_0118921763_p148381123152516"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p10838223112516"><a name="zh-cn_topic_0118921763_p10838223112516"></a><a name="zh-cn_topic_0118921763_p10838223112516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p128381023202515"><a name="zh-cn_topic_0118921763_p128381023202515"></a><a name="zh-cn_topic_0118921763_p128381023202515"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0118921763_ul1126756132511"></a><a name="zh-cn_topic_0118921763_ul1126756132511"></a><ul id="zh-cn_topic_0118921763_ul1126756132511"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row9790763"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p54854351"><a name="zh-cn_topic_0118921763_p54854351"></a><a name="zh-cn_topic_0118921763_p54854351"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p14017410"><a name="zh-cn_topic_0118921763_p14017410"></a><a name="zh-cn_topic_0118921763_p14017410"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p61668463"><a name="zh-cn_topic_0118921763_p61668463"></a><a name="zh-cn_topic_0118921763_p61668463"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row18145258"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p60479774"><a name="zh-cn_topic_0118921763_p60479774"></a><a name="zh-cn_topic_0118921763_p60479774"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p67023519"><a name="zh-cn_topic_0118921763_p67023519"></a><a name="zh-cn_topic_0118921763_p67023519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p60195924"><a name="zh-cn_topic_0118921763_p60195924"></a><a name="zh-cn_topic_0118921763_p60195924"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row4892405"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p60740564"><a name="zh-cn_topic_0118921763_p60740564"></a><a name="zh-cn_topic_0118921763_p60740564"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p21038684"><a name="zh-cn_topic_0118921763_p21038684"></a><a name="zh-cn_topic_0118921763_p21038684"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p26411828"><a name="zh-cn_topic_0118921763_p26411828"></a><a name="zh-cn_topic_0118921763_p26411828"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row1697461013341"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921763_p14855159163015"><a name="zh-cn_topic_0118921763_p14855159163015"></a><a name="zh-cn_topic_0118921763_p14855159163015"></a>app_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921763_p12855195993012"><a name="zh-cn_topic_0118921763_p12855195993012"></a><a name="zh-cn_topic_0118921763_p12855195993012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921763_p1085575910302"><a name="zh-cn_topic_0118921763_p1085575910302"></a><a name="zh-cn_topic_0118921763_p1085575910302"></a>APP类型，默认为apig</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "14b399ac-967f-4115-bb62-c0346b4537e9",
	"name": "app_001",
	"status": 1,
	"app_key": "d49b1cbf-cc81-4a5f-b2a0-61b568e376eb",
	"app_secret": "******",
	"creator": "USER",
	"remark": "第一个APP",
	"register_time": "2017-12-28T12:26:54Z",
	"update_time": "2017-12-28T12:28:07.2966182Z",
        "app_type": "apig"
}
```

## 状态码<a name="zh-cn_topic_0118921763_section25190616"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118921763_table26492330"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row38027958"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921763_p60365757"><a name="zh-cn_topic_0118921763_p60365757"></a><a name="zh-cn_topic_0118921763_p60365757"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921763_p57788140"><a name="zh-cn_topic_0118921763_p57788140"></a><a name="zh-cn_topic_0118921763_p57788140"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921763_row50327788"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p50019045"><a name="zh-cn_topic_0118921763_p50019045"></a><a name="zh-cn_topic_0118921763_p50019045"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p25010814"><a name="zh-cn_topic_0118921763_p25010814"></a><a name="zh-cn_topic_0118921763_p25010814"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row23770734"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p46381274"><a name="zh-cn_topic_0118921763_p46381274"></a><a name="zh-cn_topic_0118921763_p46381274"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p65895739"><a name="zh-cn_topic_0118921763_p65895739"></a><a name="zh-cn_topic_0118921763_p65895739"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row56190747"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p55156678"><a name="zh-cn_topic_0118921763_p55156678"></a><a name="zh-cn_topic_0118921763_p55156678"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p38505946"><a name="zh-cn_topic_0118921763_p38505946"></a><a name="zh-cn_topic_0118921763_p38505946"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row11009194"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p19329517"><a name="zh-cn_topic_0118921763_p19329517"></a><a name="zh-cn_topic_0118921763_p19329517"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p22187053"><a name="zh-cn_topic_0118921763_p22187053"></a><a name="zh-cn_topic_0118921763_p22187053"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921763_row65465751"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921763_p1125596"><a name="zh-cn_topic_0118921763_p1125596"></a><a name="zh-cn_topic_0118921763_p1125596"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921763_p24064466"><a name="zh-cn_topic_0118921763_p24064466"></a><a name="zh-cn_topic_0118921763_p24064466"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

