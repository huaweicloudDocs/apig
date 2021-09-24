# 查看流控策略详情<a name="ZH-CN_TOPIC_0000001082135111"></a>

## 功能介绍<a name="zh-cn_topic_0118922259_section21326661"></a>

查看指定流控策略的详细信息。

## URI<a name="zh-cn_topic_0118922259_section57722223"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922259_table18452253"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922259_row1143559"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922259_p25519489"><a name="zh-cn_topic_0118922259_p25519489"></a><a name="zh-cn_topic_0118922259_p25519489"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922259_p53812756"><a name="zh-cn_topic_0118922259_p53812756"></a><a name="zh-cn_topic_0118922259_p53812756"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922259_row63865959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922259_p5760162"><a name="zh-cn_topic_0118922259_p5760162"></a><a name="zh-cn_topic_0118922259_p5760162"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922259_p63919982"><a name="zh-cn_topic_0118922259_p63919982"></a><a name="zh-cn_topic_0118922259_p63919982"></a>/v1.0/apigw/throttles/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922259_table10136050"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922259_row39134681"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922259_p15792592"><a name="zh-cn_topic_0118922259_p15792592"></a><a name="zh-cn_topic_0118922259_p15792592"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922259_p4131567"><a name="zh-cn_topic_0118922259_p4131567"></a><a name="zh-cn_topic_0118922259_p4131567"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922259_p66221535"><a name="zh-cn_topic_0118922259_p66221535"></a><a name="zh-cn_topic_0118922259_p66221535"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922259_p62344136"><a name="zh-cn_topic_0118922259_p62344136"></a><a name="zh-cn_topic_0118922259_p62344136"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922259_row16710225"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922259_p11350946"><a name="zh-cn_topic_0118922259_p11350946"></a><a name="zh-cn_topic_0118922259_p11350946"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922259_p47011428"><a name="zh-cn_topic_0118922259_p47011428"></a><a name="zh-cn_topic_0118922259_p47011428"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922259_p49829310"><a name="zh-cn_topic_0118922259_p49829310"></a><a name="zh-cn_topic_0118922259_p49829310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922259_p9642329"><a name="zh-cn_topic_0118922259_p9642329"></a><a name="zh-cn_topic_0118922259_p9642329"></a>流控策略的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922259_section49737962"></a>

无

## 响应消息<a name="zh-cn_topic_0118922259_section2243136"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118922259_table64157230"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922259_row53015562"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922259_p66402118"><a name="zh-cn_topic_0118922259_p66402118"></a><a name="zh-cn_topic_0118922259_p66402118"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922259_p9862438"><a name="zh-cn_topic_0118922259_p9862438"></a><a name="zh-cn_topic_0118922259_p9862438"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922259_p60659986"><a name="zh-cn_topic_0118922259_p60659986"></a><a name="zh-cn_topic_0118922259_p60659986"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922259_row14511859"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p34609969"><a name="zh-cn_topic_0118922259_p34609969"></a><a name="zh-cn_topic_0118922259_p34609969"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p51944115"><a name="zh-cn_topic_0118922259_p51944115"></a><a name="zh-cn_topic_0118922259_p51944115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p46723810"><a name="zh-cn_topic_0118922259_p46723810"></a><a name="zh-cn_topic_0118922259_p46723810"></a>流控策略的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row17861109"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p37463762"><a name="zh-cn_topic_0118922259_p37463762"></a><a name="zh-cn_topic_0118922259_p37463762"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p14665871"><a name="zh-cn_topic_0118922259_p14665871"></a><a name="zh-cn_topic_0118922259_p14665871"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p47084884"><a name="zh-cn_topic_0118922259_p47084884"></a><a name="zh-cn_topic_0118922259_p47084884"></a>流控策略的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row21110778"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p32251423"><a name="zh-cn_topic_0118922259_p32251423"></a><a name="zh-cn_topic_0118922259_p32251423"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p62228448"><a name="zh-cn_topic_0118922259_p62228448"></a><a name="zh-cn_topic_0118922259_p62228448"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p7339559"><a name="zh-cn_topic_0118922259_p7339559"></a><a name="zh-cn_topic_0118922259_p7339559"></a>单个API流控时间内能够被访问的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row66056031"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p48938279"><a name="zh-cn_topic_0118922259_p48938279"></a><a name="zh-cn_topic_0118922259_p48938279"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p4577639"><a name="zh-cn_topic_0118922259_p4577639"></a><a name="zh-cn_topic_0118922259_p4577639"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p35244488"><a name="zh-cn_topic_0118922259_p35244488"></a><a name="zh-cn_topic_0118922259_p35244488"></a>单个用户流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row48764940"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p57646081"><a name="zh-cn_topic_0118922259_p57646081"></a><a name="zh-cn_topic_0118922259_p57646081"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p38820970"><a name="zh-cn_topic_0118922259_p38820970"></a><a name="zh-cn_topic_0118922259_p38820970"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p57490864"><a name="zh-cn_topic_0118922259_p57490864"></a><a name="zh-cn_topic_0118922259_p57490864"></a>单个APP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row6236445154113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p71235716345"><a name="zh-cn_topic_0118922259_p71235716345"></a><a name="zh-cn_topic_0118922259_p71235716345"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p612135773413"><a name="zh-cn_topic_0118922259_p612135773413"></a><a name="zh-cn_topic_0118922259_p612135773413"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p12122573347"><a name="zh-cn_topic_0118922259_p12122573347"></a><a name="zh-cn_topic_0118922259_p12122573347"></a>单个IP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row47655729"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p34908812"><a name="zh-cn_topic_0118922259_p34908812"></a><a name="zh-cn_topic_0118922259_p34908812"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p9041528"><a name="zh-cn_topic_0118922259_p9041528"></a><a name="zh-cn_topic_0118922259_p9041528"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p61275164"><a name="zh-cn_topic_0118922259_p61275164"></a><a name="zh-cn_topic_0118922259_p61275164"></a>流控的时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row14605571"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p42200623"><a name="zh-cn_topic_0118922259_p42200623"></a><a name="zh-cn_topic_0118922259_p42200623"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p62807336"><a name="zh-cn_topic_0118922259_p62807336"></a><a name="zh-cn_topic_0118922259_p62807336"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p54229461"><a name="zh-cn_topic_0118922259_p54229461"></a><a name="zh-cn_topic_0118922259_p54229461"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row18303107"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p6156698"><a name="zh-cn_topic_0118922259_p6156698"></a><a name="zh-cn_topic_0118922259_p6156698"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p28930521"><a name="zh-cn_topic_0118922259_p28930521"></a><a name="zh-cn_topic_0118922259_p28930521"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p61670889"><a name="zh-cn_topic_0118922259_p61670889"></a><a name="zh-cn_topic_0118922259_p61670889"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row18167095"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p62248579"><a name="zh-cn_topic_0118922259_p62248579"></a><a name="zh-cn_topic_0118922259_p62248579"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p8970099"><a name="zh-cn_topic_0118922259_p8970099"></a><a name="zh-cn_topic_0118922259_p8970099"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p55489391"><a name="zh-cn_topic_0118922259_p55489391"></a><a name="zh-cn_topic_0118922259_p55489391"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row29642478"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p52230504"><a name="zh-cn_topic_0118922259_p52230504"></a><a name="zh-cn_topic_0118922259_p52230504"></a>is_include_special_throttle</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p2812451"><a name="zh-cn_topic_0118922259_p2812451"></a><a name="zh-cn_topic_0118922259_p2812451"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><div class="p" id="zh-cn_topic_0118922259_p18848323122613"><a name="zh-cn_topic_0118922259_p18848323122613"></a><a name="zh-cn_topic_0118922259_p18848323122613"></a>是否包含特殊流控配置：<a name="zh-cn_topic_0118922259_ul107800420518"></a><a name="zh-cn_topic_0118922259_ul107800420518"></a><ul id="zh-cn_topic_0118922259_ul107800420518"><li>1：包含</li><li>2：不包含</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row1896612488715"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p1696617481179"><a name="zh-cn_topic_0118922259_p1696617481179"></a><a name="zh-cn_topic_0118922259_p1696617481179"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p29661548174"><a name="zh-cn_topic_0118922259_p29661548174"></a><a name="zh-cn_topic_0118922259_p29661548174"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p15805453105915"><a name="zh-cn_topic_0118922259_p15805453105915"></a><a name="zh-cn_topic_0118922259_p15805453105915"></a>流控策略的类型，取值如下：</p>
<a name="zh-cn_topic_0118922259_ul1043012241502"></a><a name="zh-cn_topic_0118922259_ul1043012241502"></a><ul id="zh-cn_topic_0118922259_ul1043012241502"><li>1   独享</li><li>2   共享</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row136066712588"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p14797139472"><a name="zh-cn_topic_0118922259_p14797139472"></a><a name="zh-cn_topic_0118922259_p14797139472"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p147913137471"><a name="zh-cn_topic_0118922259_p147913137471"></a><a name="zh-cn_topic_0118922259_p147913137471"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p11798139474"><a name="zh-cn_topic_0118922259_p11798139474"></a><a name="zh-cn_topic_0118922259_p11798139474"></a>流控绑定的API数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row18943121015817"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922259_p19770121614477"><a name="zh-cn_topic_0118922259_p19770121614477"></a><a name="zh-cn_topic_0118922259_p19770121614477"></a>enable_adaptive_control</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922259_p27566352475"><a name="zh-cn_topic_0118922259_p27566352475"></a><a name="zh-cn_topic_0118922259_p27566352475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922259_p39161837145716"><a name="zh-cn_topic_0118922259_p39161837145716"></a><a name="zh-cn_topic_0118922259_p39161837145716"></a>是否开启动态流控：</p>
<a name="zh-cn_topic_0118922259_ul17916103725711"></a><a name="zh-cn_topic_0118922259_ul17916103725711"></a><ul id="zh-cn_topic_0118922259_ul17916103725711"><li>TRUE</li><li>FALSE</li></ul>
<p id="zh-cn_topic_0118922259_p159161937155713"><a name="zh-cn_topic_0118922259_p159161937155713"></a><a name="zh-cn_topic_0118922259_p159161937155713"></a>暂不支持</p>
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

## 状态码<a name="zh-cn_topic_0118922259_section44988480"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118922259_table46774896"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922259_row11374652"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922259_p48931613"><a name="zh-cn_topic_0118922259_p48931613"></a><a name="zh-cn_topic_0118922259_p48931613"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922259_p4037682"><a name="zh-cn_topic_0118922259_p4037682"></a><a name="zh-cn_topic_0118922259_p4037682"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922259_row58616803"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922259_p50340634"><a name="zh-cn_topic_0118922259_p50340634"></a><a name="zh-cn_topic_0118922259_p50340634"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922259_p51059516"><a name="zh-cn_topic_0118922259_p51059516"></a><a name="zh-cn_topic_0118922259_p51059516"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row56882466"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922259_p44077010"><a name="zh-cn_topic_0118922259_p44077010"></a><a name="zh-cn_topic_0118922259_p44077010"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922259_p13468067"><a name="zh-cn_topic_0118922259_p13468067"></a><a name="zh-cn_topic_0118922259_p13468067"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row54103743"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922259_p20327076"><a name="zh-cn_topic_0118922259_p20327076"></a><a name="zh-cn_topic_0118922259_p20327076"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922259_p35880445"><a name="zh-cn_topic_0118922259_p35880445"></a><a name="zh-cn_topic_0118922259_p35880445"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row54488553"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922259_p51496652"><a name="zh-cn_topic_0118922259_p51496652"></a><a name="zh-cn_topic_0118922259_p51496652"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922259_p10479255"><a name="zh-cn_topic_0118922259_p10479255"></a><a name="zh-cn_topic_0118922259_p10479255"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row27204435"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922259_p56075663"><a name="zh-cn_topic_0118922259_p56075663"></a><a name="zh-cn_topic_0118922259_p56075663"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922259_p45834822"><a name="zh-cn_topic_0118922259_p45834822"></a><a name="zh-cn_topic_0118922259_p45834822"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922259_row9860220"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922259_p60480378"><a name="zh-cn_topic_0118922259_p60480378"></a><a name="zh-cn_topic_0118922259_p60480378"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922259_p1516443435315"><a name="zh-cn_topic_0118922259_p1516443435315"></a><a name="zh-cn_topic_0118922259_p1516443435315"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

