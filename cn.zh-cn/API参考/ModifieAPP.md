# 修改APP<a name="ZH-CN_TOPIC_0000001082135095"></a>

## 功能介绍<a name="zh-cn_topic_0118921759_section63138047"></a>

修改指定APP的信息。其中可修改的属性为：name、remark，当支持用户自定义key和secret的开关开启时，app\_key和app\_secret也支持修改，其它属性不可修改。

## URI<a name="zh-cn_topic_0118921759_section31371512"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921759_table37143220"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921759_row28749009"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921759_p46968374"><a name="zh-cn_topic_0118921759_p46968374"></a><a name="zh-cn_topic_0118921759_p46968374"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921759_p46341964"><a name="zh-cn_topic_0118921759_p46341964"></a><a name="zh-cn_topic_0118921759_p46341964"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921759_row62711610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921759_p46475689"><a name="zh-cn_topic_0118921759_p46475689"></a><a name="zh-cn_topic_0118921759_p46475689"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921759_p6434497"><a name="zh-cn_topic_0118921759_p6434497"></a><a name="zh-cn_topic_0118921759_p6434497"></a>/v1.0/apigw/apps/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921759_table51432233"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921759_row58308749"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921759_p25388256"><a name="zh-cn_topic_0118921759_p25388256"></a><a name="zh-cn_topic_0118921759_p25388256"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921759_p43182835"><a name="zh-cn_topic_0118921759_p43182835"></a><a name="zh-cn_topic_0118921759_p43182835"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921759_p8148718"><a name="zh-cn_topic_0118921759_p8148718"></a><a name="zh-cn_topic_0118921759_p8148718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921759_p56066426"><a name="zh-cn_topic_0118921759_p56066426"></a><a name="zh-cn_topic_0118921759_p56066426"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921759_row45086654"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921759_p28140387"><a name="zh-cn_topic_0118921759_p28140387"></a><a name="zh-cn_topic_0118921759_p28140387"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921759_p64778897"><a name="zh-cn_topic_0118921759_p64778897"></a><a name="zh-cn_topic_0118921759_p64778897"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921759_p12599279"><a name="zh-cn_topic_0118921759_p12599279"></a><a name="zh-cn_topic_0118921759_p12599279"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921759_p13908645"><a name="zh-cn_topic_0118921759_p13908645"></a><a name="zh-cn_topic_0118921759_p13908645"></a>APP的编号，可通过查询APP列表获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921759_section13908152"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921759_table52858460"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921759_row52119005"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921759_p60889838"><a name="zh-cn_topic_0118921759_p60889838"></a><a name="zh-cn_topic_0118921759_p60889838"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921759_p33129840"><a name="zh-cn_topic_0118921759_p33129840"></a><a name="zh-cn_topic_0118921759_p33129840"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921759_p66271370"><a name="zh-cn_topic_0118921759_p66271370"></a><a name="zh-cn_topic_0118921759_p66271370"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921759_p66380773"><a name="zh-cn_topic_0118921759_p66380773"></a><a name="zh-cn_topic_0118921759_p66380773"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921759_row8133545"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921759_p54837372"><a name="zh-cn_topic_0118921759_p54837372"></a><a name="zh-cn_topic_0118921759_p54837372"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921759_p12642185"><a name="zh-cn_topic_0118921759_p12642185"></a><a name="zh-cn_topic_0118921759_p12642185"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921759_p17384054"><a name="zh-cn_topic_0118921759_p17384054"></a><a name="zh-cn_topic_0118921759_p17384054"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921759_p65931115"><a name="zh-cn_topic_0118921759_p65931115"></a><a name="zh-cn_topic_0118921759_p65931115"></a>APP的名称</p>
<p id="zh-cn_topic_0118921759_p13836702"><a name="zh-cn_topic_0118921759_p13836702"></a><a name="zh-cn_topic_0118921759_p13836702"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64个字符。</p>
<div class="note" id="zh-cn_topic_0118921759_note1482512316386"><a name="zh-cn_topic_0118921759_note1482512316386"></a><a name="zh-cn_topic_0118921759_note1482512316386"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118921759_p178261538382"><a name="zh-cn_topic_0118921759_p178261538382"></a><a name="zh-cn_topic_0118921759_p178261538382"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row37808430"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921759_p42583966"><a name="zh-cn_topic_0118921759_p42583966"></a><a name="zh-cn_topic_0118921759_p42583966"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921759_p26749231"><a name="zh-cn_topic_0118921759_p26749231"></a><a name="zh-cn_topic_0118921759_p26749231"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921759_p19204104"><a name="zh-cn_topic_0118921759_p19204104"></a><a name="zh-cn_topic_0118921759_p19204104"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921759_p12028626"><a name="zh-cn_topic_0118921759_p12028626"></a><a name="zh-cn_topic_0118921759_p12028626"></a>APP描述</p>
<p id="zh-cn_topic_0118921759_p44716639"><a name="zh-cn_topic_0118921759_p44716639"></a><a name="zh-cn_topic_0118921759_p44716639"></a>字符长度不能大于255</p>
<div class="note" id="zh-cn_topic_0118921759_note19661163403814"><a name="zh-cn_topic_0118921759_note19661163403814"></a><a name="zh-cn_topic_0118921759_note19661163403814"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118921759_p066213419384"><a name="zh-cn_topic_0118921759_p066213419384"></a><a name="zh-cn_topic_0118921759_p066213419384"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row345025916519"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921759_p4115186203816"><a name="zh-cn_topic_0118921759_p4115186203816"></a><a name="zh-cn_topic_0118921759_p4115186203816"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921759_p18115669385"><a name="zh-cn_topic_0118921759_p18115669385"></a><a name="zh-cn_topic_0118921759_p18115669385"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921759_p151151266389"><a name="zh-cn_topic_0118921759_p151151266389"></a><a name="zh-cn_topic_0118921759_p151151266389"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921759_p141151066380"><a name="zh-cn_topic_0118921759_p141151066380"></a><a name="zh-cn_topic_0118921759_p141151066380"></a>APP的key</p>
<p id="zh-cn_topic_0118921759_p14879124513402"><a name="zh-cn_topic_0118921759_p14879124513402"></a><a name="zh-cn_topic_0118921759_p14879124513402"></a>支持英文，数字，“_”,“-”,且只能以英文或数字开头，8 ~ 64个字符。</p>
<div class="note" id="zh-cn_topic_0118921759_note8622433183712"><a name="zh-cn_topic_0118921759_note8622433183712"></a><a name="zh-cn_topic_0118921759_note8622433183712"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118921759_p26225334373"><a name="zh-cn_topic_0118921759_p26225334373"></a><a name="zh-cn_topic_0118921759_p26225334373"></a>只支持部分region自定义。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row13951012524"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921759_p571817817386"><a name="zh-cn_topic_0118921759_p571817817386"></a><a name="zh-cn_topic_0118921759_p571817817386"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921759_p07197813819"><a name="zh-cn_topic_0118921759_p07197813819"></a><a name="zh-cn_topic_0118921759_p07197813819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921759_p1871928203812"><a name="zh-cn_topic_0118921759_p1871928203812"></a><a name="zh-cn_topic_0118921759_p1871928203812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921759_p177191863810"><a name="zh-cn_topic_0118921759_p177191863810"></a><a name="zh-cn_topic_0118921759_p177191863810"></a>密钥</p>
<p id="zh-cn_topic_0118921759_p69053295477"><a name="zh-cn_topic_0118921759_p69053295477"></a><a name="zh-cn_topic_0118921759_p69053295477"></a>支持英文，数字，“_”,“-”,“_”,“!”,“@”,“#”,“$”,“%”,且只能以英文或数字开头，8 ~ 64个字符。</p>
<div class="note" id="zh-cn_topic_0118921759_note862799163816"><a name="zh-cn_topic_0118921759_note862799163816"></a><a name="zh-cn_topic_0118921759_note862799163816"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118921759_p26272923814"><a name="zh-cn_topic_0118921759_p26272923814"></a><a name="zh-cn_topic_0118921759_p26272923814"></a>只支持部分region自定义。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"name": "app_001",
	"remark": "第一个APP",
        "app_key": "app_key_sample",
        "app_secret": "app_secret_sample"
}
```

## 响应消息<a name="zh-cn_topic_0118921759_section52818489"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0118921759_table26102067"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921759_row9058262"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921759_p62630620"><a name="zh-cn_topic_0118921759_p62630620"></a><a name="zh-cn_topic_0118921759_p62630620"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921759_p39915430"><a name="zh-cn_topic_0118921759_p39915430"></a><a name="zh-cn_topic_0118921759_p39915430"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921759_p11924380"><a name="zh-cn_topic_0118921759_p11924380"></a><a name="zh-cn_topic_0118921759_p11924380"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921759_row26350760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p54036783"><a name="zh-cn_topic_0118921759_p54036783"></a><a name="zh-cn_topic_0118921759_p54036783"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p14903323"><a name="zh-cn_topic_0118921759_p14903323"></a><a name="zh-cn_topic_0118921759_p14903323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p66318548"><a name="zh-cn_topic_0118921759_p66318548"></a><a name="zh-cn_topic_0118921759_p66318548"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row59996025"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p27839823"><a name="zh-cn_topic_0118921759_p27839823"></a><a name="zh-cn_topic_0118921759_p27839823"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p40433190"><a name="zh-cn_topic_0118921759_p40433190"></a><a name="zh-cn_topic_0118921759_p40433190"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p53862949"><a name="zh-cn_topic_0118921759_p53862949"></a><a name="zh-cn_topic_0118921759_p53862949"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row15004500"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p7404963"><a name="zh-cn_topic_0118921759_p7404963"></a><a name="zh-cn_topic_0118921759_p7404963"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p62931119"><a name="zh-cn_topic_0118921759_p62931119"></a><a name="zh-cn_topic_0118921759_p62931119"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p64255839"><a name="zh-cn_topic_0118921759_p64255839"></a><a name="zh-cn_topic_0118921759_p64255839"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row41431640"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p519674"><a name="zh-cn_topic_0118921759_p519674"></a><a name="zh-cn_topic_0118921759_p519674"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p42093620"><a name="zh-cn_topic_0118921759_p42093620"></a><a name="zh-cn_topic_0118921759_p42093620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p54140079"><a name="zh-cn_topic_0118921759_p54140079"></a><a name="zh-cn_topic_0118921759_p54140079"></a>APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row17498668"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p8106027"><a name="zh-cn_topic_0118921759_p8106027"></a><a name="zh-cn_topic_0118921759_p8106027"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p52608446"><a name="zh-cn_topic_0118921759_p52608446"></a><a name="zh-cn_topic_0118921759_p52608446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p33425742"><a name="zh-cn_topic_0118921759_p33425742"></a><a name="zh-cn_topic_0118921759_p33425742"></a>密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row155511111916"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p148381123152516"><a name="zh-cn_topic_0118921759_p148381123152516"></a><a name="zh-cn_topic_0118921759_p148381123152516"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p10838223112516"><a name="zh-cn_topic_0118921759_p10838223112516"></a><a name="zh-cn_topic_0118921759_p10838223112516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p128381023202515"><a name="zh-cn_topic_0118921759_p128381023202515"></a><a name="zh-cn_topic_0118921759_p128381023202515"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0118921759_ul1126756132511"></a><a name="zh-cn_topic_0118921759_ul1126756132511"></a><ul id="zh-cn_topic_0118921759_ul1126756132511"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row32396224"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p6848469"><a name="zh-cn_topic_0118921759_p6848469"></a><a name="zh-cn_topic_0118921759_p6848469"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p17855131"><a name="zh-cn_topic_0118921759_p17855131"></a><a name="zh-cn_topic_0118921759_p17855131"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p36979513"><a name="zh-cn_topic_0118921759_p36979513"></a><a name="zh-cn_topic_0118921759_p36979513"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row64380169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p47411232"><a name="zh-cn_topic_0118921759_p47411232"></a><a name="zh-cn_topic_0118921759_p47411232"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p15104546"><a name="zh-cn_topic_0118921759_p15104546"></a><a name="zh-cn_topic_0118921759_p15104546"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p15508729"><a name="zh-cn_topic_0118921759_p15508729"></a><a name="zh-cn_topic_0118921759_p15508729"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row5360840"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p31574905"><a name="zh-cn_topic_0118921759_p31574905"></a><a name="zh-cn_topic_0118921759_p31574905"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p7430514"><a name="zh-cn_topic_0118921759_p7430514"></a><a name="zh-cn_topic_0118921759_p7430514"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p65000796"><a name="zh-cn_topic_0118921759_p65000796"></a><a name="zh-cn_topic_0118921759_p65000796"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row6603458153210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921759_p14855159163015"><a name="zh-cn_topic_0118921759_p14855159163015"></a><a name="zh-cn_topic_0118921759_p14855159163015"></a>app_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921759_p12855195993012"><a name="zh-cn_topic_0118921759_p12855195993012"></a><a name="zh-cn_topic_0118921759_p12855195993012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921759_p1085575910302"><a name="zh-cn_topic_0118921759_p1085575910302"></a><a name="zh-cn_topic_0118921759_p1085575910302"></a>APP类型，默认为apig</p>
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
	"update_time": "2017-12-28T12:28:07.2966182Z",
        "app_type": "apig"
}
```

## 状态码<a name="zh-cn_topic_0118921759_section58064504"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118921759_table65661620"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921759_row38386508"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921759_p22299447"><a name="zh-cn_topic_0118921759_p22299447"></a><a name="zh-cn_topic_0118921759_p22299447"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921759_p61424758"><a name="zh-cn_topic_0118921759_p61424758"></a><a name="zh-cn_topic_0118921759_p61424758"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921759_row9349490"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921759_p19111186"><a name="zh-cn_topic_0118921759_p19111186"></a><a name="zh-cn_topic_0118921759_p19111186"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921759_p4502206"><a name="zh-cn_topic_0118921759_p4502206"></a><a name="zh-cn_topic_0118921759_p4502206"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row40519861"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921759_p60883295"><a name="zh-cn_topic_0118921759_p60883295"></a><a name="zh-cn_topic_0118921759_p60883295"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921759_p32599882"><a name="zh-cn_topic_0118921759_p32599882"></a><a name="zh-cn_topic_0118921759_p32599882"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row24963487"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921759_p8776590"><a name="zh-cn_topic_0118921759_p8776590"></a><a name="zh-cn_topic_0118921759_p8776590"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921759_p191535218816"><a name="zh-cn_topic_0118921759_p191535218816"></a><a name="zh-cn_topic_0118921759_p191535218816"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row22792350"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921759_p34241051"><a name="zh-cn_topic_0118921759_p34241051"></a><a name="zh-cn_topic_0118921759_p34241051"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921759_p13949586"><a name="zh-cn_topic_0118921759_p13949586"></a><a name="zh-cn_topic_0118921759_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row64337830"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921759_p43981707"><a name="zh-cn_topic_0118921759_p43981707"></a><a name="zh-cn_topic_0118921759_p43981707"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921759_p5748492"><a name="zh-cn_topic_0118921759_p5748492"></a><a name="zh-cn_topic_0118921759_p5748492"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921759_row51736435"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921759_p29901739"><a name="zh-cn_topic_0118921759_p29901739"></a><a name="zh-cn_topic_0118921759_p29901739"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921759_p6121779"><a name="zh-cn_topic_0118921759_p6121779"></a><a name="zh-cn_topic_0118921759_p6121779"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

