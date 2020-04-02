# 将API与ACL策略进行绑定<a name="apig-phapi-180713093"></a>

## 功能介绍<a name="section4185058"></a>

将API与ACL策略进行绑定。

同一个API发布到不同的环境可以绑定不同的ACL策略；一个API在发布到特定环境后只能绑定一个同一种类型的ACL策略。

## URI<a name="section37665524"></a>

HTTPS请求方法以及URI如下表所示。

**表 1**  HTTPS请求方法以及URI

<a name="table21134163"></a>
<table><thead align="left"><tr id="row20005630"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p9843325"><a name="p9843325"></a><a name="p9843325"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p59111885"><a name="p59111885"></a><a name="p59111885"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row23333398"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p10957055"><a name="p10957055"></a><a name="p10957055"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p15106224"><a name="p15106224"></a><a name="p15106224"></a>/v1/{project_id}/apigw/instances/{instance_id}/acl-bindings</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table38510415"></a>
<table><thead align="left"><tr id="row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="p23103637"><a name="p23103637"></a><a name="p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p59455291"><a name="p59455291"></a><a name="p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="p51149303"><a name="p51149303"></a><a name="p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="p49452846"><a name="p49452846"></a><a name="p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section3445397"></a>

**表 3**  参数说明

<a name="table15644626"></a>
<table><thead align="left"><tr id="row37216067"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p61711446"><a name="p61711446"></a><a name="p61711446"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p32571238"><a name="p32571238"></a><a name="p32571238"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p21024602"><a name="p21024602"></a><a name="p21024602"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row25271195"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p33700880"><a name="p33700880"></a><a name="p33700880"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p45416737"><a name="p45416737"></a><a name="p45416737"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54877112"><a name="p54877112"></a><a name="p54877112"></a>ACL策略编号</p>
</td>
</tr>
<tr id="row24131960"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8531728"><a name="p8531728"></a><a name="p8531728"></a>publish_ids</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19981344"><a name="p19981344"></a><a name="p19981344"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38451245151916"><a name="p38451245151916"></a><a name="p38451245151916"></a>API发布记录编号</p>
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

## 响应消息<a name="section10641712"></a>

**表 4**  参数说明

<a name="table34900477"></a>
<table><thead align="left"><tr id="row37249813"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p64444853"><a name="p64444853"></a><a name="p64444853"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p52650614"><a name="p52650614"></a><a name="p52650614"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p36841343"><a name="p36841343"></a><a name="p36841343"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row31358841"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57038220"><a name="p57038220"></a><a name="p57038220"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56693087"><a name="p56693087"></a><a name="p56693087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p28737306"><a name="p28737306"></a><a name="p28737306"></a>绑定关系编号</p>
</td>
</tr>
<tr id="row57309166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11530906"><a name="p11530906"></a><a name="p11530906"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p61588161"><a name="p61588161"></a><a name="p61588161"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p22585165"><a name="p22585165"></a><a name="p22585165"></a>API编号</p>
</td>
</tr>
<tr id="row1939901"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p22914267"><a name="p22914267"></a><a name="p22914267"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44116305"><a name="p44116305"></a><a name="p44116305"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16650952"><a name="p16650952"></a><a name="p16650952"></a>环境编号</p>
</td>
</tr>
<tr id="row15640843"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p58948774"><a name="p58948774"></a><a name="p58948774"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10121365"><a name="p10121365"></a><a name="p10121365"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14524225"><a name="p14524225"></a><a name="p14524225"></a>ACL策略编号</p>
</td>
</tr>
<tr id="row63609161"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52068378"><a name="p52068378"></a><a name="p52068378"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56789084"><a name="p56789084"></a><a name="p56789084"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36513078"><a name="p36513078"></a><a name="p36513078"></a>绑定时间</p>
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

## 状态码<a name="section31008574"></a>

**表 5**  返回消息说明

<a name="table63806506"></a>
<table><thead align="left"><tr id="row17466566"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p5505760"><a name="p5505760"></a><a name="p5505760"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p43313406"><a name="p43313406"></a><a name="p43313406"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18725001"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p40330088"><a name="p40330088"></a><a name="p40330088"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p73578115452"><a name="p73578115452"></a><a name="p73578115452"></a>Created</p>
</td>
</tr>
<tr id="row6951972"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p26238821"><a name="p26238821"></a><a name="p26238821"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p44969751"><a name="p44969751"></a><a name="p44969751"></a>Bad Request</p>
</td>
</tr>
<tr id="row2074577"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p33823087"><a name="p33823087"></a><a name="p33823087"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p55315537"><a name="p55315537"></a><a name="p55315537"></a>Forbidden</p>
</td>
</tr>
<tr id="row28077792"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p59708643"><a name="p59708643"></a><a name="p59708643"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p4561952"><a name="p4561952"></a><a name="p4561952"></a>Not Found</p>
</td>
</tr>
<tr id="row41057571"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p37328935"><a name="p37328935"></a><a name="p37328935"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

