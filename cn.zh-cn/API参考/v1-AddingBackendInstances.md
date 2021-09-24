# 添加后端实例（云服务器）<a name="ZH-CN_TOPIC_0000001081976225"></a>

## 功能介绍<a name="zh-cn_topic_0225568982_section173482301428"></a>

为指定的VPC通道添加云服务器。

## URI<a name="zh-cn_topic_0225568982_section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568982_table1439319294431"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568982_row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568982_p14361448204314"><a name="zh-cn_topic_0225568982_p14361448204314"></a><a name="zh-cn_topic_0225568982_p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568982_p1936174864316"><a name="zh-cn_topic_0225568982_p1936174864316"></a><a name="zh-cn_topic_0225568982_p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568982_row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568982_p1236111482435"><a name="zh-cn_topic_0225568982_p1236111482435"></a><a name="zh-cn_topic_0225568982_p1236111482435"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568982_p11361848184318"><a name="zh-cn_topic_0225568982_p11361848184318"></a><a name="zh-cn_topic_0225568982_p11361848184318"></a>/v1/{project_id}/apigw/instances/{instance_id}/vpc-channels/{id}/members</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568982_table18784710"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568982_row37287554"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568982_p393051"><a name="zh-cn_topic_0225568982_p393051"></a><a name="zh-cn_topic_0225568982_p393051"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568982_p31837140"><a name="zh-cn_topic_0225568982_p31837140"></a><a name="zh-cn_topic_0225568982_p31837140"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568982_p28671509"><a name="zh-cn_topic_0225568982_p28671509"></a><a name="zh-cn_topic_0225568982_p28671509"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568982_p40690887"><a name="zh-cn_topic_0225568982_p40690887"></a><a name="zh-cn_topic_0225568982_p40690887"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568982_row87513398593"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568982_p55878963"><a name="zh-cn_topic_0225568982_p55878963"></a><a name="zh-cn_topic_0225568982_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568982_p29902160"><a name="zh-cn_topic_0225568982_p29902160"></a><a name="zh-cn_topic_0225568982_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568982_p6155914"><a name="zh-cn_topic_0225568982_p6155914"></a><a name="zh-cn_topic_0225568982_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568982_p28867016"><a name="zh-cn_topic_0225568982_p28867016"></a><a name="zh-cn_topic_0225568982_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row55281338195919"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568982_p1780913159538"><a name="zh-cn_topic_0225568982_p1780913159538"></a><a name="zh-cn_topic_0225568982_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568982_p9809215115310"><a name="zh-cn_topic_0225568982_p9809215115310"></a><a name="zh-cn_topic_0225568982_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568982_p1280914152538"><a name="zh-cn_topic_0225568982_p1280914152538"></a><a name="zh-cn_topic_0225568982_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568982_p1880914157537"><a name="zh-cn_topic_0225568982_p1880914157537"></a><a name="zh-cn_topic_0225568982_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row7627537"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568982_p13850780"><a name="zh-cn_topic_0225568982_p13850780"></a><a name="zh-cn_topic_0225568982_p13850780"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568982_p48171408"><a name="zh-cn_topic_0225568982_p48171408"></a><a name="zh-cn_topic_0225568982_p48171408"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568982_p9569939"><a name="zh-cn_topic_0225568982_p9569939"></a><a name="zh-cn_topic_0225568982_p9569939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568982_p36967632"><a name="zh-cn_topic_0225568982_p36967632"></a><a name="zh-cn_topic_0225568982_p36967632"></a>VPC通道的编号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568982_section73637302425"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568982_table1136319301429"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568982_row748813306425"><th class="cellrowborder" valign="top" width="15.46154615461546%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568982_p9488143084210"><a name="zh-cn_topic_0225568982_p9488143084210"></a><a name="zh-cn_topic_0225568982_p9488143084210"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568982_p148843017426"><a name="zh-cn_topic_0225568982_p148843017426"></a><a name="zh-cn_topic_0225568982_p148843017426"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568982_p9488830164214"><a name="zh-cn_topic_0225568982_p9488830164214"></a><a name="zh-cn_topic_0225568982_p9488830164214"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568982_p1048813014421"><a name="zh-cn_topic_0225568982_p1048813014421"></a><a name="zh-cn_topic_0225568982_p1048813014421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568982_row1949584023816"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568982_p54951240193817"><a name="zh-cn_topic_0225568982_p54951240193817"></a><a name="zh-cn_topic_0225568982_p54951240193817"></a>vpc_instances</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568982_p249574012387"><a name="zh-cn_topic_0225568982_p249574012387"></a><a name="zh-cn_topic_0225568982_p249574012387"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568982_p7495134011385"><a name="zh-cn_topic_0225568982_p7495134011385"></a><a name="zh-cn_topic_0225568982_p7495134011385"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568982_p14959403387"><a name="zh-cn_topic_0225568982_p14959403387"></a><a name="zh-cn_topic_0225568982_p14959403387"></a>后端实例列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  后端实例详情

<a name="zh-cn_topic_0225568982_table6144132024717"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568982_row15144122054719"><th class="cellrowborder" valign="top" width="15.46154615461546%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568982_p41441620124712"><a name="zh-cn_topic_0225568982_p41441620124712"></a><a name="zh-cn_topic_0225568982_p41441620124712"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568982_p14144820104719"><a name="zh-cn_topic_0225568982_p14144820104719"></a><a name="zh-cn_topic_0225568982_p14144820104719"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568982_p71601720114710"><a name="zh-cn_topic_0225568982_p71601720114710"></a><a name="zh-cn_topic_0225568982_p71601720114710"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568982_p1716072074719"><a name="zh-cn_topic_0225568982_p1716072074719"></a><a name="zh-cn_topic_0225568982_p1716072074719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568982_row816019209472"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568982_p11160192010473"><a name="zh-cn_topic_0225568982_p11160192010473"></a><a name="zh-cn_topic_0225568982_p11160192010473"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568982_p916052018474"><a name="zh-cn_topic_0225568982_p916052018474"></a><a name="zh-cn_topic_0225568982_p916052018474"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568982_p1916032024714"><a name="zh-cn_topic_0225568982_p1916032024714"></a><a name="zh-cn_topic_0225568982_p1916032024714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568982_p141601720174711"><a name="zh-cn_topic_0225568982_p141601720174711"></a><a name="zh-cn_topic_0225568982_p141601720174711"></a>云服务器的名称。</p>
<p id="zh-cn_topic_0225568982_p7024991"><a name="zh-cn_topic_0225568982_p7024991"></a><a name="zh-cn_topic_0225568982_p7024991"></a>支持汉字，英文，数字，“-”,“_”,“.”，1~ 64字符。</p>
<div class="note" id="zh-cn_topic_0225568982_note1155910113419"><a name="zh-cn_topic_0225568982_note1155910113419"></a><a name="zh-cn_topic_0225568982_note1155910113419"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568982_p1559011141"><a name="zh-cn_topic_0225568982_p1559011141"></a><a name="zh-cn_topic_0225568982_p1559011141"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row171743206475"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568982_p31740206478"><a name="zh-cn_topic_0225568982_p31740206478"></a><a name="zh-cn_topic_0225568982_p31740206478"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568982_p1174162084716"><a name="zh-cn_topic_0225568982_p1174162084716"></a><a name="zh-cn_topic_0225568982_p1174162084716"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568982_p1217432012470"><a name="zh-cn_topic_0225568982_p1217432012470"></a><a name="zh-cn_topic_0225568982_p1217432012470"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568982_p1825072175810"><a name="zh-cn_topic_0225568982_p1825072175810"></a><a name="zh-cn_topic_0225568982_p1825072175810"></a>云服务器的ID。</p>
<p id="zh-cn_topic_0225568982_p5927204705518"><a name="zh-cn_topic_0225568982_p5927204705518"></a><a name="zh-cn_topic_0225568982_p5927204705518"></a>支持英文，数字，“-”,“_”，1 ~ 64字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row4191162015475"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568982_p17191112094711"><a name="zh-cn_topic_0225568982_p17191112094711"></a><a name="zh-cn_topic_0225568982_p17191112094711"></a>weight</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568982_p131911920174712"><a name="zh-cn_topic_0225568982_p131911920174712"></a><a name="zh-cn_topic_0225568982_p131911920174712"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568982_p161911220194720"><a name="zh-cn_topic_0225568982_p161911220194720"></a><a name="zh-cn_topic_0225568982_p161911220194720"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568982_p1133512255618"><a name="zh-cn_topic_0225568982_p1133512255618"></a><a name="zh-cn_topic_0225568982_p1133512255618"></a>权重值。</p>
<p id="zh-cn_topic_0225568982_p4191102016478"><a name="zh-cn_topic_0225568982_p4191102016478"></a><a name="zh-cn_topic_0225568982_p4191102016478"></a>权重值越大，转发到该云服务器的请求数量越多。</p>
<p id="zh-cn_topic_0225568982_p8324165017186"><a name="zh-cn_topic_0225568982_p8324165017186"></a><a name="zh-cn_topic_0225568982_p8324165017186"></a>取值范围1 ~ 100。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "vpc_instances": [
    {
      "instance_id": "instance02",
      "instance_name": "instance_name02",
      "weight": 10
    }
  ]
}
```

## 响应消息<a name="zh-cn_topic_0225568982_section9395153012420"></a>

**表 5**  参数说明

<a name="zh-cn_topic_0225568982_table880710441918"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568982_row3807204111917"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568982_p11807545190"><a name="zh-cn_topic_0225568982_p11807545190"></a><a name="zh-cn_topic_0225568982_p11807545190"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568982_p980710417191"><a name="zh-cn_topic_0225568982_p980710417191"></a><a name="zh-cn_topic_0225568982_p980710417191"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568982_p18823344198"><a name="zh-cn_topic_0225568982_p18823344198"></a><a name="zh-cn_topic_0225568982_p18823344198"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568982_row041814181474"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p18418171824720"><a name="zh-cn_topic_0225568982_p18418171824720"></a><a name="zh-cn_topic_0225568982_p18418171824720"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p524622216472"><a name="zh-cn_topic_0225568982_p524622216472"></a><a name="zh-cn_topic_0225568982_p524622216472"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p11418121812476"><a name="zh-cn_topic_0225568982_p11418121812476"></a><a name="zh-cn_topic_0225568982_p11418121812476"></a>该VPC通道下的云服务器总数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row4933121514713"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p1693371574715"><a name="zh-cn_topic_0225568982_p1693371574715"></a><a name="zh-cn_topic_0225568982_p1693371574715"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p093312156470"><a name="zh-cn_topic_0225568982_p093312156470"></a><a name="zh-cn_topic_0225568982_p093312156470"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p1393341534713"><a name="zh-cn_topic_0225568982_p1393341534713"></a><a name="zh-cn_topic_0225568982_p1393341534713"></a>本次返回的云服务器总数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row8823245195"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p14823134111917"><a name="zh-cn_topic_0225568982_p14823134111917"></a><a name="zh-cn_topic_0225568982_p14823134111917"></a>vpc_instances</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p19823640198"><a name="zh-cn_topic_0225568982_p19823640198"></a><a name="zh-cn_topic_0225568982_p19823640198"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p78395411917"><a name="zh-cn_topic_0225568982_p78395411917"></a><a name="zh-cn_topic_0225568982_p78395411917"></a>云服务器列表。</p>
</td>
</tr>
</tbody>
</table>

**表 6**  后端实例详情

<a name="zh-cn_topic_0225568982_table2346632182717"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568982_row13464323270"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568982_p93464324278"><a name="zh-cn_topic_0225568982_p93464324278"></a><a name="zh-cn_topic_0225568982_p93464324278"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568982_p4346193213278"><a name="zh-cn_topic_0225568982_p4346193213278"></a><a name="zh-cn_topic_0225568982_p4346193213278"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568982_p53611732172712"><a name="zh-cn_topic_0225568982_p53611732172712"></a><a name="zh-cn_topic_0225568982_p53611732172712"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568982_row8361932112712"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p63611832132717"><a name="zh-cn_topic_0225568982_p63611832132717"></a><a name="zh-cn_topic_0225568982_p63611832132717"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p173611832112714"><a name="zh-cn_topic_0225568982_p173611832112714"></a><a name="zh-cn_topic_0225568982_p173611832112714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p163616323277"><a name="zh-cn_topic_0225568982_p163616323277"></a><a name="zh-cn_topic_0225568982_p163616323277"></a>后端实例对象的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row193611732112718"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p6361133242711"><a name="zh-cn_topic_0225568982_p6361133242711"></a><a name="zh-cn_topic_0225568982_p6361133242711"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p13377532192716"><a name="zh-cn_topic_0225568982_p13377532192716"></a><a name="zh-cn_topic_0225568982_p13377532192716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p4377103242715"><a name="zh-cn_topic_0225568982_p4377103242715"></a><a name="zh-cn_topic_0225568982_p4377103242715"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row1537715321276"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p1637783215276"><a name="zh-cn_topic_0225568982_p1637783215276"></a><a name="zh-cn_topic_0225568982_p1637783215276"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p037713328279"><a name="zh-cn_topic_0225568982_p037713328279"></a><a name="zh-cn_topic_0225568982_p037713328279"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p1620615311293"><a name="zh-cn_topic_0225568982_p1620615311293"></a><a name="zh-cn_topic_0225568982_p1620615311293"></a>后端实例对象的状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row11392163220272"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p6462652102914"><a name="zh-cn_topic_0225568982_p6462652102914"></a><a name="zh-cn_topic_0225568982_p6462652102914"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p15392113202710"><a name="zh-cn_topic_0225568982_p15392113202710"></a><a name="zh-cn_topic_0225568982_p15392113202710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p7643513300"><a name="zh-cn_topic_0225568982_p7643513300"></a><a name="zh-cn_topic_0225568982_p7643513300"></a>云服务器的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row1339216325273"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p12462195214295"><a name="zh-cn_topic_0225568982_p12462195214295"></a><a name="zh-cn_topic_0225568982_p12462195214295"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p103921532112711"><a name="zh-cn_topic_0225568982_p103921532112711"></a><a name="zh-cn_topic_0225568982_p103921532112711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p13641554304"><a name="zh-cn_topic_0225568982_p13641554304"></a><a name="zh-cn_topic_0225568982_p13641554304"></a>云服务器的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row2988816867"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p11276133405917"><a name="zh-cn_topic_0225568982_p11276133405917"></a><a name="zh-cn_topic_0225568982_p11276133405917"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p127653405913"><a name="zh-cn_topic_0225568982_p127653405913"></a><a name="zh-cn_topic_0225568982_p127653405913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p1027614347599"><a name="zh-cn_topic_0225568982_p1027614347599"></a><a name="zh-cn_topic_0225568982_p1027614347599"></a>云服务器的主机地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row1940916329273"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p10462165210296"><a name="zh-cn_topic_0225568982_p10462165210296"></a><a name="zh-cn_topic_0225568982_p10462165210296"></a>weight</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p5409163242719"><a name="zh-cn_topic_0225568982_p5409163242719"></a><a name="zh-cn_topic_0225568982_p5409163242719"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p3800183114208"><a name="zh-cn_topic_0225568982_p3800183114208"></a><a name="zh-cn_topic_0225568982_p3800183114208"></a>权重值。</p>
<p id="zh-cn_topic_0225568982_p1180133118202"><a name="zh-cn_topic_0225568982_p1180133118202"></a><a name="zh-cn_topic_0225568982_p1180133118202"></a>权重值越大，转发到该云服务器的请求数量越多。</p>
<p id="zh-cn_topic_0225568982_p13802231132017"><a name="zh-cn_topic_0225568982_p13802231132017"></a><a name="zh-cn_topic_0225568982_p13802231132017"></a>取值范围1 ~ 100。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row043993222711"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568982_p143917320276"><a name="zh-cn_topic_0225568982_p143917320276"></a><a name="zh-cn_topic_0225568982_p143917320276"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568982_p1043963216271"><a name="zh-cn_topic_0225568982_p1043963216271"></a><a name="zh-cn_topic_0225568982_p1043963216271"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568982_p124391632192720"><a name="zh-cn_topic_0225568982_p124391632192720"></a><a name="zh-cn_topic_0225568982_p124391632192720"></a>云服务器增加到VPC通道的时间。</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 2,
  "size": 2,
  "vpc_instances": [
    {
      "instance_id": "instance02",
      "instance_name": "instance_name02",
      "host": "127.0.0.2",
      "weight": 10,
      "id": "680e42fab429447ca23b9623107523d9",
      "vpc_id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
      "status": 1,
      "create_time": "2018-07-27T12:42:32Z"
    },
    {
      "instance_id": "instance01",
      "instance_name": "instance_name01",
      "host": "127.0.0.1",
      "weight": 10,
      "id": "c3bc73605a8b400793363c87574fbad7",
      "vpc_id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
      "status": 1,
      "create_time": "2018-07-27T12:30:48Z"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0225568982_section338043011426"></a>

**表 7**  返回消息说明

<a name="zh-cn_topic_0225568982_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568982_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568982_p174881730194216"><a name="zh-cn_topic_0225568982_p174881730194216"></a><a name="zh-cn_topic_0225568982_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568982_p848863018429"><a name="zh-cn_topic_0225568982_p848863018429"></a><a name="zh-cn_topic_0225568982_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568982_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568982_p7488163084211"><a name="zh-cn_topic_0225568982_p7488163084211"></a><a name="zh-cn_topic_0225568982_p7488163084211"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568982_p948803015424"><a name="zh-cn_topic_0225568982_p948803015424"></a><a name="zh-cn_topic_0225568982_p948803015424"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568982_p14488113015426"><a name="zh-cn_topic_0225568982_p14488113015426"></a><a name="zh-cn_topic_0225568982_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568982_p164881130154211"><a name="zh-cn_topic_0225568982_p164881130154211"></a><a name="zh-cn_topic_0225568982_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568982_p24883304428"><a name="zh-cn_topic_0225568982_p24883304428"></a><a name="zh-cn_topic_0225568982_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568982_p1848810308429"><a name="zh-cn_topic_0225568982_p1848810308429"></a><a name="zh-cn_topic_0225568982_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568982_p6488133064210"><a name="zh-cn_topic_0225568982_p6488133064210"></a><a name="zh-cn_topic_0225568982_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568982_p10488193018426"><a name="zh-cn_topic_0225568982_p10488193018426"></a><a name="zh-cn_topic_0225568982_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568982_p144883304428"><a name="zh-cn_topic_0225568982_p144883304428"></a><a name="zh-cn_topic_0225568982_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568982_p4488103094212"><a name="zh-cn_topic_0225568982_p4488103094212"></a><a name="zh-cn_topic_0225568982_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568982_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568982_p17488163014423"><a name="zh-cn_topic_0225568982_p17488163014423"></a><a name="zh-cn_topic_0225568982_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568982_p048813014216"><a name="zh-cn_topic_0225568982_p048813014216"></a><a name="zh-cn_topic_0225568982_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

