# 创建API分组<a name="apig-zh-api-180713016"></a>

## 功能介绍<a name="section66524352"></a>

API分组是API的管理单元，一个API分组等同于一个服务入口，创建API分组时，返回一个子域名作为访问入口。建议一个API分组下的API具有一定的相关性。

## URI<a name="section61848258"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table27084002"></a>
<table><thead align="left"><tr id="row40355780"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p47592766"><a name="p47592766"></a><a name="p47592766"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p29808828"><a name="p29808828"></a><a name="p29808828"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row65704871"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20494310"><a name="p20494310"></a><a name="p20494310"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p49426402"><a name="p49426402"></a><a name="p49426402"></a>/v1.0/apigw/api-groups</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section19763417"></a>

**表 2**  参数说明

<a name="table44115586"></a>
<table><thead align="left"><tr id="row63561487"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p48206846"><a name="p48206846"></a><a name="p48206846"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.2"><p id="p12440449"><a name="p12440449"></a><a name="p12440449"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p1043457"><a name="p1043457"></a><a name="p1043457"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="p17411173"><a name="p17411173"></a><a name="p17411173"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1018902"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p15422203"><a name="p15422203"></a><a name="p15422203"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="p41238908"><a name="p41238908"></a><a name="p41238908"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p52017283"><a name="p52017283"></a><a name="p52017283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="p52650357"><a name="p52650357"></a><a name="p52650357"></a>API分组的名称。</p>
<p id="p62949411"><a name="p62949411"></a><a name="p62949411"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以英文或中文开头。</p>
<div class="note" id="note451481917153"><a name="note451481917153"></a><a name="note451481917153"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1051512199159"><a name="p1051512199159"></a><a name="p1051512199159"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row25118534"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p21335372"><a name="p21335372"></a><a name="p21335372"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="p50443542"><a name="p50443542"></a><a name="p50443542"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p59395084"><a name="p59395084"></a><a name="p59395084"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="p46272536"><a name="p46272536"></a><a name="p46272536"></a>API分组描述。</p>
<p id="p44029085"><a name="p44029085"></a><a name="p44029085"></a>长度最大不超过255个字符。</p>
<div class="note" id="note75421401158"><a name="note75421401158"></a><a name="note75421401158"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p15545040191512"><a name="p15545040191512"></a><a name="p15545040191512"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"name": "api_group_001",
	"remark": "分组1"
}
```

## 响应消息<a name="section57332943"></a>

**表 3**  参数说明

<a name="table2803298"></a>
<table><thead align="left"><tr id="row9258659"><th class="cellrowborder" valign="top" width="20.02%" id="mcps1.2.4.1.1"><p id="p11753897"><a name="p11753897"></a><a name="p11753897"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.98%" id="mcps1.2.4.1.2"><p id="p12541637"><a name="p12541637"></a><a name="p12541637"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p9239644"><a name="p9239644"></a><a name="p9239644"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10213720"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p22005025"><a name="p22005025"></a><a name="p22005025"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p37576606"><a name="p37576606"></a><a name="p37576606"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p23806264"><a name="p23806264"></a><a name="p23806264"></a>编号</p>
</td>
</tr>
<tr id="row12929787"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p40679818"><a name="p40679818"></a><a name="p40679818"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p6730986"><a name="p6730986"></a><a name="p6730986"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8339011"><a name="p8339011"></a><a name="p8339011"></a>名称</p>
</td>
</tr>
<tr id="row7942236"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p39341340"><a name="p39341340"></a><a name="p39341340"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p32531944"><a name="p32531944"></a><a name="p32531944"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17841833"><a name="p17841833"></a><a name="p17841833"></a>状态</p>
</td>
</tr>
<tr id="row26358777"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p54686212"><a name="p54686212"></a><a name="p54686212"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p398200"><a name="p398200"></a><a name="p398200"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p32254203"><a name="p32254203"></a><a name="p32254203"></a>系统默认分配的子域名</p>
</td>
</tr>
<tr id="row21852379"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p25212283"><a name="p25212283"></a><a name="p25212283"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p28929023"><a name="p28929023"></a><a name="p28929023"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61549520"><a name="p61549520"></a><a name="p61549520"></a>创建时间</p>
</td>
</tr>
<tr id="row17074768"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p40878974"><a name="p40878974"></a><a name="p40878974"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p22862637"><a name="p22862637"></a><a name="p22862637"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p39934341"><a name="p39934341"></a><a name="p39934341"></a>最近修改时间</p>
</td>
</tr>
<tr id="row23864751"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p53996694"><a name="p53996694"></a><a name="p53996694"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p11656122"><a name="p11656122"></a><a name="p11656122"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4621826"><a name="p4621826"></a><a name="p4621826"></a>描述</p>
</td>
</tr>
<tr id="row19473624"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p33859681"><a name="p33859681"></a><a name="p33859681"></a>on_sell_status</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p58279602"><a name="p58279602"></a><a name="p58279602"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p23027316"><a name="p23027316"></a><a name="p23027316"></a>是否已上架云市场：</p>
<a name="ul5919254"></a><a name="ul5919254"></a><ul id="ul5919254"><li>1：已上架</li><li>2：未上架</li><li>3：审核中</li></ul>
</td>
</tr>
<tr id="row168471214124017"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p63758800"><a name="p63758800"></a><a name="p63758800"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p64189201"><a name="p64189201"></a><a name="p64189201"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p31942831"><a name="p31942831"></a><a name="p31942831"></a>流控时长内分组下的API的总访问次数限制，默认不限，请根据服务的负载能力自行设置</p>
</td>
</tr>
<tr id="row14610754017"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p66657312"><a name="p66657312"></a><a name="p66657312"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p30533155"><a name="p30533155"></a><a name="p30533155"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57266528"><a name="p57266528"></a><a name="p57266528"></a>流控时长</p>
</td>
</tr>
<tr id="row2746118401"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p5585767"><a name="p5585767"></a><a name="p5585767"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p49793976"><a name="p49793976"></a><a name="p49793976"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6780221"><a name="p6780221"></a><a name="p6780221"></a>流控的时间单位</p>
</td>
</tr>
<tr id="row984812214017"><td class="cellrowborder" valign="top" width="20.02%" headers="mcps1.2.4.1.1 "><p id="p43834197"><a name="p43834197"></a><a name="p43834197"></a>url_domains</p>
</td>
<td class="cellrowborder" valign="top" width="19.98%" headers="mcps1.2.4.1.2 "><p id="p60909101"><a name="p60909101"></a><a name="p60909101"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p34690133"><a name="p34690133"></a><a name="p34690133"></a>分组上绑定的独立域名列表</p>
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
	"remark": "分组1",
	"register_time": "2017-12-28T11:44:53.831282304Z",
	"update_time": "2017-12-28T11:44:53.831283436Z",
	"on_sell_status": 2
}
```

## 状态码<a name="section43653029"></a>

**表 4**  返回消息说明

<a name="table61067539"></a>
<table><thead align="left"><tr id="row16541512"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p64794090"><a name="p64794090"></a><a name="p64794090"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p13829924"><a name="p13829924"></a><a name="p13829924"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46482079"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6952067"><a name="p6952067"></a><a name="p6952067"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p73578115452"><a name="p73578115452"></a><a name="p73578115452"></a>Created</p>
</td>
</tr>
<tr id="row34892078"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p7686078"><a name="p7686078"></a><a name="p7686078"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p48128109554"><a name="p48128109554"></a><a name="p48128109554"></a>Bad Request</p>
</td>
</tr>
<tr id="row33115333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p65096331"><a name="p65096331"></a><a name="p65096331"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row9258873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p11771280"><a name="p11771280"></a><a name="p11771280"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row58437416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p35810232"><a name="p35810232"></a><a name="p35810232"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

