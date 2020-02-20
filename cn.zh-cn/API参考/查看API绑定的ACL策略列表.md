# 查看API绑定的ACL策略列表<a name="apig-zh-api-180713094"></a>

## 功能介绍<a name="section30108054"></a>

查看API绑定的ACL策略列表。

## URI<a name="section2537034"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table49976511"></a>
<table><thead align="left"><tr id="row26320038"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p51548346"><a name="p51548346"></a><a name="p51548346"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p14666461"><a name="p14666461"></a><a name="p14666461"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row47132730"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p59654775"><a name="p59654775"></a><a name="p59654775"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p198588"><a name="p198588"></a><a name="p198588"></a>/v1.0/apigw/acl-bindings/binded-acls[?page_no,page_size,api_id,env_id,env_name,acl_id,acl_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：api\_id、env\_id、env\_name、acl\_id、acl\_name、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table43029199"></a>
<table><thead align="left"><tr id="row45836208"><th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.1"><p id="p21745369"><a name="p21745369"></a><a name="p21745369"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.891089108910892%" id="mcps1.2.5.1.2"><p id="p16544499"><a name="p16544499"></a><a name="p16544499"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="p65036070"><a name="p65036070"></a><a name="p65036070"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.37623762376238%" id="mcps1.2.5.1.4"><p id="p33430297"><a name="p33430297"></a><a name="p33430297"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row23499508"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p24412000"><a name="p24412000"></a><a name="p24412000"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p31214980"><a name="p31214980"></a><a name="p31214980"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p45385481"><a name="p45385481"></a><a name="p45385481"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="p10285592386"><a name="p10285592386"></a><a name="p10285592386"></a>API编号</p>
</td>
</tr>
<tr id="row8153146123920"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p1815376143911"><a name="p1815376143911"></a><a name="p1815376143911"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p663174018395"><a name="p663174018395"></a><a name="p663174018395"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p191531693911"><a name="p191531693911"></a><a name="p191531693911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="p9153136133912"><a name="p9153136133912"></a><a name="p9153136133912"></a>环境编号</p>
</td>
</tr>
<tr id="row135689703917"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p456820713391"><a name="p456820713391"></a><a name="p456820713391"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p155683793917"><a name="p155683793917"></a><a name="p155683793917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p3568677398"><a name="p3568677398"></a><a name="p3568677398"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="p1756817103915"><a name="p1756817103915"></a><a name="p1756817103915"></a>环境名称</p>
</td>
</tr>
<tr id="row12818171110390"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p14818121114395"><a name="p14818121114395"></a><a name="p14818121114395"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p1781851114392"><a name="p1781851114392"></a><a name="p1781851114392"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p1581801119394"><a name="p1581801119394"></a><a name="p1581801119394"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="p138183119399"><a name="p138183119399"></a><a name="p138183119399"></a>ACL策略编号</p>
</td>
</tr>
<tr id="row1885014156393"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p5850815103913"><a name="p5850815103913"></a><a name="p5850815103913"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p1885031520392"><a name="p1885031520392"></a><a name="p1885031520392"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p38501215163918"><a name="p38501215163918"></a><a name="p38501215163918"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="p10850101517392"><a name="p10850101517392"></a><a name="p10850101517392"></a>ACL策略名称</p>
</td>
</tr>
<tr id="row1346256"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p41937917"><a name="p41937917"></a><a name="p41937917"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p41528135"><a name="p41528135"></a><a name="p41528135"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p8335765"><a name="p8335765"></a><a name="p8335765"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="p4108368"><a name="p4108368"></a><a name="p4108368"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row36975313"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="p42210394"><a name="p42210394"></a><a name="p42210394"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p63598723"><a name="p63598723"></a><a name="p63598723"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p51222900"><a name="p51222900"></a><a name="p51222900"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="p55414230"><a name="p55414230"></a><a name="p55414230"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section22833309"></a>

无

## 响应消息<a name="section37558732"></a>

**表 3**  参数说明

<a name="table25559313"></a>
<table><thead align="left"><tr id="row3221530"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p59617344"><a name="p59617344"></a><a name="p59617344"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p64275559"><a name="p64275559"></a><a name="p64275559"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p38937782"><a name="p38937782"></a><a name="p38937782"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row66952662"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p54456559"><a name="p54456559"></a><a name="p54456559"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48905128"><a name="p48905128"></a><a name="p48905128"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1892393"><a name="p1892393"></a><a name="p1892393"></a>绑定的ACL总数</p>
</td>
</tr>
<tr id="row17031540"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37377525"><a name="p37377525"></a><a name="p37377525"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7680723"><a name="p7680723"></a><a name="p7680723"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p86659249416"><a name="p86659249416"></a><a name="p86659249416"></a>本次查询返回的ACL数量</p>
</td>
</tr>
<tr id="row29211812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17346535"><a name="p17346535"></a><a name="p17346535"></a>acls</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62892132"><a name="p62892132"></a><a name="p62892132"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p178717349415"><a name="p178717349415"></a><a name="p178717349415"></a>本次查询返回的ACL列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  acls参数说明

<a name="table13010379"></a>
<table><thead align="left"><tr id="row3739801"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p34488497"><a name="p34488497"></a><a name="p34488497"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p42104857"><a name="p42104857"></a><a name="p42104857"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p55050233"><a name="p55050233"></a><a name="p55050233"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row29883898"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4676675"><a name="p4676675"></a><a name="p4676675"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p43266429"><a name="p43266429"></a><a name="p43266429"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p530655114215"><a name="p530655114215"></a><a name="p530655114215"></a>ACL策略编号</p>
</td>
</tr>
<tr id="row61266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4962556"><a name="p4962556"></a><a name="p4962556"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66422738"><a name="p66422738"></a><a name="p66422738"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11532734"><a name="p11532734"></a><a name="p11532734"></a>ACL策略名称</p>
</td>
</tr>
<tr id="row36685742"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18755155"><a name="p18755155"></a><a name="p18755155"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42772609"><a name="p42772609"></a><a name="p42772609"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p42029279"><a name="p42029279"></a><a name="p42029279"></a>ACL策略类型</p>
<a name="ul42719191"></a><a name="ul42719191"></a><ul id="ul42719191"><li>PERMIT  (白名单类型)</li><li>DENY     (黑名单类型)</li></ul>
</td>
</tr>
<tr id="row3777868"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37571883"><a name="p37571883"></a><a name="p37571883"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23423707"><a name="p23423707"></a><a name="p23423707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p199592391421"><a name="p199592391421"></a><a name="p199592391421"></a>ACL策略值</p>
</td>
</tr>
<tr id="row30231461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p32829237"><a name="p32829237"></a><a name="p32829237"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p41922513"><a name="p41922513"></a><a name="p41922513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p40280418"><a name="p40280418"></a><a name="p40280418"></a>ACL策略作用的对象类型：</p>
<a name="ul26979450"></a><a name="ul26979450"></a><ul id="ul26979450"><li>IP</li><li>DOMAIN</li><li>ADMIN</li></ul>
</td>
</tr>
<tr id="row5122434"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12264033"><a name="p12264033"></a><a name="p12264033"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4756161164311"><a name="p4756161164311"></a><a name="p4756161164311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14251221184314"><a name="p14251221184314"></a><a name="p14251221184314"></a>生效的环境编号</p>
</td>
</tr>
<tr id="row718813412436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13188163410432"><a name="p13188163410432"></a><a name="p13188163410432"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p518883414319"><a name="p518883414319"></a><a name="p518883414319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p618883411437"><a name="p618883411437"></a><a name="p618883411437"></a>生效的环境名称</p>
</td>
</tr>
<tr id="row17974664417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1879716654420"><a name="p1879716654420"></a><a name="p1879716654420"></a>bind_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p67971163442"><a name="p67971163442"></a><a name="p67971163442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1379756114412"><a name="p1379756114412"></a><a name="p1379756114412"></a>绑定关系编号</p>
</td>
</tr>
<tr id="row1037151810447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6371101813440"><a name="p6371101813440"></a><a name="p6371101813440"></a>bind_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7371101816445"><a name="p7371101816445"></a><a name="p7371101816445"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p123711318104419"><a name="p123711318104419"></a><a name="p123711318104419"></a>绑定时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 1,
  "size": 1,
  "acls": [
    {
      "acl_id": "206bb985d8a04ec09f13c3e51ef77095",
      "acl_name": "acl_001",
      "entity_type": "IP",
      "acl_type": "PERMIT",
      "acl_value": "192.168.1.14,192.168.2.0/24,192.168.1.8-192.168.1.110",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "bind_id": "4ffc0da71ddd4c22add8ff801e19846c",
      "bind_time": "2018-07-27T11:27:10Z"
    }
  ]
}
```

## 状态码<a name="section4173192"></a>

**表 5**  返回消息说明

<a name="table44048907"></a>
<table><thead align="left"><tr id="row38596474"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p39306698"><a name="p39306698"></a><a name="p39306698"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p29725950"><a name="p29725950"></a><a name="p29725950"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row58991743"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p13601844"><a name="p13601844"></a><a name="p13601844"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p28007557"><a name="p28007557"></a><a name="p28007557"></a>OK</p>
</td>
</tr>
<tr id="row50741428"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p16415036"><a name="p16415036"></a><a name="p16415036"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p54549524"><a name="p54549524"></a><a name="p54549524"></a>Bad Request</p>
</td>
</tr>
<tr id="row21183669"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p38155657"><a name="p38155657"></a><a name="p38155657"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p3600513"><a name="p3600513"></a><a name="p3600513"></a>Forbidden</p>
</td>
</tr>
<tr id="row32404622"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p7528760"><a name="p7528760"></a><a name="p7528760"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p5849851"><a name="p5849851"></a><a name="p5849851"></a>Not Found</p>
</td>
</tr>
<tr id="row52648661"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p36683119"><a name="p36683119"></a><a name="p36683119"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p18542645"><a name="p18542645"></a><a name="p18542645"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

