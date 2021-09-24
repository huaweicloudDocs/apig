# 创建ACL策略<a name="ZH-CN_TOPIC_0000001081837295"></a>

## 功能介绍<a name="zh-cn_topic_0118924496_section54754916"></a>

增加一个ACL策略，策略类型通过字段acl\_type来确定（permit或者deny），限制的对象的类型可以为IP或者DOMAIN，这里的DOMAIN对应的acl\_value的值为您的租户名称， 而非“www.exampleDomain.com"之类的网络域名。

## URI<a name="zh-cn_topic_0118924496_section23032199"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924496_table45962929"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924496_row32355322"><th class="cellrowborder" valign="top" width="34%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924496_p3535427"><a name="zh-cn_topic_0118924496_p3535427"></a><a name="zh-cn_topic_0118924496_p3535427"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924496_p17934205"><a name="zh-cn_topic_0118924496_p17934205"></a><a name="zh-cn_topic_0118924496_p17934205"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924496_row43384528"><td class="cellrowborder" valign="top" width="34%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924496_p24485859"><a name="zh-cn_topic_0118924496_p24485859"></a><a name="zh-cn_topic_0118924496_p24485859"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924496_p37197534"><a name="zh-cn_topic_0118924496_p37197534"></a><a name="zh-cn_topic_0118924496_p37197534"></a>/v1.0/apigw/acls</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924496_section5963201"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118924496_table60210282"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924496_row49033866"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924496_p12320215"><a name="zh-cn_topic_0118924496_p12320215"></a><a name="zh-cn_topic_0118924496_p12320215"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924496_p58413377"><a name="zh-cn_topic_0118924496_p58413377"></a><a name="zh-cn_topic_0118924496_p58413377"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924496_p33863087"><a name="zh-cn_topic_0118924496_p33863087"></a><a name="zh-cn_topic_0118924496_p33863087"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924496_row58555530"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p45377465"><a name="zh-cn_topic_0118924496_p45377465"></a><a name="zh-cn_topic_0118924496_p45377465"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p51696037"><a name="zh-cn_topic_0118924496_p51696037"></a><a name="zh-cn_topic_0118924496_p51696037"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p64172706"><a name="zh-cn_topic_0118924496_p64172706"></a><a name="zh-cn_topic_0118924496_p64172706"></a>ACL策略名称。</p>
<p id="zh-cn_topic_0118924496_p7024991"><a name="zh-cn_topic_0118924496_p7024991"></a><a name="zh-cn_topic_0118924496_p7024991"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0118924496_note1155910113419"><a name="zh-cn_topic_0118924496_note1155910113419"></a><a name="zh-cn_topic_0118924496_note1155910113419"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118924496_p1559011141"><a name="zh-cn_topic_0118924496_p1559011141"></a><a name="zh-cn_topic_0118924496_p1559011141"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row38338270"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p18392160"><a name="zh-cn_topic_0118924496_p18392160"></a><a name="zh-cn_topic_0118924496_p18392160"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p13369978"><a name="zh-cn_topic_0118924496_p13369978"></a><a name="zh-cn_topic_0118924496_p13369978"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p9226453"><a name="zh-cn_topic_0118924496_p9226453"></a><a name="zh-cn_topic_0118924496_p9226453"></a>类型</p>
<a name="zh-cn_topic_0118924496_ul15929218"></a><a name="zh-cn_topic_0118924496_ul15929218"></a><ul id="zh-cn_topic_0118924496_ul15929218"><li>PERMIT  (白名单类型)</li><li>DENY     (黑名单类型)</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row2567020"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p6602105"><a name="zh-cn_topic_0118924496_p6602105"></a><a name="zh-cn_topic_0118924496_p6602105"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p65008486"><a name="zh-cn_topic_0118924496_p65008486"></a><a name="zh-cn_topic_0118924496_p65008486"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p31195995"><a name="zh-cn_topic_0118924496_p31195995"></a><a name="zh-cn_topic_0118924496_p31195995"></a>ACL策略值，支持一个或多个值，使用英文半角逗号分隔</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row12328505"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p59084814"><a name="zh-cn_topic_0118924496_p59084814"></a><a name="zh-cn_topic_0118924496_p59084814"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p21140607"><a name="zh-cn_topic_0118924496_p21140607"></a><a name="zh-cn_topic_0118924496_p21140607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p34667638"><a name="zh-cn_topic_0118924496_p34667638"></a><a name="zh-cn_topic_0118924496_p34667638"></a>对象类型：</p>
<a name="zh-cn_topic_0118924496_ul43573286"></a><a name="zh-cn_topic_0118924496_ul43573286"></a><ul id="zh-cn_topic_0118924496_ul43573286"><li>IP</li><li>DOMAIN</li></ul>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
        "acl_name": "test001",
	"acl_type": "PERMIT",
        "acl_value": "192.168.1.5,192.168.10.0/24,192.168.12.12-192.168.12.19",
        "entity_type": "IP"
}
```

## 响应消息<a name="zh-cn_topic_0118924496_section13257254"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924496_table52850162"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924496_row50824653"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924496_p23156239"><a name="zh-cn_topic_0118924496_p23156239"></a><a name="zh-cn_topic_0118924496_p23156239"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924496_p63716094"><a name="zh-cn_topic_0118924496_p63716094"></a><a name="zh-cn_topic_0118924496_p63716094"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924496_p60729985"><a name="zh-cn_topic_0118924496_p60729985"></a><a name="zh-cn_topic_0118924496_p60729985"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924496_row20181761"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p24109925"><a name="zh-cn_topic_0118924496_p24109925"></a><a name="zh-cn_topic_0118924496_p24109925"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p6746902"><a name="zh-cn_topic_0118924496_p6746902"></a><a name="zh-cn_topic_0118924496_p6746902"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p9628155"><a name="zh-cn_topic_0118924496_p9628155"></a><a name="zh-cn_topic_0118924496_p9628155"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row19544532"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p39603299"><a name="zh-cn_topic_0118924496_p39603299"></a><a name="zh-cn_topic_0118924496_p39603299"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p53750683"><a name="zh-cn_topic_0118924496_p53750683"></a><a name="zh-cn_topic_0118924496_p53750683"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p58838051"><a name="zh-cn_topic_0118924496_p58838051"></a><a name="zh-cn_topic_0118924496_p58838051"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row59780412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p10375232"><a name="zh-cn_topic_0118924496_p10375232"></a><a name="zh-cn_topic_0118924496_p10375232"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p35087464"><a name="zh-cn_topic_0118924496_p35087464"></a><a name="zh-cn_topic_0118924496_p35087464"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p23512349"><a name="zh-cn_topic_0118924496_p23512349"></a><a name="zh-cn_topic_0118924496_p23512349"></a>类型</p>
<a name="zh-cn_topic_0118924496_ul10284551"></a><a name="zh-cn_topic_0118924496_ul10284551"></a><ul id="zh-cn_topic_0118924496_ul10284551"><li>PERMIT（白名单类型）</li><li>DENY（黑名单类型）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row48354380"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p24390678"><a name="zh-cn_topic_0118924496_p24390678"></a><a name="zh-cn_topic_0118924496_p24390678"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p29487884"><a name="zh-cn_topic_0118924496_p29487884"></a><a name="zh-cn_topic_0118924496_p29487884"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p39708440"><a name="zh-cn_topic_0118924496_p39708440"></a><a name="zh-cn_topic_0118924496_p39708440"></a>ACL策略值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row21831640"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p23532445"><a name="zh-cn_topic_0118924496_p23532445"></a><a name="zh-cn_topic_0118924496_p23532445"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p27079915"><a name="zh-cn_topic_0118924496_p27079915"></a><a name="zh-cn_topic_0118924496_p27079915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p45989481"><a name="zh-cn_topic_0118924496_p45989481"></a><a name="zh-cn_topic_0118924496_p45989481"></a>对象类型：</p>
<a name="zh-cn_topic_0118924496_ul11252145"></a><a name="zh-cn_topic_0118924496_ul11252145"></a><ul id="zh-cn_topic_0118924496_ul11252145"><li>IP</li><li>DOMAIN</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row15532822"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924496_p50199061"><a name="zh-cn_topic_0118924496_p50199061"></a><a name="zh-cn_topic_0118924496_p50199061"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924496_p39592165"><a name="zh-cn_topic_0118924496_p39592165"></a><a name="zh-cn_topic_0118924496_p39592165"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924496_p52848814"><a name="zh-cn_topic_0118924496_p52848814"></a><a name="zh-cn_topic_0118924496_p52848814"></a>更新时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "d402b35e-1054-4280-b1c5-0d741a28c995",
        "acl_name": "test",
        "entity_type": "IP",
	"acl_type": "PERMIT",
        "acl_value": "192.168.1.5,192.168.10.0/24,192.168.12.12-192.168.12.19",
	"update_time": "2017-11-18T14:27:36.918578+08:00"
}
```

## 状态码<a name="zh-cn_topic_0118924496_section53668811"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118924496_table37529561"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924496_row14168275"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924496_p6779631"><a name="zh-cn_topic_0118924496_p6779631"></a><a name="zh-cn_topic_0118924496_p6779631"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924496_p12279235"><a name="zh-cn_topic_0118924496_p12279235"></a><a name="zh-cn_topic_0118924496_p12279235"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924496_row55094008"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924496_p33429686"><a name="zh-cn_topic_0118924496_p33429686"></a><a name="zh-cn_topic_0118924496_p33429686"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924496_p73578115452"><a name="zh-cn_topic_0118924496_p73578115452"></a><a name="zh-cn_topic_0118924496_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row9723588"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924496_p49413182"><a name="zh-cn_topic_0118924496_p49413182"></a><a name="zh-cn_topic_0118924496_p49413182"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924496_p43044796"><a name="zh-cn_topic_0118924496_p43044796"></a><a name="zh-cn_topic_0118924496_p43044796"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924496_row51858848"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924496_p39817184"><a name="zh-cn_topic_0118924496_p39817184"></a><a name="zh-cn_topic_0118924496_p39817184"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924496_p6744143"><a name="zh-cn_topic_0118924496_p6744143"></a><a name="zh-cn_topic_0118924496_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

