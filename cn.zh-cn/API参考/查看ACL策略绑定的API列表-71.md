# 查看ACL策略绑定的API列表<a name="apig-phapi-180713095"></a>

## 功能介绍<a name="section48108351"></a>

查看ACL策略绑定的API列表。

## URI<a name="section30321983"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table13964245"></a>
<table><thead align="left"><tr id="row5927404"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p10357747"><a name="p10357747"></a><a name="p10357747"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p33671141"><a name="p33671141"></a><a name="p33671141"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row43007916"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p61089200"><a name="p61089200"></a><a name="p61089200"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p49278168"><a name="p49278168"></a><a name="p49278168"></a><span id="ph12755113119449"><a name="ph12755113119449"></a><a name="ph12755113119449"></a>/v1/{project_id}/apigw/instances/{instance_id}</span>/acl-bindings/binded-apis[?page_no、page_size、acl_id、env_id、api_id、api_name、group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：acl\_id、api\_id、 api\_name、group\_id、env\_id、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table10360252"></a>
<table><thead align="left"><tr id="row41405455"><th class="cellrowborder" valign="top" width="15.841584158415841%" id="mcps1.2.5.1.1"><p id="p65507579"><a name="p65507579"></a><a name="p65507579"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="10.891089108910892%" id="mcps1.2.5.1.2"><p id="p4513716"><a name="p4513716"></a><a name="p4513716"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="p30066721"><a name="p30066721"></a><a name="p30066721"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.386138613861384%" id="mcps1.2.5.1.4"><p id="p19485355"><a name="p19485355"></a><a name="p19485355"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16221172692017"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row205056259205"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row34809913"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p1030708"><a name="p1030708"></a><a name="p1030708"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p16378499"><a name="p16378499"></a><a name="p16378499"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p51590031"><a name="p51590031"></a><a name="p51590031"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p1646885914475"><a name="p1646885914475"></a><a name="p1646885914475"></a>ACL策略编号</p>
</td>
</tr>
<tr id="row2484101164812"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p16484161114486"><a name="p16484161114486"></a><a name="p16484161114486"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p144848118484"><a name="p144848118484"></a><a name="p144848118484"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1348431110481"><a name="p1348431110481"></a><a name="p1348431110481"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p1048411117487"><a name="p1048411117487"></a><a name="p1048411117487"></a>API编号</p>
</td>
</tr>
<tr id="row0718514154812"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p127181814134815"><a name="p127181814134815"></a><a name="p127181814134815"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p1271811444814"><a name="p1271811444814"></a><a name="p1271811444814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1718161412482"><a name="p1718161412482"></a><a name="p1718161412482"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p57181914184815"><a name="p57181914184815"></a><a name="p57181914184815"></a>API名称</p>
</td>
</tr>
<tr id="row28168760"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p67077082"><a name="p67077082"></a><a name="p67077082"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p64534548"><a name="p64534548"></a><a name="p64534548"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p59915919"><a name="p59915919"></a><a name="p59915919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p1650420563482"><a name="p1650420563482"></a><a name="p1650420563482"></a>API分组编号</p>
</td>
</tr>
<tr id="row57943819"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p62937758"><a name="p62937758"></a><a name="p62937758"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p64793646"><a name="p64793646"></a><a name="p64793646"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p13793954"><a name="p13793954"></a><a name="p13793954"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p43568483"><a name="p43568483"></a><a name="p43568483"></a>环境编号</p>
</td>
</tr>
<tr id="row56572027"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p18931481"><a name="p18931481"></a><a name="p18931481"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p57055032"><a name="p57055032"></a><a name="p57055032"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p58054912"><a name="p58054912"></a><a name="p58054912"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p4827416"><a name="p4827416"></a><a name="p4827416"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row43446745"><td class="cellrowborder" valign="top" width="15.841584158415841%" headers="mcps1.2.5.1.1 "><p id="p29525485"><a name="p29525485"></a><a name="p29525485"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="10.891089108910892%" headers="mcps1.2.5.1.2 "><p id="p42754085"><a name="p42754085"></a><a name="p42754085"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p40528874"><a name="p40528874"></a><a name="p40528874"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.386138613861384%" headers="mcps1.2.5.1.4 "><p id="p61613347"><a name="p61613347"></a><a name="p61613347"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section4462397"></a>

无

## 响应消息<a name="section25909887"></a>

**表 3**  参数说明

<a name="table32429224"></a>
<table><thead align="left"><tr id="row59168832"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p27946094"><a name="p27946094"></a><a name="p27946094"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p49041181"><a name="p49041181"></a><a name="p49041181"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p12912757"><a name="p12912757"></a><a name="p12912757"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39300381"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29214269"><a name="p29214269"></a><a name="p29214269"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17545598"><a name="p17545598"></a><a name="p17545598"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11907335"><a name="p11907335"></a><a name="p11907335"></a>绑定的API总数</p>
</td>
</tr>
<tr id="row40057159"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p23404432"><a name="p23404432"></a><a name="p23404432"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16710838"><a name="p16710838"></a><a name="p16710838"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p33956381496"><a name="p33956381496"></a><a name="p33956381496"></a>本次查询返回的API数量</p>
</td>
</tr>
<tr id="row35496610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p56653166"><a name="p56653166"></a><a name="p56653166"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p25503730"><a name="p25503730"></a><a name="p25503730"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15692174994918"><a name="p15692174994918"></a><a name="p15692174994918"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table3064469"></a>
<table><thead align="left"><tr id="row17586128"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p15190255"><a name="p15190255"></a><a name="p15190255"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p22451167"><a name="p22451167"></a><a name="p22451167"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p6605256"><a name="p6605256"></a><a name="p6605256"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row65263697"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51868066"><a name="p51868066"></a><a name="p51868066"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p40563812"><a name="p40563812"></a><a name="p40563812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1453935013506"><a name="p1453935013506"></a><a name="p1453935013506"></a>API编号</p>
</td>
</tr>
<tr id="row43119028"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20789256105012"><a name="p20789256105012"></a><a name="p20789256105012"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p40085061"><a name="p40085061"></a><a name="p40085061"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p25664504"><a name="p25664504"></a><a name="p25664504"></a>API名称</p>
</td>
</tr>
<tr id="row29653949"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53159658"><a name="p53159658"></a><a name="p53159658"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10965023"><a name="p10965023"></a><a name="p10965023"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p35541923185110"><a name="p35541923185110"></a><a name="p35541923185110"></a>API分组名称</p>
</td>
</tr>
<tr id="row7547442"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7363043"><a name="p7363043"></a><a name="p7363043"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1191319458510"><a name="p1191319458510"></a><a name="p1191319458510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11585105035114"><a name="p11585105035114"></a><a name="p11585105035114"></a>API类型</p>
</td>
</tr>
<tr id="row49156898"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p956911568513"><a name="p956911568513"></a><a name="p956911568513"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p60317603"><a name="p60317603"></a><a name="p60317603"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p92258595214"><a name="p92258595214"></a><a name="p92258595214"></a>API的描述信息</p>
</td>
</tr>
<tr id="row06631111185215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12663111113524"><a name="p12663111113524"></a><a name="p12663111113524"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p196631311125212"><a name="p196631311125212"></a><a name="p196631311125212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4663191125213"><a name="p4663191125213"></a><a name="p4663191125213"></a>生效的环境编号</p>
</td>
</tr>
<tr id="row116261023115215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1762652365210"><a name="p1762652365210"></a><a name="p1762652365210"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1962632335216"><a name="p1962632335216"></a><a name="p1962632335216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2062619238522"><a name="p2062619238522"></a><a name="p2062619238522"></a>生效的环境名称</p>
</td>
</tr>
<tr id="row142059343525"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p720503415521"><a name="p720503415521"></a><a name="p720503415521"></a>bind_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p172051834165217"><a name="p172051834165217"></a><a name="p172051834165217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p120563414529"><a name="p120563414529"></a><a name="p120563414529"></a>绑定关系编号</p>
</td>
</tr>
<tr id="row1781494885219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p138141648125212"><a name="p138141648125212"></a><a name="p138141648125212"></a>bind_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14814184816526"><a name="p14814184816526"></a><a name="p14814184816526"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8814124825211"><a name="p8814124825211"></a><a name="p8814124825211"></a>绑定时间</p>
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
      "bind_time": "2018-07-27T11:27:10Z"
    }
  ]
}
```

## 状态码<a name="section40161578"></a>

**表 5**  返回消息说明

<a name="table48484883"></a>
<table><thead align="left"><tr id="row52625885"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p34838322"><a name="p34838322"></a><a name="p34838322"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p3331856"><a name="p3331856"></a><a name="p3331856"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1444894"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p49927556"><a name="p49927556"></a><a name="p49927556"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p17600235"><a name="p17600235"></a><a name="p17600235"></a>OK</p>
</td>
</tr>
<tr id="row24184390"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p12778577"><a name="p12778577"></a><a name="p12778577"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p28431792"><a name="p28431792"></a><a name="p28431792"></a>Bad Request</p>
</td>
</tr>
<tr id="row54559539"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p57246508"><a name="p57246508"></a><a name="p57246508"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6455533"><a name="p6455533"></a><a name="p6455533"></a>Forbidden</p>
</td>
</tr>
<tr id="row58099800"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p8463385"><a name="p8463385"></a><a name="p8463385"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14445623"><a name="p14445623"></a><a name="p14445623"></a>Not Found</p>
</td>
</tr>
<tr id="row62901748"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p61876840"><a name="p61876840"></a><a name="p61876840"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

