# 发布API<a name="apig-zh-api-180713028"></a>

## 功能介绍<a name="section6627989"></a>

将一个指定的API发布到一个指定的环境，API只有发布后，才能够被调用，且只能在该环境上才能被调用。未发布的API无法被调用。

## URI<a name="section59651907"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table42014202"></a>
<table><thead align="left"><tr id="row11048869"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p22543169"><a name="p22543169"></a><a name="p22543169"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p14057426"><a name="p14057426"></a><a name="p14057426"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row64909760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p23199218"><a name="p23199218"></a><a name="p23199218"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p88529"><a name="p88529"></a><a name="p88529"></a>/v1.0/apigw/apis/publish/{api_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table796764"></a>
<table><thead align="left"><tr id="row53401841"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p30581871"><a name="p30581871"></a><a name="p30581871"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p61212526"><a name="p61212526"></a><a name="p61212526"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p59267606"><a name="p59267606"></a><a name="p59267606"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p35946766"><a name="p35946766"></a><a name="p35946766"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26006910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p26184975"><a name="p26184975"></a><a name="p26184975"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p40608232"><a name="p40608232"></a><a name="p40608232"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p932530"><a name="p932530"></a><a name="p932530"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p8426133"><a name="p8426133"></a><a name="p8426133"></a>API的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section67105121"></a>

**表 3**  参数说明

<a name="table11428152"></a>
<table><thead align="left"><tr id="row63593960"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p50837158"><a name="p50837158"></a><a name="p50837158"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p24169108"><a name="p24169108"></a><a name="p24169108"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p11540698"><a name="p11540698"></a><a name="p11540698"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p62381345"><a name="p62381345"></a><a name="p62381345"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19724176"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p54154448"><a name="p54154448"></a><a name="p54154448"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p24434185"><a name="p24434185"></a><a name="p24434185"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p33011938"><a name="p33011938"></a><a name="p33011938"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p56721283"><a name="p56721283"></a><a name="p56721283"></a>环境的编号，即：API需要发布到哪个环境</p>
</td>
</tr>
<tr id="row10755391"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p65880381"><a name="p65880381"></a><a name="p65880381"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p34710655"><a name="p34710655"></a><a name="p34710655"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p60099694"><a name="p60099694"></a><a name="p60099694"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p36237041"><a name="p36237041"></a><a name="p36237041"></a>对本次发布动作的简述</p>
<p id="p43019771"><a name="p43019771"></a><a name="p43019771"></a>字符长度不超过255</p>
<div class="note" id="note1834710250914"><a name="note1834710250914"></a><a name="note1834710250914"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p22422298915"><a name="p22422298915"></a><a name="p22422298915"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
	"remark": "发布到生产环境"
}
```

## 响应消息<a name="section66805754"></a>

**表 4**  参数说明

<a name="table2981672313"></a>
<table><thead align="left"><tr id="row898177103111"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="p109837183116"><a name="p109837183116"></a><a name="p109837183116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="p1098474319"><a name="p1098474319"></a><a name="p1098474319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="p1398197193117"><a name="p1398197193117"></a><a name="p1398197193117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49812719314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p18981672315"><a name="p18981672315"></a><a name="p18981672315"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p209815717318"><a name="p209815717318"></a><a name="p209815717318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p8980773120"><a name="p8980773120"></a><a name="p8980773120"></a>发布记录的ID</p>
</td>
</tr>
<tr id="row119827123112"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p159814710314"><a name="p159814710314"></a><a name="p159814710314"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p1698871311"><a name="p1698871311"></a><a name="p1698871311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p109897153112"><a name="p109897153112"></a><a name="p109897153112"></a>API编号</p>
</td>
</tr>
<tr id="row998187163114"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p129814713315"><a name="p129814713315"></a><a name="p129814713315"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p13987723113"><a name="p13987723113"></a><a name="p13987723113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p109819712314"><a name="p109819712314"></a><a name="p109819712314"></a>发布的环境编号</p>
</td>
</tr>
<tr id="row4981679311"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p1098147143114"><a name="p1098147143114"></a><a name="p1098147143114"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p998197113114"><a name="p998197113114"></a><a name="p998197113114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p99816773110"><a name="p99816773110"></a><a name="p99816773110"></a>发布描述</p>
</td>
</tr>
<tr id="row129897193111"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p998117163115"><a name="p998117163115"></a><a name="p998117163115"></a>publish_time</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p59813711317"><a name="p59813711317"></a><a name="p59813711317"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p5989733118"><a name="p5989733118"></a><a name="p5989733118"></a>发布时间</p>
</td>
</tr>
<tr id="row864017241176"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p12640172461714"><a name="p12640172461714"></a><a name="p12640172461714"></a>version_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p6640102461713"><a name="p6640102461713"></a><a name="p6640102461713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p19640152410176"><a name="p19640152410176"></a><a name="p19640152410176"></a>版本号</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "publish_id": "5b729aa252764739be2c37ef0d66dc63",
  "api_id": "7addcd00cfab433984b1d8bf2fe08aaa",
  "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
  "version_id": "3d9dcb733ba34352b0d02f85fd16b026",
  "remark": "string",
  "publish_time": "2018-07-26T13:18:04.1079916Z"
}
```

## 状态码<a name="section67075185"></a>

**表 5**  返回消息说明

<a name="table15714732"></a>
<table><thead align="left"><tr id="row24997277"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p11513591"><a name="p11513591"></a><a name="p11513591"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p60185706"><a name="p60185706"></a><a name="p60185706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row43203997"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9862840"><a name="p9862840"></a><a name="p9862840"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p73578115452"><a name="p73578115452"></a><a name="p73578115452"></a>Created</p>
</td>
</tr>
<tr id="row9362312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20149775"><a name="p20149775"></a><a name="p20149775"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p21519099"><a name="p21519099"></a><a name="p21519099"></a>Bad Request</p>
</td>
</tr>
<tr id="row59454171"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p51058521"><a name="p51058521"></a><a name="p51058521"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row43351211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p21787193"><a name="p21787193"></a><a name="p21787193"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row45172181"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p35068062"><a name="p35068062"></a><a name="p35068062"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p21940743"><a name="p21940743"></a><a name="p21940743"></a>Not Found</p>
</td>
</tr>
<tr id="row63248959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22892027"><a name="p22892027"></a><a name="p22892027"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

