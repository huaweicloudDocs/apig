# 绑定签名密钥<a name="ZH-CN_TOPIC_0000001082135213"></a>

## 功能介绍<a name="zh-cn_topic_0225568943_section12427613"></a>

签名密钥创建后，需要绑定到API才能生效。将签名密钥绑定到API后，则API网关请求后端服务时就会使用这个签名密钥进行加密签名，后端服务可以校验这个签名来验证请求来源。

将指定的签名密钥绑定到一个或多个已发布的API上。

同一个API发布到不同的环境可以绑定不同的签名密钥；一个API在发布到特定环境后只能绑定一个签名密钥。

## URI<a name="zh-cn_topic_0225568943_section44739658"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法

<a name="zh-cn_topic_0225568943_table19534294"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568943_row53547179"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568943_p42354227"><a name="zh-cn_topic_0225568943_p42354227"></a><a name="zh-cn_topic_0225568943_p42354227"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568943_p8140339"><a name="zh-cn_topic_0225568943_p8140339"></a><a name="zh-cn_topic_0225568943_p8140339"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568943_row55387732"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568943_p57221309"><a name="zh-cn_topic_0225568943_p57221309"></a><a name="zh-cn_topic_0225568943_p57221309"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568943_p4414487"><a name="zh-cn_topic_0225568943_p4414487"></a><a name="zh-cn_topic_0225568943_p4414487"></a>/v1/{project_id}/apigw/instances/{instance_id}/sign-bindings</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568943_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568943_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568943_p23103637"><a name="zh-cn_topic_0225568943_p23103637"></a><a name="zh-cn_topic_0225568943_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568943_p59455291"><a name="zh-cn_topic_0225568943_p59455291"></a><a name="zh-cn_topic_0225568943_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568943_p51149303"><a name="zh-cn_topic_0225568943_p51149303"></a><a name="zh-cn_topic_0225568943_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568943_p49452846"><a name="zh-cn_topic_0225568943_p49452846"></a><a name="zh-cn_topic_0225568943_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568943_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568943_p55878963"><a name="zh-cn_topic_0225568943_p55878963"></a><a name="zh-cn_topic_0225568943_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568943_p29902160"><a name="zh-cn_topic_0225568943_p29902160"></a><a name="zh-cn_topic_0225568943_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568943_p6155914"><a name="zh-cn_topic_0225568943_p6155914"></a><a name="zh-cn_topic_0225568943_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568943_p28867016"><a name="zh-cn_topic_0225568943_p28867016"></a><a name="zh-cn_topic_0225568943_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568943_p1780913159538"><a name="zh-cn_topic_0225568943_p1780913159538"></a><a name="zh-cn_topic_0225568943_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568943_p9809215115310"><a name="zh-cn_topic_0225568943_p9809215115310"></a><a name="zh-cn_topic_0225568943_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568943_p1280914152538"><a name="zh-cn_topic_0225568943_p1280914152538"></a><a name="zh-cn_topic_0225568943_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568943_p1880914157537"><a name="zh-cn_topic_0225568943_p1880914157537"></a><a name="zh-cn_topic_0225568943_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568943_section3743"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568943_table64045020"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568943_row14048815"><th class="cellrowborder" valign="top" width="15.308469153084689%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568943_p64212251"><a name="zh-cn_topic_0225568943_p64212251"></a><a name="zh-cn_topic_0225568943_p64212251"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568943_p33809876"><a name="zh-cn_topic_0225568943_p33809876"></a><a name="zh-cn_topic_0225568943_p33809876"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.288571142885708%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568943_p54245441"><a name="zh-cn_topic_0225568943_p54245441"></a><a name="zh-cn_topic_0225568943_p54245441"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.11438856114388%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568943_p31804619"><a name="zh-cn_topic_0225568943_p31804619"></a><a name="zh-cn_topic_0225568943_p31804619"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568943_row26037337"><td class="cellrowborder" valign="top" width="15.308469153084689%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568943_p28649556"><a name="zh-cn_topic_0225568943_p28649556"></a><a name="zh-cn_topic_0225568943_p28649556"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568943_p38912675"><a name="zh-cn_topic_0225568943_p38912675"></a><a name="zh-cn_topic_0225568943_p38912675"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568943_p64918959"><a name="zh-cn_topic_0225568943_p64918959"></a><a name="zh-cn_topic_0225568943_p64918959"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.11438856114388%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568943_p23944287"><a name="zh-cn_topic_0225568943_p23944287"></a><a name="zh-cn_topic_0225568943_p23944287"></a>签名密钥编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row7080698"><td class="cellrowborder" valign="top" width="15.308469153084689%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568943_p36665652"><a name="zh-cn_topic_0225568943_p36665652"></a><a name="zh-cn_topic_0225568943_p36665652"></a>publish_ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568943_p17127855"><a name="zh-cn_topic_0225568943_p17127855"></a><a name="zh-cn_topic_0225568943_p17127855"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.288571142885708%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568943_p45179027"><a name="zh-cn_topic_0225568943_p45179027"></a><a name="zh-cn_topic_0225568943_p45179027"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="56.11438856114388%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568943_p35622534"><a name="zh-cn_topic_0225568943_p35622534"></a><a name="zh-cn_topic_0225568943_p35622534"></a>API的发布记录编号</p>
</td>
</tr>
</tbody>
</table>

请求参数样例：

```
{
  "sign_id": "3a793b65a9034bdfae08924f149bfb4a",
  "publish_ids": [
    "374a6d5a-20c7-4ea1-82e1-19fce4556956",
    "65e6fe53-1ac3-4481-ba36-9f0bc6f22057"
  ]
}
```

## 响应消息<a name="zh-cn_topic_0225568943_section303246"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568943_table50099799"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568943_row33619400"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568943_p38816869"><a name="zh-cn_topic_0225568943_p38816869"></a><a name="zh-cn_topic_0225568943_p38816869"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568943_p57158666"><a name="zh-cn_topic_0225568943_p57158666"></a><a name="zh-cn_topic_0225568943_p57158666"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568943_p66449248"><a name="zh-cn_topic_0225568943_p66449248"></a><a name="zh-cn_topic_0225568943_p66449248"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568943_row13680014"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p34339389"><a name="zh-cn_topic_0225568943_p34339389"></a><a name="zh-cn_topic_0225568943_p34339389"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p30027157"><a name="zh-cn_topic_0225568943_p30027157"></a><a name="zh-cn_topic_0225568943_p30027157"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p16280637"><a name="zh-cn_topic_0225568943_p16280637"></a><a name="zh-cn_topic_0225568943_p16280637"></a>API与签名密钥的绑定关系列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  字典类型响应参数

<a name="zh-cn_topic_0225568943_table43663197"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568943_row22855600"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568943_p39364310"><a name="zh-cn_topic_0225568943_p39364310"></a><a name="zh-cn_topic_0225568943_p39364310"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568943_p34392512"><a name="zh-cn_topic_0225568943_p34392512"></a><a name="zh-cn_topic_0225568943_p34392512"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568943_p34330070"><a name="zh-cn_topic_0225568943_p34330070"></a><a name="zh-cn_topic_0225568943_p34330070"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568943_row29272322"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p22247849"><a name="zh-cn_topic_0225568943_p22247849"></a><a name="zh-cn_topic_0225568943_p22247849"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p57245365"><a name="zh-cn_topic_0225568943_p57245365"></a><a name="zh-cn_topic_0225568943_p57245365"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p6363022"><a name="zh-cn_topic_0225568943_p6363022"></a><a name="zh-cn_topic_0225568943_p6363022"></a>绑定关系的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row57267203"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p8131833"><a name="zh-cn_topic_0225568943_p8131833"></a><a name="zh-cn_topic_0225568943_p8131833"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p54698736"><a name="zh-cn_topic_0225568943_p54698736"></a><a name="zh-cn_topic_0225568943_p54698736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p1412623"><a name="zh-cn_topic_0225568943_p1412623"></a><a name="zh-cn_topic_0225568943_p1412623"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row12713614"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p23169789"><a name="zh-cn_topic_0225568943_p23169789"></a><a name="zh-cn_topic_0225568943_p23169789"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p64813609"><a name="zh-cn_topic_0225568943_p64813609"></a><a name="zh-cn_topic_0225568943_p64813609"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p15410937"><a name="zh-cn_topic_0225568943_p15410937"></a><a name="zh-cn_topic_0225568943_p15410937"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row4480706"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p27392900"><a name="zh-cn_topic_0225568943_p27392900"></a><a name="zh-cn_topic_0225568943_p27392900"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p4232414"><a name="zh-cn_topic_0225568943_p4232414"></a><a name="zh-cn_topic_0225568943_p4232414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p7281273"><a name="zh-cn_topic_0225568943_p7281273"></a><a name="zh-cn_topic_0225568943_p7281273"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row65531462"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p6448229"><a name="zh-cn_topic_0225568943_p6448229"></a><a name="zh-cn_topic_0225568943_p6448229"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p52544536"><a name="zh-cn_topic_0225568943_p52544536"></a><a name="zh-cn_topic_0225568943_p52544536"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p28249032"><a name="zh-cn_topic_0225568943_p28249032"></a><a name="zh-cn_topic_0225568943_p28249032"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row52914698"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p58232127"><a name="zh-cn_topic_0225568943_p58232127"></a><a name="zh-cn_topic_0225568943_p58232127"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p19181861"><a name="zh-cn_topic_0225568943_p19181861"></a><a name="zh-cn_topic_0225568943_p19181861"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p10226915"><a name="zh-cn_topic_0225568943_p10226915"></a><a name="zh-cn_topic_0225568943_p10226915"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row24933379"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p6337850"><a name="zh-cn_topic_0225568943_p6337850"></a><a name="zh-cn_topic_0225568943_p6337850"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p43603804"><a name="zh-cn_topic_0225568943_p43603804"></a><a name="zh-cn_topic_0225568943_p43603804"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p42247251"><a name="zh-cn_topic_0225568943_p42247251"></a><a name="zh-cn_topic_0225568943_p42247251"></a>签名密钥的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row44680946"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p62386883"><a name="zh-cn_topic_0225568943_p62386883"></a><a name="zh-cn_topic_0225568943_p62386883"></a>sign_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p20172764"><a name="zh-cn_topic_0225568943_p20172764"></a><a name="zh-cn_topic_0225568943_p20172764"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p23381222"><a name="zh-cn_topic_0225568943_p23381222"></a><a name="zh-cn_topic_0225568943_p23381222"></a>签名密钥的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row9104413"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p66368851"><a name="zh-cn_topic_0225568943_p66368851"></a><a name="zh-cn_topic_0225568943_p66368851"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p7167821"><a name="zh-cn_topic_0225568943_p7167821"></a><a name="zh-cn_topic_0225568943_p7167821"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p43722611"><a name="zh-cn_topic_0225568943_p43722611"></a><a name="zh-cn_topic_0225568943_p43722611"></a>签名密钥的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row57959187"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p64182567"><a name="zh-cn_topic_0225568943_p64182567"></a><a name="zh-cn_topic_0225568943_p64182567"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p31405468"><a name="zh-cn_topic_0225568943_p31405468"></a><a name="zh-cn_topic_0225568943_p31405468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p60815002"><a name="zh-cn_topic_0225568943_p60815002"></a><a name="zh-cn_topic_0225568943_p60815002"></a>签名密钥的密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row10464107"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p42286344"><a name="zh-cn_topic_0225568943_p42286344"></a><a name="zh-cn_topic_0225568943_p42286344"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p2641858"><a name="zh-cn_topic_0225568943_p2641858"></a><a name="zh-cn_topic_0225568943_p2641858"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p12663936"><a name="zh-cn_topic_0225568943_p12663936"></a><a name="zh-cn_topic_0225568943_p12663936"></a>API所属环境的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row46866564"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p38095364"><a name="zh-cn_topic_0225568943_p38095364"></a><a name="zh-cn_topic_0225568943_p38095364"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p65825661"><a name="zh-cn_topic_0225568943_p65825661"></a><a name="zh-cn_topic_0225568943_p65825661"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p30278294"><a name="zh-cn_topic_0225568943_p30278294"></a><a name="zh-cn_topic_0225568943_p30278294"></a>API所属环境的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row4069190"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p61168946"><a name="zh-cn_topic_0225568943_p61168946"></a><a name="zh-cn_topic_0225568943_p61168946"></a>binding_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p55737619"><a name="zh-cn_topic_0225568943_p55737619"></a><a name="zh-cn_topic_0225568943_p55737619"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p18453329"><a name="zh-cn_topic_0225568943_p18453329"></a><a name="zh-cn_topic_0225568943_p18453329"></a>绑定时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row18964185723219"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568943_p1098354195018"><a name="zh-cn_topic_0225568943_p1098354195018"></a><a name="zh-cn_topic_0225568943_p1098354195018"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568943_p1598254185016"><a name="zh-cn_topic_0225568943_p1598254185016"></a><a name="zh-cn_topic_0225568943_p1598254185016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568943_p99875418509"><a name="zh-cn_topic_0225568943_p99875418509"></a><a name="zh-cn_topic_0225568943_p99875418509"></a>API发布ID</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
[
  {
    "id": "d8426fb090e442c4a56a35e451bea085",
    "api_id": "3c6769c6-ec61-4b45-b478-c60310dbaa1b",
    "api_name": "bbb",
    "api_remark": "",
    "group_name": "asd",
    "api_type": 1,
    "sign_id": "3a793b65a9034bdfae08924f149bfb4a",
    "sign_name": "signature01",
    "sign_key": "abcd_1234",
    "sign_secret": "******",
    "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
    "env_name": "RELEASE",
    "binding_time": "2018-02-07T03:17:26.396039456Z",
    "publish_id": "23234202f5834ab69113fc1b790b6bed"
  },
  {
    "id": "97952732e6d7452d99de02db99acce27",
    "api_id": "d85c502a-f916-47e8-bba0-50537a2d1af2",
    "api_name": "aaa",
    "api_remark": "",
    "group_name": "asd",
    "api_type": 1,
    "sign_id": "3a793b65a9034bdfae08924f149bfb4a",
    "sign_name": "signature01",
    "sign_key": "abcd_1234",
    "sign_secret": "******",
    "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
    "env_name": "RELEASE",
    "binding_time": "2018-02-07T03:17:26.39803282Z",
    "publish_id": "6581f68efddc4ff0815e156ec6ecfb52"
  }
]
```

## 状态码<a name="zh-cn_topic_0225568943_section33694"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0225568943_table42581536"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568943_row29329421"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568943_p26872901"><a name="zh-cn_topic_0225568943_p26872901"></a><a name="zh-cn_topic_0225568943_p26872901"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568943_p61665884"><a name="zh-cn_topic_0225568943_p61665884"></a><a name="zh-cn_topic_0225568943_p61665884"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568943_row58600025"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568943_p48981555"><a name="zh-cn_topic_0225568943_p48981555"></a><a name="zh-cn_topic_0225568943_p48981555"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568943_p73578115452"><a name="zh-cn_topic_0225568943_p73578115452"></a><a name="zh-cn_topic_0225568943_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row5638153"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568943_p54037245"><a name="zh-cn_topic_0225568943_p54037245"></a><a name="zh-cn_topic_0225568943_p54037245"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568943_p14940754"><a name="zh-cn_topic_0225568943_p14940754"></a><a name="zh-cn_topic_0225568943_p14940754"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row249064"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568943_p20174257"><a name="zh-cn_topic_0225568943_p20174257"></a><a name="zh-cn_topic_0225568943_p20174257"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568943_p23502126"><a name="zh-cn_topic_0225568943_p23502126"></a><a name="zh-cn_topic_0225568943_p23502126"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row10192548"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568943_p20290059"><a name="zh-cn_topic_0225568943_p20290059"></a><a name="zh-cn_topic_0225568943_p20290059"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568943_p32882074"><a name="zh-cn_topic_0225568943_p32882074"></a><a name="zh-cn_topic_0225568943_p32882074"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row27503217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568943_p13168080"><a name="zh-cn_topic_0225568943_p13168080"></a><a name="zh-cn_topic_0225568943_p13168080"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568943_p15296380"><a name="zh-cn_topic_0225568943_p15296380"></a><a name="zh-cn_topic_0225568943_p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568943_row2963020"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568943_p38678029"><a name="zh-cn_topic_0225568943_p38678029"></a><a name="zh-cn_topic_0225568943_p38678029"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568943_p6744143"><a name="zh-cn_topic_0225568943_p6744143"></a><a name="zh-cn_topic_0225568943_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

