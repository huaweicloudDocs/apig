# 修改流控策略<a name="ZH-CN_TOPIC_0000001081976117"></a>

## 功能介绍<a name="zh-cn_topic_0118922257_section259811"></a>

修改指定流控策略的详细信息。

## URI<a name="zh-cn_topic_0118922257_section2338307"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922257_table27759637"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922257_row1039285"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922257_p17073270"><a name="zh-cn_topic_0118922257_p17073270"></a><a name="zh-cn_topic_0118922257_p17073270"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922257_p40757631"><a name="zh-cn_topic_0118922257_p40757631"></a><a name="zh-cn_topic_0118922257_p40757631"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922257_row13033849"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922257_p49108876"><a name="zh-cn_topic_0118922257_p49108876"></a><a name="zh-cn_topic_0118922257_p49108876"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922257_p18395999"><a name="zh-cn_topic_0118922257_p18395999"></a><a name="zh-cn_topic_0118922257_p18395999"></a>/v1.0/apigw/throttles/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922257_table13680922"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922257_row53894077"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922257_p3344091"><a name="zh-cn_topic_0118922257_p3344091"></a><a name="zh-cn_topic_0118922257_p3344091"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922257_p2435921"><a name="zh-cn_topic_0118922257_p2435921"></a><a name="zh-cn_topic_0118922257_p2435921"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922257_p63091912"><a name="zh-cn_topic_0118922257_p63091912"></a><a name="zh-cn_topic_0118922257_p63091912"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922257_p10171239"><a name="zh-cn_topic_0118922257_p10171239"></a><a name="zh-cn_topic_0118922257_p10171239"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922257_row18564055"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p27293504"><a name="zh-cn_topic_0118922257_p27293504"></a><a name="zh-cn_topic_0118922257_p27293504"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p63290185"><a name="zh-cn_topic_0118922257_p63290185"></a><a name="zh-cn_topic_0118922257_p63290185"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p26231322"><a name="zh-cn_topic_0118922257_p26231322"></a><a name="zh-cn_topic_0118922257_p26231322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p44362332"><a name="zh-cn_topic_0118922257_p44362332"></a><a name="zh-cn_topic_0118922257_p44362332"></a>流控策略编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922257_section21044768"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118922257_table36579126"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922257_row15332661"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922257_p33986018"><a name="zh-cn_topic_0118922257_p33986018"></a><a name="zh-cn_topic_0118922257_p33986018"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="11.110000000000001%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922257_p1404055"><a name="zh-cn_topic_0118922257_p1404055"></a><a name="zh-cn_topic_0118922257_p1404055"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922257_p46619645"><a name="zh-cn_topic_0118922257_p46619645"></a><a name="zh-cn_topic_0118922257_p46619645"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922257_p18094907"><a name="zh-cn_topic_0118922257_p18094907"></a><a name="zh-cn_topic_0118922257_p18094907"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922257_row56401402"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p5110882"><a name="zh-cn_topic_0118922257_p5110882"></a><a name="zh-cn_topic_0118922257_p5110882"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p11328282"><a name="zh-cn_topic_0118922257_p11328282"></a><a name="zh-cn_topic_0118922257_p11328282"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p45175626"><a name="zh-cn_topic_0118922257_p45175626"></a><a name="zh-cn_topic_0118922257_p45175626"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p35347099"><a name="zh-cn_topic_0118922257_p35347099"></a><a name="zh-cn_topic_0118922257_p35347099"></a>流控策略名称。</p>
<p id="zh-cn_topic_0118922257_p65340636"><a name="zh-cn_topic_0118922257_p65340636"></a><a name="zh-cn_topic_0118922257_p65340636"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0118922257_note19624735759"><a name="zh-cn_topic_0118922257_note19624735759"></a><a name="zh-cn_topic_0118922257_note19624735759"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118922257_p19625835459"><a name="zh-cn_topic_0118922257_p19625835459"></a><a name="zh-cn_topic_0118922257_p19625835459"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row16380687"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p51767275"><a name="zh-cn_topic_0118922257_p51767275"></a><a name="zh-cn_topic_0118922257_p51767275"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p32399743"><a name="zh-cn_topic_0118922257_p32399743"></a><a name="zh-cn_topic_0118922257_p32399743"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p7133556"><a name="zh-cn_topic_0118922257_p7133556"></a><a name="zh-cn_topic_0118922257_p7133556"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p40947186"><a name="zh-cn_topic_0118922257_p40947186"></a><a name="zh-cn_topic_0118922257_p40947186"></a>API流量限制是指时长内一个API能够被访问的次数上限。该值不超过系统默认配额限制，系统默认配额为200tps，用户可根据实际情况修改该系统默认配额。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row54163104"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p25135322"><a name="zh-cn_topic_0118922257_p25135322"></a><a name="zh-cn_topic_0118922257_p25135322"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p22695192"><a name="zh-cn_topic_0118922257_p22695192"></a><a name="zh-cn_topic_0118922257_p22695192"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p26371267"><a name="zh-cn_topic_0118922257_p26371267"></a><a name="zh-cn_topic_0118922257_p26371267"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p55697858"><a name="zh-cn_topic_0118922257_p55697858"></a><a name="zh-cn_topic_0118922257_p55697858"></a>用户流量限制是指一个API在时长之内每一个用户能访问的次数上限，该数值不超过API流量限制值。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row2876014"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p31630543"><a name="zh-cn_topic_0118922257_p31630543"></a><a name="zh-cn_topic_0118922257_p31630543"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p11937185"><a name="zh-cn_topic_0118922257_p11937185"></a><a name="zh-cn_topic_0118922257_p11937185"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p27387915"><a name="zh-cn_topic_0118922257_p27387915"></a><a name="zh-cn_topic_0118922257_p27387915"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p3828662"><a name="zh-cn_topic_0118922257_p3828662"></a><a name="zh-cn_topic_0118922257_p3828662"></a>APP流量限制是指一个API在时长之内被每个APP访问的次数上限，该数值不超过用户流量限制值。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row9670163410328"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p787433222711"><a name="zh-cn_topic_0118922257_p787433222711"></a><a name="zh-cn_topic_0118922257_p787433222711"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p787443219272"><a name="zh-cn_topic_0118922257_p787443219272"></a><a name="zh-cn_topic_0118922257_p787443219272"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p288943212278"><a name="zh-cn_topic_0118922257_p288943212278"></a><a name="zh-cn_topic_0118922257_p288943212278"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p18889193272718"><a name="zh-cn_topic_0118922257_p18889193272718"></a><a name="zh-cn_topic_0118922257_p18889193272718"></a>源IP流量限制是指一个API在时长之内被每个IP访问的次数上限，该数值不超过API流量限制值。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row39631642"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p56046429"><a name="zh-cn_topic_0118922257_p56046429"></a><a name="zh-cn_topic_0118922257_p56046429"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p43466909"><a name="zh-cn_topic_0118922257_p43466909"></a><a name="zh-cn_topic_0118922257_p43466909"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p31158721"><a name="zh-cn_topic_0118922257_p31158721"></a><a name="zh-cn_topic_0118922257_p31158721"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p40828466"><a name="zh-cn_topic_0118922257_p40828466"></a><a name="zh-cn_topic_0118922257_p40828466"></a>流量控制的时长单位。与“流量限制次数”配合使用，表示单位时间内的API请求次数上限。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row34725008"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p61262303"><a name="zh-cn_topic_0118922257_p61262303"></a><a name="zh-cn_topic_0118922257_p61262303"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p63299543"><a name="zh-cn_topic_0118922257_p63299543"></a><a name="zh-cn_topic_0118922257_p63299543"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p26989343"><a name="zh-cn_topic_0118922257_p26989343"></a><a name="zh-cn_topic_0118922257_p26989343"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p38653151"><a name="zh-cn_topic_0118922257_p38653151"></a><a name="zh-cn_topic_0118922257_p38653151"></a>流控的时间单位：</p>
<a name="zh-cn_topic_0118922257_ul47601667"></a><a name="zh-cn_topic_0118922257_ul47601667"></a><ul id="zh-cn_topic_0118922257_ul47601667"><li>SECOND</li><li>MINUTE</li><li>HOUR</li><li>DAY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row43223922"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p11476776"><a name="zh-cn_topic_0118922257_p11476776"></a><a name="zh-cn_topic_0118922257_p11476776"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p57203700"><a name="zh-cn_topic_0118922257_p57203700"></a><a name="zh-cn_topic_0118922257_p57203700"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p2988091"><a name="zh-cn_topic_0118922257_p2988091"></a><a name="zh-cn_topic_0118922257_p2988091"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p40708839"><a name="zh-cn_topic_0118922257_p40708839"></a><a name="zh-cn_topic_0118922257_p40708839"></a>流控策略描述</p>
<p id="zh-cn_topic_0118922257_p14626405"><a name="zh-cn_topic_0118922257_p14626405"></a><a name="zh-cn_topic_0118922257_p14626405"></a>字符长度不超过255。</p>
<div class="note" id="zh-cn_topic_0118922257_note1058191014617"><a name="zh-cn_topic_0118922257_note1058191014617"></a><a name="zh-cn_topic_0118922257_note1058191014617"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118922257_p5581181016612"><a name="zh-cn_topic_0118922257_p5581181016612"></a><a name="zh-cn_topic_0118922257_p5581181016612"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row0484201077"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p104841811779"><a name="zh-cn_topic_0118922257_p104841811779"></a><a name="zh-cn_topic_0118922257_p104841811779"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p5484711077"><a name="zh-cn_topic_0118922257_p5484711077"></a><a name="zh-cn_topic_0118922257_p5484711077"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p748451375"><a name="zh-cn_topic_0118922257_p748451375"></a><a name="zh-cn_topic_0118922257_p748451375"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p15805453105915"><a name="zh-cn_topic_0118922257_p15805453105915"></a><a name="zh-cn_topic_0118922257_p15805453105915"></a>流控策略的类型，取值如下：</p>
<a name="zh-cn_topic_0118922257_ul1043012241502"></a><a name="zh-cn_topic_0118922257_ul1043012241502"></a><ul id="zh-cn_topic_0118922257_ul1043012241502"><li>1：独享，表示绑定到流控策略的单个API流控时间内能够被调用多少次</li><li>2：共享，表示绑定到流控策略的所有API流控时间内能够被调用多少次</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row165349494563"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922257_p189261354175913"><a name="zh-cn_topic_0118922257_p189261354175913"></a><a name="zh-cn_topic_0118922257_p189261354175913"></a>enable_adaptive_control</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922257_p792615541592"><a name="zh-cn_topic_0118922257_p792615541592"></a><a name="zh-cn_topic_0118922257_p792615541592"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922257_p15926654165919"><a name="zh-cn_topic_0118922257_p15926654165919"></a><a name="zh-cn_topic_0118922257_p15926654165919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922257_p173718104565"><a name="zh-cn_topic_0118922257_p173718104565"></a><a name="zh-cn_topic_0118922257_p173718104565"></a>是否开启动态流控：</p>
<a name="zh-cn_topic_0118922257_ul173711210185620"></a><a name="zh-cn_topic_0118922257_ul173711210185620"></a><ul id="zh-cn_topic_0118922257_ul173711210185620"><li>TRUE</li><li>FALSE</li></ul>
<p id="zh-cn_topic_0118922257_p209261544595"><a name="zh-cn_topic_0118922257_p209261544595"></a><a name="zh-cn_topic_0118922257_p209261544595"></a>暂不支持</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"api_call_limits": 1000,
        "user_call_limits": 500,
	"app_call_limits": 300,
        "ip_call_limits": 600,
	"name": "每秒1000次",
	"remark": "API每秒1000次，用户500次，APP300次，IP600次",
	"time_interval": 1,
	"time_unit": "SECOND"
}
```

## 响应消息<a name="zh-cn_topic_0118922257_section26904637"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0118922257_table41188542"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922257_row17122516"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922257_p44746546"><a name="zh-cn_topic_0118922257_p44746546"></a><a name="zh-cn_topic_0118922257_p44746546"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922257_p591613"><a name="zh-cn_topic_0118922257_p591613"></a><a name="zh-cn_topic_0118922257_p591613"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922257_p47920668"><a name="zh-cn_topic_0118922257_p47920668"></a><a name="zh-cn_topic_0118922257_p47920668"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922257_row56368888"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p2477176"><a name="zh-cn_topic_0118922257_p2477176"></a><a name="zh-cn_topic_0118922257_p2477176"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p66433540"><a name="zh-cn_topic_0118922257_p66433540"></a><a name="zh-cn_topic_0118922257_p66433540"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p12407685"><a name="zh-cn_topic_0118922257_p12407685"></a><a name="zh-cn_topic_0118922257_p12407685"></a>流控策略的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row44560309"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p52615296"><a name="zh-cn_topic_0118922257_p52615296"></a><a name="zh-cn_topic_0118922257_p52615296"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p33980596"><a name="zh-cn_topic_0118922257_p33980596"></a><a name="zh-cn_topic_0118922257_p33980596"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p964855"><a name="zh-cn_topic_0118922257_p964855"></a><a name="zh-cn_topic_0118922257_p964855"></a>流控策略的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row8683703"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p32291351"><a name="zh-cn_topic_0118922257_p32291351"></a><a name="zh-cn_topic_0118922257_p32291351"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p65462619"><a name="zh-cn_topic_0118922257_p65462619"></a><a name="zh-cn_topic_0118922257_p65462619"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p871916"><a name="zh-cn_topic_0118922257_p871916"></a><a name="zh-cn_topic_0118922257_p871916"></a>单个API流控时间内能够被访问的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row7847244"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p31647034"><a name="zh-cn_topic_0118922257_p31647034"></a><a name="zh-cn_topic_0118922257_p31647034"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p13273001"><a name="zh-cn_topic_0118922257_p13273001"></a><a name="zh-cn_topic_0118922257_p13273001"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p1371329"><a name="zh-cn_topic_0118922257_p1371329"></a><a name="zh-cn_topic_0118922257_p1371329"></a>单个用户流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row12341963"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p60174962"><a name="zh-cn_topic_0118922257_p60174962"></a><a name="zh-cn_topic_0118922257_p60174962"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p42333782"><a name="zh-cn_topic_0118922257_p42333782"></a><a name="zh-cn_topic_0118922257_p42333782"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p6484318"><a name="zh-cn_topic_0118922257_p6484318"></a><a name="zh-cn_topic_0118922257_p6484318"></a>单个APP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row06447015331"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p71235716345"><a name="zh-cn_topic_0118922257_p71235716345"></a><a name="zh-cn_topic_0118922257_p71235716345"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p612135773413"><a name="zh-cn_topic_0118922257_p612135773413"></a><a name="zh-cn_topic_0118922257_p612135773413"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p12122573347"><a name="zh-cn_topic_0118922257_p12122573347"></a><a name="zh-cn_topic_0118922257_p12122573347"></a>单个IP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row58358867"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p29447821"><a name="zh-cn_topic_0118922257_p29447821"></a><a name="zh-cn_topic_0118922257_p29447821"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p36463328"><a name="zh-cn_topic_0118922257_p36463328"></a><a name="zh-cn_topic_0118922257_p36463328"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p739571"><a name="zh-cn_topic_0118922257_p739571"></a><a name="zh-cn_topic_0118922257_p739571"></a>流控的时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row6656140"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p2276450"><a name="zh-cn_topic_0118922257_p2276450"></a><a name="zh-cn_topic_0118922257_p2276450"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p50174798"><a name="zh-cn_topic_0118922257_p50174798"></a><a name="zh-cn_topic_0118922257_p50174798"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p37626805"><a name="zh-cn_topic_0118922257_p37626805"></a><a name="zh-cn_topic_0118922257_p37626805"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row3096931"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p49524881"><a name="zh-cn_topic_0118922257_p49524881"></a><a name="zh-cn_topic_0118922257_p49524881"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p52092399"><a name="zh-cn_topic_0118922257_p52092399"></a><a name="zh-cn_topic_0118922257_p52092399"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p58734757"><a name="zh-cn_topic_0118922257_p58734757"></a><a name="zh-cn_topic_0118922257_p58734757"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row58850769"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p2182975"><a name="zh-cn_topic_0118922257_p2182975"></a><a name="zh-cn_topic_0118922257_p2182975"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p42603290"><a name="zh-cn_topic_0118922257_p42603290"></a><a name="zh-cn_topic_0118922257_p42603290"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p28314441"><a name="zh-cn_topic_0118922257_p28314441"></a><a name="zh-cn_topic_0118922257_p28314441"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row53503380"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p38806493"><a name="zh-cn_topic_0118922257_p38806493"></a><a name="zh-cn_topic_0118922257_p38806493"></a>is_include_special_throttle</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p56318190"><a name="zh-cn_topic_0118922257_p56318190"></a><a name="zh-cn_topic_0118922257_p56318190"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p132991651162513"><a name="zh-cn_topic_0118922257_p132991651162513"></a><a name="zh-cn_topic_0118922257_p132991651162513"></a>是否包含特殊流控配置：</p>
<a name="zh-cn_topic_0118922257_ul107800420518"></a><a name="zh-cn_topic_0118922257_ul107800420518"></a><ul id="zh-cn_topic_0118922257_ul107800420518"><li>1：包含</li><li>2：不包含</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row862715275"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p16621715679"><a name="zh-cn_topic_0118922257_p16621715679"></a><a name="zh-cn_topic_0118922257_p16621715679"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p156210151879"><a name="zh-cn_topic_0118922257_p156210151879"></a><a name="zh-cn_topic_0118922257_p156210151879"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p34377220718"><a name="zh-cn_topic_0118922257_p34377220718"></a><a name="zh-cn_topic_0118922257_p34377220718"></a>流控策略的类型，取值如下：</p>
<a name="zh-cn_topic_0118922257_ul2437522975"></a><a name="zh-cn_topic_0118922257_ul2437522975"></a><ul id="zh-cn_topic_0118922257_ul2437522975"><li>1   独享</li><li>2   共享</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row6883317155714"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p14797139472"><a name="zh-cn_topic_0118922257_p14797139472"></a><a name="zh-cn_topic_0118922257_p14797139472"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p147913137471"><a name="zh-cn_topic_0118922257_p147913137471"></a><a name="zh-cn_topic_0118922257_p147913137471"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p11798139474"><a name="zh-cn_topic_0118922257_p11798139474"></a><a name="zh-cn_topic_0118922257_p11798139474"></a>流控绑定的API数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row87946216574"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922257_p19770121614477"><a name="zh-cn_topic_0118922257_p19770121614477"></a><a name="zh-cn_topic_0118922257_p19770121614477"></a>enable_adaptive_control</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922257_p27566352475"><a name="zh-cn_topic_0118922257_p27566352475"></a><a name="zh-cn_topic_0118922257_p27566352475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922257_p39161837145716"><a name="zh-cn_topic_0118922257_p39161837145716"></a><a name="zh-cn_topic_0118922257_p39161837145716"></a>是否开启动态流控：</p>
<a name="zh-cn_topic_0118922257_ul17916103725711"></a><a name="zh-cn_topic_0118922257_ul17916103725711"></a><ul id="zh-cn_topic_0118922257_ul17916103725711"><li>TRUE</li><li>FALSE</li></ul>
<p id="zh-cn_topic_0118922257_p159161937155713"><a name="zh-cn_topic_0118922257_p159161937155713"></a><a name="zh-cn_topic_0118922257_p159161937155713"></a>暂不支持</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "0325b671-2d50-4614-9868-22102262695d",
	"name": "每秒1000次",
	"api_call_limits": 1000,
	"user_call_limits": 500,
	"app_call_limits": 300,
        "ip_call_limits": 600,
	"time_interval": 1,
	"time_unit": "SECOND",
	"create_time": "2017-12-29T01:55:59Z",
	"remark": "API每秒1000次，用户500次，APP300次，IP600次",
	"is_inclu_special_throttle": 2,
        "type":1,
	"bind_num": 0,
        "enable_adaptive_control": "FALSE"
}
```

## 状态码<a name="zh-cn_topic_0118922257_section55185187"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118922257_table7940832"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922257_row8599479"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922257_p25469194"><a name="zh-cn_topic_0118922257_p25469194"></a><a name="zh-cn_topic_0118922257_p25469194"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922257_p49738842"><a name="zh-cn_topic_0118922257_p49738842"></a><a name="zh-cn_topic_0118922257_p49738842"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922257_row2314382"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922257_p53247247"><a name="zh-cn_topic_0118922257_p53247247"></a><a name="zh-cn_topic_0118922257_p53247247"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922257_p18059716"><a name="zh-cn_topic_0118922257_p18059716"></a><a name="zh-cn_topic_0118922257_p18059716"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row28319717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922257_p12195780"><a name="zh-cn_topic_0118922257_p12195780"></a><a name="zh-cn_topic_0118922257_p12195780"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922257_p48334156"><a name="zh-cn_topic_0118922257_p48334156"></a><a name="zh-cn_topic_0118922257_p48334156"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row32354222"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922257_p3446341"><a name="zh-cn_topic_0118922257_p3446341"></a><a name="zh-cn_topic_0118922257_p3446341"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922257_p10718233"><a name="zh-cn_topic_0118922257_p10718233"></a><a name="zh-cn_topic_0118922257_p10718233"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row29355237"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922257_p28963998"><a name="zh-cn_topic_0118922257_p28963998"></a><a name="zh-cn_topic_0118922257_p28963998"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922257_p64382536"><a name="zh-cn_topic_0118922257_p64382536"></a><a name="zh-cn_topic_0118922257_p64382536"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row42571919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922257_p25773413"><a name="zh-cn_topic_0118922257_p25773413"></a><a name="zh-cn_topic_0118922257_p25773413"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922257_p7271679"><a name="zh-cn_topic_0118922257_p7271679"></a><a name="zh-cn_topic_0118922257_p7271679"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922257_row65445113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922257_p66562805"><a name="zh-cn_topic_0118922257_p66562805"></a><a name="zh-cn_topic_0118922257_p66562805"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922257_p14947689"><a name="zh-cn_topic_0118922257_p14947689"></a><a name="zh-cn_topic_0118922257_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

