# 绑定流控策略<a name="ZH-CN_TOPIC_0000001081837359"></a>

## 功能介绍<a name="zh-cn_topic_0225568870_section55163998"></a>

将流控策略应用于API，则所有对该API的访问将会受到该流控策略的限制。当一定时间内的访问次数超过流控策略设置的API最大访问次数限制后，后续的访问将会被拒绝，从而能够较好的保护后端API免受异常流量的冲击，保障服务的稳定运行。

为指定的API绑定流控策略，绑定时，需要指定在哪个环境上生效。

同一个API发布到不同的环境可以绑定不同的流控策略；一个API在发布到特定环境后只能绑定一个默认的流控策略。

## URI<a name="zh-cn_topic_0225568870_section26713936"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法及URI

<a name="zh-cn_topic_0225568870_table52780230"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568870_row19624408"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568870_p46073215"><a name="zh-cn_topic_0225568870_p46073215"></a><a name="zh-cn_topic_0225568870_p46073215"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568870_p40942926"><a name="zh-cn_topic_0225568870_p40942926"></a><a name="zh-cn_topic_0225568870_p40942926"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568870_row28042734"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568870_p56868999"><a name="zh-cn_topic_0225568870_p56868999"></a><a name="zh-cn_topic_0225568870_p56868999"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568870_p42986176"><a name="zh-cn_topic_0225568870_p42986176"></a><a name="zh-cn_topic_0225568870_p42986176"></a>/v1/{project_id}/apigw/instances/{instance_id}/throttle-bindings</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568870_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568870_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568870_p23103637"><a name="zh-cn_topic_0225568870_p23103637"></a><a name="zh-cn_topic_0225568870_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568870_p59455291"><a name="zh-cn_topic_0225568870_p59455291"></a><a name="zh-cn_topic_0225568870_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568870_p51149303"><a name="zh-cn_topic_0225568870_p51149303"></a><a name="zh-cn_topic_0225568870_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568870_p49452846"><a name="zh-cn_topic_0225568870_p49452846"></a><a name="zh-cn_topic_0225568870_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568870_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568870_p55878963"><a name="zh-cn_topic_0225568870_p55878963"></a><a name="zh-cn_topic_0225568870_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568870_p29902160"><a name="zh-cn_topic_0225568870_p29902160"></a><a name="zh-cn_topic_0225568870_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568870_p6155914"><a name="zh-cn_topic_0225568870_p6155914"></a><a name="zh-cn_topic_0225568870_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568870_p28867016"><a name="zh-cn_topic_0225568870_p28867016"></a><a name="zh-cn_topic_0225568870_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568870_p1780913159538"><a name="zh-cn_topic_0225568870_p1780913159538"></a><a name="zh-cn_topic_0225568870_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568870_p9809215115310"><a name="zh-cn_topic_0225568870_p9809215115310"></a><a name="zh-cn_topic_0225568870_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568870_p1280914152538"><a name="zh-cn_topic_0225568870_p1280914152538"></a><a name="zh-cn_topic_0225568870_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568870_p1880914157537"><a name="zh-cn_topic_0225568870_p1880914157537"></a><a name="zh-cn_topic_0225568870_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568870_section39098839"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568870_table59328193"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568870_row65892668"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568870_p35705855"><a name="zh-cn_topic_0225568870_p35705855"></a><a name="zh-cn_topic_0225568870_p35705855"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568870_p6493180"><a name="zh-cn_topic_0225568870_p6493180"></a><a name="zh-cn_topic_0225568870_p6493180"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568870_p56185561"><a name="zh-cn_topic_0225568870_p56185561"></a><a name="zh-cn_topic_0225568870_p56185561"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568870_p54736574"><a name="zh-cn_topic_0225568870_p54736574"></a><a name="zh-cn_topic_0225568870_p54736574"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568870_row4477524"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568870_p27135170"><a name="zh-cn_topic_0225568870_p27135170"></a><a name="zh-cn_topic_0225568870_p27135170"></a>publish_ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568870_p50465201"><a name="zh-cn_topic_0225568870_p50465201"></a><a name="zh-cn_topic_0225568870_p50465201"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568870_p61149513"><a name="zh-cn_topic_0225568870_p61149513"></a><a name="zh-cn_topic_0225568870_p61149513"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568870_p54163505"><a name="zh-cn_topic_0225568870_p54163505"></a><a name="zh-cn_topic_0225568870_p54163505"></a>API的发布记录编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row25183262"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568870_p26578342"><a name="zh-cn_topic_0225568870_p26578342"></a><a name="zh-cn_topic_0225568870_p26578342"></a>strategy_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568870_p5362107"><a name="zh-cn_topic_0225568870_p5362107"></a><a name="zh-cn_topic_0225568870_p5362107"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568870_p31677508"><a name="zh-cn_topic_0225568870_p31677508"></a><a name="zh-cn_topic_0225568870_p31677508"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568870_p15741354"><a name="zh-cn_topic_0225568870_p15741354"></a><a name="zh-cn_topic_0225568870_p15741354"></a>流控策略编号</p>
</td>
</tr>
</tbody>
</table>

请求参数样例：

```
{
  "publish_ids": [
    "374a6d5a-20c7-4ea1-82e1-19fce4556956",
    "65e6fe53-1ac3-4481-ba36-9f0bc6f22057"
  ],
  "strategy_id": "0325b671-2d50-4614-9868-22102262695d"
}
```

## 响应消息<a name="zh-cn_topic_0225568870_section12889389"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568870_table26449895"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568870_row31982042"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568870_p40408637"><a name="zh-cn_topic_0225568870_p40408637"></a><a name="zh-cn_topic_0225568870_p40408637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568870_p51874144"><a name="zh-cn_topic_0225568870_p51874144"></a><a name="zh-cn_topic_0225568870_p51874144"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568870_p41056107"><a name="zh-cn_topic_0225568870_p41056107"></a><a name="zh-cn_topic_0225568870_p41056107"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568870_row37210375"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568870_p61250395"><a name="zh-cn_topic_0225568870_p61250395"></a><a name="zh-cn_topic_0225568870_p61250395"></a>throttle_applys</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568870_p62334992"><a name="zh-cn_topic_0225568870_p62334992"></a><a name="zh-cn_topic_0225568870_p62334992"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568870_p15969614"><a name="zh-cn_topic_0225568870_p15969614"></a><a name="zh-cn_topic_0225568870_p15969614"></a>API与流控策略的绑定关系列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  throttle\_applys参数说明

<a name="zh-cn_topic_0225568870_table9508799"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568870_row12431416"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568870_p311800"><a name="zh-cn_topic_0225568870_p311800"></a><a name="zh-cn_topic_0225568870_p311800"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568870_p25255857"><a name="zh-cn_topic_0225568870_p25255857"></a><a name="zh-cn_topic_0225568870_p25255857"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568870_p32458506"><a name="zh-cn_topic_0225568870_p32458506"></a><a name="zh-cn_topic_0225568870_p32458506"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568870_row11893291"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568870_p23832509"><a name="zh-cn_topic_0225568870_p23832509"></a><a name="zh-cn_topic_0225568870_p23832509"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568870_p51385063"><a name="zh-cn_topic_0225568870_p51385063"></a><a name="zh-cn_topic_0225568870_p51385063"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568870_p1440594"><a name="zh-cn_topic_0225568870_p1440594"></a><a name="zh-cn_topic_0225568870_p1440594"></a>绑定关系的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row12965351"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568870_p43560534"><a name="zh-cn_topic_0225568870_p43560534"></a><a name="zh-cn_topic_0225568870_p43560534"></a>strategy_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568870_p38742361"><a name="zh-cn_topic_0225568870_p38742361"></a><a name="zh-cn_topic_0225568870_p38742361"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568870_p51123545"><a name="zh-cn_topic_0225568870_p51123545"></a><a name="zh-cn_topic_0225568870_p51123545"></a>流控策略的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row57458723"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568870_p23644968"><a name="zh-cn_topic_0225568870_p23644968"></a><a name="zh-cn_topic_0225568870_p23644968"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568870_p36194270"><a name="zh-cn_topic_0225568870_p36194270"></a><a name="zh-cn_topic_0225568870_p36194270"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568870_p46054764"><a name="zh-cn_topic_0225568870_p46054764"></a><a name="zh-cn_topic_0225568870_p46054764"></a>API的发布记录编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row11839700"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568870_p19491675"><a name="zh-cn_topic_0225568870_p19491675"></a><a name="zh-cn_topic_0225568870_p19491675"></a>scope</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568870_p35321805"><a name="zh-cn_topic_0225568870_p35321805"></a><a name="zh-cn_topic_0225568870_p35321805"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568870_p42493972"><a name="zh-cn_topic_0225568870_p42493972"></a><a name="zh-cn_topic_0225568870_p42493972"></a>策略作用域，取值如下：</p>
<a name="zh-cn_topic_0225568870_ul46901435"></a><a name="zh-cn_topic_0225568870_ul46901435"></a><ul id="zh-cn_topic_0225568870_ul46901435"><li>1: 整个API</li><li>2: 单个用户</li><li>3: 单个APP</li></ul>
<p id="zh-cn_topic_0225568870_p26177605"><a name="zh-cn_topic_0225568870_p26177605"></a><a name="zh-cn_topic_0225568870_p26177605"></a>目前只支持1</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row34271861"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568870_p24557342"><a name="zh-cn_topic_0225568870_p24557342"></a><a name="zh-cn_topic_0225568870_p24557342"></a>apply_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568870_p42987684"><a name="zh-cn_topic_0225568870_p42987684"></a><a name="zh-cn_topic_0225568870_p42987684"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568870_p59450350"><a name="zh-cn_topic_0225568870_p59450350"></a><a name="zh-cn_topic_0225568870_p59450350"></a>绑定时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"throttle_applys": [{
		"id": "507c6a9f-8322-4dc2-8ba5-b4d74e3690d3",
		"strategy_id": "0325b671-2d50-4614-9868-22102262695d",
		"publish_id": "374a6d5a-20c7-4ea1-82e1-19fce4556956",
		"scope": 1,
		"apply_time": "2017-12-29T03:01:11.138456Z"
	},
	{
		"id": "90f05978-06a3-4096-8bea-b5e2fa12b843",
		"strategy_id": "0325b671-2d50-4614-9868-22102262695d",
		"publish_id": "65e6fe53-1ac3-4481-ba36-9f0bc6f22057",
		"scope": 1,
		"apply_time": "2017-12-29T03:01:11.138456Z"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568870_section16345235"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0225568870_table42630114"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568870_row12146276"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568870_p44324291"><a name="zh-cn_topic_0225568870_p44324291"></a><a name="zh-cn_topic_0225568870_p44324291"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568870_p33497843"><a name="zh-cn_topic_0225568870_p33497843"></a><a name="zh-cn_topic_0225568870_p33497843"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568870_row28970780"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568870_p64931813"><a name="zh-cn_topic_0225568870_p64931813"></a><a name="zh-cn_topic_0225568870_p64931813"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568870_p24985462"><a name="zh-cn_topic_0225568870_p24985462"></a><a name="zh-cn_topic_0225568870_p24985462"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row23542569"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568870_p27899962"><a name="zh-cn_topic_0225568870_p27899962"></a><a name="zh-cn_topic_0225568870_p27899962"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568870_p45304488"><a name="zh-cn_topic_0225568870_p45304488"></a><a name="zh-cn_topic_0225568870_p45304488"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row5087213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568870_p9411121"><a name="zh-cn_topic_0225568870_p9411121"></a><a name="zh-cn_topic_0225568870_p9411121"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568870_p24103300"><a name="zh-cn_topic_0225568870_p24103300"></a><a name="zh-cn_topic_0225568870_p24103300"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row15603116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568870_p55892892"><a name="zh-cn_topic_0225568870_p55892892"></a><a name="zh-cn_topic_0225568870_p55892892"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568870_p31030384"><a name="zh-cn_topic_0225568870_p31030384"></a><a name="zh-cn_topic_0225568870_p31030384"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row10838003"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568870_p5463065"><a name="zh-cn_topic_0225568870_p5463065"></a><a name="zh-cn_topic_0225568870_p5463065"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568870_p39855127"><a name="zh-cn_topic_0225568870_p39855127"></a><a name="zh-cn_topic_0225568870_p39855127"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568870_row23151831"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568870_p63359054"><a name="zh-cn_topic_0225568870_p63359054"></a><a name="zh-cn_topic_0225568870_p63359054"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568870_p6744143"><a name="zh-cn_topic_0225568870_p6744143"></a><a name="zh-cn_topic_0225568870_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

