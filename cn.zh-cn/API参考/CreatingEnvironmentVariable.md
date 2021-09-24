# 新建变量<a name="ZH-CN_TOPIC_0000001082135107"></a>

## 功能介绍<a name="zh-cn_topic_0118922250_section39792518"></a>

将API发布到不同的环境后，对于不同的环境，可能会有不同的环境变量，比如，API的服务部署地址，请求的版本号等。

用户可以定义不同的环境变量，用户在定义API时，在API的定义中使用这些变量，当调用API时，API网关会将这些变量替换成真实的变量值，以达到不同环境的区分效果。

环境变量定义在API分组上，该分组下的所有API都可以使用这些变量。

>![](public_sys-resources/icon-note.gif) **说明：** 
>1.  环境变量的变量名称必须保持唯一，即一个分组在同一个环境上不能有两个同名的变量
>2.  环境变量区分大小写，即变量ABC与变量abc是两个不同的变量
>3.  设置了环境变量后，使用到该变量的API的调试功能将不可使用。
>4.  定义了环境变量后，使用到环境变量的地方应该以对称的\#标识环境变量，当API发布到相应的环境后，会对环境变量的值进行替换，如：定义的API的URL为：[https://\#address\#:8080](https://#address#:8080)，环境变量address在RELEASE环境上的值为：192.168.1.5，则API发布到RELEASE环境后的真实的URL为：https://192.168.1.5:8080。

## URI<a name="zh-cn_topic_0118922250_section22588350"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922250_table57013820"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922250_row30962147"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922250_p24906010"><a name="zh-cn_topic_0118922250_p24906010"></a><a name="zh-cn_topic_0118922250_p24906010"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922250_p4120892"><a name="zh-cn_topic_0118922250_p4120892"></a><a name="zh-cn_topic_0118922250_p4120892"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922250_row65356851"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922250_p59413607"><a name="zh-cn_topic_0118922250_p59413607"></a><a name="zh-cn_topic_0118922250_p59413607"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922250_p47772863"><a name="zh-cn_topic_0118922250_p47772863"></a><a name="zh-cn_topic_0118922250_p47772863"></a>/v1.0/apigw/env-variables</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922250_section1968564"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118922250_table44396708"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922250_row44687699"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922250_p62933903"><a name="zh-cn_topic_0118922250_p62933903"></a><a name="zh-cn_topic_0118922250_p62933903"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922250_p64481350"><a name="zh-cn_topic_0118922250_p64481350"></a><a name="zh-cn_topic_0118922250_p64481350"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922250_p55606882"><a name="zh-cn_topic_0118922250_p55606882"></a><a name="zh-cn_topic_0118922250_p55606882"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.99999999999999%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922250_p7863627"><a name="zh-cn_topic_0118922250_p7863627"></a><a name="zh-cn_topic_0118922250_p7863627"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922250_row32974056"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922250_p53652898"><a name="zh-cn_topic_0118922250_p53652898"></a><a name="zh-cn_topic_0118922250_p53652898"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922250_p50917472"><a name="zh-cn_topic_0118922250_p50917472"></a><a name="zh-cn_topic_0118922250_p50917472"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922250_p30674571"><a name="zh-cn_topic_0118922250_p30674571"></a><a name="zh-cn_topic_0118922250_p30674571"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922250_p1612298"><a name="zh-cn_topic_0118922250_p1612298"></a><a name="zh-cn_topic_0118922250_p1612298"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row34514806"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922250_p44235863"><a name="zh-cn_topic_0118922250_p44235863"></a><a name="zh-cn_topic_0118922250_p44235863"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922250_p26335145"><a name="zh-cn_topic_0118922250_p26335145"></a><a name="zh-cn_topic_0118922250_p26335145"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922250_p52771987"><a name="zh-cn_topic_0118922250_p52771987"></a><a name="zh-cn_topic_0118922250_p52771987"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922250_p46672574"><a name="zh-cn_topic_0118922250_p46672574"></a><a name="zh-cn_topic_0118922250_p46672574"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row112866"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922250_p9142181"><a name="zh-cn_topic_0118922250_p9142181"></a><a name="zh-cn_topic_0118922250_p9142181"></a>variable_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922250_p2319205"><a name="zh-cn_topic_0118922250_p2319205"></a><a name="zh-cn_topic_0118922250_p2319205"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922250_p53637897"><a name="zh-cn_topic_0118922250_p53637897"></a><a name="zh-cn_topic_0118922250_p53637897"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922250_p49702394"><a name="zh-cn_topic_0118922250_p49702394"></a><a name="zh-cn_topic_0118922250_p49702394"></a>变量名</p>
<p id="zh-cn_topic_0118922250_p61367576"><a name="zh-cn_topic_0118922250_p61367576"></a><a name="zh-cn_topic_0118922250_p61367576"></a>支持英文字母、数字、英文格式的下划线、中划线，必须以英文字母开头，3 ~ 32个字符。在API定义中等于#Name的值#部分（区分大小写），发布到环境里的API被变量值替换。</p>
<div class="note" id="zh-cn_topic_0118922250_note721519264594"><a name="zh-cn_topic_0118922250_note721519264594"></a><a name="zh-cn_topic_0118922250_note721519264594"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118922250_p0215112605912"><a name="zh-cn_topic_0118922250_p0215112605912"></a><a name="zh-cn_topic_0118922250_p0215112605912"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row12471392"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922250_p3549860"><a name="zh-cn_topic_0118922250_p3549860"></a><a name="zh-cn_topic_0118922250_p3549860"></a>variable_value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922250_p19103244"><a name="zh-cn_topic_0118922250_p19103244"></a><a name="zh-cn_topic_0118922250_p19103244"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922250_p3858945"><a name="zh-cn_topic_0118922250_p3858945"></a><a name="zh-cn_topic_0118922250_p3858945"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.99999999999999%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922250_p44139114"><a name="zh-cn_topic_0118922250_p44139114"></a><a name="zh-cn_topic_0118922250_p44139114"></a>变量值</p>
<p id="zh-cn_topic_0118922250_p180919567297"><a name="zh-cn_topic_0118922250_p180919567297"></a><a name="zh-cn_topic_0118922250_p180919567297"></a>支持英文字母、数字、英文格式的下划线、中划线，斜线（/）、点、冒号，1 ~ 255个字符。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"env_id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
	"group_id": "73c58022-f20d-495a-a188-85d718647f09",
	"variable_name": "address",
	"variable_value": "192.168.1.5"
}
```

## 响应消息<a name="zh-cn_topic_0118922250_section25236006"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118922250_table44126582"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922250_row19577177"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922250_p42247518"><a name="zh-cn_topic_0118922250_p42247518"></a><a name="zh-cn_topic_0118922250_p42247518"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922250_p66605783"><a name="zh-cn_topic_0118922250_p66605783"></a><a name="zh-cn_topic_0118922250_p66605783"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922250_p26359341"><a name="zh-cn_topic_0118922250_p26359341"></a><a name="zh-cn_topic_0118922250_p26359341"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922250_row54731847"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922250_p4094605"><a name="zh-cn_topic_0118922250_p4094605"></a><a name="zh-cn_topic_0118922250_p4094605"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922250_p63227625"><a name="zh-cn_topic_0118922250_p63227625"></a><a name="zh-cn_topic_0118922250_p63227625"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922250_p21163968"><a name="zh-cn_topic_0118922250_p21163968"></a><a name="zh-cn_topic_0118922250_p21163968"></a>环境变量的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row56257990"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922250_p60603364"><a name="zh-cn_topic_0118922250_p60603364"></a><a name="zh-cn_topic_0118922250_p60603364"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922250_p9925426"><a name="zh-cn_topic_0118922250_p9925426"></a><a name="zh-cn_topic_0118922250_p9925426"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922250_p65762008"><a name="zh-cn_topic_0118922250_p65762008"></a><a name="zh-cn_topic_0118922250_p65762008"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row54987164"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922250_p24775290"><a name="zh-cn_topic_0118922250_p24775290"></a><a name="zh-cn_topic_0118922250_p24775290"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922250_p60641477"><a name="zh-cn_topic_0118922250_p60641477"></a><a name="zh-cn_topic_0118922250_p60641477"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922250_p13012580"><a name="zh-cn_topic_0118922250_p13012580"></a><a name="zh-cn_topic_0118922250_p13012580"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row50004359"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922250_p23821248"><a name="zh-cn_topic_0118922250_p23821248"></a><a name="zh-cn_topic_0118922250_p23821248"></a>variable_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922250_p50472897"><a name="zh-cn_topic_0118922250_p50472897"></a><a name="zh-cn_topic_0118922250_p50472897"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922250_p61772851"><a name="zh-cn_topic_0118922250_p61772851"></a><a name="zh-cn_topic_0118922250_p61772851"></a>变量名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row19084749"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922250_p2360875"><a name="zh-cn_topic_0118922250_p2360875"></a><a name="zh-cn_topic_0118922250_p2360875"></a>variable_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922250_p57013197"><a name="zh-cn_topic_0118922250_p57013197"></a><a name="zh-cn_topic_0118922250_p57013197"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922250_p54666268"><a name="zh-cn_topic_0118922250_p54666268"></a><a name="zh-cn_topic_0118922250_p54666268"></a>变量值</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "104185e5-3e8f-4c63-a7e5-ef4117bf870c",
	"env_id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
	"group_id": "73c58022-f20d-495a-a188-85d718647f09",
	"variable_name": "address",
	"variable_value": "192.168.1.5"
}
```

## 状态码<a name="zh-cn_topic_0118922250_section17717081"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118922250_table9599777"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922250_row55812053"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922250_p24482463"><a name="zh-cn_topic_0118922250_p24482463"></a><a name="zh-cn_topic_0118922250_p24482463"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922250_p36922477"><a name="zh-cn_topic_0118922250_p36922477"></a><a name="zh-cn_topic_0118922250_p36922477"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922250_row37930664"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922250_p52484919"><a name="zh-cn_topic_0118922250_p52484919"></a><a name="zh-cn_topic_0118922250_p52484919"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922250_p23420035"><a name="zh-cn_topic_0118922250_p23420035"></a><a name="zh-cn_topic_0118922250_p23420035"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row9453723"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922250_p27554060"><a name="zh-cn_topic_0118922250_p27554060"></a><a name="zh-cn_topic_0118922250_p27554060"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922250_p17286382"><a name="zh-cn_topic_0118922250_p17286382"></a><a name="zh-cn_topic_0118922250_p17286382"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row21359712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922250_p52415150"><a name="zh-cn_topic_0118922250_p52415150"></a><a name="zh-cn_topic_0118922250_p52415150"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922250_p17768768"><a name="zh-cn_topic_0118922250_p17768768"></a><a name="zh-cn_topic_0118922250_p17768768"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row25701191"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922250_p1421690"><a name="zh-cn_topic_0118922250_p1421690"></a><a name="zh-cn_topic_0118922250_p1421690"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922250_p48048103"><a name="zh-cn_topic_0118922250_p48048103"></a><a name="zh-cn_topic_0118922250_p48048103"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row29779746"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922250_p63349206"><a name="zh-cn_topic_0118922250_p63349206"></a><a name="zh-cn_topic_0118922250_p63349206"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922250_p31012055"><a name="zh-cn_topic_0118922250_p31012055"></a><a name="zh-cn_topic_0118922250_p31012055"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922250_row10673039"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922250_p59209837"><a name="zh-cn_topic_0118922250_p59209837"></a><a name="zh-cn_topic_0118922250_p59209837"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922250_p14947689"><a name="zh-cn_topic_0118922250_p14947689"></a><a name="zh-cn_topic_0118922250_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

