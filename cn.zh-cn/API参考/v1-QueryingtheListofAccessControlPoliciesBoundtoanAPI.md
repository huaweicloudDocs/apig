# 查看API绑定的ACL策略列表<a name="ZH-CN_TOPIC_0000001082221285"></a>

## 功能介绍<a name="zh-cn_topic_0225568894_section30108054"></a>

查看API绑定的ACL策略列表。

## URI<a name="zh-cn_topic_0225568894_section2537034"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568894_table49976511"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568894_row26320038"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568894_p51548346"><a name="zh-cn_topic_0225568894_p51548346"></a><a name="zh-cn_topic_0225568894_p51548346"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568894_p14666461"><a name="zh-cn_topic_0225568894_p14666461"></a><a name="zh-cn_topic_0225568894_p14666461"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568894_row47132730"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568894_p59654775"><a name="zh-cn_topic_0225568894_p59654775"></a><a name="zh-cn_topic_0225568894_p59654775"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568894_p198588"><a name="zh-cn_topic_0225568894_p198588"></a><a name="zh-cn_topic_0225568894_p198588"></a>/v1/{project_id}/apigw/instances/{instance_id}/acl-bindings/binded-acls[?page_no,page_size,api_id,env_id,env_name,acl_id,acl_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：api\_id、env\_id、env\_name、acl\_id、acl\_name、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568894_table43029199"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568894_row45836208"><th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568894_p21745369"><a name="zh-cn_topic_0225568894_p21745369"></a><a name="zh-cn_topic_0225568894_p21745369"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.891089108910892%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568894_p16544499"><a name="zh-cn_topic_0225568894_p16544499"></a><a name="zh-cn_topic_0225568894_p16544499"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568894_p65036070"><a name="zh-cn_topic_0225568894_p65036070"></a><a name="zh-cn_topic_0225568894_p65036070"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="62.37623762376238%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568894_p33430297"><a name="zh-cn_topic_0225568894_p33430297"></a><a name="zh-cn_topic_0225568894_p33430297"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568894_row218810113201"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p55878963"><a name="zh-cn_topic_0225568894_p55878963"></a><a name="zh-cn_topic_0225568894_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p29902160"><a name="zh-cn_topic_0225568894_p29902160"></a><a name="zh-cn_topic_0225568894_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p6155914"><a name="zh-cn_topic_0225568894_p6155914"></a><a name="zh-cn_topic_0225568894_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p28867016"><a name="zh-cn_topic_0225568894_p28867016"></a><a name="zh-cn_topic_0225568894_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row655213103206"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p1780913159538"><a name="zh-cn_topic_0225568894_p1780913159538"></a><a name="zh-cn_topic_0225568894_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p9809215115310"><a name="zh-cn_topic_0225568894_p9809215115310"></a><a name="zh-cn_topic_0225568894_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p1280914152538"><a name="zh-cn_topic_0225568894_p1280914152538"></a><a name="zh-cn_topic_0225568894_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p1880914157537"><a name="zh-cn_topic_0225568894_p1880914157537"></a><a name="zh-cn_topic_0225568894_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row23499508"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p24412000"><a name="zh-cn_topic_0225568894_p24412000"></a><a name="zh-cn_topic_0225568894_p24412000"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p31214980"><a name="zh-cn_topic_0225568894_p31214980"></a><a name="zh-cn_topic_0225568894_p31214980"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p45385481"><a name="zh-cn_topic_0225568894_p45385481"></a><a name="zh-cn_topic_0225568894_p45385481"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p10285592386"><a name="zh-cn_topic_0225568894_p10285592386"></a><a name="zh-cn_topic_0225568894_p10285592386"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row8153146123920"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p1815376143911"><a name="zh-cn_topic_0225568894_p1815376143911"></a><a name="zh-cn_topic_0225568894_p1815376143911"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p663174018395"><a name="zh-cn_topic_0225568894_p663174018395"></a><a name="zh-cn_topic_0225568894_p663174018395"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p191531693911"><a name="zh-cn_topic_0225568894_p191531693911"></a><a name="zh-cn_topic_0225568894_p191531693911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p9153136133912"><a name="zh-cn_topic_0225568894_p9153136133912"></a><a name="zh-cn_topic_0225568894_p9153136133912"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row135689703917"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p456820713391"><a name="zh-cn_topic_0225568894_p456820713391"></a><a name="zh-cn_topic_0225568894_p456820713391"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p155683793917"><a name="zh-cn_topic_0225568894_p155683793917"></a><a name="zh-cn_topic_0225568894_p155683793917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p3568677398"><a name="zh-cn_topic_0225568894_p3568677398"></a><a name="zh-cn_topic_0225568894_p3568677398"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p1756817103915"><a name="zh-cn_topic_0225568894_p1756817103915"></a><a name="zh-cn_topic_0225568894_p1756817103915"></a>环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row12818171110390"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p14818121114395"><a name="zh-cn_topic_0225568894_p14818121114395"></a><a name="zh-cn_topic_0225568894_p14818121114395"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p1781851114392"><a name="zh-cn_topic_0225568894_p1781851114392"></a><a name="zh-cn_topic_0225568894_p1781851114392"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p1581801119394"><a name="zh-cn_topic_0225568894_p1581801119394"></a><a name="zh-cn_topic_0225568894_p1581801119394"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p138183119399"><a name="zh-cn_topic_0225568894_p138183119399"></a><a name="zh-cn_topic_0225568894_p138183119399"></a>ACL策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row1885014156393"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p5850815103913"><a name="zh-cn_topic_0225568894_p5850815103913"></a><a name="zh-cn_topic_0225568894_p5850815103913"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p1885031520392"><a name="zh-cn_topic_0225568894_p1885031520392"></a><a name="zh-cn_topic_0225568894_p1885031520392"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p38501215163918"><a name="zh-cn_topic_0225568894_p38501215163918"></a><a name="zh-cn_topic_0225568894_p38501215163918"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p10850101517392"><a name="zh-cn_topic_0225568894_p10850101517392"></a><a name="zh-cn_topic_0225568894_p10850101517392"></a>ACL策略名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row1346256"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p41937917"><a name="zh-cn_topic_0225568894_p41937917"></a><a name="zh-cn_topic_0225568894_p41937917"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p41528135"><a name="zh-cn_topic_0225568894_p41528135"></a><a name="zh-cn_topic_0225568894_p41528135"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p8335765"><a name="zh-cn_topic_0225568894_p8335765"></a><a name="zh-cn_topic_0225568894_p8335765"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p4108368"><a name="zh-cn_topic_0225568894_p4108368"></a><a name="zh-cn_topic_0225568894_p4108368"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row36975313"><td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568894_p42210394"><a name="zh-cn_topic_0225568894_p42210394"></a><a name="zh-cn_topic_0225568894_p42210394"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568894_p63598723"><a name="zh-cn_topic_0225568894_p63598723"></a><a name="zh-cn_topic_0225568894_p63598723"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568894_p51222900"><a name="zh-cn_topic_0225568894_p51222900"></a><a name="zh-cn_topic_0225568894_p51222900"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="62.37623762376238%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568894_p55414230"><a name="zh-cn_topic_0225568894_p55414230"></a><a name="zh-cn_topic_0225568894_p55414230"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568894_section22833309"></a>

无

## 响应消息<a name="zh-cn_topic_0225568894_section37558732"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568894_table25559313"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568894_row3221530"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568894_p59617344"><a name="zh-cn_topic_0225568894_p59617344"></a><a name="zh-cn_topic_0225568894_p59617344"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568894_p64275559"><a name="zh-cn_topic_0225568894_p64275559"></a><a name="zh-cn_topic_0225568894_p64275559"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568894_p38937782"><a name="zh-cn_topic_0225568894_p38937782"></a><a name="zh-cn_topic_0225568894_p38937782"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568894_row66952662"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p54456559"><a name="zh-cn_topic_0225568894_p54456559"></a><a name="zh-cn_topic_0225568894_p54456559"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p48905128"><a name="zh-cn_topic_0225568894_p48905128"></a><a name="zh-cn_topic_0225568894_p48905128"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p1892393"><a name="zh-cn_topic_0225568894_p1892393"></a><a name="zh-cn_topic_0225568894_p1892393"></a>绑定的ACL总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row17031540"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p37377525"><a name="zh-cn_topic_0225568894_p37377525"></a><a name="zh-cn_topic_0225568894_p37377525"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p7680723"><a name="zh-cn_topic_0225568894_p7680723"></a><a name="zh-cn_topic_0225568894_p7680723"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p86659249416"><a name="zh-cn_topic_0225568894_p86659249416"></a><a name="zh-cn_topic_0225568894_p86659249416"></a>本次查询返回的ACL数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row29211812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p17346535"><a name="zh-cn_topic_0225568894_p17346535"></a><a name="zh-cn_topic_0225568894_p17346535"></a>acls</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p62892132"><a name="zh-cn_topic_0225568894_p62892132"></a><a name="zh-cn_topic_0225568894_p62892132"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p178717349415"><a name="zh-cn_topic_0225568894_p178717349415"></a><a name="zh-cn_topic_0225568894_p178717349415"></a>本次查询返回的ACL列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  acls参数说明

<a name="zh-cn_topic_0225568894_table13010379"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568894_row3739801"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568894_p34488497"><a name="zh-cn_topic_0225568894_p34488497"></a><a name="zh-cn_topic_0225568894_p34488497"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568894_p42104857"><a name="zh-cn_topic_0225568894_p42104857"></a><a name="zh-cn_topic_0225568894_p42104857"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568894_p55050233"><a name="zh-cn_topic_0225568894_p55050233"></a><a name="zh-cn_topic_0225568894_p55050233"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568894_row29883898"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p4676675"><a name="zh-cn_topic_0225568894_p4676675"></a><a name="zh-cn_topic_0225568894_p4676675"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p43266429"><a name="zh-cn_topic_0225568894_p43266429"></a><a name="zh-cn_topic_0225568894_p43266429"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p530655114215"><a name="zh-cn_topic_0225568894_p530655114215"></a><a name="zh-cn_topic_0225568894_p530655114215"></a>ACL策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row61266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p4962556"><a name="zh-cn_topic_0225568894_p4962556"></a><a name="zh-cn_topic_0225568894_p4962556"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p66422738"><a name="zh-cn_topic_0225568894_p66422738"></a><a name="zh-cn_topic_0225568894_p66422738"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p11532734"><a name="zh-cn_topic_0225568894_p11532734"></a><a name="zh-cn_topic_0225568894_p11532734"></a>ACL策略名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row36685742"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p18755155"><a name="zh-cn_topic_0225568894_p18755155"></a><a name="zh-cn_topic_0225568894_p18755155"></a>acl_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p42772609"><a name="zh-cn_topic_0225568894_p42772609"></a><a name="zh-cn_topic_0225568894_p42772609"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p42029279"><a name="zh-cn_topic_0225568894_p42029279"></a><a name="zh-cn_topic_0225568894_p42029279"></a>ACL策略类型</p>
<a name="zh-cn_topic_0225568894_ul42719191"></a><a name="zh-cn_topic_0225568894_ul42719191"></a><ul id="zh-cn_topic_0225568894_ul42719191"><li>PERMIT  (白名单类型)</li><li>DENY     (黑名单类型)</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row3777868"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p37571883"><a name="zh-cn_topic_0225568894_p37571883"></a><a name="zh-cn_topic_0225568894_p37571883"></a>acl_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p23423707"><a name="zh-cn_topic_0225568894_p23423707"></a><a name="zh-cn_topic_0225568894_p23423707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p199592391421"><a name="zh-cn_topic_0225568894_p199592391421"></a><a name="zh-cn_topic_0225568894_p199592391421"></a>ACL策略值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row30231461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p32829237"><a name="zh-cn_topic_0225568894_p32829237"></a><a name="zh-cn_topic_0225568894_p32829237"></a>entity_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p41922513"><a name="zh-cn_topic_0225568894_p41922513"></a><a name="zh-cn_topic_0225568894_p41922513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p40280418"><a name="zh-cn_topic_0225568894_p40280418"></a><a name="zh-cn_topic_0225568894_p40280418"></a>ACL策略作用的对象类型：</p>
<a name="zh-cn_topic_0225568894_ul26979450"></a><a name="zh-cn_topic_0225568894_ul26979450"></a><ul id="zh-cn_topic_0225568894_ul26979450"><li>IP</li><li>DOMAIN</li><li>ADMIN</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row5122434"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p12264033"><a name="zh-cn_topic_0225568894_p12264033"></a><a name="zh-cn_topic_0225568894_p12264033"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p4756161164311"><a name="zh-cn_topic_0225568894_p4756161164311"></a><a name="zh-cn_topic_0225568894_p4756161164311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p14251221184314"><a name="zh-cn_topic_0225568894_p14251221184314"></a><a name="zh-cn_topic_0225568894_p14251221184314"></a>生效的环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row718813412436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p13188163410432"><a name="zh-cn_topic_0225568894_p13188163410432"></a><a name="zh-cn_topic_0225568894_p13188163410432"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p518883414319"><a name="zh-cn_topic_0225568894_p518883414319"></a><a name="zh-cn_topic_0225568894_p518883414319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p618883411437"><a name="zh-cn_topic_0225568894_p618883411437"></a><a name="zh-cn_topic_0225568894_p618883411437"></a>生效的环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row17974664417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p1879716654420"><a name="zh-cn_topic_0225568894_p1879716654420"></a><a name="zh-cn_topic_0225568894_p1879716654420"></a>bind_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p67971163442"><a name="zh-cn_topic_0225568894_p67971163442"></a><a name="zh-cn_topic_0225568894_p67971163442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p1379756114412"><a name="zh-cn_topic_0225568894_p1379756114412"></a><a name="zh-cn_topic_0225568894_p1379756114412"></a>绑定关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row1037151810447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568894_p6371101813440"><a name="zh-cn_topic_0225568894_p6371101813440"></a><a name="zh-cn_topic_0225568894_p6371101813440"></a>bind_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568894_p7371101816445"><a name="zh-cn_topic_0225568894_p7371101816445"></a><a name="zh-cn_topic_0225568894_p7371101816445"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568894_p123711318104419"><a name="zh-cn_topic_0225568894_p123711318104419"></a><a name="zh-cn_topic_0225568894_p123711318104419"></a>绑定时间</p>
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

## 状态码<a name="zh-cn_topic_0225568894_section4173192"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568894_table44048907"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568894_row38596474"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568894_p39306698"><a name="zh-cn_topic_0225568894_p39306698"></a><a name="zh-cn_topic_0225568894_p39306698"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568894_p29725950"><a name="zh-cn_topic_0225568894_p29725950"></a><a name="zh-cn_topic_0225568894_p29725950"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568894_row58991743"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568894_p13601844"><a name="zh-cn_topic_0225568894_p13601844"></a><a name="zh-cn_topic_0225568894_p13601844"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568894_p28007557"><a name="zh-cn_topic_0225568894_p28007557"></a><a name="zh-cn_topic_0225568894_p28007557"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row50741428"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568894_p16415036"><a name="zh-cn_topic_0225568894_p16415036"></a><a name="zh-cn_topic_0225568894_p16415036"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568894_p54549524"><a name="zh-cn_topic_0225568894_p54549524"></a><a name="zh-cn_topic_0225568894_p54549524"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row21183669"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568894_p38155657"><a name="zh-cn_topic_0225568894_p38155657"></a><a name="zh-cn_topic_0225568894_p38155657"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568894_p3600513"><a name="zh-cn_topic_0225568894_p3600513"></a><a name="zh-cn_topic_0225568894_p3600513"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row32404622"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568894_p7528760"><a name="zh-cn_topic_0225568894_p7528760"></a><a name="zh-cn_topic_0225568894_p7528760"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568894_p5849851"><a name="zh-cn_topic_0225568894_p5849851"></a><a name="zh-cn_topic_0225568894_p5849851"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568894_row52648661"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568894_p36683119"><a name="zh-cn_topic_0225568894_p36683119"></a><a name="zh-cn_topic_0225568894_p36683119"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568894_p18542645"><a name="zh-cn_topic_0225568894_p18542645"></a><a name="zh-cn_topic_0225568894_p18542645"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

