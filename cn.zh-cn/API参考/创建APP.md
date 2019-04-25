# 创建APP<a name="apig-zh-api-180713036"></a>

## 功能介绍<a name="section61362801"></a>

APP即应用，是一个可以访问API的身份标识。将API授权给APP后，APP即可调用API。

创建一个APP。

## URI<a name="section15394303"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table66835314"></a>
<table><thead align="left"><tr id="row49580837"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p56624893"><a name="p56624893"></a><a name="p56624893"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p23213605"><a name="p23213605"></a><a name="p23213605"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row1253829"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p34451334"><a name="p34451334"></a><a name="p34451334"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p39094671"><a name="p39094671"></a><a name="p39094671"></a>/v1.0/apigw/apps</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section4331004"></a>

**表 2**  参数说明

<a name="table12551817"></a>
<table><thead align="left"><tr id="row63926902"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p10696570"><a name="p10696570"></a><a name="p10696570"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p61115871"><a name="p61115871"></a><a name="p61115871"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p51438541"><a name="p51438541"></a><a name="p51438541"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p5772267"><a name="p5772267"></a><a name="p5772267"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row64900449"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p22445016"><a name="p22445016"></a><a name="p22445016"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p6106999"><a name="p6106999"></a><a name="p6106999"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p24904935"><a name="p24904935"></a><a name="p24904935"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p4033872"><a name="p4033872"></a><a name="p4033872"></a>APP的名称</p>
<p id="p55011617"><a name="p55011617"></a><a name="p55011617"></a>支持汉字，英文，数字，“_”，且只能以英文和汉字开头，3 ~ 64个字符。</p>
<div class="note" id="note18685133019272"><a name="note18685133019272"></a><a name="note18685133019272"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1068523022711"><a name="p1068523022711"></a><a name="p1068523022711"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row36149089"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p42395109"><a name="p42395109"></a><a name="p42395109"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p11451768"><a name="p11451768"></a><a name="p11451768"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p55178053"><a name="p55178053"></a><a name="p55178053"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p40237298"><a name="p40237298"></a><a name="p40237298"></a>APP描述。</p>
<p id="p6416869"><a name="p6416869"></a><a name="p6416869"></a>字符长度不能大于255</p>
<div class="note" id="note2159356132719"><a name="note2159356132719"></a><a name="note2159356132719"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1715911562275"><a name="p1715911562275"></a><a name="p1715911562275"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "name": "app_001",
  "remark": "first app"
}
```

## 响应消息<a name="section15267056"></a>

**表 3**  参数说明

<a name="table20910139"></a>
<table><thead align="left"><tr id="row9919741"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p65301594"><a name="p65301594"></a><a name="p65301594"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p54937751"><a name="p54937751"></a><a name="p54937751"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p20772828"><a name="p20772828"></a><a name="p20772828"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4877522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p59535008"><a name="p59535008"></a><a name="p59535008"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57606383"><a name="p57606383"></a><a name="p57606383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p35605479"><a name="p35605479"></a><a name="p35605479"></a>编号</p>
</td>
</tr>
<tr id="row52013857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52372904"><a name="p52372904"></a><a name="p52372904"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14346860"><a name="p14346860"></a><a name="p14346860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p21245012"><a name="p21245012"></a><a name="p21245012"></a>名称</p>
</td>
</tr>
<tr id="row56987385"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52575507"><a name="p52575507"></a><a name="p52575507"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p30757702"><a name="p30757702"></a><a name="p30757702"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8345913"><a name="p8345913"></a><a name="p8345913"></a>状态</p>
</td>
</tr>
<tr id="row8004354"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44372920"><a name="p44372920"></a><a name="p44372920"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p37436804"><a name="p37436804"></a><a name="p37436804"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12482251"><a name="p12482251"></a><a name="p12482251"></a>APP的key</p>
</td>
</tr>
<tr id="row45231401"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39864887"><a name="p39864887"></a><a name="p39864887"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7830389"><a name="p7830389"></a><a name="p7830389"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30281739"><a name="p30281739"></a><a name="p30281739"></a>密钥</p>
</td>
</tr>
<tr id="row4100199"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63680693"><a name="p63680693"></a><a name="p63680693"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57862512"><a name="p57862512"></a><a name="p57862512"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56351871"><a name="p56351871"></a><a name="p56351871"></a>注册时间</p>
</td>
</tr>
<tr id="row37404794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9889443"><a name="p9889443"></a><a name="p9889443"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62847380"><a name="p62847380"></a><a name="p62847380"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57473014"><a name="p57473014"></a><a name="p57473014"></a>描述</p>
</td>
</tr>
<tr id="row47495080"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p21896310"><a name="p21896310"></a><a name="p21896310"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p28770696"><a name="p28770696"></a><a name="p28770696"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48725063"><a name="p48725063"></a><a name="p48725063"></a>更新时间</p>
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
	"remark": "第一个应用",
	"register_time": "2017-12-28T12:26:54.2345858Z",
	"update_time": "2017-12-28T12:26:54.2345858Z"
}
```

## 状态码<a name="section38979041"></a>

**表 4**  返回消息说明

<a name="table665003"></a>
<table><thead align="left"><tr id="row9107269"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p66600187"><a name="p66600187"></a><a name="p66600187"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p25906037"><a name="p25906037"></a><a name="p25906037"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18014235"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p49866967"><a name="p49866967"></a><a name="p49866967"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p12692494"><a name="p12692494"></a><a name="p12692494"></a>Created</p>
</td>
</tr>
<tr id="row47123588"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p58914306"><a name="p58914306"></a><a name="p58914306"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p7329456"><a name="p7329456"></a><a name="p7329456"></a>Bad Request</p>
</td>
</tr>
<tr id="row65965104"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p41573226"><a name="p41573226"></a><a name="p41573226"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row40784364"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p15199212"><a name="p15199212"></a><a name="p15199212"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row7263502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p51472750"><a name="p51472750"></a><a name="p51472750"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p8543194"><a name="p8543194"></a><a name="p8543194"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

