# 查看ACL策略未绑定的API列表<a name="apig-phapi-180713096"></a>

## 功能介绍<a name="section61570312"></a>

查看ACL策略未绑定的API列表，需要API已发布。

## URI<a name="section17261904"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table7075937"></a>
<table><thead align="left"><tr id="row65440801"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p66213500"><a name="p66213500"></a><a name="p66213500"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p61693288"><a name="p61693288"></a><a name="p61693288"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row31100428"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p36106769"><a name="p36106769"></a><a name="p36106769"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p38967199"><a name="p38967199"></a><a name="p38967199"></a>/v1/{project_id}/apigw/instances/{instance_id}/acl-bindings/unbinded-apis[?page_no、page_size、acl_id、env_id、api_id、api_name、group-id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：acl\_id、env\_id、api\_id、group\_id、api\_name、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table45607562"></a>
<table><thead align="left"><tr id="row21909387"><th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.1"><p id="p29829884"><a name="p29829884"></a><a name="p29829884"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="9%" id="mcps1.2.5.1.2"><p id="p301534"><a name="p301534"></a><a name="p301534"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="9%" id="mcps1.2.5.1.3"><p id="p24424280"><a name="p24424280"></a><a name="p24424280"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="66%" id="mcps1.2.5.1.4"><p id="p32209683"><a name="p32209683"></a><a name="p32209683"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row15590143542015"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row172471935182017"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row58847543"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p1921642"><a name="p1921642"></a><a name="p1921642"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p21435351"><a name="p21435351"></a><a name="p21435351"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p58541860"><a name="p58541860"></a><a name="p58541860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p17951547165618"><a name="p17951547165618"></a><a name="p17951547165618"></a>ACL策略编号</p>
</td>
</tr>
<tr id="row62887495"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p60722300"><a name="p60722300"></a><a name="p60722300"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p19559245"><a name="p19559245"></a><a name="p19559245"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p40795044"><a name="p40795044"></a><a name="p40795044"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p16064230"><a name="p16064230"></a><a name="p16064230"></a>环境编号</p>
</td>
</tr>
<tr id="row10360348"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p33881836"><a name="p33881836"></a><a name="p33881836"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p60074205"><a name="p60074205"></a><a name="p60074205"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p34172438"><a name="p34172438"></a><a name="p34172438"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p16504128"><a name="p16504128"></a><a name="p16504128"></a>API分组编号</p>
</td>
</tr>
<tr id="row14319431"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p19023261"><a name="p19023261"></a><a name="p19023261"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p64489143"><a name="p64489143"></a><a name="p64489143"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p56238077"><a name="p56238077"></a><a name="p56238077"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p58990425"><a name="p58990425"></a><a name="p58990425"></a>API编号</p>
</td>
</tr>
<tr id="row61151777"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p54346934"><a name="p54346934"></a><a name="p54346934"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p40025556"><a name="p40025556"></a><a name="p40025556"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p20844578"><a name="p20844578"></a><a name="p20844578"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p10689224"><a name="p10689224"></a><a name="p10689224"></a>API名称</p>
</td>
</tr>
<tr id="row29094156"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p7816426"><a name="p7816426"></a><a name="p7816426"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p29150773"><a name="p29150773"></a><a name="p29150773"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p12402388"><a name="p12402388"></a><a name="p12402388"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p65069360"><a name="p65069360"></a><a name="p65069360"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row48753328"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="p56705457"><a name="p56705457"></a><a name="p56705457"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="p29739299"><a name="p29739299"></a><a name="p29739299"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="p60073005"><a name="p60073005"></a><a name="p60073005"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="p34075256"><a name="p34075256"></a><a name="p34075256"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section21139415"></a>

无

## 响应消息<a name="section34571087"></a>

**表 3**  参数说明

<a name="table11928633"></a>
<table><thead align="left"><tr id="row60512777"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p2587895"><a name="p2587895"></a><a name="p2587895"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p8292946"><a name="p8292946"></a><a name="p8292946"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p640001"><a name="p640001"></a><a name="p640001"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51840109"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p38299261"><a name="p38299261"></a><a name="p38299261"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p15232409"><a name="p15232409"></a><a name="p15232409"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p34954265718"><a name="p34954265718"></a><a name="p34954265718"></a>符合条件的API总数</p>
</td>
</tr>
<tr id="row31464194"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p65571805"><a name="p65571805"></a><a name="p65571805"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9716001"><a name="p9716001"></a><a name="p9716001"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48798580"><a name="p48798580"></a><a name="p48798580"></a>本次查询返回的API个数</p>
</td>
</tr>
<tr id="row36534044"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6467596"><a name="p6467596"></a><a name="p6467596"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p54113248"><a name="p54113248"></a><a name="p54113248"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p21096961"><a name="p21096961"></a><a name="p21096961"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table55654921"></a>
<table><thead align="left"><tr id="row66950944"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p54317399"><a name="p54317399"></a><a name="p54317399"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p37633227"><a name="p37633227"></a><a name="p37633227"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p28392547"><a name="p28392547"></a><a name="p28392547"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18094984"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p56407585"><a name="p56407585"></a><a name="p56407585"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5611671"><a name="p5611671"></a><a name="p5611671"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p51892177"><a name="p51892177"></a><a name="p51892177"></a>API的ID。</p>
</td>
</tr>
<tr id="row64376411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47106807"><a name="p47106807"></a><a name="p47106807"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57555019"><a name="p57555019"></a><a name="p57555019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p31444992"><a name="p31444992"></a><a name="p31444992"></a>API名称</p>
</td>
</tr>
<tr id="row14569478"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39277103"><a name="p39277103"></a><a name="p39277103"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p27328780"><a name="p27328780"></a><a name="p27328780"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66147590"><a name="p66147590"></a><a name="p66147590"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row58457401"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37429032"><a name="p37429032"></a><a name="p37429032"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11852776"><a name="p11852776"></a><a name="p11852776"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20550817"><a name="p20550817"></a><a name="p20550817"></a>API所属分组的名称。</p>
</td>
</tr>
<tr id="row4920279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p62998338"><a name="p62998338"></a><a name="p62998338"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2591766"><a name="p2591766"></a><a name="p2591766"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8606457"><a name="p8606457"></a><a name="p8606457"></a>API开放状态</p>
</td>
</tr>
<tr id="row57391748"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18220050"><a name="p18220050"></a><a name="p18220050"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66537956"><a name="p66537956"></a><a name="p66537956"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20865379"><a name="p20865379"></a><a name="p20865379"></a>API描述</p>
</td>
</tr>
<tr id="row57771451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48975920"><a name="p48975920"></a><a name="p48975920"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7626561"><a name="p7626561"></a><a name="p7626561"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13771736"><a name="p13771736"></a><a name="p13771736"></a>发布的环境名</p>
</td>
</tr>
<tr id="row56836760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40374832"><a name="p40374832"></a><a name="p40374832"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p49135936"><a name="p49135936"></a><a name="p49135936"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20587889"><a name="p20587889"></a><a name="p20587889"></a>发布的环境id</p>
</td>
</tr>
<tr id="row51073277"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p43294786"><a name="p43294786"></a><a name="p43294786"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17216763"><a name="p17216763"></a><a name="p17216763"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52380561"><a name="p52380561"></a><a name="p52380561"></a>API发布记录编号</p>
</td>
</tr>
<tr id="row1663002"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p485445"><a name="p485445"></a><a name="p485445"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p39321089"><a name="p39321089"></a><a name="p39321089"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30891637"><a name="p30891637"></a><a name="p30891637"></a>绑定的其他同类型的ACL策略名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 1,
  "size": 1,
  "apis": [
    {
      "name": "bbbbb",
      "type": 1,
      "remark": "aaa",
      "group_id": "70f1b578da9b4dfe889b4c33d1b995c2",
      "id": "91c26288acea4448be205265d77dae22",
      "group_name": "test001",
      "run_env_name": "RELEASE",
      "run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "publish_id": "a6e06a00c382436eb524fa2dd343cb6d"
    }
  ]
}
```

## 状态码<a name="section56037015"></a>

**表 5**  返回消息说明

<a name="table28132847"></a>
<table><thead align="left"><tr id="row3719443"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p32839460"><a name="p32839460"></a><a name="p32839460"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p42750569"><a name="p42750569"></a><a name="p42750569"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row40244042"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p38542001"><a name="p38542001"></a><a name="p38542001"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p34894339"><a name="p34894339"></a><a name="p34894339"></a>OK</p>
</td>
</tr>
<tr id="row45613601"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3714177"><a name="p3714177"></a><a name="p3714177"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p32412930"><a name="p32412930"></a><a name="p32412930"></a>Bad Request</p>
</td>
</tr>
<tr id="row23280918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6706219"><a name="p6706219"></a><a name="p6706219"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6332852"><a name="p6332852"></a><a name="p6332852"></a>Forbidden</p>
</td>
</tr>
<tr id="row56995672"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p53246699"><a name="p53246699"></a><a name="p53246699"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p18015334"><a name="p18015334"></a><a name="p18015334"></a>Not Found</p>
</td>
</tr>
<tr id="row27920282"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p46950406"><a name="p46950406"></a><a name="p46950406"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p44886509"><a name="p44886509"></a><a name="p44886509"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

