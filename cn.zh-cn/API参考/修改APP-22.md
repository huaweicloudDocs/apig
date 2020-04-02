# 修改APP<a name="apig-phapi-180713037"></a>

## 功能介绍<a name="section63138047"></a>

修改指定APP的信息。其中可修改的属性为：name、remark，当支持用户自定义key和secret的开关开启时，app\_key和app\_secret也支持修改，其它属性不可修改。

## URI<a name="section31371512"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table37143220"></a>
<table><thead align="left"><tr id="row28749009"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p46968374"><a name="p46968374"></a><a name="p46968374"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p46341964"><a name="p46341964"></a><a name="p46341964"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row62711610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p46475689"><a name="p46475689"></a><a name="p46475689"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6434497"><a name="p6434497"></a><a name="p6434497"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table51432233"></a>
<table><thead align="left"><tr id="row58308749"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p25388256"><a name="p25388256"></a><a name="p25388256"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p43182835"><a name="p43182835"></a><a name="p43182835"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p8148718"><a name="p8148718"></a><a name="p8148718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p56066426"><a name="p56066426"></a><a name="p56066426"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18537163314383"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row1534363315387"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row45086654"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p28140387"><a name="p28140387"></a><a name="p28140387"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p64778897"><a name="p64778897"></a><a name="p64778897"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p12599279"><a name="p12599279"></a><a name="p12599279"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p13908645"><a name="p13908645"></a><a name="p13908645"></a>APP的编号，可通过查询APP列表获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section13908152"></a>

**表 3**  参数说明

<a name="table52858460"></a>
<table><thead align="left"><tr id="row52119005"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p60889838"><a name="p60889838"></a><a name="p60889838"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p33129840"><a name="p33129840"></a><a name="p33129840"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p66271370"><a name="p66271370"></a><a name="p66271370"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p66380773"><a name="p66380773"></a><a name="p66380773"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8133545"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p54837372"><a name="p54837372"></a><a name="p54837372"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p12642185"><a name="p12642185"></a><a name="p12642185"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p17384054"><a name="p17384054"></a><a name="p17384054"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p65931115"><a name="p65931115"></a><a name="p65931115"></a>APP的名称</p>
<p id="p13836702"><a name="p13836702"></a><a name="p13836702"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64个字符。</p>
<div class="note" id="note1482512316386"><a name="note1482512316386"></a><a name="note1482512316386"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p178261538382"><a name="p178261538382"></a><a name="p178261538382"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row37808430"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p42583966"><a name="p42583966"></a><a name="p42583966"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p26749231"><a name="p26749231"></a><a name="p26749231"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p19204104"><a name="p19204104"></a><a name="p19204104"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p12028626"><a name="p12028626"></a><a name="p12028626"></a>APP描述</p>
<p id="p44716639"><a name="p44716639"></a><a name="p44716639"></a>字符长度不能大于255</p>
<div class="note" id="note19661163403814"><a name="note19661163403814"></a><a name="note19661163403814"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p066213419384"><a name="p066213419384"></a><a name="p066213419384"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row345025916519"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p4115186203816"><a name="p4115186203816"></a><a name="p4115186203816"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p18115669385"><a name="p18115669385"></a><a name="p18115669385"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p151151266389"><a name="p151151266389"></a><a name="p151151266389"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p141151066380"><a name="p141151066380"></a><a name="p141151066380"></a>APP的key</p>
<p id="p14879124513402"><a name="p14879124513402"></a><a name="p14879124513402"></a>支持英文，数字，“_”,“-”,且只能以英文或数字开头，8 ~ 64个字符。</p>
<p id="p610473083912"><a name="p610473083912"></a><a name="p610473083912"></a>用户自定义APP的key需要开启配额开关</p>
</td>
</tr>
<tr id="row13951012524"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p571817817386"><a name="p571817817386"></a><a name="p571817817386"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p07197813819"><a name="p07197813819"></a><a name="p07197813819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1871928203812"><a name="p1871928203812"></a><a name="p1871928203812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p177191863810"><a name="p177191863810"></a><a name="p177191863810"></a>密钥</p>
<p id="p69053295477"><a name="p69053295477"></a><a name="p69053295477"></a>支持英文，数字，“_”,“-”,“_”,“!”,“@”,“#”,“$”,“%”,且只能以英文或数字开头，8 ~ 64个字符。</p>
<p id="p790520296470"><a name="p790520296470"></a><a name="p790520296470"></a>用户自定义APP的密钥需要开启配额开关</p>
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

## 响应消息<a name="section52818489"></a>

**表 4**  参数说明

<a name="table26102067"></a>
<table><thead align="left"><tr id="row9058262"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p62630620"><a name="p62630620"></a><a name="p62630620"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p39915430"><a name="p39915430"></a><a name="p39915430"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p11924380"><a name="p11924380"></a><a name="p11924380"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26350760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p54036783"><a name="p54036783"></a><a name="p54036783"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14903323"><a name="p14903323"></a><a name="p14903323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66318548"><a name="p66318548"></a><a name="p66318548"></a>编号</p>
</td>
</tr>
<tr id="row59996025"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p27839823"><a name="p27839823"></a><a name="p27839823"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p40433190"><a name="p40433190"></a><a name="p40433190"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53862949"><a name="p53862949"></a><a name="p53862949"></a>名称</p>
</td>
</tr>
<tr id="row15004500"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7404963"><a name="p7404963"></a><a name="p7404963"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62931119"><a name="p62931119"></a><a name="p62931119"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p64255839"><a name="p64255839"></a><a name="p64255839"></a>状态</p>
</td>
</tr>
<tr id="row41431640"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p519674"><a name="p519674"></a><a name="p519674"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42093620"><a name="p42093620"></a><a name="p42093620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54140079"><a name="p54140079"></a><a name="p54140079"></a>APP的key</p>
</td>
</tr>
<tr id="row17498668"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8106027"><a name="p8106027"></a><a name="p8106027"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p52608446"><a name="p52608446"></a><a name="p52608446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p33425742"><a name="p33425742"></a><a name="p33425742"></a>密钥</p>
</td>
</tr>
<tr id="row155511111916"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p148381123152516"><a name="p148381123152516"></a><a name="p148381123152516"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10838223112516"><a name="p10838223112516"></a><a name="p10838223112516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p128381023202515"><a name="p128381023202515"></a><a name="p128381023202515"></a>APP的创建者，取值如下：</p>
<a name="ul1126756132511"></a><a name="ul1126756132511"></a><ul id="ul1126756132511"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="row32396224"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6848469"><a name="p6848469"></a><a name="p6848469"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17855131"><a name="p17855131"></a><a name="p17855131"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36979513"><a name="p36979513"></a><a name="p36979513"></a>注册时间</p>
</td>
</tr>
<tr id="row64380169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47411232"><a name="p47411232"></a><a name="p47411232"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15104546"><a name="p15104546"></a><a name="p15104546"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15508729"><a name="p15508729"></a><a name="p15508729"></a>描述</p>
</td>
</tr>
<tr id="row5360840"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p31574905"><a name="p31574905"></a><a name="p31574905"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7430514"><a name="p7430514"></a><a name="p7430514"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65000796"><a name="p65000796"></a><a name="p65000796"></a>更新时间</p>
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
	"update_time": "2017-12-28T12:28:07.2966182Z"
}
```

## 状态码<a name="section58064504"></a>

**表 5**  返回消息说明

<a name="table65661620"></a>
<table><thead align="left"><tr id="row38386508"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p22299447"><a name="p22299447"></a><a name="p22299447"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p61424758"><a name="p61424758"></a><a name="p61424758"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row9349490"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p19111186"><a name="p19111186"></a><a name="p19111186"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p4502206"><a name="p4502206"></a><a name="p4502206"></a>OK</p>
</td>
</tr>
<tr id="row40519861"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p60883295"><a name="p60883295"></a><a name="p60883295"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p32599882"><a name="p32599882"></a><a name="p32599882"></a>Bad Request</p>
</td>
</tr>
<tr id="row24963487"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p8776590"><a name="p8776590"></a><a name="p8776590"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p191535218816"><a name="p191535218816"></a><a name="p191535218816"></a>Unauthorized</p>
</td>
</tr>
<tr id="row22792350"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p34241051"><a name="p34241051"></a><a name="p34241051"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row64337830"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p43981707"><a name="p43981707"></a><a name="p43981707"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p5748492"><a name="p5748492"></a><a name="p5748492"></a>Not Found</p>
</td>
</tr>
<tr id="row51736435"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p29901739"><a name="p29901739"></a><a name="p29901739"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6121779"><a name="p6121779"></a><a name="p6121779"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

