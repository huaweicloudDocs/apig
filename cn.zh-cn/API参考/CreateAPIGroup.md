# 创建API分组<a name="ZH-CN_TOPIC_0000001081837255"></a>

## 功能介绍<a name="zh-cn_topic_0118921484_section66524352"></a>

API分组是API的管理单元，一个API分组等同于一个服务入口，创建API分组时，返回一个子域名作为访问入口。建议一个API分组下的API具有一定的相关性。

## URI<a name="zh-cn_topic_0118921484_section61848258"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921484_table27084002"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921484_row40355780"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921484_p47592766"><a name="zh-cn_topic_0118921484_p47592766"></a><a name="zh-cn_topic_0118921484_p47592766"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921484_p29808828"><a name="zh-cn_topic_0118921484_p29808828"></a><a name="zh-cn_topic_0118921484_p29808828"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921484_row65704871"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921484_p20494310"><a name="zh-cn_topic_0118921484_p20494310"></a><a name="zh-cn_topic_0118921484_p20494310"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921484_p49426402"><a name="zh-cn_topic_0118921484_p49426402"></a><a name="zh-cn_topic_0118921484_p49426402"></a>/v1.0/apigw/api-groups</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921484_section19763417"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118921484_table44115586"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921484_row63561487"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921484_p48206846"><a name="zh-cn_topic_0118921484_p48206846"></a><a name="zh-cn_topic_0118921484_p48206846"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921484_p12440449"><a name="zh-cn_topic_0118921484_p12440449"></a><a name="zh-cn_topic_0118921484_p12440449"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921484_p1043457"><a name="zh-cn_topic_0118921484_p1043457"></a><a name="zh-cn_topic_0118921484_p1043457"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921484_p17411173"><a name="zh-cn_topic_0118921484_p17411173"></a><a name="zh-cn_topic_0118921484_p17411173"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921484_row1018902"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921484_p15422203"><a name="zh-cn_topic_0118921484_p15422203"></a><a name="zh-cn_topic_0118921484_p15422203"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921484_p41238908"><a name="zh-cn_topic_0118921484_p41238908"></a><a name="zh-cn_topic_0118921484_p41238908"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921484_p52017283"><a name="zh-cn_topic_0118921484_p52017283"></a><a name="zh-cn_topic_0118921484_p52017283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921484_p52650357"><a name="zh-cn_topic_0118921484_p52650357"></a><a name="zh-cn_topic_0118921484_p52650357"></a>API分组的名称。</p>
<p id="zh-cn_topic_0118921484_p62949411"><a name="zh-cn_topic_0118921484_p62949411"></a><a name="zh-cn_topic_0118921484_p62949411"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以英文或中文开头。</p>
<div class="note" id="zh-cn_topic_0118921484_note451481917153"><a name="zh-cn_topic_0118921484_note451481917153"></a><a name="zh-cn_topic_0118921484_note451481917153"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118921484_p1051512199159"><a name="zh-cn_topic_0118921484_p1051512199159"></a><a name="zh-cn_topic_0118921484_p1051512199159"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row25118534"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921484_p21335372"><a name="zh-cn_topic_0118921484_p21335372"></a><a name="zh-cn_topic_0118921484_p21335372"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921484_p50443542"><a name="zh-cn_topic_0118921484_p50443542"></a><a name="zh-cn_topic_0118921484_p50443542"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921484_p59395084"><a name="zh-cn_topic_0118921484_p59395084"></a><a name="zh-cn_topic_0118921484_p59395084"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921484_p46272536"><a name="zh-cn_topic_0118921484_p46272536"></a><a name="zh-cn_topic_0118921484_p46272536"></a>API分组描述。</p>
<p id="zh-cn_topic_0118921484_p44029085"><a name="zh-cn_topic_0118921484_p44029085"></a><a name="zh-cn_topic_0118921484_p44029085"></a>长度最大不超过255个字符。</p>
<div class="note" id="zh-cn_topic_0118921484_note75421401158"><a name="zh-cn_topic_0118921484_note75421401158"></a><a name="zh-cn_topic_0118921484_note75421401158"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118921484_p15545040191512"><a name="zh-cn_topic_0118921484_p15545040191512"></a><a name="zh-cn_topic_0118921484_p15545040191512"></a>中文字符必须为UTF-8或者unicode编码。</p>
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

## 响应消息<a name="zh-cn_topic_0118921484_section57332943"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921484_table2803298"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921484_row9258659"><th class="cellrowborder" valign="top" width="20.05%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921484_p11753897"><a name="zh-cn_topic_0118921484_p11753897"></a><a name="zh-cn_topic_0118921484_p11753897"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.950000000000003%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921484_p12541637"><a name="zh-cn_topic_0118921484_p12541637"></a><a name="zh-cn_topic_0118921484_p12541637"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921484_p9239644"><a name="zh-cn_topic_0118921484_p9239644"></a><a name="zh-cn_topic_0118921484_p9239644"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921484_row10213720"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p22005025"><a name="zh-cn_topic_0118921484_p22005025"></a><a name="zh-cn_topic_0118921484_p22005025"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p37576606"><a name="zh-cn_topic_0118921484_p37576606"></a><a name="zh-cn_topic_0118921484_p37576606"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p23806264"><a name="zh-cn_topic_0118921484_p23806264"></a><a name="zh-cn_topic_0118921484_p23806264"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row12929787"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p40679818"><a name="zh-cn_topic_0118921484_p40679818"></a><a name="zh-cn_topic_0118921484_p40679818"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p6730986"><a name="zh-cn_topic_0118921484_p6730986"></a><a name="zh-cn_topic_0118921484_p6730986"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p8339011"><a name="zh-cn_topic_0118921484_p8339011"></a><a name="zh-cn_topic_0118921484_p8339011"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row7942236"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p39341340"><a name="zh-cn_topic_0118921484_p39341340"></a><a name="zh-cn_topic_0118921484_p39341340"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p32531944"><a name="zh-cn_topic_0118921484_p32531944"></a><a name="zh-cn_topic_0118921484_p32531944"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p17841833"><a name="zh-cn_topic_0118921484_p17841833"></a><a name="zh-cn_topic_0118921484_p17841833"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row26358777"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p54686212"><a name="zh-cn_topic_0118921484_p54686212"></a><a name="zh-cn_topic_0118921484_p54686212"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p398200"><a name="zh-cn_topic_0118921484_p398200"></a><a name="zh-cn_topic_0118921484_p398200"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p32254203"><a name="zh-cn_topic_0118921484_p32254203"></a><a name="zh-cn_topic_0118921484_p32254203"></a>系统默认分配的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row18727834192412"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p3727334122410"><a name="zh-cn_topic_0118921484_p3727334122410"></a><a name="zh-cn_topic_0118921484_p3727334122410"></a>sl_domains</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p167271034142413"><a name="zh-cn_topic_0118921484_p167271034142413"></a><a name="zh-cn_topic_0118921484_p167271034142413"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p141141744162418"><a name="zh-cn_topic_0118921484_p141141744162418"></a><a name="zh-cn_topic_0118921484_p141141744162418"></a>系统默认分配的子域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row21852379"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p25212283"><a name="zh-cn_topic_0118921484_p25212283"></a><a name="zh-cn_topic_0118921484_p25212283"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p28929023"><a name="zh-cn_topic_0118921484_p28929023"></a><a name="zh-cn_topic_0118921484_p28929023"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p61549520"><a name="zh-cn_topic_0118921484_p61549520"></a><a name="zh-cn_topic_0118921484_p61549520"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row17074768"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p40878974"><a name="zh-cn_topic_0118921484_p40878974"></a><a name="zh-cn_topic_0118921484_p40878974"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p22862637"><a name="zh-cn_topic_0118921484_p22862637"></a><a name="zh-cn_topic_0118921484_p22862637"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p39934341"><a name="zh-cn_topic_0118921484_p39934341"></a><a name="zh-cn_topic_0118921484_p39934341"></a>最近修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row23864751"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p53996694"><a name="zh-cn_topic_0118921484_p53996694"></a><a name="zh-cn_topic_0118921484_p53996694"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p11656122"><a name="zh-cn_topic_0118921484_p11656122"></a><a name="zh-cn_topic_0118921484_p11656122"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p4621826"><a name="zh-cn_topic_0118921484_p4621826"></a><a name="zh-cn_topic_0118921484_p4621826"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row19473624"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p33859681"><a name="zh-cn_topic_0118921484_p33859681"></a><a name="zh-cn_topic_0118921484_p33859681"></a>on_sell_status</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p58279602"><a name="zh-cn_topic_0118921484_p58279602"></a><a name="zh-cn_topic_0118921484_p58279602"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p23027316"><a name="zh-cn_topic_0118921484_p23027316"></a><a name="zh-cn_topic_0118921484_p23027316"></a>是否已上架云市场：</p>
<a name="zh-cn_topic_0118921484_ul5919254"></a><a name="zh-cn_topic_0118921484_ul5919254"></a><ul id="zh-cn_topic_0118921484_ul5919254"><li>1：已上架</li><li>2：未上架</li><li>3：审核中</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row168471214124017"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p63758800"><a name="zh-cn_topic_0118921484_p63758800"></a><a name="zh-cn_topic_0118921484_p63758800"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p64189201"><a name="zh-cn_topic_0118921484_p64189201"></a><a name="zh-cn_topic_0118921484_p64189201"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p31942831"><a name="zh-cn_topic_0118921484_p31942831"></a><a name="zh-cn_topic_0118921484_p31942831"></a>流控时长内分组下的API的总访问次数限制，默认不限，请根据服务的负载能力自行设置</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row14610754017"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p66657312"><a name="zh-cn_topic_0118921484_p66657312"></a><a name="zh-cn_topic_0118921484_p66657312"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p30533155"><a name="zh-cn_topic_0118921484_p30533155"></a><a name="zh-cn_topic_0118921484_p30533155"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p57266528"><a name="zh-cn_topic_0118921484_p57266528"></a><a name="zh-cn_topic_0118921484_p57266528"></a>流控时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row2746118401"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p5585767"><a name="zh-cn_topic_0118921484_p5585767"></a><a name="zh-cn_topic_0118921484_p5585767"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p49793976"><a name="zh-cn_topic_0118921484_p49793976"></a><a name="zh-cn_topic_0118921484_p49793976"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p6780221"><a name="zh-cn_topic_0118921484_p6780221"></a><a name="zh-cn_topic_0118921484_p6780221"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row984812214017"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p43834197"><a name="zh-cn_topic_0118921484_p43834197"></a><a name="zh-cn_topic_0118921484_p43834197"></a>url_domains</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p60909101"><a name="zh-cn_topic_0118921484_p60909101"></a><a name="zh-cn_topic_0118921484_p60909101"></a>Array of <a href="#zh-cn_topic_0118921484_table9811220">UrlDomainsResp</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p34690133"><a name="zh-cn_topic_0118921484_p34690133"></a><a name="zh-cn_topic_0118921484_p34690133"></a>分组上绑定的独立域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row952525213213"><td class="cellrowborder" valign="top" width="20.05%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p3525152172119"><a name="zh-cn_topic_0118921484_p3525152172119"></a><a name="zh-cn_topic_0118921484_p3525152172119"></a>is_default</p>
</td>
<td class="cellrowborder" valign="top" width="19.950000000000003%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p4525952142112"><a name="zh-cn_topic_0118921484_p4525952142112"></a><a name="zh-cn_topic_0118921484_p4525952142112"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p15525652152119"><a name="zh-cn_topic_0118921484_p15525652152119"></a><a name="zh-cn_topic_0118921484_p15525652152119"></a>是否为默认分组，默认为非默认分组：</p>
<a name="zh-cn_topic_0118921484_ul1170161912317"></a><a name="zh-cn_topic_0118921484_ul1170161912317"></a><ul id="zh-cn_topic_0118921484_ul1170161912317"><li>1：默认分组</li><li>2：非默认分组</li></ul>
</td>
</tr>
</tbody>
</table>

**表 4**  UrlDomainsResp

<a name="zh-cn_topic_0118921484_table9811220"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921484_row18394177"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921484_p13533375"><a name="zh-cn_topic_0118921484_p13533375"></a><a name="zh-cn_topic_0118921484_p13533375"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921484_p22461630"><a name="zh-cn_topic_0118921484_p22461630"></a><a name="zh-cn_topic_0118921484_p22461630"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921484_p7452774"><a name="zh-cn_topic_0118921484_p7452774"></a><a name="zh-cn_topic_0118921484_p7452774"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921484_row66803806"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p42399182"><a name="zh-cn_topic_0118921484_p42399182"></a><a name="zh-cn_topic_0118921484_p42399182"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p11781727"><a name="zh-cn_topic_0118921484_p11781727"></a><a name="zh-cn_topic_0118921484_p11781727"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p14795832"><a name="zh-cn_topic_0118921484_p14795832"></a><a name="zh-cn_topic_0118921484_p14795832"></a>域名编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row66053632"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p48743961"><a name="zh-cn_topic_0118921484_p48743961"></a><a name="zh-cn_topic_0118921484_p48743961"></a>domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p55946767"><a name="zh-cn_topic_0118921484_p55946767"></a><a name="zh-cn_topic_0118921484_p55946767"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p35394249"><a name="zh-cn_topic_0118921484_p35394249"></a><a name="zh-cn_topic_0118921484_p35394249"></a>访问域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row50112787"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p32603951"><a name="zh-cn_topic_0118921484_p32603951"></a><a name="zh-cn_topic_0118921484_p32603951"></a>cname_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p23674371"><a name="zh-cn_topic_0118921484_p23674371"></a><a name="zh-cn_topic_0118921484_p23674371"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p38575928"><a name="zh-cn_topic_0118921484_p38575928"></a><a name="zh-cn_topic_0118921484_p38575928"></a>域名cname状态：</p>
<a name="zh-cn_topic_0118921484_ul11639038"></a><a name="zh-cn_topic_0118921484_ul11639038"></a><ul id="zh-cn_topic_0118921484_ul11639038"><li>1：未解析</li><li>2：解析中</li><li>3：解析成功</li><li>4：解析失败</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row11732266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p10789489"><a name="zh-cn_topic_0118921484_p10789489"></a><a name="zh-cn_topic_0118921484_p10789489"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p1533408"><a name="zh-cn_topic_0118921484_p1533408"></a><a name="zh-cn_topic_0118921484_p1533408"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p57097248"><a name="zh-cn_topic_0118921484_p57097248"></a><a name="zh-cn_topic_0118921484_p57097248"></a>SSL证书编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row967016619319"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921484_p667011623113"><a name="zh-cn_topic_0118921484_p667011623113"></a><a name="zh-cn_topic_0118921484_p667011623113"></a>ssl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921484_p967017623110"><a name="zh-cn_topic_0118921484_p967017623110"></a><a name="zh-cn_topic_0118921484_p967017623110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921484_p76701261314"><a name="zh-cn_topic_0118921484_p76701261314"></a><a name="zh-cn_topic_0118921484_p76701261314"></a>SSL证书名称</p>
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
	"remark": "分组1",
	"register_time": "2017-12-28T11:44:53.831282304Z",
	"update_time": "2017-12-28T11:44:53.831283436Z",
	"on_sell_status": 2,
        "is_default": 2
}
```

## 状态码<a name="zh-cn_topic_0118921484_section43653029"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118921484_table61067539"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921484_row16541512"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921484_p64794090"><a name="zh-cn_topic_0118921484_p64794090"></a><a name="zh-cn_topic_0118921484_p64794090"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921484_p13829924"><a name="zh-cn_topic_0118921484_p13829924"></a><a name="zh-cn_topic_0118921484_p13829924"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921484_row46482079"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921484_p6952067"><a name="zh-cn_topic_0118921484_p6952067"></a><a name="zh-cn_topic_0118921484_p6952067"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921484_p73578115452"><a name="zh-cn_topic_0118921484_p73578115452"></a><a name="zh-cn_topic_0118921484_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row34892078"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921484_p7686078"><a name="zh-cn_topic_0118921484_p7686078"></a><a name="zh-cn_topic_0118921484_p7686078"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921484_p48128109554"><a name="zh-cn_topic_0118921484_p48128109554"></a><a name="zh-cn_topic_0118921484_p48128109554"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row33115333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921484_p65096331"><a name="zh-cn_topic_0118921484_p65096331"></a><a name="zh-cn_topic_0118921484_p65096331"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921484_p9203142078"><a name="zh-cn_topic_0118921484_p9203142078"></a><a name="zh-cn_topic_0118921484_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row9258873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921484_p11771280"><a name="zh-cn_topic_0118921484_p11771280"></a><a name="zh-cn_topic_0118921484_p11771280"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921484_p13949586"><a name="zh-cn_topic_0118921484_p13949586"></a><a name="zh-cn_topic_0118921484_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921484_row58437416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921484_p35810232"><a name="zh-cn_topic_0118921484_p35810232"></a><a name="zh-cn_topic_0118921484_p35810232"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921484_p14947689"><a name="zh-cn_topic_0118921484_p14947689"></a><a name="zh-cn_topic_0118921484_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

