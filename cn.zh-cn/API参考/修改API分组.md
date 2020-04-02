# 修改API分组<a name="apig-zh-api-180713017"></a>

## 功能介绍<a name="section60874305"></a>

修改API分组属性。其中name和remark可修改，其他属性不可修改。

## URI<a name="section10997834"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table7576160"></a>
<table><thead align="left"><tr id="row18958597"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p59251354"><a name="p59251354"></a><a name="p59251354"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p34630347"><a name="p34630347"></a><a name="p34630347"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row53594754"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p46207780"><a name="p46207780"></a><a name="p46207780"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p51842715"><a name="p51842715"></a><a name="p51842715"></a>/v1.0/apigw/api-groups/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table38510415"></a>
<table><thead align="left"><tr id="row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="p23103637"><a name="p23103637"></a><a name="p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p59455291"><a name="p59455291"></a><a name="p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="p51149303"><a name="p51149303"></a><a name="p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="p49452846"><a name="p49452846"></a><a name="p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>API分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section31871645"></a>

**表 3**  参数说明

<a name="table56526963"></a>
<table><thead align="left"><tr id="row46508794"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p9115995"><a name="p9115995"></a><a name="p9115995"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.2"><p id="p198169"><a name="p198169"></a><a name="p198169"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p16051739"><a name="p16051739"></a><a name="p16051739"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="p25122506"><a name="p25122506"></a><a name="p25122506"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row21657101"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9394765"><a name="p9394765"></a><a name="p9394765"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="p22778481"><a name="p22778481"></a><a name="p22778481"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p33117666"><a name="p33117666"></a><a name="p33117666"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="p65285255"><a name="p65285255"></a><a name="p65285255"></a>名称。</p>
<p id="p12766479"><a name="p12766479"></a><a name="p12766479"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以中文或英文开头。</p>
<div class="note" id="note52191124182510"><a name="note52191124182510"></a><a name="note52191124182510"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p3221202452516"><a name="p3221202452516"></a><a name="p3221202452516"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row60409228"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p61309300"><a name="p61309300"></a><a name="p61309300"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="p67106281"><a name="p67106281"></a><a name="p67106281"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p66899666"><a name="p66899666"></a><a name="p66899666"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="p50163864"><a name="p50163864"></a><a name="p50163864"></a>描述。</p>
<p id="p62234932"><a name="p62234932"></a><a name="p62234932"></a>字符串长度最大不超过255。</p>
<div class="note" id="note1065115482519"><a name="note1065115482519"></a><a name="note1065115482519"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p12672545258"><a name="p12672545258"></a><a name="p12672545258"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"name": "api_group_001",
	"remark": "分组001"
}
```

## 响应消息<a name="section31466478"></a>

**表 4**  参数说明

<a name="table60205371"></a>
<table><thead align="left"><tr id="row46929233"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p43171496"><a name="p43171496"></a><a name="p43171496"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p7230308"><a name="p7230308"></a><a name="p7230308"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p48784109"><a name="p48784109"></a><a name="p48784109"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row59198762"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p30370436"><a name="p30370436"></a><a name="p30370436"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44086242"><a name="p44086242"></a><a name="p44086242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14215853"><a name="p14215853"></a><a name="p14215853"></a>编号</p>
</td>
</tr>
<tr id="row60833814"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28591919"><a name="p28591919"></a><a name="p28591919"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34244072"><a name="p34244072"></a><a name="p34244072"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p22306409"><a name="p22306409"></a><a name="p22306409"></a>名称</p>
</td>
</tr>
<tr id="row66539956"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p21027381"><a name="p21027381"></a><a name="p21027381"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p25496339"><a name="p25496339"></a><a name="p25496339"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p51937589"><a name="p51937589"></a><a name="p51937589"></a>状态</p>
</td>
</tr>
<tr id="row64785124"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13103655"><a name="p13103655"></a><a name="p13103655"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p54763172"><a name="p54763172"></a><a name="p54763172"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6631937"><a name="p6631937"></a><a name="p6631937"></a>系统默认分配的子域名</p>
</td>
</tr>
<tr id="row235125816260"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9351105813265"><a name="p9351105813265"></a><a name="p9351105813265"></a>sl_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15351658152613"><a name="p15351658152613"></a><a name="p15351658152613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2035118583263"><a name="p2035118583263"></a><a name="p2035118583263"></a>系统默认分配的子域名列表</p>
</td>
</tr>
<tr id="row59687435"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2844060"><a name="p2844060"></a><a name="p2844060"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p29042273"><a name="p29042273"></a><a name="p29042273"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3613890"><a name="p3613890"></a><a name="p3613890"></a>创建时间</p>
</td>
</tr>
<tr id="row32525017"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17280753"><a name="p17280753"></a><a name="p17280753"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57563737"><a name="p57563737"></a><a name="p57563737"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p32151097"><a name="p32151097"></a><a name="p32151097"></a>最近修改时间</p>
</td>
</tr>
<tr id="row20924422"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17156622"><a name="p17156622"></a><a name="p17156622"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47509155"><a name="p47509155"></a><a name="p47509155"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p23036332"><a name="p23036332"></a><a name="p23036332"></a>描述</p>
</td>
</tr>
<tr id="row6000400"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16270371"><a name="p16270371"></a><a name="p16270371"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42831646"><a name="p42831646"></a><a name="p42831646"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46811306"><a name="p46811306"></a><a name="p46811306"></a>流控时长内分组下的API的总访问次数限制，默认不限，请根据服务的负载能力自行设置</p>
</td>
</tr>
<tr id="row18648574"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p34139493"><a name="p34139493"></a><a name="p34139493"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13835569"><a name="p13835569"></a><a name="p13835569"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46939338"><a name="p46939338"></a><a name="p46939338"></a>流控时长</p>
</td>
</tr>
<tr id="row19800863"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p60366037"><a name="p60366037"></a><a name="p60366037"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57810828"><a name="p57810828"></a><a name="p57810828"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52165483"><a name="p52165483"></a><a name="p52165483"></a>流控的时间单位</p>
</td>
</tr>
<tr id="row66836170"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p45020665"><a name="p45020665"></a><a name="p45020665"></a>url_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22795237"><a name="p22795237"></a><a name="p22795237"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p34474869"><a name="p34474869"></a><a name="p34474869"></a>分组上绑定的独立域名列表</p>
</td>
</tr>
<tr id="row41838366"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p33464480"><a name="p33464480"></a><a name="p33464480"></a>on_sell_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p26268346"><a name="p26268346"></a><a name="p26268346"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p47361301"><a name="p47361301"></a><a name="p47361301"></a>是否已上架云市场：</p>
<a name="ul23598530"></a><a name="ul23598530"></a><ul id="ul23598530"><li>1：已上架</li><li>2：未上架</li><li>3：审核中</li></ul>
</td>
</tr>
</tbody>
</table>

**表 5**  url\_domains参数说明

<a name="table9811220"></a>
<table><thead align="left"><tr id="row18394177"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p13533375"><a name="p13533375"></a><a name="p13533375"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p22461630"><a name="p22461630"></a><a name="p22461630"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p7452774"><a name="p7452774"></a><a name="p7452774"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row66803806"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p42399182"><a name="p42399182"></a><a name="p42399182"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11781727"><a name="p11781727"></a><a name="p11781727"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14795832"><a name="p14795832"></a><a name="p14795832"></a>域名编号</p>
</td>
</tr>
<tr id="row66053632"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48743961"><a name="p48743961"></a><a name="p48743961"></a>domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p55946767"><a name="p55946767"></a><a name="p55946767"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p35394249"><a name="p35394249"></a><a name="p35394249"></a>访问域名</p>
</td>
</tr>
<tr id="row50112787"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p32603951"><a name="p32603951"></a><a name="p32603951"></a>cname_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23674371"><a name="p23674371"></a><a name="p23674371"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38575928"><a name="p38575928"></a><a name="p38575928"></a>域名cname状态：</p>
<a name="ul11639038"></a><a name="ul11639038"></a><ul id="ul11639038"><li>1：未解析</li><li>2：解析中</li><li>3：解析成功</li><li>4：解析失败</li></ul>
</td>
</tr>
<tr id="row11732266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10789489"><a name="p10789489"></a><a name="p10789489"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1533408"><a name="p1533408"></a><a name="p1533408"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57097248"><a name="p57097248"></a><a name="p57097248"></a>SSL证书编号</p>
</td>
</tr>
<tr id="row967016619319"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p667011623113"><a name="p667011623113"></a><a name="p667011623113"></a>ssl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p967017623110"><a name="p967017623110"></a><a name="p967017623110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p76701261314"><a name="p76701261314"></a><a name="p76701261314"></a>SSL证书名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "7efb2b91-155a-4f6a-9f45-c5c95a6e4950",
	"name": "api_group_001",
	"status": 1,
	"sl_domain": "0e91b83b-0774-4e8e-b187-2d695ed4743b.apigw.example.com",
        "sl_domains": ["0e91b83b-0774-4e8e-b187-2d695ed4743b.apigw.example.com","0e91b83b-0774-4e8e-b187-2d695ed4743b.apigw.example.cn"],
	"remark": "分组001",
	"register_time": "2017-12-28T11:44:53Z",
	"update_time": "2017-12-28T11:49:01.048600577Z",
	"on_sell_status": 2
}
```

## 状态码<a name="section18409356"></a>

**表 6**  返回消息说明

<a name="table16737159"></a>
<table><thead align="left"><tr id="row283921"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p22997658"><a name="p22997658"></a><a name="p22997658"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p50870979"><a name="p50870979"></a><a name="p50870979"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26908596"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p32112662"><a name="p32112662"></a><a name="p32112662"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row56246166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p59645608"><a name="p59645608"></a><a name="p59645608"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p66564967"><a name="p66564967"></a><a name="p66564967"></a>Bad Request</p>
</td>
</tr>
<tr id="row62213794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6152591"><a name="p6152591"></a><a name="p6152591"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p28597852"><a name="p28597852"></a><a name="p28597852"></a>Unauthorized</p>
</td>
</tr>
<tr id="row56054078"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p44086463"><a name="p44086463"></a><a name="p44086463"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row60994581"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p41614068"><a name="p41614068"></a><a name="p41614068"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p15296380"><a name="p15296380"></a><a name="p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="row3449694"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p10989813"><a name="p10989813"></a><a name="p10989813"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1315733818249"><a name="p1315733818249"></a><a name="p1315733818249"></a>Conflict</p>
</td>
</tr>
<tr id="row25619477"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p61911758"><a name="p61911758"></a><a name="p61911758"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1767615692518"><a name="p1767615692518"></a><a name="p1767615692518"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

