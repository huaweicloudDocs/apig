# 修改签名密钥<a name="ZH-CN_TOPIC_0000001081976213"></a>

## 功能介绍<a name="zh-cn_topic_0225568937_section41224746"></a>

修改指定签名密钥的详细信息。

## URI<a name="zh-cn_topic_0225568937_section35478397"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568937_table59329349"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568937_row22745357"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568937_p30434635"><a name="zh-cn_topic_0225568937_p30434635"></a><a name="zh-cn_topic_0225568937_p30434635"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568937_p49286410"><a name="zh-cn_topic_0225568937_p49286410"></a><a name="zh-cn_topic_0225568937_p49286410"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568937_row32776306"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568937_p37635114"><a name="zh-cn_topic_0225568937_p37635114"></a><a name="zh-cn_topic_0225568937_p37635114"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568937_p28545370"><a name="zh-cn_topic_0225568937_p28545370"></a><a name="zh-cn_topic_0225568937_p28545370"></a>/v1/{project_id}/apigw/instances/{instance_id}/signs/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568937_table5827335"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568937_row60220277"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568937_p46004251"><a name="zh-cn_topic_0225568937_p46004251"></a><a name="zh-cn_topic_0225568937_p46004251"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568937_p35356887"><a name="zh-cn_topic_0225568937_p35356887"></a><a name="zh-cn_topic_0225568937_p35356887"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568937_p45335566"><a name="zh-cn_topic_0225568937_p45335566"></a><a name="zh-cn_topic_0225568937_p45335566"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568937_p48302250"><a name="zh-cn_topic_0225568937_p48302250"></a><a name="zh-cn_topic_0225568937_p48302250"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568937_row13835173313503"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568937_p55878963"><a name="zh-cn_topic_0225568937_p55878963"></a><a name="zh-cn_topic_0225568937_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568937_p29902160"><a name="zh-cn_topic_0225568937_p29902160"></a><a name="zh-cn_topic_0225568937_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568937_p6155914"><a name="zh-cn_topic_0225568937_p6155914"></a><a name="zh-cn_topic_0225568937_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568937_p28867016"><a name="zh-cn_topic_0225568937_p28867016"></a><a name="zh-cn_topic_0225568937_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row1127443316504"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568937_p1780913159538"><a name="zh-cn_topic_0225568937_p1780913159538"></a><a name="zh-cn_topic_0225568937_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568937_p9809215115310"><a name="zh-cn_topic_0225568937_p9809215115310"></a><a name="zh-cn_topic_0225568937_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568937_p1280914152538"><a name="zh-cn_topic_0225568937_p1280914152538"></a><a name="zh-cn_topic_0225568937_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568937_p1880914157537"><a name="zh-cn_topic_0225568937_p1880914157537"></a><a name="zh-cn_topic_0225568937_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row20168211"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568937_p23012400"><a name="zh-cn_topic_0225568937_p23012400"></a><a name="zh-cn_topic_0225568937_p23012400"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568937_p52065130"><a name="zh-cn_topic_0225568937_p52065130"></a><a name="zh-cn_topic_0225568937_p52065130"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568937_p56525992"><a name="zh-cn_topic_0225568937_p56525992"></a><a name="zh-cn_topic_0225568937_p56525992"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568937_p15202643"><a name="zh-cn_topic_0225568937_p15202643"></a><a name="zh-cn_topic_0225568937_p15202643"></a>签名密钥编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568937_section50870124"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568937_table9764325"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568937_row36235803"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568937_p49418950"><a name="zh-cn_topic_0225568937_p49418950"></a><a name="zh-cn_topic_0225568937_p49418950"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="11.110000000000001%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568937_p56063914"><a name="zh-cn_topic_0225568937_p56063914"></a><a name="zh-cn_topic_0225568937_p56063914"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568937_p1295450"><a name="zh-cn_topic_0225568937_p1295450"></a><a name="zh-cn_topic_0225568937_p1295450"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568937_p4859217"><a name="zh-cn_topic_0225568937_p4859217"></a><a name="zh-cn_topic_0225568937_p4859217"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568937_row52708562"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568937_p41535136"><a name="zh-cn_topic_0225568937_p41535136"></a><a name="zh-cn_topic_0225568937_p41535136"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568937_p8902895"><a name="zh-cn_topic_0225568937_p8902895"></a><a name="zh-cn_topic_0225568937_p8902895"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568937_p50045927"><a name="zh-cn_topic_0225568937_p50045927"></a><a name="zh-cn_topic_0225568937_p50045927"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568937_p27188271"><a name="zh-cn_topic_0225568937_p27188271"></a><a name="zh-cn_topic_0225568937_p27188271"></a>签名密钥的名称。</p>
<p id="zh-cn_topic_0225568937_p23134828"><a name="zh-cn_topic_0225568937_p23134828"></a><a name="zh-cn_topic_0225568937_p23134828"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0225568937_note412210359485"><a name="zh-cn_topic_0225568937_note412210359485"></a><a name="zh-cn_topic_0225568937_note412210359485"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568937_p1122173518481"><a name="zh-cn_topic_0225568937_p1122173518481"></a><a name="zh-cn_topic_0225568937_p1122173518481"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row46050118"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568937_p66911810"><a name="zh-cn_topic_0225568937_p66911810"></a><a name="zh-cn_topic_0225568937_p66911810"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568937_p51147542"><a name="zh-cn_topic_0225568937_p51147542"></a><a name="zh-cn_topic_0225568937_p51147542"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568937_p49310201"><a name="zh-cn_topic_0225568937_p49310201"></a><a name="zh-cn_topic_0225568937_p49310201"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568937_p34703382"><a name="zh-cn_topic_0225568937_p34703382"></a><a name="zh-cn_topic_0225568937_p34703382"></a>签名密钥的key。</p>
<p id="zh-cn_topic_0225568937_p65832877"><a name="zh-cn_topic_0225568937_p65832877"></a><a name="zh-cn_topic_0225568937_p65832877"></a>支持英文，数字，下划线，中划线，且只能以数字或英文字母开头，8 ~ 32字符。</p>
<p id="zh-cn_topic_0225568937_p9329870"><a name="zh-cn_topic_0225568937_p9329870"></a><a name="zh-cn_topic_0225568937_p9329870"></a>未填写时后台自动生成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row34860829"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568937_p23480388"><a name="zh-cn_topic_0225568937_p23480388"></a><a name="zh-cn_topic_0225568937_p23480388"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568937_p22863307"><a name="zh-cn_topic_0225568937_p22863307"></a><a name="zh-cn_topic_0225568937_p22863307"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568937_p39988541"><a name="zh-cn_topic_0225568937_p39988541"></a><a name="zh-cn_topic_0225568937_p39988541"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568937_p15760103411438"><a name="zh-cn_topic_0225568937_p15760103411438"></a><a name="zh-cn_topic_0225568937_p15760103411438"></a>签名密钥的密钥。</p>
<p id="zh-cn_topic_0225568937_p17846404"><a name="zh-cn_topic_0225568937_p17846404"></a><a name="zh-cn_topic_0225568937_p17846404"></a>支持英文，数字，下划线，中划线，!，@，#，$，%，且只能以数字或英文字母开头，16 ~ 64字符。</p>
<p id="zh-cn_topic_0225568937_p182071619113719"><a name="zh-cn_topic_0225568937_p182071619113719"></a><a name="zh-cn_topic_0225568937_p182071619113719"></a>未填写时后台自动生成。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"name": "signature01",
	"sign_key": "abcd_1234",
	"sign_secret": "******"
}
```

## 响应消息<a name="zh-cn_topic_0225568937_section26839366"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568937_table29766870"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568937_row15144968"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568937_p18782868"><a name="zh-cn_topic_0225568937_p18782868"></a><a name="zh-cn_topic_0225568937_p18782868"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568937_p2503109"><a name="zh-cn_topic_0225568937_p2503109"></a><a name="zh-cn_topic_0225568937_p2503109"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568937_p12827669"><a name="zh-cn_topic_0225568937_p12827669"></a><a name="zh-cn_topic_0225568937_p12827669"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568937_row23239175"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568937_p3325060"><a name="zh-cn_topic_0225568937_p3325060"></a><a name="zh-cn_topic_0225568937_p3325060"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568937_p894433"><a name="zh-cn_topic_0225568937_p894433"></a><a name="zh-cn_topic_0225568937_p894433"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568937_p5340230"><a name="zh-cn_topic_0225568937_p5340230"></a><a name="zh-cn_topic_0225568937_p5340230"></a>签名密钥的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row48062076"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568937_p714049"><a name="zh-cn_topic_0225568937_p714049"></a><a name="zh-cn_topic_0225568937_p714049"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568937_p57837986"><a name="zh-cn_topic_0225568937_p57837986"></a><a name="zh-cn_topic_0225568937_p57837986"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568937_p54365321"><a name="zh-cn_topic_0225568937_p54365321"></a><a name="zh-cn_topic_0225568937_p54365321"></a>签名密钥的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row19525841"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568937_p38089273"><a name="zh-cn_topic_0225568937_p38089273"></a><a name="zh-cn_topic_0225568937_p38089273"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568937_p65332249"><a name="zh-cn_topic_0225568937_p65332249"></a><a name="zh-cn_topic_0225568937_p65332249"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568937_p57420826"><a name="zh-cn_topic_0225568937_p57420826"></a><a name="zh-cn_topic_0225568937_p57420826"></a>签名密钥的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row47025390"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568937_p50960259"><a name="zh-cn_topic_0225568937_p50960259"></a><a name="zh-cn_topic_0225568937_p50960259"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568937_p34140300"><a name="zh-cn_topic_0225568937_p34140300"></a><a name="zh-cn_topic_0225568937_p34140300"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568937_p13900914"><a name="zh-cn_topic_0225568937_p13900914"></a><a name="zh-cn_topic_0225568937_p13900914"></a>签名密钥的密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row57999363"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568937_p327934"><a name="zh-cn_topic_0225568937_p327934"></a><a name="zh-cn_topic_0225568937_p327934"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568937_p26562698"><a name="zh-cn_topic_0225568937_p26562698"></a><a name="zh-cn_topic_0225568937_p26562698"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568937_p4094926"><a name="zh-cn_topic_0225568937_p4094926"></a><a name="zh-cn_topic_0225568937_p4094926"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row36854341"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568937_p32411665"><a name="zh-cn_topic_0225568937_p32411665"></a><a name="zh-cn_topic_0225568937_p32411665"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568937_p8099242"><a name="zh-cn_topic_0225568937_p8099242"></a><a name="zh-cn_topic_0225568937_p8099242"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568937_p52058871"><a name="zh-cn_topic_0225568937_p52058871"></a><a name="zh-cn_topic_0225568937_p52058871"></a>更新时间</p>
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

## 状态码<a name="zh-cn_topic_0225568937_section55177934"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568937_table17361562"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568937_row27903249"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568937_p45570711"><a name="zh-cn_topic_0225568937_p45570711"></a><a name="zh-cn_topic_0225568937_p45570711"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568937_p2161061"><a name="zh-cn_topic_0225568937_p2161061"></a><a name="zh-cn_topic_0225568937_p2161061"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568937_row31910236"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568937_p34592308"><a name="zh-cn_topic_0225568937_p34592308"></a><a name="zh-cn_topic_0225568937_p34592308"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568937_p50513540"><a name="zh-cn_topic_0225568937_p50513540"></a><a name="zh-cn_topic_0225568937_p50513540"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row51968681"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568937_p48713633"><a name="zh-cn_topic_0225568937_p48713633"></a><a name="zh-cn_topic_0225568937_p48713633"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568937_p53490214"><a name="zh-cn_topic_0225568937_p53490214"></a><a name="zh-cn_topic_0225568937_p53490214"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row11649880"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568937_p4116251"><a name="zh-cn_topic_0225568937_p4116251"></a><a name="zh-cn_topic_0225568937_p4116251"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568937_p64980894"><a name="zh-cn_topic_0225568937_p64980894"></a><a name="zh-cn_topic_0225568937_p64980894"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row47957135"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568937_p59322709"><a name="zh-cn_topic_0225568937_p59322709"></a><a name="zh-cn_topic_0225568937_p59322709"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568937_p40410161"><a name="zh-cn_topic_0225568937_p40410161"></a><a name="zh-cn_topic_0225568937_p40410161"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row28147129"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568937_p65325006"><a name="zh-cn_topic_0225568937_p65325006"></a><a name="zh-cn_topic_0225568937_p65325006"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568937_p15296380"><a name="zh-cn_topic_0225568937_p15296380"></a><a name="zh-cn_topic_0225568937_p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568937_row41745357"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568937_p25930762"><a name="zh-cn_topic_0225568937_p25930762"></a><a name="zh-cn_topic_0225568937_p25930762"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568937_p20016996"><a name="zh-cn_topic_0225568937_p20016996"></a><a name="zh-cn_topic_0225568937_p20016996"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

