# 修改API分组<a name="ZH-CN_TOPIC_0000001081976161"></a>

## 功能介绍<a name="zh-cn_topic_0225568807_section60874305"></a>

修改API分组属性。其中name和remark可修改，其他属性不可修改。

## URI<a name="zh-cn_topic_0225568807_section10997834"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568807_table7576160"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568807_row18958597"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568807_p59251354"><a name="zh-cn_topic_0225568807_p59251354"></a><a name="zh-cn_topic_0225568807_p59251354"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568807_p34630347"><a name="zh-cn_topic_0225568807_p34630347"></a><a name="zh-cn_topic_0225568807_p34630347"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568807_row53594754"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p46207780"><a name="zh-cn_topic_0225568807_p46207780"></a><a name="zh-cn_topic_0225568807_p46207780"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p516914488266"><a name="zh-cn_topic_0225568807_p516914488266"></a><a name="zh-cn_topic_0225568807_p516914488266"></a>/v1/{project_id}/apigw/instances/{instance_id}/api-groups/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568807_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568807_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568807_p23103637"><a name="zh-cn_topic_0225568807_p23103637"></a><a name="zh-cn_topic_0225568807_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568807_p59455291"><a name="zh-cn_topic_0225568807_p59455291"></a><a name="zh-cn_topic_0225568807_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568807_p51149303"><a name="zh-cn_topic_0225568807_p51149303"></a><a name="zh-cn_topic_0225568807_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568807_p49452846"><a name="zh-cn_topic_0225568807_p49452846"></a><a name="zh-cn_topic_0225568807_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568807_row123241413191316"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568807_p13125151611313"><a name="zh-cn_topic_0225568807_p13125151611313"></a><a name="zh-cn_topic_0225568807_p13125151611313"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568807_p1012511620138"><a name="zh-cn_topic_0225568807_p1012511620138"></a><a name="zh-cn_topic_0225568807_p1012511620138"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568807_p212591651317"><a name="zh-cn_topic_0225568807_p212591651317"></a><a name="zh-cn_topic_0225568807_p212591651317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568807_p112520160138"><a name="zh-cn_topic_0225568807_p112520160138"></a><a name="zh-cn_topic_0225568807_p112520160138"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row51194135132"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568807_p1780913159538"><a name="zh-cn_topic_0225568807_p1780913159538"></a><a name="zh-cn_topic_0225568807_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568807_p9809215115310"><a name="zh-cn_topic_0225568807_p9809215115310"></a><a name="zh-cn_topic_0225568807_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568807_p1280914152538"><a name="zh-cn_topic_0225568807_p1280914152538"></a><a name="zh-cn_topic_0225568807_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568807_p1880914157537"><a name="zh-cn_topic_0225568807_p1880914157537"></a><a name="zh-cn_topic_0225568807_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568807_p55878963"><a name="zh-cn_topic_0225568807_p55878963"></a><a name="zh-cn_topic_0225568807_p55878963"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568807_p29902160"><a name="zh-cn_topic_0225568807_p29902160"></a><a name="zh-cn_topic_0225568807_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568807_p6155914"><a name="zh-cn_topic_0225568807_p6155914"></a><a name="zh-cn_topic_0225568807_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568807_p28867016"><a name="zh-cn_topic_0225568807_p28867016"></a><a name="zh-cn_topic_0225568807_p28867016"></a>API分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568807_section31871645"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568807_table56526963"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568807_row46508794"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568807_p9115995"><a name="zh-cn_topic_0225568807_p9115995"></a><a name="zh-cn_topic_0225568807_p9115995"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568807_p198169"><a name="zh-cn_topic_0225568807_p198169"></a><a name="zh-cn_topic_0225568807_p198169"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568807_p16051739"><a name="zh-cn_topic_0225568807_p16051739"></a><a name="zh-cn_topic_0225568807_p16051739"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568807_p25122506"><a name="zh-cn_topic_0225568807_p25122506"></a><a name="zh-cn_topic_0225568807_p25122506"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568807_row21657101"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568807_p9394765"><a name="zh-cn_topic_0225568807_p9394765"></a><a name="zh-cn_topic_0225568807_p9394765"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568807_p22778481"><a name="zh-cn_topic_0225568807_p22778481"></a><a name="zh-cn_topic_0225568807_p22778481"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568807_p33117666"><a name="zh-cn_topic_0225568807_p33117666"></a><a name="zh-cn_topic_0225568807_p33117666"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568807_p65285255"><a name="zh-cn_topic_0225568807_p65285255"></a><a name="zh-cn_topic_0225568807_p65285255"></a>名称。</p>
<p id="zh-cn_topic_0225568807_p12766479"><a name="zh-cn_topic_0225568807_p12766479"></a><a name="zh-cn_topic_0225568807_p12766479"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以中文或英文开头。</p>
<div class="note" id="zh-cn_topic_0225568807_note52191124182510"><a name="zh-cn_topic_0225568807_note52191124182510"></a><a name="zh-cn_topic_0225568807_note52191124182510"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568807_p3221202452516"><a name="zh-cn_topic_0225568807_p3221202452516"></a><a name="zh-cn_topic_0225568807_p3221202452516"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row60409228"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568807_p61309300"><a name="zh-cn_topic_0225568807_p61309300"></a><a name="zh-cn_topic_0225568807_p61309300"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568807_p67106281"><a name="zh-cn_topic_0225568807_p67106281"></a><a name="zh-cn_topic_0225568807_p67106281"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568807_p66899666"><a name="zh-cn_topic_0225568807_p66899666"></a><a name="zh-cn_topic_0225568807_p66899666"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568807_p50163864"><a name="zh-cn_topic_0225568807_p50163864"></a><a name="zh-cn_topic_0225568807_p50163864"></a>描述。</p>
<p id="zh-cn_topic_0225568807_p62234932"><a name="zh-cn_topic_0225568807_p62234932"></a><a name="zh-cn_topic_0225568807_p62234932"></a>字符串长度最大不超过255。</p>
<div class="note" id="zh-cn_topic_0225568807_note1065115482519"><a name="zh-cn_topic_0225568807_note1065115482519"></a><a name="zh-cn_topic_0225568807_note1065115482519"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568807_p12672545258"><a name="zh-cn_topic_0225568807_p12672545258"></a><a name="zh-cn_topic_0225568807_p12672545258"></a>中文字符必须为UTF-8或者unicode编码。</p>
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

## 响应消息<a name="zh-cn_topic_0225568807_section31466478"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568807_table60205371"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568807_row46929233"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568807_p43171496"><a name="zh-cn_topic_0225568807_p43171496"></a><a name="zh-cn_topic_0225568807_p43171496"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568807_p7230308"><a name="zh-cn_topic_0225568807_p7230308"></a><a name="zh-cn_topic_0225568807_p7230308"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568807_p48784109"><a name="zh-cn_topic_0225568807_p48784109"></a><a name="zh-cn_topic_0225568807_p48784109"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568807_row59198762"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p30370436"><a name="zh-cn_topic_0225568807_p30370436"></a><a name="zh-cn_topic_0225568807_p30370436"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p44086242"><a name="zh-cn_topic_0225568807_p44086242"></a><a name="zh-cn_topic_0225568807_p44086242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p14215853"><a name="zh-cn_topic_0225568807_p14215853"></a><a name="zh-cn_topic_0225568807_p14215853"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row60833814"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p28591919"><a name="zh-cn_topic_0225568807_p28591919"></a><a name="zh-cn_topic_0225568807_p28591919"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p34244072"><a name="zh-cn_topic_0225568807_p34244072"></a><a name="zh-cn_topic_0225568807_p34244072"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p22306409"><a name="zh-cn_topic_0225568807_p22306409"></a><a name="zh-cn_topic_0225568807_p22306409"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row66539956"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p21027381"><a name="zh-cn_topic_0225568807_p21027381"></a><a name="zh-cn_topic_0225568807_p21027381"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p25496339"><a name="zh-cn_topic_0225568807_p25496339"></a><a name="zh-cn_topic_0225568807_p25496339"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p51937589"><a name="zh-cn_topic_0225568807_p51937589"></a><a name="zh-cn_topic_0225568807_p51937589"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row64785124"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p13103655"><a name="zh-cn_topic_0225568807_p13103655"></a><a name="zh-cn_topic_0225568807_p13103655"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p54763172"><a name="zh-cn_topic_0225568807_p54763172"></a><a name="zh-cn_topic_0225568807_p54763172"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p6631937"><a name="zh-cn_topic_0225568807_p6631937"></a><a name="zh-cn_topic_0225568807_p6631937"></a>系统默认分配的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row59687435"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p2844060"><a name="zh-cn_topic_0225568807_p2844060"></a><a name="zh-cn_topic_0225568807_p2844060"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p29042273"><a name="zh-cn_topic_0225568807_p29042273"></a><a name="zh-cn_topic_0225568807_p29042273"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p3613890"><a name="zh-cn_topic_0225568807_p3613890"></a><a name="zh-cn_topic_0225568807_p3613890"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row32525017"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p17280753"><a name="zh-cn_topic_0225568807_p17280753"></a><a name="zh-cn_topic_0225568807_p17280753"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p57563737"><a name="zh-cn_topic_0225568807_p57563737"></a><a name="zh-cn_topic_0225568807_p57563737"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p32151097"><a name="zh-cn_topic_0225568807_p32151097"></a><a name="zh-cn_topic_0225568807_p32151097"></a>最近修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row20924422"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p17156622"><a name="zh-cn_topic_0225568807_p17156622"></a><a name="zh-cn_topic_0225568807_p17156622"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p47509155"><a name="zh-cn_topic_0225568807_p47509155"></a><a name="zh-cn_topic_0225568807_p47509155"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p23036332"><a name="zh-cn_topic_0225568807_p23036332"></a><a name="zh-cn_topic_0225568807_p23036332"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row6000400"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p16270371"><a name="zh-cn_topic_0225568807_p16270371"></a><a name="zh-cn_topic_0225568807_p16270371"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p42831646"><a name="zh-cn_topic_0225568807_p42831646"></a><a name="zh-cn_topic_0225568807_p42831646"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p46811306"><a name="zh-cn_topic_0225568807_p46811306"></a><a name="zh-cn_topic_0225568807_p46811306"></a>流控时长内分组下的API的总访问次数限制，默认不限，请根据服务的负载能力自行设置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row18648574"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p34139493"><a name="zh-cn_topic_0225568807_p34139493"></a><a name="zh-cn_topic_0225568807_p34139493"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p13835569"><a name="zh-cn_topic_0225568807_p13835569"></a><a name="zh-cn_topic_0225568807_p13835569"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p46939338"><a name="zh-cn_topic_0225568807_p46939338"></a><a name="zh-cn_topic_0225568807_p46939338"></a>流控时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row19800863"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p60366037"><a name="zh-cn_topic_0225568807_p60366037"></a><a name="zh-cn_topic_0225568807_p60366037"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p57810828"><a name="zh-cn_topic_0225568807_p57810828"></a><a name="zh-cn_topic_0225568807_p57810828"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p52165483"><a name="zh-cn_topic_0225568807_p52165483"></a><a name="zh-cn_topic_0225568807_p52165483"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row66836170"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p45020665"><a name="zh-cn_topic_0225568807_p45020665"></a><a name="zh-cn_topic_0225568807_p45020665"></a>url_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p22795237"><a name="zh-cn_topic_0225568807_p22795237"></a><a name="zh-cn_topic_0225568807_p22795237"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p34474869"><a name="zh-cn_topic_0225568807_p34474869"></a><a name="zh-cn_topic_0225568807_p34474869"></a>分组上绑定的独立域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row41838366"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p33464480"><a name="zh-cn_topic_0225568807_p33464480"></a><a name="zh-cn_topic_0225568807_p33464480"></a>on_sell_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p26268346"><a name="zh-cn_topic_0225568807_p26268346"></a><a name="zh-cn_topic_0225568807_p26268346"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p47361301"><a name="zh-cn_topic_0225568807_p47361301"></a><a name="zh-cn_topic_0225568807_p47361301"></a>是否已上架云市场：</p>
<a name="zh-cn_topic_0225568807_ul23598530"></a><a name="zh-cn_topic_0225568807_ul23598530"></a><ul id="zh-cn_topic_0225568807_ul23598530"><li>1：已上架</li><li>2：未上架</li><li>3：审核中</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row93273174419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p3525152172119"><a name="zh-cn_topic_0225568807_p3525152172119"></a><a name="zh-cn_topic_0225568807_p3525152172119"></a>is_default</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p4525952142112"><a name="zh-cn_topic_0225568807_p4525952142112"></a><a name="zh-cn_topic_0225568807_p4525952142112"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p15525652152119"><a name="zh-cn_topic_0225568807_p15525652152119"></a><a name="zh-cn_topic_0225568807_p15525652152119"></a>是否为默认分组，默认为非默认分组：</p>
<a name="zh-cn_topic_0225568807_ul1170161912317"></a><a name="zh-cn_topic_0225568807_ul1170161912317"></a><ul id="zh-cn_topic_0225568807_ul1170161912317"><li>1：默认分组</li><li>2：非默认分组</li></ul>
</td>
</tr>
</tbody>
</table>

**表 5**  url\_domains参数说明

<a name="zh-cn_topic_0225568807_table9811220"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568807_row18394177"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568807_p13533375"><a name="zh-cn_topic_0225568807_p13533375"></a><a name="zh-cn_topic_0225568807_p13533375"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568807_p22461630"><a name="zh-cn_topic_0225568807_p22461630"></a><a name="zh-cn_topic_0225568807_p22461630"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568807_p7452774"><a name="zh-cn_topic_0225568807_p7452774"></a><a name="zh-cn_topic_0225568807_p7452774"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568807_row66803806"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p42399182"><a name="zh-cn_topic_0225568807_p42399182"></a><a name="zh-cn_topic_0225568807_p42399182"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p11781727"><a name="zh-cn_topic_0225568807_p11781727"></a><a name="zh-cn_topic_0225568807_p11781727"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p14795832"><a name="zh-cn_topic_0225568807_p14795832"></a><a name="zh-cn_topic_0225568807_p14795832"></a>域名编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row66053632"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p48743961"><a name="zh-cn_topic_0225568807_p48743961"></a><a name="zh-cn_topic_0225568807_p48743961"></a>domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p55946767"><a name="zh-cn_topic_0225568807_p55946767"></a><a name="zh-cn_topic_0225568807_p55946767"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p35394249"><a name="zh-cn_topic_0225568807_p35394249"></a><a name="zh-cn_topic_0225568807_p35394249"></a>访问域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row50112787"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p32603951"><a name="zh-cn_topic_0225568807_p32603951"></a><a name="zh-cn_topic_0225568807_p32603951"></a>cname_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p23674371"><a name="zh-cn_topic_0225568807_p23674371"></a><a name="zh-cn_topic_0225568807_p23674371"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p38575928"><a name="zh-cn_topic_0225568807_p38575928"></a><a name="zh-cn_topic_0225568807_p38575928"></a>域名cname状态：</p>
<a name="zh-cn_topic_0225568807_ul11639038"></a><a name="zh-cn_topic_0225568807_ul11639038"></a><ul id="zh-cn_topic_0225568807_ul11639038"><li>1：未解析</li><li>2：解析中</li><li>3：解析成功</li><li>4：解析失败</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row11732266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p10789489"><a name="zh-cn_topic_0225568807_p10789489"></a><a name="zh-cn_topic_0225568807_p10789489"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p1533408"><a name="zh-cn_topic_0225568807_p1533408"></a><a name="zh-cn_topic_0225568807_p1533408"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p57097248"><a name="zh-cn_topic_0225568807_p57097248"></a><a name="zh-cn_topic_0225568807_p57097248"></a>SSL证书编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row967016619319"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568807_p667011623113"><a name="zh-cn_topic_0225568807_p667011623113"></a><a name="zh-cn_topic_0225568807_p667011623113"></a>ssl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568807_p967017623110"><a name="zh-cn_topic_0225568807_p967017623110"></a><a name="zh-cn_topic_0225568807_p967017623110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568807_p76701261314"><a name="zh-cn_topic_0225568807_p76701261314"></a><a name="zh-cn_topic_0225568807_p76701261314"></a>SSL证书名称</p>
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
	"remark": "分组001",
	"register_time": "2017-12-28T11:44:53Z",
	"update_time": "2017-12-28T11:49:01.048600577Z",
	"on_sell_status": 2,
        "is_default": 2
}
```

## 状态码<a name="zh-cn_topic_0225568807_section18409356"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0225568807_table16737159"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568807_row283921"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568807_p22997658"><a name="zh-cn_topic_0225568807_p22997658"></a><a name="zh-cn_topic_0225568807_p22997658"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568807_p50870979"><a name="zh-cn_topic_0225568807_p50870979"></a><a name="zh-cn_topic_0225568807_p50870979"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568807_row26908596"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p32112662"><a name="zh-cn_topic_0225568807_p32112662"></a><a name="zh-cn_topic_0225568807_p32112662"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p50988816"><a name="zh-cn_topic_0225568807_p50988816"></a><a name="zh-cn_topic_0225568807_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row56246166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p59645608"><a name="zh-cn_topic_0225568807_p59645608"></a><a name="zh-cn_topic_0225568807_p59645608"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p66564967"><a name="zh-cn_topic_0225568807_p66564967"></a><a name="zh-cn_topic_0225568807_p66564967"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row62213794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p6152591"><a name="zh-cn_topic_0225568807_p6152591"></a><a name="zh-cn_topic_0225568807_p6152591"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p28597852"><a name="zh-cn_topic_0225568807_p28597852"></a><a name="zh-cn_topic_0225568807_p28597852"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row56054078"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p44086463"><a name="zh-cn_topic_0225568807_p44086463"></a><a name="zh-cn_topic_0225568807_p44086463"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p13949586"><a name="zh-cn_topic_0225568807_p13949586"></a><a name="zh-cn_topic_0225568807_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row60994581"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p41614068"><a name="zh-cn_topic_0225568807_p41614068"></a><a name="zh-cn_topic_0225568807_p41614068"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p15296380"><a name="zh-cn_topic_0225568807_p15296380"></a><a name="zh-cn_topic_0225568807_p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row3449694"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p10989813"><a name="zh-cn_topic_0225568807_p10989813"></a><a name="zh-cn_topic_0225568807_p10989813"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p1315733818249"><a name="zh-cn_topic_0225568807_p1315733818249"></a><a name="zh-cn_topic_0225568807_p1315733818249"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568807_row25619477"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568807_p61911758"><a name="zh-cn_topic_0225568807_p61911758"></a><a name="zh-cn_topic_0225568807_p61911758"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568807_p1767615692518"><a name="zh-cn_topic_0225568807_p1767615692518"></a><a name="zh-cn_topic_0225568807_p1767615692518"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

