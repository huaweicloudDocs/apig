# 将API与ACL策略进行绑定<a name="ZH-CN_TOPIC_0000001081976203"></a>

## 功能介绍<a name="zh-cn_topic_0225568893_section4185058"></a>

将API与ACL策略进行绑定。

同一个API发布到不同的环境可以绑定不同的ACL策略；一个API在发布到特定环境后只能绑定一个同一种类型的ACL策略。

## URI<a name="zh-cn_topic_0225568893_section37665524"></a>

HTTPS请求方法以及URI如下表所示。

**表 1**  HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568893_table21134163"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568893_row20005630"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568893_p9843325"><a name="zh-cn_topic_0225568893_p9843325"></a><a name="zh-cn_topic_0225568893_p9843325"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568893_p59111885"><a name="zh-cn_topic_0225568893_p59111885"></a><a name="zh-cn_topic_0225568893_p59111885"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568893_row23333398"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568893_p10957055"><a name="zh-cn_topic_0225568893_p10957055"></a><a name="zh-cn_topic_0225568893_p10957055"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568893_p15106224"><a name="zh-cn_topic_0225568893_p15106224"></a><a name="zh-cn_topic_0225568893_p15106224"></a>/v1/{project_id}/apigw/instances/{instance_id}/acl-bindings</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568893_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568893_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568893_p23103637"><a name="zh-cn_topic_0225568893_p23103637"></a><a name="zh-cn_topic_0225568893_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568893_p59455291"><a name="zh-cn_topic_0225568893_p59455291"></a><a name="zh-cn_topic_0225568893_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568893_p51149303"><a name="zh-cn_topic_0225568893_p51149303"></a><a name="zh-cn_topic_0225568893_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568893_p49452846"><a name="zh-cn_topic_0225568893_p49452846"></a><a name="zh-cn_topic_0225568893_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568893_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568893_p55878963"><a name="zh-cn_topic_0225568893_p55878963"></a><a name="zh-cn_topic_0225568893_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568893_p29902160"><a name="zh-cn_topic_0225568893_p29902160"></a><a name="zh-cn_topic_0225568893_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568893_p6155914"><a name="zh-cn_topic_0225568893_p6155914"></a><a name="zh-cn_topic_0225568893_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568893_p28867016"><a name="zh-cn_topic_0225568893_p28867016"></a><a name="zh-cn_topic_0225568893_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568893_p1780913159538"><a name="zh-cn_topic_0225568893_p1780913159538"></a><a name="zh-cn_topic_0225568893_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568893_p9809215115310"><a name="zh-cn_topic_0225568893_p9809215115310"></a><a name="zh-cn_topic_0225568893_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568893_p1280914152538"><a name="zh-cn_topic_0225568893_p1280914152538"></a><a name="zh-cn_topic_0225568893_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568893_p1880914157537"><a name="zh-cn_topic_0225568893_p1880914157537"></a><a name="zh-cn_topic_0225568893_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568893_section3445397"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568893_table15644626"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568893_row37216067"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568893_p61711446"><a name="zh-cn_topic_0225568893_p61711446"></a><a name="zh-cn_topic_0225568893_p61711446"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568893_p32571238"><a name="zh-cn_topic_0225568893_p32571238"></a><a name="zh-cn_topic_0225568893_p32571238"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568893_p21024602"><a name="zh-cn_topic_0225568893_p21024602"></a><a name="zh-cn_topic_0225568893_p21024602"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568893_row25271195"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568893_p33700880"><a name="zh-cn_topic_0225568893_p33700880"></a><a name="zh-cn_topic_0225568893_p33700880"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568893_p45416737"><a name="zh-cn_topic_0225568893_p45416737"></a><a name="zh-cn_topic_0225568893_p45416737"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568893_p54877112"><a name="zh-cn_topic_0225568893_p54877112"></a><a name="zh-cn_topic_0225568893_p54877112"></a>ACL策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row24131960"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568893_p8531728"><a name="zh-cn_topic_0225568893_p8531728"></a><a name="zh-cn_topic_0225568893_p8531728"></a>publish_ids</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568893_p19981344"><a name="zh-cn_topic_0225568893_p19981344"></a><a name="zh-cn_topic_0225568893_p19981344"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568893_p38451245151916"><a name="zh-cn_topic_0225568893_p38451245151916"></a><a name="zh-cn_topic_0225568893_p38451245151916"></a>API发布记录编号</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "acl_id": "206bb985d8a04ec09f13c3e51ef77095",
  "publish_ids": [
    "1bc8b2b741a04bd4af3ef9d7cd003104"
  ]
}
```

## 响应消息<a name="zh-cn_topic_0225568893_section10641712"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568893_table34900477"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568893_row37249813"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568893_p64444853"><a name="zh-cn_topic_0225568893_p64444853"></a><a name="zh-cn_topic_0225568893_p64444853"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568893_p52650614"><a name="zh-cn_topic_0225568893_p52650614"></a><a name="zh-cn_topic_0225568893_p52650614"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568893_p36841343"><a name="zh-cn_topic_0225568893_p36841343"></a><a name="zh-cn_topic_0225568893_p36841343"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568893_row31358841"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568893_p57038220"><a name="zh-cn_topic_0225568893_p57038220"></a><a name="zh-cn_topic_0225568893_p57038220"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568893_p56693087"><a name="zh-cn_topic_0225568893_p56693087"></a><a name="zh-cn_topic_0225568893_p56693087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568893_p28737306"><a name="zh-cn_topic_0225568893_p28737306"></a><a name="zh-cn_topic_0225568893_p28737306"></a>绑定关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row57309166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568893_p11530906"><a name="zh-cn_topic_0225568893_p11530906"></a><a name="zh-cn_topic_0225568893_p11530906"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568893_p61588161"><a name="zh-cn_topic_0225568893_p61588161"></a><a name="zh-cn_topic_0225568893_p61588161"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568893_p22585165"><a name="zh-cn_topic_0225568893_p22585165"></a><a name="zh-cn_topic_0225568893_p22585165"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row1939901"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568893_p22914267"><a name="zh-cn_topic_0225568893_p22914267"></a><a name="zh-cn_topic_0225568893_p22914267"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568893_p44116305"><a name="zh-cn_topic_0225568893_p44116305"></a><a name="zh-cn_topic_0225568893_p44116305"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568893_p16650952"><a name="zh-cn_topic_0225568893_p16650952"></a><a name="zh-cn_topic_0225568893_p16650952"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row15640843"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568893_p58948774"><a name="zh-cn_topic_0225568893_p58948774"></a><a name="zh-cn_topic_0225568893_p58948774"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568893_p10121365"><a name="zh-cn_topic_0225568893_p10121365"></a><a name="zh-cn_topic_0225568893_p10121365"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568893_p14524225"><a name="zh-cn_topic_0225568893_p14524225"></a><a name="zh-cn_topic_0225568893_p14524225"></a>ACL策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row63609161"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568893_p52068378"><a name="zh-cn_topic_0225568893_p52068378"></a><a name="zh-cn_topic_0225568893_p52068378"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568893_p56789084"><a name="zh-cn_topic_0225568893_p56789084"></a><a name="zh-cn_topic_0225568893_p56789084"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568893_p36513078"><a name="zh-cn_topic_0225568893_p36513078"></a><a name="zh-cn_topic_0225568893_p36513078"></a>绑定时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
[
  {
    "id": "4ffc0da71ddd4c22add8ff801e19846c",
    "api_id": "aebacac6095942b4b2dd2b209bb7b9bc",
    "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
    "acl_id": "206bb985d8a04ec09f13c3e51ef77095",
    "create_time": "2018-07-27T11:27:10.7470224Z"
  }
]
```

## 状态码<a name="zh-cn_topic_0225568893_section31008574"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568893_table63806506"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568893_row17466566"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568893_p5505760"><a name="zh-cn_topic_0225568893_p5505760"></a><a name="zh-cn_topic_0225568893_p5505760"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568893_p43313406"><a name="zh-cn_topic_0225568893_p43313406"></a><a name="zh-cn_topic_0225568893_p43313406"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568893_row18725001"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568893_p40330088"><a name="zh-cn_topic_0225568893_p40330088"></a><a name="zh-cn_topic_0225568893_p40330088"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568893_p73578115452"><a name="zh-cn_topic_0225568893_p73578115452"></a><a name="zh-cn_topic_0225568893_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row6951972"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568893_p26238821"><a name="zh-cn_topic_0225568893_p26238821"></a><a name="zh-cn_topic_0225568893_p26238821"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568893_p44969751"><a name="zh-cn_topic_0225568893_p44969751"></a><a name="zh-cn_topic_0225568893_p44969751"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row2074577"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568893_p33823087"><a name="zh-cn_topic_0225568893_p33823087"></a><a name="zh-cn_topic_0225568893_p33823087"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568893_p55315537"><a name="zh-cn_topic_0225568893_p55315537"></a><a name="zh-cn_topic_0225568893_p55315537"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row28077792"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568893_p59708643"><a name="zh-cn_topic_0225568893_p59708643"></a><a name="zh-cn_topic_0225568893_p59708643"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568893_p4561952"><a name="zh-cn_topic_0225568893_p4561952"></a><a name="zh-cn_topic_0225568893_p4561952"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568893_row41057571"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568893_p37328935"><a name="zh-cn_topic_0225568893_p37328935"></a><a name="zh-cn_topic_0225568893_p37328935"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568893_p6744143"><a name="zh-cn_topic_0225568893_p6744143"></a><a name="zh-cn_topic_0225568893_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

