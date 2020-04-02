# 移除指定的ACL策略的值<a name="apig-phapi-180713088"></a>

## 功能介绍<a name="section2712129"></a>

从指定的ACL策略中删除一个或多个策略值。

## URI<a name="section24409161"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table16458109"></a>
<table><thead align="left"><tr id="row14566900"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p39068245"><a name="p39068245"></a><a name="p39068245"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p10411242"><a name="p10411242"></a><a name="p10411242"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row38004251"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p58445522"><a name="p58445522"></a><a name="p58445522"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p36466804"><a name="p36466804"></a><a name="p36466804"></a>/v1/{project_id}/apigw/instances/{instance_id}/acls/aclvalue/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table1021163"></a>
<table><thead align="left"><tr id="row39955125"><th class="cellrowborder" valign="top" width="23.169999999999998%" id="mcps1.2.5.1.1"><p id="p15139691"><a name="p15139691"></a><a name="p15139691"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="23.150000000000002%" id="mcps1.2.5.1.2"><p id="p18355429"><a name="p18355429"></a><a name="p18355429"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.470000000000002%" id="mcps1.2.5.1.3"><p id="p10394763"><a name="p10394763"></a><a name="p10394763"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.21%" id="mcps1.2.5.1.4"><p id="p36669511"><a name="p36669511"></a><a name="p36669511"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row130317081910"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.150000000000002%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.21%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row1877615913189"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="23.150000000000002%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.21%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row17440382"><td class="cellrowborder" valign="top" width="23.169999999999998%" headers="mcps1.2.5.1.1 "><p id="p3384858"><a name="p3384858"></a><a name="p3384858"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="23.150000000000002%" headers="mcps1.2.5.1.2 "><p id="p5738115"><a name="p5738115"></a><a name="p5738115"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.470000000000002%" headers="mcps1.2.5.1.3 "><p id="p62134176"><a name="p62134176"></a><a name="p62134176"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.21%" headers="mcps1.2.5.1.4 "><p id="p66812378"><a name="p66812378"></a><a name="p66812378"></a>ACL策略的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section18355857"></a>

输入要删除的黑白名单的值，支持同时多个值的输入，以英文半角逗号分隔。

```
{
	"acl_value": "a987945sdfg-adfa8788-dfa-adfadd423"
}
```

## 响应消息<a name="section10429421"></a>

**表 3**  参数说明

<a name="table20100575"></a>
<table><thead align="left"><tr id="row3029282"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p44045288"><a name="p44045288"></a><a name="p44045288"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p10898546"><a name="p10898546"></a><a name="p10898546"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p10367016"><a name="p10367016"></a><a name="p10367016"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34422004"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p36718907"><a name="p36718907"></a><a name="p36718907"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p21441511"><a name="p21441511"></a><a name="p21441511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p59040864"><a name="p59040864"></a><a name="p59040864"></a>编号</p>
</td>
</tr>
<tr id="row61605733"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24008443"><a name="p24008443"></a><a name="p24008443"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p65635730"><a name="p65635730"></a><a name="p65635730"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14893905"><a name="p14893905"></a><a name="p14893905"></a>名称</p>
</td>
</tr>
<tr id="row66936288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53130223"><a name="p53130223"></a><a name="p53130223"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8580795"><a name="p8580795"></a><a name="p8580795"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p23955755"><a name="p23955755"></a><a name="p23955755"></a>类型</p>
<a name="ul14275204"></a><a name="ul14275204"></a><ul id="ul14275204"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="row4750104"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p49214182"><a name="p49214182"></a><a name="p49214182"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p26925816"><a name="p26925816"></a><a name="p26925816"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p33507511"><a name="p33507511"></a><a name="p33507511"></a>ACL策略的值</p>
</td>
</tr>
<tr id="row33132146"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p66458207"><a name="p66458207"></a><a name="p66458207"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14405676"><a name="p14405676"></a><a name="p14405676"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p26009089"><a name="p26009089"></a><a name="p26009089"></a>对象类型：</p>
<a name="ul32755215"></a><a name="ul32755215"></a><ul id="ul32755215"><li>IP</li><li>DOMAIN</li><li>ADMIN</li></ul>
</td>
</tr>
<tr id="row54905061"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18124996"><a name="p18124996"></a><a name="p18124996"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p58838604"><a name="p58838604"></a><a name="p58838604"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1197604"><a name="p1197604"></a><a name="p1197604"></a>更新时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "d402b35e-1054-4280-b1c5-0d741a28c995",
	"acl_name": "goodone",
	"entity_type": "DOMAIN",
	"acl_type": "PERMIT",
	"acl_value": "19asdfaf-adfadf",
	"update_time": "2017-11-18T14:27:36.918578+08:00"
}
```

## 状态码<a name="section30984986"></a>

**表 4**  返回消息说明

<a name="table62970069"></a>
<table><thead align="left"><tr id="row18783306"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p45052843"><a name="p45052843"></a><a name="p45052843"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p25401705"><a name="p25401705"></a><a name="p25401705"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row44272235"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p29281306"><a name="p29281306"></a><a name="p29281306"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row5453642"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p39091847"><a name="p39091847"></a><a name="p39091847"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row43798322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p58003159"><a name="p58003159"></a><a name="p58003159"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p635416"><a name="p635416"></a><a name="p635416"></a>Not Found</p>
</td>
</tr>
<tr id="row5718751"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p60565719"><a name="p60565719"></a><a name="p60565719"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

