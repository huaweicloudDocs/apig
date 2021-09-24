# 查看ACL策略绑定的API列表<a name="ZH-CN_TOPIC_0000001082221209"></a>

## 功能介绍<a name="zh-cn_topic_0118924507_section48108351"></a>

查看ACL策略绑定的API列表。

## URI<a name="zh-cn_topic_0118924507_section30321983"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924507_table13964245"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924507_row5927404"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924507_p10357747"><a name="zh-cn_topic_0118924507_p10357747"></a><a name="zh-cn_topic_0118924507_p10357747"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924507_p33671141"><a name="zh-cn_topic_0118924507_p33671141"></a><a name="zh-cn_topic_0118924507_p33671141"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924507_row43007916"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924507_p61089200"><a name="zh-cn_topic_0118924507_p61089200"></a><a name="zh-cn_topic_0118924507_p61089200"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924507_p49278168"><a name="zh-cn_topic_0118924507_p49278168"></a><a name="zh-cn_topic_0118924507_p49278168"></a>/v1.0/apigw/acl-bindings/binded-apis[?page_no、page_size、acl_id、env_id、api_id、api_name、group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：acl\_id、api\_id、 api\_name、group\_id、env\_id、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924507_table10360252"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924507_row41405455"><th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924507_p65507579"><a name="zh-cn_topic_0118924507_p65507579"></a><a name="zh-cn_topic_0118924507_p65507579"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.891089108910892%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924507_p4513716"><a name="zh-cn_topic_0118924507_p4513716"></a><a name="zh-cn_topic_0118924507_p4513716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924507_p30066721"><a name="zh-cn_topic_0118924507_p30066721"></a><a name="zh-cn_topic_0118924507_p30066721"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.386138613861384%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924507_p19485355"><a name="zh-cn_topic_0118924507_p19485355"></a><a name="zh-cn_topic_0118924507_p19485355"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924507_row34809913"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924507_p1030708"><a name="zh-cn_topic_0118924507_p1030708"></a><a name="zh-cn_topic_0118924507_p1030708"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924507_p16378499"><a name="zh-cn_topic_0118924507_p16378499"></a><a name="zh-cn_topic_0118924507_p16378499"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924507_p51590031"><a name="zh-cn_topic_0118924507_p51590031"></a><a name="zh-cn_topic_0118924507_p51590031"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924507_p1646885914475"><a name="zh-cn_topic_0118924507_p1646885914475"></a><a name="zh-cn_topic_0118924507_p1646885914475"></a>ACL策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row2484101164812"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924507_p16484161114486"><a name="zh-cn_topic_0118924507_p16484161114486"></a><a name="zh-cn_topic_0118924507_p16484161114486"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924507_p144848118484"><a name="zh-cn_topic_0118924507_p144848118484"></a><a name="zh-cn_topic_0118924507_p144848118484"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924507_p1348431110481"><a name="zh-cn_topic_0118924507_p1348431110481"></a><a name="zh-cn_topic_0118924507_p1348431110481"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924507_p1048411117487"><a name="zh-cn_topic_0118924507_p1048411117487"></a><a name="zh-cn_topic_0118924507_p1048411117487"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row0718514154812"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924507_p127181814134815"><a name="zh-cn_topic_0118924507_p127181814134815"></a><a name="zh-cn_topic_0118924507_p127181814134815"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924507_p1271811444814"><a name="zh-cn_topic_0118924507_p1271811444814"></a><a name="zh-cn_topic_0118924507_p1271811444814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924507_p1718161412482"><a name="zh-cn_topic_0118924507_p1718161412482"></a><a name="zh-cn_topic_0118924507_p1718161412482"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924507_p57181914184815"><a name="zh-cn_topic_0118924507_p57181914184815"></a><a name="zh-cn_topic_0118924507_p57181914184815"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row28168760"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924507_p67077082"><a name="zh-cn_topic_0118924507_p67077082"></a><a name="zh-cn_topic_0118924507_p67077082"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924507_p64534548"><a name="zh-cn_topic_0118924507_p64534548"></a><a name="zh-cn_topic_0118924507_p64534548"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924507_p59915919"><a name="zh-cn_topic_0118924507_p59915919"></a><a name="zh-cn_topic_0118924507_p59915919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924507_p1650420563482"><a name="zh-cn_topic_0118924507_p1650420563482"></a><a name="zh-cn_topic_0118924507_p1650420563482"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row57943819"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924507_p62937758"><a name="zh-cn_topic_0118924507_p62937758"></a><a name="zh-cn_topic_0118924507_p62937758"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924507_p64793646"><a name="zh-cn_topic_0118924507_p64793646"></a><a name="zh-cn_topic_0118924507_p64793646"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924507_p13793954"><a name="zh-cn_topic_0118924507_p13793954"></a><a name="zh-cn_topic_0118924507_p13793954"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924507_p43568483"><a name="zh-cn_topic_0118924507_p43568483"></a><a name="zh-cn_topic_0118924507_p43568483"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row56572027"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924507_p18931481"><a name="zh-cn_topic_0118924507_p18931481"></a><a name="zh-cn_topic_0118924507_p18931481"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924507_p57055032"><a name="zh-cn_topic_0118924507_p57055032"></a><a name="zh-cn_topic_0118924507_p57055032"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924507_p58054912"><a name="zh-cn_topic_0118924507_p58054912"></a><a name="zh-cn_topic_0118924507_p58054912"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924507_p4827416"><a name="zh-cn_topic_0118924507_p4827416"></a><a name="zh-cn_topic_0118924507_p4827416"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row43446745"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924507_p29525485"><a name="zh-cn_topic_0118924507_p29525485"></a><a name="zh-cn_topic_0118924507_p29525485"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924507_p42754085"><a name="zh-cn_topic_0118924507_p42754085"></a><a name="zh-cn_topic_0118924507_p42754085"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924507_p40528874"><a name="zh-cn_topic_0118924507_p40528874"></a><a name="zh-cn_topic_0118924507_p40528874"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924507_p61613347"><a name="zh-cn_topic_0118924507_p61613347"></a><a name="zh-cn_topic_0118924507_p61613347"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924507_section4462397"></a>

无

## 响应消息<a name="zh-cn_topic_0118924507_section25909887"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924507_table32429224"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924507_row59168832"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924507_p27946094"><a name="zh-cn_topic_0118924507_p27946094"></a><a name="zh-cn_topic_0118924507_p27946094"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924507_p49041181"><a name="zh-cn_topic_0118924507_p49041181"></a><a name="zh-cn_topic_0118924507_p49041181"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924507_p12912757"><a name="zh-cn_topic_0118924507_p12912757"></a><a name="zh-cn_topic_0118924507_p12912757"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924507_row39300381"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p29214269"><a name="zh-cn_topic_0118924507_p29214269"></a><a name="zh-cn_topic_0118924507_p29214269"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p17545598"><a name="zh-cn_topic_0118924507_p17545598"></a><a name="zh-cn_topic_0118924507_p17545598"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p11907335"><a name="zh-cn_topic_0118924507_p11907335"></a><a name="zh-cn_topic_0118924507_p11907335"></a>绑定的API总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row40057159"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p23404432"><a name="zh-cn_topic_0118924507_p23404432"></a><a name="zh-cn_topic_0118924507_p23404432"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p16710838"><a name="zh-cn_topic_0118924507_p16710838"></a><a name="zh-cn_topic_0118924507_p16710838"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p33956381496"><a name="zh-cn_topic_0118924507_p33956381496"></a><a name="zh-cn_topic_0118924507_p33956381496"></a>本次查询返回的API数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row35496610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p56653166"><a name="zh-cn_topic_0118924507_p56653166"></a><a name="zh-cn_topic_0118924507_p56653166"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p25503730"><a name="zh-cn_topic_0118924507_p25503730"></a><a name="zh-cn_topic_0118924507_p25503730"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p15692174994918"><a name="zh-cn_topic_0118924507_p15692174994918"></a><a name="zh-cn_topic_0118924507_p15692174994918"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="zh-cn_topic_0118924507_table3064469"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924507_row17586128"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924507_p15190255"><a name="zh-cn_topic_0118924507_p15190255"></a><a name="zh-cn_topic_0118924507_p15190255"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924507_p22451167"><a name="zh-cn_topic_0118924507_p22451167"></a><a name="zh-cn_topic_0118924507_p22451167"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924507_p6605256"><a name="zh-cn_topic_0118924507_p6605256"></a><a name="zh-cn_topic_0118924507_p6605256"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924507_row65263697"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p51868066"><a name="zh-cn_topic_0118924507_p51868066"></a><a name="zh-cn_topic_0118924507_p51868066"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p40563812"><a name="zh-cn_topic_0118924507_p40563812"></a><a name="zh-cn_topic_0118924507_p40563812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p1453935013506"><a name="zh-cn_topic_0118924507_p1453935013506"></a><a name="zh-cn_topic_0118924507_p1453935013506"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row43119028"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p20789256105012"><a name="zh-cn_topic_0118924507_p20789256105012"></a><a name="zh-cn_topic_0118924507_p20789256105012"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p40085061"><a name="zh-cn_topic_0118924507_p40085061"></a><a name="zh-cn_topic_0118924507_p40085061"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p25664504"><a name="zh-cn_topic_0118924507_p25664504"></a><a name="zh-cn_topic_0118924507_p25664504"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row29653949"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p53159658"><a name="zh-cn_topic_0118924507_p53159658"></a><a name="zh-cn_topic_0118924507_p53159658"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p10965023"><a name="zh-cn_topic_0118924507_p10965023"></a><a name="zh-cn_topic_0118924507_p10965023"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p35541923185110"><a name="zh-cn_topic_0118924507_p35541923185110"></a><a name="zh-cn_topic_0118924507_p35541923185110"></a>API分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row7547442"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p7363043"><a name="zh-cn_topic_0118924507_p7363043"></a><a name="zh-cn_topic_0118924507_p7363043"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p1191319458510"><a name="zh-cn_topic_0118924507_p1191319458510"></a><a name="zh-cn_topic_0118924507_p1191319458510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p11585105035114"><a name="zh-cn_topic_0118924507_p11585105035114"></a><a name="zh-cn_topic_0118924507_p11585105035114"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row49156898"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p956911568513"><a name="zh-cn_topic_0118924507_p956911568513"></a><a name="zh-cn_topic_0118924507_p956911568513"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p60317603"><a name="zh-cn_topic_0118924507_p60317603"></a><a name="zh-cn_topic_0118924507_p60317603"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p92258595214"><a name="zh-cn_topic_0118924507_p92258595214"></a><a name="zh-cn_topic_0118924507_p92258595214"></a>API的描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row06631111185215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p12663111113524"><a name="zh-cn_topic_0118924507_p12663111113524"></a><a name="zh-cn_topic_0118924507_p12663111113524"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p196631311125212"><a name="zh-cn_topic_0118924507_p196631311125212"></a><a name="zh-cn_topic_0118924507_p196631311125212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p4663191125213"><a name="zh-cn_topic_0118924507_p4663191125213"></a><a name="zh-cn_topic_0118924507_p4663191125213"></a>生效的环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row116261023115215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p1762652365210"><a name="zh-cn_topic_0118924507_p1762652365210"></a><a name="zh-cn_topic_0118924507_p1762652365210"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p1962632335216"><a name="zh-cn_topic_0118924507_p1962632335216"></a><a name="zh-cn_topic_0118924507_p1962632335216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p2062619238522"><a name="zh-cn_topic_0118924507_p2062619238522"></a><a name="zh-cn_topic_0118924507_p2062619238522"></a>生效的环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row142059343525"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p720503415521"><a name="zh-cn_topic_0118924507_p720503415521"></a><a name="zh-cn_topic_0118924507_p720503415521"></a>bind_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p172051834165217"><a name="zh-cn_topic_0118924507_p172051834165217"></a><a name="zh-cn_topic_0118924507_p172051834165217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p120563414529"><a name="zh-cn_topic_0118924507_p120563414529"></a><a name="zh-cn_topic_0118924507_p120563414529"></a>绑定关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row1781494885219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p138141648125212"><a name="zh-cn_topic_0118924507_p138141648125212"></a><a name="zh-cn_topic_0118924507_p138141648125212"></a>bind_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p14814184816526"><a name="zh-cn_topic_0118924507_p14814184816526"></a><a name="zh-cn_topic_0118924507_p14814184816526"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p8814124825211"><a name="zh-cn_topic_0118924507_p8814124825211"></a><a name="zh-cn_topic_0118924507_p8814124825211"></a>绑定时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row7463144019362"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924507_p15348153673314"><a name="zh-cn_topic_0118924507_p15348153673314"></a><a name="zh-cn_topic_0118924507_p15348153673314"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924507_p18348143623317"><a name="zh-cn_topic_0118924507_p18348143623317"></a><a name="zh-cn_topic_0118924507_p18348143623317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924507_p10348436123312"><a name="zh-cn_topic_0118924507_p10348436123312"></a><a name="zh-cn_topic_0118924507_p10348436123312"></a>API发布记录编号</p>
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
      "api_id": "aebacac6095942b4b2dd2b209bb7b9bc",
      "api_name": "aaa",
      "group_name": "test001",
      "api_type": 1,
      "api_remark": "aaa",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "bind_id": "4ffc0da71ddd4c22add8ff801e19846c",
      "bind_time": "2018-07-27T11:27:10Z",
      "publish_id": "1bc8b2b741a04bd4af3ef9d7cd003104"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0118924507_section40161578"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924507_table48484883"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924507_row52625885"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924507_p34838322"><a name="zh-cn_topic_0118924507_p34838322"></a><a name="zh-cn_topic_0118924507_p34838322"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924507_p3331856"><a name="zh-cn_topic_0118924507_p3331856"></a><a name="zh-cn_topic_0118924507_p3331856"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924507_row1444894"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924507_p49927556"><a name="zh-cn_topic_0118924507_p49927556"></a><a name="zh-cn_topic_0118924507_p49927556"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924507_p17600235"><a name="zh-cn_topic_0118924507_p17600235"></a><a name="zh-cn_topic_0118924507_p17600235"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row24184390"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924507_p12778577"><a name="zh-cn_topic_0118924507_p12778577"></a><a name="zh-cn_topic_0118924507_p12778577"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924507_p28431792"><a name="zh-cn_topic_0118924507_p28431792"></a><a name="zh-cn_topic_0118924507_p28431792"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row54559539"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924507_p57246508"><a name="zh-cn_topic_0118924507_p57246508"></a><a name="zh-cn_topic_0118924507_p57246508"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924507_p6455533"><a name="zh-cn_topic_0118924507_p6455533"></a><a name="zh-cn_topic_0118924507_p6455533"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row58099800"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924507_p8463385"><a name="zh-cn_topic_0118924507_p8463385"></a><a name="zh-cn_topic_0118924507_p8463385"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924507_p14445623"><a name="zh-cn_topic_0118924507_p14445623"></a><a name="zh-cn_topic_0118924507_p14445623"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924507_row62901748"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924507_p61876840"><a name="zh-cn_topic_0118924507_p61876840"></a><a name="zh-cn_topic_0118924507_p61876840"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924507_p6744143"><a name="zh-cn_topic_0118924507_p6744143"></a><a name="zh-cn_topic_0118924507_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

