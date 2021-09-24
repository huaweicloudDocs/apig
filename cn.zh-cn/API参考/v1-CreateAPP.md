# 创建APP<a name="ZH-CN_TOPIC_0000001082221253"></a>

## 功能介绍<a name="zh-cn_topic_0225568833_section61362801"></a>

APP即应用，是一个可以访问API的身份标识。将API授权给APP后，APP即可调用API。

创建一个APP。

## URI<a name="zh-cn_topic_0225568833_section15394303"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568833_table66835314"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568833_row49580837"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568833_p56624893"><a name="zh-cn_topic_0225568833_p56624893"></a><a name="zh-cn_topic_0225568833_p56624893"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568833_p23213605"><a name="zh-cn_topic_0225568833_p23213605"></a><a name="zh-cn_topic_0225568833_p23213605"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568833_row1253829"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568833_p34451334"><a name="zh-cn_topic_0225568833_p34451334"></a><a name="zh-cn_topic_0225568833_p34451334"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568833_p39094671"><a name="zh-cn_topic_0225568833_p39094671"></a><a name="zh-cn_topic_0225568833_p39094671"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568833_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568833_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568833_p23103637"><a name="zh-cn_topic_0225568833_p23103637"></a><a name="zh-cn_topic_0225568833_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568833_p59455291"><a name="zh-cn_topic_0225568833_p59455291"></a><a name="zh-cn_topic_0225568833_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568833_p51149303"><a name="zh-cn_topic_0225568833_p51149303"></a><a name="zh-cn_topic_0225568833_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568833_p49452846"><a name="zh-cn_topic_0225568833_p49452846"></a><a name="zh-cn_topic_0225568833_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568833_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568833_p55878963"><a name="zh-cn_topic_0225568833_p55878963"></a><a name="zh-cn_topic_0225568833_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568833_p29902160"><a name="zh-cn_topic_0225568833_p29902160"></a><a name="zh-cn_topic_0225568833_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568833_p6155914"><a name="zh-cn_topic_0225568833_p6155914"></a><a name="zh-cn_topic_0225568833_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568833_p28867016"><a name="zh-cn_topic_0225568833_p28867016"></a><a name="zh-cn_topic_0225568833_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568833_p1780913159538"><a name="zh-cn_topic_0225568833_p1780913159538"></a><a name="zh-cn_topic_0225568833_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568833_p9809215115310"><a name="zh-cn_topic_0225568833_p9809215115310"></a><a name="zh-cn_topic_0225568833_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568833_p1280914152538"><a name="zh-cn_topic_0225568833_p1280914152538"></a><a name="zh-cn_topic_0225568833_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568833_p1880914157537"><a name="zh-cn_topic_0225568833_p1880914157537"></a><a name="zh-cn_topic_0225568833_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568833_section4331004"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568833_table12551817"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568833_row63926902"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568833_p10696570"><a name="zh-cn_topic_0225568833_p10696570"></a><a name="zh-cn_topic_0225568833_p10696570"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568833_p61115871"><a name="zh-cn_topic_0225568833_p61115871"></a><a name="zh-cn_topic_0225568833_p61115871"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568833_p51438541"><a name="zh-cn_topic_0225568833_p51438541"></a><a name="zh-cn_topic_0225568833_p51438541"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568833_p5772267"><a name="zh-cn_topic_0225568833_p5772267"></a><a name="zh-cn_topic_0225568833_p5772267"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568833_row64900449"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568833_p22445016"><a name="zh-cn_topic_0225568833_p22445016"></a><a name="zh-cn_topic_0225568833_p22445016"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568833_p6106999"><a name="zh-cn_topic_0225568833_p6106999"></a><a name="zh-cn_topic_0225568833_p6106999"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568833_p24904935"><a name="zh-cn_topic_0225568833_p24904935"></a><a name="zh-cn_topic_0225568833_p24904935"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568833_p4033872"><a name="zh-cn_topic_0225568833_p4033872"></a><a name="zh-cn_topic_0225568833_p4033872"></a>APP的名称</p>
<p id="zh-cn_topic_0225568833_p55011617"><a name="zh-cn_topic_0225568833_p55011617"></a><a name="zh-cn_topic_0225568833_p55011617"></a>支持汉字，英文，数字，“_”，且只能以英文和汉字开头，3 ~ 64个字符。</p>
<div class="note" id="zh-cn_topic_0225568833_note18685133019272"><a name="zh-cn_topic_0225568833_note18685133019272"></a><a name="zh-cn_topic_0225568833_note18685133019272"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568833_p1068523022711"><a name="zh-cn_topic_0225568833_p1068523022711"></a><a name="zh-cn_topic_0225568833_p1068523022711"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row36149089"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568833_p42395109"><a name="zh-cn_topic_0225568833_p42395109"></a><a name="zh-cn_topic_0225568833_p42395109"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568833_p11451768"><a name="zh-cn_topic_0225568833_p11451768"></a><a name="zh-cn_topic_0225568833_p11451768"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568833_p55178053"><a name="zh-cn_topic_0225568833_p55178053"></a><a name="zh-cn_topic_0225568833_p55178053"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568833_p40237298"><a name="zh-cn_topic_0225568833_p40237298"></a><a name="zh-cn_topic_0225568833_p40237298"></a>APP描述。</p>
<p id="zh-cn_topic_0225568833_p6416869"><a name="zh-cn_topic_0225568833_p6416869"></a><a name="zh-cn_topic_0225568833_p6416869"></a>字符长度不能大于255</p>
<div class="note" id="zh-cn_topic_0225568833_note2159356132719"><a name="zh-cn_topic_0225568833_note2159356132719"></a><a name="zh-cn_topic_0225568833_note2159356132719"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568833_p1715911562275"><a name="zh-cn_topic_0225568833_p1715911562275"></a><a name="zh-cn_topic_0225568833_p1715911562275"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row111420614382"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568833_p4115186203816"><a name="zh-cn_topic_0225568833_p4115186203816"></a><a name="zh-cn_topic_0225568833_p4115186203816"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568833_p18115669385"><a name="zh-cn_topic_0225568833_p18115669385"></a><a name="zh-cn_topic_0225568833_p18115669385"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568833_p151151266389"><a name="zh-cn_topic_0225568833_p151151266389"></a><a name="zh-cn_topic_0225568833_p151151266389"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568833_p141151066380"><a name="zh-cn_topic_0225568833_p141151066380"></a><a name="zh-cn_topic_0225568833_p141151066380"></a>APP的key</p>
<p id="zh-cn_topic_0225568833_p14879124513402"><a name="zh-cn_topic_0225568833_p14879124513402"></a><a name="zh-cn_topic_0225568833_p14879124513402"></a>支持英文，数字，“_”,“-”,且只能以英文或数字开头，8 ~ 64个字符。</p>
<p id="zh-cn_topic_0225568833_p610473083912"><a name="zh-cn_topic_0225568833_p610473083912"></a><a name="zh-cn_topic_0225568833_p610473083912"></a></p>
<div class="note" id="zh-cn_topic_0225568833_note8622433183712"><a name="zh-cn_topic_0225568833_note8622433183712"></a><a name="zh-cn_topic_0225568833_note8622433183712"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568833_p26225334373"><a name="zh-cn_topic_0225568833_p26225334373"></a><a name="zh-cn_topic_0225568833_p26225334373"></a>只支持部分region自定义。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row147181873819"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568833_p571817817386"><a name="zh-cn_topic_0225568833_p571817817386"></a><a name="zh-cn_topic_0225568833_p571817817386"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568833_p07197813819"><a name="zh-cn_topic_0225568833_p07197813819"></a><a name="zh-cn_topic_0225568833_p07197813819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568833_p1871928203812"><a name="zh-cn_topic_0225568833_p1871928203812"></a><a name="zh-cn_topic_0225568833_p1871928203812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568833_p177191863810"><a name="zh-cn_topic_0225568833_p177191863810"></a><a name="zh-cn_topic_0225568833_p177191863810"></a>密钥</p>
<p id="zh-cn_topic_0225568833_p69053295477"><a name="zh-cn_topic_0225568833_p69053295477"></a><a name="zh-cn_topic_0225568833_p69053295477"></a>支持英文，数字，“_”,“-”,“_”,“!”,“@”,“#”,“$”,“%”,且只能以英文或数字开头，8 ~ 64个字符。</p>
<p id="zh-cn_topic_0225568833_p790520296470"><a name="zh-cn_topic_0225568833_p790520296470"></a><a name="zh-cn_topic_0225568833_p790520296470"></a></p>
<div class="note" id="zh-cn_topic_0225568833_note388252002711"><a name="zh-cn_topic_0225568833_note388252002711"></a><a name="zh-cn_topic_0225568833_note388252002711"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568833_p1388222082716"><a name="zh-cn_topic_0225568833_p1388222082716"></a><a name="zh-cn_topic_0225568833_p1388222082716"></a>只支持部分region自定义。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "name": "app_001",
  "remark": "first app",
  "app_key": "app_key_sample",
  "app_secret": "app_secret_sample"
}
```

## 响应消息<a name="zh-cn_topic_0225568833_section15267056"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568833_table20910139"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568833_row9919741"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568833_p65301594"><a name="zh-cn_topic_0225568833_p65301594"></a><a name="zh-cn_topic_0225568833_p65301594"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568833_p54937751"><a name="zh-cn_topic_0225568833_p54937751"></a><a name="zh-cn_topic_0225568833_p54937751"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568833_p20772828"><a name="zh-cn_topic_0225568833_p20772828"></a><a name="zh-cn_topic_0225568833_p20772828"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568833_row4877522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p59535008"><a name="zh-cn_topic_0225568833_p59535008"></a><a name="zh-cn_topic_0225568833_p59535008"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p57606383"><a name="zh-cn_topic_0225568833_p57606383"></a><a name="zh-cn_topic_0225568833_p57606383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p35605479"><a name="zh-cn_topic_0225568833_p35605479"></a><a name="zh-cn_topic_0225568833_p35605479"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row52013857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p52372904"><a name="zh-cn_topic_0225568833_p52372904"></a><a name="zh-cn_topic_0225568833_p52372904"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p14346860"><a name="zh-cn_topic_0225568833_p14346860"></a><a name="zh-cn_topic_0225568833_p14346860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p21245012"><a name="zh-cn_topic_0225568833_p21245012"></a><a name="zh-cn_topic_0225568833_p21245012"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row56987385"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p52575507"><a name="zh-cn_topic_0225568833_p52575507"></a><a name="zh-cn_topic_0225568833_p52575507"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p30757702"><a name="zh-cn_topic_0225568833_p30757702"></a><a name="zh-cn_topic_0225568833_p30757702"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p8345913"><a name="zh-cn_topic_0225568833_p8345913"></a><a name="zh-cn_topic_0225568833_p8345913"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row8004354"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p44372920"><a name="zh-cn_topic_0225568833_p44372920"></a><a name="zh-cn_topic_0225568833_p44372920"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p37436804"><a name="zh-cn_topic_0225568833_p37436804"></a><a name="zh-cn_topic_0225568833_p37436804"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p12482251"><a name="zh-cn_topic_0225568833_p12482251"></a><a name="zh-cn_topic_0225568833_p12482251"></a>APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row45231401"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p39864887"><a name="zh-cn_topic_0225568833_p39864887"></a><a name="zh-cn_topic_0225568833_p39864887"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p7830389"><a name="zh-cn_topic_0225568833_p7830389"></a><a name="zh-cn_topic_0225568833_p7830389"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p30281739"><a name="zh-cn_topic_0225568833_p30281739"></a><a name="zh-cn_topic_0225568833_p30281739"></a>密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row17581831677"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p148381123152516"><a name="zh-cn_topic_0225568833_p148381123152516"></a><a name="zh-cn_topic_0225568833_p148381123152516"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p10838223112516"><a name="zh-cn_topic_0225568833_p10838223112516"></a><a name="zh-cn_topic_0225568833_p10838223112516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p128381023202515"><a name="zh-cn_topic_0225568833_p128381023202515"></a><a name="zh-cn_topic_0225568833_p128381023202515"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0225568833_ul1126756132511"></a><a name="zh-cn_topic_0225568833_ul1126756132511"></a><ul id="zh-cn_topic_0225568833_ul1126756132511"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row4100199"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p63680693"><a name="zh-cn_topic_0225568833_p63680693"></a><a name="zh-cn_topic_0225568833_p63680693"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p57862512"><a name="zh-cn_topic_0225568833_p57862512"></a><a name="zh-cn_topic_0225568833_p57862512"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p56351871"><a name="zh-cn_topic_0225568833_p56351871"></a><a name="zh-cn_topic_0225568833_p56351871"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row37404794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p9889443"><a name="zh-cn_topic_0225568833_p9889443"></a><a name="zh-cn_topic_0225568833_p9889443"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p62847380"><a name="zh-cn_topic_0225568833_p62847380"></a><a name="zh-cn_topic_0225568833_p62847380"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p57473014"><a name="zh-cn_topic_0225568833_p57473014"></a><a name="zh-cn_topic_0225568833_p57473014"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row47495080"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p21896310"><a name="zh-cn_topic_0225568833_p21896310"></a><a name="zh-cn_topic_0225568833_p21896310"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p28770696"><a name="zh-cn_topic_0225568833_p28770696"></a><a name="zh-cn_topic_0225568833_p28770696"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p48725063"><a name="zh-cn_topic_0225568833_p48725063"></a><a name="zh-cn_topic_0225568833_p48725063"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row14138615144813"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568833_p14855159163015"><a name="zh-cn_topic_0225568833_p14855159163015"></a><a name="zh-cn_topic_0225568833_p14855159163015"></a>app_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568833_p12855195993012"><a name="zh-cn_topic_0225568833_p12855195993012"></a><a name="zh-cn_topic_0225568833_p12855195993012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568833_p1085575910302"><a name="zh-cn_topic_0225568833_p1085575910302"></a><a name="zh-cn_topic_0225568833_p1085575910302"></a>APP类型，默认为apig</p>
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
	"remark": "第一个应用",
	"register_time": "2017-12-28T12:26:54.2345858Z",
	"update_time": "2017-12-28T12:26:54.2345858Z",
        "app_type": "apig"
}
```

## 状态码<a name="zh-cn_topic_0225568833_section38979041"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568833_table665003"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568833_row9107269"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568833_p66600187"><a name="zh-cn_topic_0225568833_p66600187"></a><a name="zh-cn_topic_0225568833_p66600187"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568833_p25906037"><a name="zh-cn_topic_0225568833_p25906037"></a><a name="zh-cn_topic_0225568833_p25906037"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568833_row18014235"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568833_p49866967"><a name="zh-cn_topic_0225568833_p49866967"></a><a name="zh-cn_topic_0225568833_p49866967"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568833_p12692494"><a name="zh-cn_topic_0225568833_p12692494"></a><a name="zh-cn_topic_0225568833_p12692494"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row47123588"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568833_p58914306"><a name="zh-cn_topic_0225568833_p58914306"></a><a name="zh-cn_topic_0225568833_p58914306"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568833_p7329456"><a name="zh-cn_topic_0225568833_p7329456"></a><a name="zh-cn_topic_0225568833_p7329456"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row65965104"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568833_p41573226"><a name="zh-cn_topic_0225568833_p41573226"></a><a name="zh-cn_topic_0225568833_p41573226"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568833_p9203142078"><a name="zh-cn_topic_0225568833_p9203142078"></a><a name="zh-cn_topic_0225568833_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row40784364"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568833_p15199212"><a name="zh-cn_topic_0225568833_p15199212"></a><a name="zh-cn_topic_0225568833_p15199212"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568833_p13949586"><a name="zh-cn_topic_0225568833_p13949586"></a><a name="zh-cn_topic_0225568833_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568833_row7263502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568833_p51472750"><a name="zh-cn_topic_0225568833_p51472750"></a><a name="zh-cn_topic_0225568833_p51472750"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568833_p8543194"><a name="zh-cn_topic_0225568833_p8543194"></a><a name="zh-cn_topic_0225568833_p8543194"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

