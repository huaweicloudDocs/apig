# 重置密钥<a name="ZH-CN_TOPIC_0000001081837341"></a>

## 功能介绍<a name="zh-cn_topic_0225568835_section47629430"></a>

重置指定APP的密钥。

## URI<a name="zh-cn_topic_0225568835_section26011693"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568835_table60402647"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568835_row59047728"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568835_p18136646"><a name="zh-cn_topic_0225568835_p18136646"></a><a name="zh-cn_topic_0225568835_p18136646"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568835_p59782258"><a name="zh-cn_topic_0225568835_p59782258"></a><a name="zh-cn_topic_0225568835_p59782258"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568835_row10524697"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568835_p47194149"><a name="zh-cn_topic_0225568835_p47194149"></a><a name="zh-cn_topic_0225568835_p47194149"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568835_p64629758"><a name="zh-cn_topic_0225568835_p64629758"></a><a name="zh-cn_topic_0225568835_p64629758"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps/secret/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568835_table519051"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568835_row48098925"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568835_p3698841"><a name="zh-cn_topic_0225568835_p3698841"></a><a name="zh-cn_topic_0225568835_p3698841"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568835_p31170665"><a name="zh-cn_topic_0225568835_p31170665"></a><a name="zh-cn_topic_0225568835_p31170665"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568835_p41795909"><a name="zh-cn_topic_0225568835_p41795909"></a><a name="zh-cn_topic_0225568835_p41795909"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568835_p30025494"><a name="zh-cn_topic_0225568835_p30025494"></a><a name="zh-cn_topic_0225568835_p30025494"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568835_row98218424384"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568835_p55878963"><a name="zh-cn_topic_0225568835_p55878963"></a><a name="zh-cn_topic_0225568835_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568835_p29902160"><a name="zh-cn_topic_0225568835_p29902160"></a><a name="zh-cn_topic_0225568835_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568835_p6155914"><a name="zh-cn_topic_0225568835_p6155914"></a><a name="zh-cn_topic_0225568835_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568835_p28867016"><a name="zh-cn_topic_0225568835_p28867016"></a><a name="zh-cn_topic_0225568835_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row13486842153816"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568835_p1780913159538"><a name="zh-cn_topic_0225568835_p1780913159538"></a><a name="zh-cn_topic_0225568835_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568835_p9809215115310"><a name="zh-cn_topic_0225568835_p9809215115310"></a><a name="zh-cn_topic_0225568835_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568835_p1280914152538"><a name="zh-cn_topic_0225568835_p1280914152538"></a><a name="zh-cn_topic_0225568835_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568835_p1880914157537"><a name="zh-cn_topic_0225568835_p1880914157537"></a><a name="zh-cn_topic_0225568835_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row16145988"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568835_p32756662"><a name="zh-cn_topic_0225568835_p32756662"></a><a name="zh-cn_topic_0225568835_p32756662"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568835_p36043989"><a name="zh-cn_topic_0225568835_p36043989"></a><a name="zh-cn_topic_0225568835_p36043989"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568835_p33881992"><a name="zh-cn_topic_0225568835_p33881992"></a><a name="zh-cn_topic_0225568835_p33881992"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568835_p60086840"><a name="zh-cn_topic_0225568835_p60086840"></a><a name="zh-cn_topic_0225568835_p60086840"></a>APP的编号，可通过查询APP列表获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568835_section32778653"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568835_table52858460"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568835_row52119005"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568835_p60889838"><a name="zh-cn_topic_0225568835_p60889838"></a><a name="zh-cn_topic_0225568835_p60889838"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568835_p33129840"><a name="zh-cn_topic_0225568835_p33129840"></a><a name="zh-cn_topic_0225568835_p33129840"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568835_p66271370"><a name="zh-cn_topic_0225568835_p66271370"></a><a name="zh-cn_topic_0225568835_p66271370"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568835_p66380773"><a name="zh-cn_topic_0225568835_p66380773"></a><a name="zh-cn_topic_0225568835_p66380773"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568835_row13951012524"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568835_p571817817386"><a name="zh-cn_topic_0225568835_p571817817386"></a><a name="zh-cn_topic_0225568835_p571817817386"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568835_p07197813819"><a name="zh-cn_topic_0225568835_p07197813819"></a><a name="zh-cn_topic_0225568835_p07197813819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568835_p1871928203812"><a name="zh-cn_topic_0225568835_p1871928203812"></a><a name="zh-cn_topic_0225568835_p1871928203812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568835_p177191863810"><a name="zh-cn_topic_0225568835_p177191863810"></a><a name="zh-cn_topic_0225568835_p177191863810"></a>密钥</p>
<p id="zh-cn_topic_0225568835_p69053295477"><a name="zh-cn_topic_0225568835_p69053295477"></a><a name="zh-cn_topic_0225568835_p69053295477"></a>支持英文，数字，“_”,“-”,“_”,“!”,“@”,“#”,“$”,“%”,且只能以英文或数字开头，8 ~ 64个字符。</p>
<p id="zh-cn_topic_0225568835_p790520296470"><a name="zh-cn_topic_0225568835_p790520296470"></a><a name="zh-cn_topic_0225568835_p790520296470"></a></p>
<div class="note" id="zh-cn_topic_0225568835_note8622433183712"><a name="zh-cn_topic_0225568835_note8622433183712"></a><a name="zh-cn_topic_0225568835_note8622433183712"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568835_p26225334373"><a name="zh-cn_topic_0225568835_p26225334373"></a><a name="zh-cn_topic_0225568835_p26225334373"></a>只支持部分region自定义。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
        "app_secret": "app_secret_sample"
}
```

## 响应消息<a name="zh-cn_topic_0225568835_section37825199"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568835_table32464282"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568835_row38958777"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568835_p1544355"><a name="zh-cn_topic_0225568835_p1544355"></a><a name="zh-cn_topic_0225568835_p1544355"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568835_p57983950"><a name="zh-cn_topic_0225568835_p57983950"></a><a name="zh-cn_topic_0225568835_p57983950"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568835_p66188386"><a name="zh-cn_topic_0225568835_p66188386"></a><a name="zh-cn_topic_0225568835_p66188386"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568835_row59659013"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p541922"><a name="zh-cn_topic_0225568835_p541922"></a><a name="zh-cn_topic_0225568835_p541922"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p43895711"><a name="zh-cn_topic_0225568835_p43895711"></a><a name="zh-cn_topic_0225568835_p43895711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p65891684"><a name="zh-cn_topic_0225568835_p65891684"></a><a name="zh-cn_topic_0225568835_p65891684"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row56154250"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p52200367"><a name="zh-cn_topic_0225568835_p52200367"></a><a name="zh-cn_topic_0225568835_p52200367"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p371312"><a name="zh-cn_topic_0225568835_p371312"></a><a name="zh-cn_topic_0225568835_p371312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p30076343"><a name="zh-cn_topic_0225568835_p30076343"></a><a name="zh-cn_topic_0225568835_p30076343"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row2251631"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p48164407"><a name="zh-cn_topic_0225568835_p48164407"></a><a name="zh-cn_topic_0225568835_p48164407"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p9002871"><a name="zh-cn_topic_0225568835_p9002871"></a><a name="zh-cn_topic_0225568835_p9002871"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p58143960"><a name="zh-cn_topic_0225568835_p58143960"></a><a name="zh-cn_topic_0225568835_p58143960"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row53533596"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p41254033"><a name="zh-cn_topic_0225568835_p41254033"></a><a name="zh-cn_topic_0225568835_p41254033"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p53242362"><a name="zh-cn_topic_0225568835_p53242362"></a><a name="zh-cn_topic_0225568835_p53242362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p17664064"><a name="zh-cn_topic_0225568835_p17664064"></a><a name="zh-cn_topic_0225568835_p17664064"></a>APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row24758849"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p59309724"><a name="zh-cn_topic_0225568835_p59309724"></a><a name="zh-cn_topic_0225568835_p59309724"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p39358344"><a name="zh-cn_topic_0225568835_p39358344"></a><a name="zh-cn_topic_0225568835_p39358344"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p33909292"><a name="zh-cn_topic_0225568835_p33909292"></a><a name="zh-cn_topic_0225568835_p33909292"></a>密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row18772019108"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p148381123152516"><a name="zh-cn_topic_0225568835_p148381123152516"></a><a name="zh-cn_topic_0225568835_p148381123152516"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p10838223112516"><a name="zh-cn_topic_0225568835_p10838223112516"></a><a name="zh-cn_topic_0225568835_p10838223112516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p128381023202515"><a name="zh-cn_topic_0225568835_p128381023202515"></a><a name="zh-cn_topic_0225568835_p128381023202515"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0225568835_ul1126756132511"></a><a name="zh-cn_topic_0225568835_ul1126756132511"></a><ul id="zh-cn_topic_0225568835_ul1126756132511"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row36748179"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p23812543"><a name="zh-cn_topic_0225568835_p23812543"></a><a name="zh-cn_topic_0225568835_p23812543"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p49767864"><a name="zh-cn_topic_0225568835_p49767864"></a><a name="zh-cn_topic_0225568835_p49767864"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p4665189"><a name="zh-cn_topic_0225568835_p4665189"></a><a name="zh-cn_topic_0225568835_p4665189"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row41986707"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p45480106"><a name="zh-cn_topic_0225568835_p45480106"></a><a name="zh-cn_topic_0225568835_p45480106"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p60009961"><a name="zh-cn_topic_0225568835_p60009961"></a><a name="zh-cn_topic_0225568835_p60009961"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p28968697"><a name="zh-cn_topic_0225568835_p28968697"></a><a name="zh-cn_topic_0225568835_p28968697"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row59391687"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568835_p45997331"><a name="zh-cn_topic_0225568835_p45997331"></a><a name="zh-cn_topic_0225568835_p45997331"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568835_p34796291"><a name="zh-cn_topic_0225568835_p34796291"></a><a name="zh-cn_topic_0225568835_p34796291"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568835_p67036159"><a name="zh-cn_topic_0225568835_p67036159"></a><a name="zh-cn_topic_0225568835_p67036159"></a>更新时间</p>
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
	"update_time": "2017-12-28T12:29:35.571Z"
}
```

## 状态码<a name="zh-cn_topic_0225568835_section26572421"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568835_table32291757"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568835_row31810066"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568835_p26478586"><a name="zh-cn_topic_0225568835_p26478586"></a><a name="zh-cn_topic_0225568835_p26478586"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568835_p64390706"><a name="zh-cn_topic_0225568835_p64390706"></a><a name="zh-cn_topic_0225568835_p64390706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568835_row48264674"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568835_p17124531"><a name="zh-cn_topic_0225568835_p17124531"></a><a name="zh-cn_topic_0225568835_p17124531"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568835_p44909772"><a name="zh-cn_topic_0225568835_p44909772"></a><a name="zh-cn_topic_0225568835_p44909772"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row1534772"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568835_p57207693"><a name="zh-cn_topic_0225568835_p57207693"></a><a name="zh-cn_topic_0225568835_p57207693"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568835_p3311555"><a name="zh-cn_topic_0225568835_p3311555"></a><a name="zh-cn_topic_0225568835_p3311555"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row29803996"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568835_p65313447"><a name="zh-cn_topic_0225568835_p65313447"></a><a name="zh-cn_topic_0225568835_p65313447"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568835_p55897859"><a name="zh-cn_topic_0225568835_p55897859"></a><a name="zh-cn_topic_0225568835_p55897859"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row33318687"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568835_p14459094"><a name="zh-cn_topic_0225568835_p14459094"></a><a name="zh-cn_topic_0225568835_p14459094"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568835_p30335986"><a name="zh-cn_topic_0225568835_p30335986"></a><a name="zh-cn_topic_0225568835_p30335986"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row4588426"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568835_p36118200"><a name="zh-cn_topic_0225568835_p36118200"></a><a name="zh-cn_topic_0225568835_p36118200"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568835_p39893054"><a name="zh-cn_topic_0225568835_p39893054"></a><a name="zh-cn_topic_0225568835_p39893054"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568835_row23493170"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568835_p23898608"><a name="zh-cn_topic_0225568835_p23898608"></a><a name="zh-cn_topic_0225568835_p23898608"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568835_p14947689"><a name="zh-cn_topic_0225568835_p14947689"></a><a name="zh-cn_topic_0225568835_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

