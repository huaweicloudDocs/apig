# 查看API已绑定的APP列表<a name="ZH-CN_TOPIC_0000001082135177"></a>

## 功能介绍<a name="zh-cn_topic_0225568845_section60304671"></a>

查询API绑定的APP列表。

## URI<a name="zh-cn_topic_0225568845_section5871134"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568845_table3327925"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568845_row9195991"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568845_p6677806"><a name="zh-cn_topic_0225568845_p6677806"></a><a name="zh-cn_topic_0225568845_p6677806"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568845_p4031405"><a name="zh-cn_topic_0225568845_p4031405"></a><a name="zh-cn_topic_0225568845_p4031405"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568845_row58108413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568845_p9161030"><a name="zh-cn_topic_0225568845_p9161030"></a><a name="zh-cn_topic_0225568845_p9161030"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568845_p3845935"><a name="zh-cn_topic_0225568845_p3845935"></a><a name="zh-cn_topic_0225568845_p3845935"></a>/v1/{project_id}/apigw/instances/{instance_id}/app-auths/binded-apps[?page_size, page_no, api_id, app_name, app_id, env_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：api\_id、app\_name、app\_id、env\_id、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568845_table19989692"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568845_row1031739"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568845_p16462024"><a name="zh-cn_topic_0225568845_p16462024"></a><a name="zh-cn_topic_0225568845_p16462024"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568845_p58355549"><a name="zh-cn_topic_0225568845_p58355549"></a><a name="zh-cn_topic_0225568845_p58355549"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568845_p29179043"><a name="zh-cn_topic_0225568845_p29179043"></a><a name="zh-cn_topic_0225568845_p29179043"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568845_p14692289"><a name="zh-cn_topic_0225568845_p14692289"></a><a name="zh-cn_topic_0225568845_p14692289"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568845_row0480125664618"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p55878963"><a name="zh-cn_topic_0225568845_p55878963"></a><a name="zh-cn_topic_0225568845_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p29902160"><a name="zh-cn_topic_0225568845_p29902160"></a><a name="zh-cn_topic_0225568845_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p6155914"><a name="zh-cn_topic_0225568845_p6155914"></a><a name="zh-cn_topic_0225568845_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p28867016"><a name="zh-cn_topic_0225568845_p28867016"></a><a name="zh-cn_topic_0225568845_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row32861856174611"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p1780913159538"><a name="zh-cn_topic_0225568845_p1780913159538"></a><a name="zh-cn_topic_0225568845_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p9809215115310"><a name="zh-cn_topic_0225568845_p9809215115310"></a><a name="zh-cn_topic_0225568845_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p1280914152538"><a name="zh-cn_topic_0225568845_p1280914152538"></a><a name="zh-cn_topic_0225568845_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p1880914157537"><a name="zh-cn_topic_0225568845_p1880914157537"></a><a name="zh-cn_topic_0225568845_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row49224800"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p27785896"><a name="zh-cn_topic_0225568845_p27785896"></a><a name="zh-cn_topic_0225568845_p27785896"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p36065088"><a name="zh-cn_topic_0225568845_p36065088"></a><a name="zh-cn_topic_0225568845_p36065088"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p35590992"><a name="zh-cn_topic_0225568845_p35590992"></a><a name="zh-cn_topic_0225568845_p35590992"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p64298113"><a name="zh-cn_topic_0225568845_p64298113"></a><a name="zh-cn_topic_0225568845_p64298113"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row41812109"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p31337682"><a name="zh-cn_topic_0225568845_p31337682"></a><a name="zh-cn_topic_0225568845_p31337682"></a>app_name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p55324299"><a name="zh-cn_topic_0225568845_p55324299"></a><a name="zh-cn_topic_0225568845_p55324299"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p52083233"><a name="zh-cn_topic_0225568845_p52083233"></a><a name="zh-cn_topic_0225568845_p52083233"></a>string</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p57992315"><a name="zh-cn_topic_0225568845_p57992315"></a><a name="zh-cn_topic_0225568845_p57992315"></a>APP名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row52168789"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p64922385"><a name="zh-cn_topic_0225568845_p64922385"></a><a name="zh-cn_topic_0225568845_p64922385"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p24221829"><a name="zh-cn_topic_0225568845_p24221829"></a><a name="zh-cn_topic_0225568845_p24221829"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p15811162"><a name="zh-cn_topic_0225568845_p15811162"></a><a name="zh-cn_topic_0225568845_p15811162"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p5635768"><a name="zh-cn_topic_0225568845_p5635768"></a><a name="zh-cn_topic_0225568845_p5635768"></a>APP编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row50721913"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p14834294"><a name="zh-cn_topic_0225568845_p14834294"></a><a name="zh-cn_topic_0225568845_p14834294"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p60727184"><a name="zh-cn_topic_0225568845_p60727184"></a><a name="zh-cn_topic_0225568845_p60727184"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p19954862"><a name="zh-cn_topic_0225568845_p19954862"></a><a name="zh-cn_topic_0225568845_p19954862"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p5731129"><a name="zh-cn_topic_0225568845_p5731129"></a><a name="zh-cn_topic_0225568845_p5731129"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row51580162"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p17243611"><a name="zh-cn_topic_0225568845_p17243611"></a><a name="zh-cn_topic_0225568845_p17243611"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p54555220"><a name="zh-cn_topic_0225568845_p54555220"></a><a name="zh-cn_topic_0225568845_p54555220"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p56896661"><a name="zh-cn_topic_0225568845_p56896661"></a><a name="zh-cn_topic_0225568845_p56896661"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p45226823"><a name="zh-cn_topic_0225568845_p45226823"></a><a name="zh-cn_topic_0225568845_p45226823"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row4388225"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568845_p19901983"><a name="zh-cn_topic_0225568845_p19901983"></a><a name="zh-cn_topic_0225568845_p19901983"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568845_p1447937"><a name="zh-cn_topic_0225568845_p1447937"></a><a name="zh-cn_topic_0225568845_p1447937"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568845_p50174096"><a name="zh-cn_topic_0225568845_p50174096"></a><a name="zh-cn_topic_0225568845_p50174096"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568845_p37569971"><a name="zh-cn_topic_0225568845_p37569971"></a><a name="zh-cn_topic_0225568845_p37569971"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568845_section52840210"></a>

无

## 响应消息<a name="zh-cn_topic_0225568845_section52198597"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568845_table30742358"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568845_row64433482"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568845_p51729548"><a name="zh-cn_topic_0225568845_p51729548"></a><a name="zh-cn_topic_0225568845_p51729548"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568845_p29343846"><a name="zh-cn_topic_0225568845_p29343846"></a><a name="zh-cn_topic_0225568845_p29343846"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568845_p28041345"><a name="zh-cn_topic_0225568845_p28041345"></a><a name="zh-cn_topic_0225568845_p28041345"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568845_row56756485"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p33872536"><a name="zh-cn_topic_0225568845_p33872536"></a><a name="zh-cn_topic_0225568845_p33872536"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p59320933"><a name="zh-cn_topic_0225568845_p59320933"></a><a name="zh-cn_topic_0225568845_p59320933"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p40266258"><a name="zh-cn_topic_0225568845_p40266258"></a><a name="zh-cn_topic_0225568845_p40266258"></a>符合条件的APP总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row26852004"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p27528709"><a name="zh-cn_topic_0225568845_p27528709"></a><a name="zh-cn_topic_0225568845_p27528709"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p15232922"><a name="zh-cn_topic_0225568845_p15232922"></a><a name="zh-cn_topic_0225568845_p15232922"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p25907147"><a name="zh-cn_topic_0225568845_p25907147"></a><a name="zh-cn_topic_0225568845_p25907147"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row31837738"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p28720018"><a name="zh-cn_topic_0225568845_p28720018"></a><a name="zh-cn_topic_0225568845_p28720018"></a>auths</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p44620106"><a name="zh-cn_topic_0225568845_p44620106"></a><a name="zh-cn_topic_0225568845_p44620106"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p57458810"><a name="zh-cn_topic_0225568845_p57458810"></a><a name="zh-cn_topic_0225568845_p57458810"></a>本次返回的APP列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  auths参数说明

<a name="zh-cn_topic_0225568845_table47367247"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568845_row41214097"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568845_p50007540"><a name="zh-cn_topic_0225568845_p50007540"></a><a name="zh-cn_topic_0225568845_p50007540"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568845_p24078911"><a name="zh-cn_topic_0225568845_p24078911"></a><a name="zh-cn_topic_0225568845_p24078911"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568845_p4234779"><a name="zh-cn_topic_0225568845_p4234779"></a><a name="zh-cn_topic_0225568845_p4234779"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568845_row7472815"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p1318308"><a name="zh-cn_topic_0225568845_p1318308"></a><a name="zh-cn_topic_0225568845_p1318308"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p39674146"><a name="zh-cn_topic_0225568845_p39674146"></a><a name="zh-cn_topic_0225568845_p39674146"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p59489232"><a name="zh-cn_topic_0225568845_p59489232"></a><a name="zh-cn_topic_0225568845_p59489232"></a>授权关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row65641040"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p15324042"><a name="zh-cn_topic_0225568845_p15324042"></a><a name="zh-cn_topic_0225568845_p15324042"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p33287880"><a name="zh-cn_topic_0225568845_p33287880"></a><a name="zh-cn_topic_0225568845_p33287880"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p11963763"><a name="zh-cn_topic_0225568845_p11963763"></a><a name="zh-cn_topic_0225568845_p11963763"></a>API的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row40565004"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p64539909"><a name="zh-cn_topic_0225568845_p64539909"></a><a name="zh-cn_topic_0225568845_p64539909"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p60350110"><a name="zh-cn_topic_0225568845_p60350110"></a><a name="zh-cn_topic_0225568845_p60350110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p56520703"><a name="zh-cn_topic_0225568845_p56520703"></a><a name="zh-cn_topic_0225568845_p56520703"></a>API的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row38924282"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p65859163"><a name="zh-cn_topic_0225568845_p65859163"></a><a name="zh-cn_topic_0225568845_p65859163"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p32992025"><a name="zh-cn_topic_0225568845_p32992025"></a><a name="zh-cn_topic_0225568845_p32992025"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p55108379"><a name="zh-cn_topic_0225568845_p55108379"></a><a name="zh-cn_topic_0225568845_p55108379"></a>API绑定的分组</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row26213370"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p42908189"><a name="zh-cn_topic_0225568845_p42908189"></a><a name="zh-cn_topic_0225568845_p42908189"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p53011322"><a name="zh-cn_topic_0225568845_p53011322"></a><a name="zh-cn_topic_0225568845_p53011322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p66058679"><a name="zh-cn_topic_0225568845_p66058679"></a><a name="zh-cn_topic_0225568845_p66058679"></a>API的描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row57657201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p39721698"><a name="zh-cn_topic_0225568845_p39721698"></a><a name="zh-cn_topic_0225568845_p39721698"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p63340935"><a name="zh-cn_topic_0225568845_p63340935"></a><a name="zh-cn_topic_0225568845_p63340935"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p30342088"><a name="zh-cn_topic_0225568845_p30342088"></a><a name="zh-cn_topic_0225568845_p30342088"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row4643343"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p40566535"><a name="zh-cn_topic_0225568845_p40566535"></a><a name="zh-cn_topic_0225568845_p40566535"></a>envname</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p64663887"><a name="zh-cn_topic_0225568845_p64663887"></a><a name="zh-cn_topic_0225568845_p64663887"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p3283471"><a name="zh-cn_topic_0225568845_p3283471"></a><a name="zh-cn_topic_0225568845_p3283471"></a>api授权绑定的环境</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row29551244"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p44840564"><a name="zh-cn_topic_0225568845_p44840564"></a><a name="zh-cn_topic_0225568845_p44840564"></a>auth_role</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p8207081"><a name="zh-cn_topic_0225568845_p8207081"></a><a name="zh-cn_topic_0225568845_p8207081"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p60793810"><a name="zh-cn_topic_0225568845_p60793810"></a><a name="zh-cn_topic_0225568845_p60793810"></a>授权者</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row10273382"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p26837593"><a name="zh-cn_topic_0225568845_p26837593"></a><a name="zh-cn_topic_0225568845_p26837593"></a>auth_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p26361396"><a name="zh-cn_topic_0225568845_p26361396"></a><a name="zh-cn_topic_0225568845_p26361396"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p54898336"><a name="zh-cn_topic_0225568845_p54898336"></a><a name="zh-cn_topic_0225568845_p54898336"></a>授权创建的时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row24322980"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p24004331"><a name="zh-cn_topic_0225568845_p24004331"></a><a name="zh-cn_topic_0225568845_p24004331"></a>appid</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p65302679"><a name="zh-cn_topic_0225568845_p65302679"></a><a name="zh-cn_topic_0225568845_p65302679"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p55025680"><a name="zh-cn_topic_0225568845_p55025680"></a><a name="zh-cn_topic_0225568845_p55025680"></a>APP的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row25469077"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p49729323"><a name="zh-cn_topic_0225568845_p49729323"></a><a name="zh-cn_topic_0225568845_p49729323"></a>app_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p1543362"><a name="zh-cn_topic_0225568845_p1543362"></a><a name="zh-cn_topic_0225568845_p1543362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p57903489"><a name="zh-cn_topic_0225568845_p57903489"></a><a name="zh-cn_topic_0225568845_p57903489"></a>APP的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row51369360"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p168607"><a name="zh-cn_topic_0225568845_p168607"></a><a name="zh-cn_topic_0225568845_p168607"></a>app_creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p13657195"><a name="zh-cn_topic_0225568845_p13657195"></a><a name="zh-cn_topic_0225568845_p13657195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p32490971"><a name="zh-cn_topic_0225568845_p32490971"></a><a name="zh-cn_topic_0225568845_p32490971"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0225568845_ul23983284"></a><a name="zh-cn_topic_0225568845_ul23983284"></a><ul id="zh-cn_topic_0225568845_ul23983284"><li>USER：租户自己创建</li><li>MARKET：API市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row173091559125318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p4811351104314"><a name="zh-cn_topic_0225568845_p4811351104314"></a><a name="zh-cn_topic_0225568845_p4811351104314"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p198155113430"><a name="zh-cn_topic_0225568845_p198155113430"></a><a name="zh-cn_topic_0225568845_p198155113430"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p881351134310"><a name="zh-cn_topic_0225568845_p881351134310"></a><a name="zh-cn_topic_0225568845_p881351134310"></a>API发布ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row625911112547"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p1568553194417"><a name="zh-cn_topic_0225568845_p1568553194417"></a><a name="zh-cn_topic_0225568845_p1568553194417"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p16853304410"><a name="zh-cn_topic_0225568845_p16853304410"></a><a name="zh-cn_topic_0225568845_p16853304410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p1568573164414"><a name="zh-cn_topic_0225568845_p1568573164414"></a><a name="zh-cn_topic_0225568845_p1568573164414"></a>环境ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row11936113125415"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p1794914196448"><a name="zh-cn_topic_0225568845_p1794914196448"></a><a name="zh-cn_topic_0225568845_p1794914196448"></a>app_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p394941994418"><a name="zh-cn_topic_0225568845_p394941994418"></a><a name="zh-cn_topic_0225568845_p394941994418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p99491419144419"><a name="zh-cn_topic_0225568845_p99491419144419"></a><a name="zh-cn_topic_0225568845_p99491419144419"></a>APP的描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row75816675416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568845_p11131335446"><a name="zh-cn_topic_0225568845_p11131335446"></a><a name="zh-cn_topic_0225568845_p11131335446"></a>app_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568845_p4113113318448"><a name="zh-cn_topic_0225568845_p4113113318448"></a><a name="zh-cn_topic_0225568845_p4113113318448"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568845_p141138332445"><a name="zh-cn_topic_0225568845_p141138332445"></a><a name="zh-cn_topic_0225568845_p141138332445"></a>APP类型</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 1,
	"size": 1,
	"auths": [{
		"id": "cfa688d8-094b-445a-b270-6aeb0b70a84a",
		"api_id": "6632a062-9dcf-4f18-9646-3cabb925a290",
		"api_name": "查询API列表",
		"group_name": "api_group_001",
		"api_type": 1,
		"api_remark": "查询API列表",
		"envname": "RELEASE",
		"auth_role": "PROVIDER",
		"auth_time": "2017-12-28T12:46:43Z",
		"appid": "14b399ac-967f-4115-bb62-c0346b4537e9",
		"app_name": "app_001",
		"app_creator": "USER",
                "publish_id": "fe9d8ea9f9424594abc3bbe8d861c0f0",
                "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
                "app_remark": "",
                "app_type": "apig"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568845_section5799844"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568845_table5726167"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568845_row30002454"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568845_p14279749"><a name="zh-cn_topic_0225568845_p14279749"></a><a name="zh-cn_topic_0225568845_p14279749"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568845_p15809053"><a name="zh-cn_topic_0225568845_p15809053"></a><a name="zh-cn_topic_0225568845_p15809053"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568845_row5464901"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568845_p40003813"><a name="zh-cn_topic_0225568845_p40003813"></a><a name="zh-cn_topic_0225568845_p40003813"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568845_p19083430"><a name="zh-cn_topic_0225568845_p19083430"></a><a name="zh-cn_topic_0225568845_p19083430"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row37533146"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568845_p20285999"><a name="zh-cn_topic_0225568845_p20285999"></a><a name="zh-cn_topic_0225568845_p20285999"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568845_p32553208"><a name="zh-cn_topic_0225568845_p32553208"></a><a name="zh-cn_topic_0225568845_p32553208"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row24543420"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568845_p41859983"><a name="zh-cn_topic_0225568845_p41859983"></a><a name="zh-cn_topic_0225568845_p41859983"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568845_p35215434"><a name="zh-cn_topic_0225568845_p35215434"></a><a name="zh-cn_topic_0225568845_p35215434"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row48503454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568845_p36465738"><a name="zh-cn_topic_0225568845_p36465738"></a><a name="zh-cn_topic_0225568845_p36465738"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568845_p934769"><a name="zh-cn_topic_0225568845_p934769"></a><a name="zh-cn_topic_0225568845_p934769"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row8412927"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568845_p10358509"><a name="zh-cn_topic_0225568845_p10358509"></a><a name="zh-cn_topic_0225568845_p10358509"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568845_p33732875"><a name="zh-cn_topic_0225568845_p33732875"></a><a name="zh-cn_topic_0225568845_p33732875"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568845_row35160419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568845_p29421709"><a name="zh-cn_topic_0225568845_p29421709"></a><a name="zh-cn_topic_0225568845_p29421709"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568845_p14947689"><a name="zh-cn_topic_0225568845_p14947689"></a><a name="zh-cn_topic_0225568845_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

