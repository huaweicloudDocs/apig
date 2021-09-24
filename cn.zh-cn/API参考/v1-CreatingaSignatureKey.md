# 创建签名密钥<a name="ZH-CN_TOPIC_0000001081837381"></a>

## 功能介绍<a name="zh-cn_topic_0225568936_section32899949"></a>

为了保护API的安全性，建议租户为API的访问提供一套保护机制，即租户开放的API，需要对请求来源进行认证，不符合认证的请求直接拒绝访问。

其中，签名密钥就是API安全保护机制的一种。

租户创建一个签名密钥，并将签名密钥与API进行绑定，则API网关在请求这个API时，就会使用绑定的签名密钥对请求参数进行数据加密，生成签名。当租户的后端服务收到请求时，可以校验这个签名，如果签名校验不通过，则该请求不是API网关发出的请求，租户可以拒绝这个请求，从而保证API的安全性，避免API被未知来源的请求攻击。

## URI<a name="zh-cn_topic_0225568936_section27664085"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568936_table41707817"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568936_row58843872"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568936_p1624321"><a name="zh-cn_topic_0225568936_p1624321"></a><a name="zh-cn_topic_0225568936_p1624321"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568936_p64461142"><a name="zh-cn_topic_0225568936_p64461142"></a><a name="zh-cn_topic_0225568936_p64461142"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568936_row53969991"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568936_p9493182"><a name="zh-cn_topic_0225568936_p9493182"></a><a name="zh-cn_topic_0225568936_p9493182"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568936_p30750240"><a name="zh-cn_topic_0225568936_p30750240"></a><a name="zh-cn_topic_0225568936_p30750240"></a>/v1/{project_id}/apigw/instances/{instance_id}/signs</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568936_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568936_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568936_p23103637"><a name="zh-cn_topic_0225568936_p23103637"></a><a name="zh-cn_topic_0225568936_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568936_p59455291"><a name="zh-cn_topic_0225568936_p59455291"></a><a name="zh-cn_topic_0225568936_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568936_p51149303"><a name="zh-cn_topic_0225568936_p51149303"></a><a name="zh-cn_topic_0225568936_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568936_p49452846"><a name="zh-cn_topic_0225568936_p49452846"></a><a name="zh-cn_topic_0225568936_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568936_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568936_p55878963"><a name="zh-cn_topic_0225568936_p55878963"></a><a name="zh-cn_topic_0225568936_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568936_p29902160"><a name="zh-cn_topic_0225568936_p29902160"></a><a name="zh-cn_topic_0225568936_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568936_p6155914"><a name="zh-cn_topic_0225568936_p6155914"></a><a name="zh-cn_topic_0225568936_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568936_p28867016"><a name="zh-cn_topic_0225568936_p28867016"></a><a name="zh-cn_topic_0225568936_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568936_p1780913159538"><a name="zh-cn_topic_0225568936_p1780913159538"></a><a name="zh-cn_topic_0225568936_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568936_p9809215115310"><a name="zh-cn_topic_0225568936_p9809215115310"></a><a name="zh-cn_topic_0225568936_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568936_p1280914152538"><a name="zh-cn_topic_0225568936_p1280914152538"></a><a name="zh-cn_topic_0225568936_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568936_p1880914157537"><a name="zh-cn_topic_0225568936_p1880914157537"></a><a name="zh-cn_topic_0225568936_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568936_section47650173"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568936_table2564886"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568936_row39382573"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568936_p35871824"><a name="zh-cn_topic_0225568936_p35871824"></a><a name="zh-cn_topic_0225568936_p35871824"></a><strong id="zh-cn_topic_0225568936_b54410961"><a name="zh-cn_topic_0225568936_b54410961"></a><a name="zh-cn_topic_0225568936_b54410961"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="11.110000000000001%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568936_p45211703"><a name="zh-cn_topic_0225568936_p45211703"></a><a name="zh-cn_topic_0225568936_p45211703"></a><strong id="zh-cn_topic_0225568936_b255714485613"><a name="zh-cn_topic_0225568936_b255714485613"></a><a name="zh-cn_topic_0225568936_b255714485613"></a>是否必选</strong></p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568936_p8879947"><a name="zh-cn_topic_0225568936_p8879947"></a><a name="zh-cn_topic_0225568936_p8879947"></a><strong id="zh-cn_topic_0225568936_b12810666"><a name="zh-cn_topic_0225568936_b12810666"></a><a name="zh-cn_topic_0225568936_b12810666"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568936_p31031046"><a name="zh-cn_topic_0225568936_p31031046"></a><a name="zh-cn_topic_0225568936_p31031046"></a><strong id="zh-cn_topic_0225568936_b10843966"><a name="zh-cn_topic_0225568936_b10843966"></a><a name="zh-cn_topic_0225568936_b10843966"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568936_row5946028"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568936_p11866226"><a name="zh-cn_topic_0225568936_p11866226"></a><a name="zh-cn_topic_0225568936_p11866226"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568936_p21640249"><a name="zh-cn_topic_0225568936_p21640249"></a><a name="zh-cn_topic_0225568936_p21640249"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568936_p8029736"><a name="zh-cn_topic_0225568936_p8029736"></a><a name="zh-cn_topic_0225568936_p8029736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568936_p46428904"><a name="zh-cn_topic_0225568936_p46428904"></a><a name="zh-cn_topic_0225568936_p46428904"></a>签名密钥的名称。</p>
<p id="zh-cn_topic_0225568936_p23804074"><a name="zh-cn_topic_0225568936_p23804074"></a><a name="zh-cn_topic_0225568936_p23804074"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0225568936_note1389815157433"><a name="zh-cn_topic_0225568936_note1389815157433"></a><a name="zh-cn_topic_0225568936_note1389815157433"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568936_p108991115154319"><a name="zh-cn_topic_0225568936_p108991115154319"></a><a name="zh-cn_topic_0225568936_p108991115154319"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row826071"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568936_p66911810"><a name="zh-cn_topic_0225568936_p66911810"></a><a name="zh-cn_topic_0225568936_p66911810"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568936_p51147542"><a name="zh-cn_topic_0225568936_p51147542"></a><a name="zh-cn_topic_0225568936_p51147542"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568936_p49310201"><a name="zh-cn_topic_0225568936_p49310201"></a><a name="zh-cn_topic_0225568936_p49310201"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568936_p34703382"><a name="zh-cn_topic_0225568936_p34703382"></a><a name="zh-cn_topic_0225568936_p34703382"></a>签名密钥的key。</p>
<p id="zh-cn_topic_0225568936_p65832877"><a name="zh-cn_topic_0225568936_p65832877"></a><a name="zh-cn_topic_0225568936_p65832877"></a>支持英文，数字，下划线，中划线，且只能以数字或英文字母开头，8 ~ 32字符。</p>
<p id="zh-cn_topic_0225568936_p9329870"><a name="zh-cn_topic_0225568936_p9329870"></a><a name="zh-cn_topic_0225568936_p9329870"></a>未填写时后台自动生成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row16859971"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568936_p23480388"><a name="zh-cn_topic_0225568936_p23480388"></a><a name="zh-cn_topic_0225568936_p23480388"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568936_p22863307"><a name="zh-cn_topic_0225568936_p22863307"></a><a name="zh-cn_topic_0225568936_p22863307"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568936_p39988541"><a name="zh-cn_topic_0225568936_p39988541"></a><a name="zh-cn_topic_0225568936_p39988541"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568936_p15760103411438"><a name="zh-cn_topic_0225568936_p15760103411438"></a><a name="zh-cn_topic_0225568936_p15760103411438"></a>签名密钥的密钥。</p>
<p id="zh-cn_topic_0225568936_p17846404"><a name="zh-cn_topic_0225568936_p17846404"></a><a name="zh-cn_topic_0225568936_p17846404"></a>支持英文，数字，下划线，中划线，!，@，#，$，%，且只能以数字或英文字母开头，16 ~ 64字符。</p>
<p id="zh-cn_topic_0225568936_p182071619113719"><a name="zh-cn_topic_0225568936_p182071619113719"></a><a name="zh-cn_topic_0225568936_p182071619113719"></a>未填写时后台自动生成。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"name": "signature01",
	"sign_key": "abcd_123",
	"sign_secret": "******"
}
```

## 响应消息<a name="zh-cn_topic_0225568936_section34458777"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568936_table20176688"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568936_row48802096"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568936_p60655680"><a name="zh-cn_topic_0225568936_p60655680"></a><a name="zh-cn_topic_0225568936_p60655680"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568936_p60358653"><a name="zh-cn_topic_0225568936_p60358653"></a><a name="zh-cn_topic_0225568936_p60358653"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568936_p45152596"><a name="zh-cn_topic_0225568936_p45152596"></a><a name="zh-cn_topic_0225568936_p45152596"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568936_row32899729"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568936_p47632363"><a name="zh-cn_topic_0225568936_p47632363"></a><a name="zh-cn_topic_0225568936_p47632363"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568936_p33016177"><a name="zh-cn_topic_0225568936_p33016177"></a><a name="zh-cn_topic_0225568936_p33016177"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568936_p57064717"><a name="zh-cn_topic_0225568936_p57064717"></a><a name="zh-cn_topic_0225568936_p57064717"></a>签名密钥的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row43820405"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568936_p59791946"><a name="zh-cn_topic_0225568936_p59791946"></a><a name="zh-cn_topic_0225568936_p59791946"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568936_p11309480"><a name="zh-cn_topic_0225568936_p11309480"></a><a name="zh-cn_topic_0225568936_p11309480"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568936_p43652662"><a name="zh-cn_topic_0225568936_p43652662"></a><a name="zh-cn_topic_0225568936_p43652662"></a>签名密钥的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row57329638"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568936_p13189120"><a name="zh-cn_topic_0225568936_p13189120"></a><a name="zh-cn_topic_0225568936_p13189120"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568936_p61685790"><a name="zh-cn_topic_0225568936_p61685790"></a><a name="zh-cn_topic_0225568936_p61685790"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568936_p30493097"><a name="zh-cn_topic_0225568936_p30493097"></a><a name="zh-cn_topic_0225568936_p30493097"></a>签名密钥的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row6002418"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568936_p16433867"><a name="zh-cn_topic_0225568936_p16433867"></a><a name="zh-cn_topic_0225568936_p16433867"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568936_p56074820"><a name="zh-cn_topic_0225568936_p56074820"></a><a name="zh-cn_topic_0225568936_p56074820"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568936_p45766533"><a name="zh-cn_topic_0225568936_p45766533"></a><a name="zh-cn_topic_0225568936_p45766533"></a>签名密钥的密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row9245616"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568936_p10697457"><a name="zh-cn_topic_0225568936_p10697457"></a><a name="zh-cn_topic_0225568936_p10697457"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568936_p61187727"><a name="zh-cn_topic_0225568936_p61187727"></a><a name="zh-cn_topic_0225568936_p61187727"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568936_p57258865"><a name="zh-cn_topic_0225568936_p57258865"></a><a name="zh-cn_topic_0225568936_p57258865"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row45567744"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568936_p67108611"><a name="zh-cn_topic_0225568936_p67108611"></a><a name="zh-cn_topic_0225568936_p67108611"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568936_p67088448"><a name="zh-cn_topic_0225568936_p67088448"></a><a name="zh-cn_topic_0225568936_p67088448"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568936_p65455197"><a name="zh-cn_topic_0225568936_p65455197"></a><a name="zh-cn_topic_0225568936_p65455197"></a>更新时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"name": "signature01",
	"sign_key": "abcd_123",
	"sign_secret": "******",
	"id": "3a793b65a9034bdfae08924f149bfb4a",
	"create_time": "2018-02-06T12:17:36.039953112Z",
	"update_time": "2018-02-06T12:17:36.039954198Z"
}
```

## 状态码<a name="zh-cn_topic_0225568936_section26198374"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568936_table48963168"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568936_row42034035"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568936_p49313649"><a name="zh-cn_topic_0225568936_p49313649"></a><a name="zh-cn_topic_0225568936_p49313649"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568936_p46407939"><a name="zh-cn_topic_0225568936_p46407939"></a><a name="zh-cn_topic_0225568936_p46407939"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568936_row8520349"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568936_p19059693"><a name="zh-cn_topic_0225568936_p19059693"></a><a name="zh-cn_topic_0225568936_p19059693"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568936_p331318"><a name="zh-cn_topic_0225568936_p331318"></a><a name="zh-cn_topic_0225568936_p331318"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row2981863"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568936_p40204311"><a name="zh-cn_topic_0225568936_p40204311"></a><a name="zh-cn_topic_0225568936_p40204311"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568936_p35323731"><a name="zh-cn_topic_0225568936_p35323731"></a><a name="zh-cn_topic_0225568936_p35323731"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row49478130"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568936_p48305580"><a name="zh-cn_topic_0225568936_p48305580"></a><a name="zh-cn_topic_0225568936_p48305580"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568936_p20437927"><a name="zh-cn_topic_0225568936_p20437927"></a><a name="zh-cn_topic_0225568936_p20437927"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row49723620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568936_p1081443"><a name="zh-cn_topic_0225568936_p1081443"></a><a name="zh-cn_topic_0225568936_p1081443"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568936_p20488054"><a name="zh-cn_topic_0225568936_p20488054"></a><a name="zh-cn_topic_0225568936_p20488054"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568936_row50174763"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568936_p37623992"><a name="zh-cn_topic_0225568936_p37623992"></a><a name="zh-cn_topic_0225568936_p37623992"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568936_p6744143"><a name="zh-cn_topic_0225568936_p6744143"></a><a name="zh-cn_topic_0225568936_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

