# 修改环境<a name="ZH-CN_TOPIC_0000001081837277"></a>

## 功能介绍<a name="zh-cn_topic_0118922245_section37058740"></a>

修改指定环境的信息。其中可修改的属性为：name、remark，其它属性不可修改。

## URI<a name="zh-cn_topic_0118922245_section65093204"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922245_table7557150"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922245_row49653828"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922245_p62537130"><a name="zh-cn_topic_0118922245_p62537130"></a><a name="zh-cn_topic_0118922245_p62537130"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922245_p32342740"><a name="zh-cn_topic_0118922245_p32342740"></a><a name="zh-cn_topic_0118922245_p32342740"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922245_row2516266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922245_p2491030"><a name="zh-cn_topic_0118922245_p2491030"></a><a name="zh-cn_topic_0118922245_p2491030"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922245_p446845"><a name="zh-cn_topic_0118922245_p446845"></a><a name="zh-cn_topic_0118922245_p446845"></a>/v1.0/apigw/envs/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922245_table36194505"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922245_row46126471"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922245_p45256674"><a name="zh-cn_topic_0118922245_p45256674"></a><a name="zh-cn_topic_0118922245_p45256674"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922245_p41911953"><a name="zh-cn_topic_0118922245_p41911953"></a><a name="zh-cn_topic_0118922245_p41911953"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922245_p39425021"><a name="zh-cn_topic_0118922245_p39425021"></a><a name="zh-cn_topic_0118922245_p39425021"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922245_p39310093"><a name="zh-cn_topic_0118922245_p39310093"></a><a name="zh-cn_topic_0118922245_p39310093"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922245_row30000937"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922245_p14156858"><a name="zh-cn_topic_0118922245_p14156858"></a><a name="zh-cn_topic_0118922245_p14156858"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922245_p5854888"><a name="zh-cn_topic_0118922245_p5854888"></a><a name="zh-cn_topic_0118922245_p5854888"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922245_p4483930"><a name="zh-cn_topic_0118922245_p4483930"></a><a name="zh-cn_topic_0118922245_p4483930"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922245_p27654073"><a name="zh-cn_topic_0118922245_p27654073"></a><a name="zh-cn_topic_0118922245_p27654073"></a>环境的ID，可通过查询环境信息获取该ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922245_section48967929"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118922245_table25387436"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922245_row61507814"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922245_p16077015"><a name="zh-cn_topic_0118922245_p16077015"></a><a name="zh-cn_topic_0118922245_p16077015"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922245_p27169870"><a name="zh-cn_topic_0118922245_p27169870"></a><a name="zh-cn_topic_0118922245_p27169870"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922245_p53275824"><a name="zh-cn_topic_0118922245_p53275824"></a><a name="zh-cn_topic_0118922245_p53275824"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.99999999999999%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922245_p20374503"><a name="zh-cn_topic_0118922245_p20374503"></a><a name="zh-cn_topic_0118922245_p20374503"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922245_row39722075"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922245_p63371507"><a name="zh-cn_topic_0118922245_p63371507"></a><a name="zh-cn_topic_0118922245_p63371507"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922245_p32818456"><a name="zh-cn_topic_0118922245_p32818456"></a><a name="zh-cn_topic_0118922245_p32818456"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922245_p41049265"><a name="zh-cn_topic_0118922245_p41049265"></a><a name="zh-cn_topic_0118922245_p41049265"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922245_p36656167"><a name="zh-cn_topic_0118922245_p36656167"></a><a name="zh-cn_topic_0118922245_p36656167"></a>环境的名称</p>
<p id="zh-cn_topic_0118922245_p13017963"><a name="zh-cn_topic_0118922245_p13017963"></a><a name="zh-cn_topic_0118922245_p13017963"></a>支持英文，数字，下划线，且只能以英文字母开头，3 ~ 64字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row39662742"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922245_p58565567"><a name="zh-cn_topic_0118922245_p58565567"></a><a name="zh-cn_topic_0118922245_p58565567"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922245_p46190492"><a name="zh-cn_topic_0118922245_p46190492"></a><a name="zh-cn_topic_0118922245_p46190492"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922245_p50442390"><a name="zh-cn_topic_0118922245_p50442390"></a><a name="zh-cn_topic_0118922245_p50442390"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922245_p59301780"><a name="zh-cn_topic_0118922245_p59301780"></a><a name="zh-cn_topic_0118922245_p59301780"></a>描述信息</p>
<p id="zh-cn_topic_0118922245_p12889592"><a name="zh-cn_topic_0118922245_p12889592"></a><a name="zh-cn_topic_0118922245_p12889592"></a>字符长度不能大于255。</p>
<div class="note" id="zh-cn_topic_0118922245_note3630132716553"><a name="zh-cn_topic_0118922245_note3630132716553"></a><a name="zh-cn_topic_0118922245_note3630132716553"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118922245_p1163010271552"><a name="zh-cn_topic_0118922245_p1163010271552"></a><a name="zh-cn_topic_0118922245_p1163010271552"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"name": "DEVELOP",
	"remark": "开发环境"
}
```

## 响应消息<a name="zh-cn_topic_0118922245_section6979290"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0118922245_table62791297"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922245_row18005532"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922245_p49161963"><a name="zh-cn_topic_0118922245_p49161963"></a><a name="zh-cn_topic_0118922245_p49161963"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922245_p22696055"><a name="zh-cn_topic_0118922245_p22696055"></a><a name="zh-cn_topic_0118922245_p22696055"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922245_p26441127"><a name="zh-cn_topic_0118922245_p26441127"></a><a name="zh-cn_topic_0118922245_p26441127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922245_row61356515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922245_p3821844"><a name="zh-cn_topic_0118922245_p3821844"></a><a name="zh-cn_topic_0118922245_p3821844"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922245_p41133986"><a name="zh-cn_topic_0118922245_p41133986"></a><a name="zh-cn_topic_0118922245_p41133986"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922245_p43518580"><a name="zh-cn_topic_0118922245_p43518580"></a><a name="zh-cn_topic_0118922245_p43518580"></a>环境ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row56122907"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922245_p49661582"><a name="zh-cn_topic_0118922245_p49661582"></a><a name="zh-cn_topic_0118922245_p49661582"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922245_p63165243"><a name="zh-cn_topic_0118922245_p63165243"></a><a name="zh-cn_topic_0118922245_p63165243"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922245_p16111048"><a name="zh-cn_topic_0118922245_p16111048"></a><a name="zh-cn_topic_0118922245_p16111048"></a>环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row10781706"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922245_p902987"><a name="zh-cn_topic_0118922245_p902987"></a><a name="zh-cn_topic_0118922245_p902987"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922245_p6033088"><a name="zh-cn_topic_0118922245_p6033088"></a><a name="zh-cn_topic_0118922245_p6033088"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922245_p18918097"><a name="zh-cn_topic_0118922245_p18918097"></a><a name="zh-cn_topic_0118922245_p18918097"></a>创建环境的时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row36045152"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922245_p33976232"><a name="zh-cn_topic_0118922245_p33976232"></a><a name="zh-cn_topic_0118922245_p33976232"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922245_p611392"><a name="zh-cn_topic_0118922245_p611392"></a><a name="zh-cn_topic_0118922245_p611392"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922245_p49522768"><a name="zh-cn_topic_0118922245_p49522768"></a><a name="zh-cn_topic_0118922245_p49522768"></a>描述信息</p>
</td>
</tr>
</tbody>
</table>

响应参数样例：

```
{
	"id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
	"name": "DEVELOP",
	"remark": "开发环境",
	"create_time": "2017-12-28T12:50:47Z"
}
```

## 状态码<a name="zh-cn_topic_0118922245_section38058178"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118922245_table29667622"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922245_row33628505"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922245_p39554365"><a name="zh-cn_topic_0118922245_p39554365"></a><a name="zh-cn_topic_0118922245_p39554365"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922245_p49786990"><a name="zh-cn_topic_0118922245_p49786990"></a><a name="zh-cn_topic_0118922245_p49786990"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922245_row6214355"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922245_p33600724"><a name="zh-cn_topic_0118922245_p33600724"></a><a name="zh-cn_topic_0118922245_p33600724"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922245_p37304155"><a name="zh-cn_topic_0118922245_p37304155"></a><a name="zh-cn_topic_0118922245_p37304155"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row193075"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922245_p15639099"><a name="zh-cn_topic_0118922245_p15639099"></a><a name="zh-cn_topic_0118922245_p15639099"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922245_p58807483"><a name="zh-cn_topic_0118922245_p58807483"></a><a name="zh-cn_topic_0118922245_p58807483"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row59505304"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922245_p55200320"><a name="zh-cn_topic_0118922245_p55200320"></a><a name="zh-cn_topic_0118922245_p55200320"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922245_p42040949"><a name="zh-cn_topic_0118922245_p42040949"></a><a name="zh-cn_topic_0118922245_p42040949"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row42824223"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922245_p46210066"><a name="zh-cn_topic_0118922245_p46210066"></a><a name="zh-cn_topic_0118922245_p46210066"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922245_p52027845"><a name="zh-cn_topic_0118922245_p52027845"></a><a name="zh-cn_topic_0118922245_p52027845"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row65597422"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922245_p11790948"><a name="zh-cn_topic_0118922245_p11790948"></a><a name="zh-cn_topic_0118922245_p11790948"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922245_p15542768"><a name="zh-cn_topic_0118922245_p15542768"></a><a name="zh-cn_topic_0118922245_p15542768"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922245_row5667184"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922245_p56388789"><a name="zh-cn_topic_0118922245_p56388789"></a><a name="zh-cn_topic_0118922245_p56388789"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922245_p14947689"><a name="zh-cn_topic_0118922245_p14947689"></a><a name="zh-cn_topic_0118922245_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

