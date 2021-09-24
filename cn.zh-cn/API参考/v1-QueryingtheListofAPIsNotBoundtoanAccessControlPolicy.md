# 查看ACL策略未绑定的API列表<a name="ZH-CN_TOPIC_0000001081837373"></a>

## 功能介绍<a name="zh-cn_topic_0225568896_section61570312"></a>

查看ACL策略未绑定的API列表，需要API已发布。

## URI<a name="zh-cn_topic_0225568896_section17261904"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568896_table7075937"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568896_row65440801"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568896_p66213500"><a name="zh-cn_topic_0225568896_p66213500"></a><a name="zh-cn_topic_0225568896_p66213500"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568896_p61693288"><a name="zh-cn_topic_0225568896_p61693288"></a><a name="zh-cn_topic_0225568896_p61693288"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568896_row31100428"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568896_p36106769"><a name="zh-cn_topic_0225568896_p36106769"></a><a name="zh-cn_topic_0225568896_p36106769"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568896_p38967199"><a name="zh-cn_topic_0225568896_p38967199"></a><a name="zh-cn_topic_0225568896_p38967199"></a>/v1/{project_id}/apigw/instances/{instance_id}/acl-bindings/unbinded-apis[?page_no、page_size、acl_id、env_id、api_id、api_name、group-id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：acl\_id、env\_id、api\_id、group\_id、api\_name、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568896_table45607562"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568896_row21909387"><th class="cellrowborder" valign="top" width="16%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568896_p29829884"><a name="zh-cn_topic_0225568896_p29829884"></a><a name="zh-cn_topic_0225568896_p29829884"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="9%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568896_p301534"><a name="zh-cn_topic_0225568896_p301534"></a><a name="zh-cn_topic_0225568896_p301534"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="9%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568896_p24424280"><a name="zh-cn_topic_0225568896_p24424280"></a><a name="zh-cn_topic_0225568896_p24424280"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="66%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568896_p32209683"><a name="zh-cn_topic_0225568896_p32209683"></a><a name="zh-cn_topic_0225568896_p32209683"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568896_row15590143542015"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p55878963"><a name="zh-cn_topic_0225568896_p55878963"></a><a name="zh-cn_topic_0225568896_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p29902160"><a name="zh-cn_topic_0225568896_p29902160"></a><a name="zh-cn_topic_0225568896_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p6155914"><a name="zh-cn_topic_0225568896_p6155914"></a><a name="zh-cn_topic_0225568896_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p28867016"><a name="zh-cn_topic_0225568896_p28867016"></a><a name="zh-cn_topic_0225568896_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row172471935182017"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p1780913159538"><a name="zh-cn_topic_0225568896_p1780913159538"></a><a name="zh-cn_topic_0225568896_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p9809215115310"><a name="zh-cn_topic_0225568896_p9809215115310"></a><a name="zh-cn_topic_0225568896_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p1280914152538"><a name="zh-cn_topic_0225568896_p1280914152538"></a><a name="zh-cn_topic_0225568896_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p1880914157537"><a name="zh-cn_topic_0225568896_p1880914157537"></a><a name="zh-cn_topic_0225568896_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row58847543"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p1921642"><a name="zh-cn_topic_0225568896_p1921642"></a><a name="zh-cn_topic_0225568896_p1921642"></a>acl_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p21435351"><a name="zh-cn_topic_0225568896_p21435351"></a><a name="zh-cn_topic_0225568896_p21435351"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p58541860"><a name="zh-cn_topic_0225568896_p58541860"></a><a name="zh-cn_topic_0225568896_p58541860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p17951547165618"><a name="zh-cn_topic_0225568896_p17951547165618"></a><a name="zh-cn_topic_0225568896_p17951547165618"></a>ACL策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row62887495"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p60722300"><a name="zh-cn_topic_0225568896_p60722300"></a><a name="zh-cn_topic_0225568896_p60722300"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p19559245"><a name="zh-cn_topic_0225568896_p19559245"></a><a name="zh-cn_topic_0225568896_p19559245"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p40795044"><a name="zh-cn_topic_0225568896_p40795044"></a><a name="zh-cn_topic_0225568896_p40795044"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p16064230"><a name="zh-cn_topic_0225568896_p16064230"></a><a name="zh-cn_topic_0225568896_p16064230"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row10360348"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p33881836"><a name="zh-cn_topic_0225568896_p33881836"></a><a name="zh-cn_topic_0225568896_p33881836"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p60074205"><a name="zh-cn_topic_0225568896_p60074205"></a><a name="zh-cn_topic_0225568896_p60074205"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p34172438"><a name="zh-cn_topic_0225568896_p34172438"></a><a name="zh-cn_topic_0225568896_p34172438"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p16504128"><a name="zh-cn_topic_0225568896_p16504128"></a><a name="zh-cn_topic_0225568896_p16504128"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row14319431"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p19023261"><a name="zh-cn_topic_0225568896_p19023261"></a><a name="zh-cn_topic_0225568896_p19023261"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p64489143"><a name="zh-cn_topic_0225568896_p64489143"></a><a name="zh-cn_topic_0225568896_p64489143"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p56238077"><a name="zh-cn_topic_0225568896_p56238077"></a><a name="zh-cn_topic_0225568896_p56238077"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p58990425"><a name="zh-cn_topic_0225568896_p58990425"></a><a name="zh-cn_topic_0225568896_p58990425"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row61151777"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p54346934"><a name="zh-cn_topic_0225568896_p54346934"></a><a name="zh-cn_topic_0225568896_p54346934"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p40025556"><a name="zh-cn_topic_0225568896_p40025556"></a><a name="zh-cn_topic_0225568896_p40025556"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p20844578"><a name="zh-cn_topic_0225568896_p20844578"></a><a name="zh-cn_topic_0225568896_p20844578"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p10689224"><a name="zh-cn_topic_0225568896_p10689224"></a><a name="zh-cn_topic_0225568896_p10689224"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row29094156"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p7816426"><a name="zh-cn_topic_0225568896_p7816426"></a><a name="zh-cn_topic_0225568896_p7816426"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p29150773"><a name="zh-cn_topic_0225568896_p29150773"></a><a name="zh-cn_topic_0225568896_p29150773"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p12402388"><a name="zh-cn_topic_0225568896_p12402388"></a><a name="zh-cn_topic_0225568896_p12402388"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p65069360"><a name="zh-cn_topic_0225568896_p65069360"></a><a name="zh-cn_topic_0225568896_p65069360"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row48753328"><td class="cellrowborder" valign="top" width="16%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568896_p56705457"><a name="zh-cn_topic_0225568896_p56705457"></a><a name="zh-cn_topic_0225568896_p56705457"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568896_p29739299"><a name="zh-cn_topic_0225568896_p29739299"></a><a name="zh-cn_topic_0225568896_p29739299"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="9%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568896_p60073005"><a name="zh-cn_topic_0225568896_p60073005"></a><a name="zh-cn_topic_0225568896_p60073005"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="66%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568896_p34075256"><a name="zh-cn_topic_0225568896_p34075256"></a><a name="zh-cn_topic_0225568896_p34075256"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568896_section21139415"></a>

无

## 响应消息<a name="zh-cn_topic_0225568896_section34571087"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568896_table11928633"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568896_row60512777"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568896_p2587895"><a name="zh-cn_topic_0225568896_p2587895"></a><a name="zh-cn_topic_0225568896_p2587895"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568896_p8292946"><a name="zh-cn_topic_0225568896_p8292946"></a><a name="zh-cn_topic_0225568896_p8292946"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568896_p640001"><a name="zh-cn_topic_0225568896_p640001"></a><a name="zh-cn_topic_0225568896_p640001"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568896_row51840109"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p38299261"><a name="zh-cn_topic_0225568896_p38299261"></a><a name="zh-cn_topic_0225568896_p38299261"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p15232409"><a name="zh-cn_topic_0225568896_p15232409"></a><a name="zh-cn_topic_0225568896_p15232409"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p34954265718"><a name="zh-cn_topic_0225568896_p34954265718"></a><a name="zh-cn_topic_0225568896_p34954265718"></a>符合条件的API总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row31464194"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p65571805"><a name="zh-cn_topic_0225568896_p65571805"></a><a name="zh-cn_topic_0225568896_p65571805"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p9716001"><a name="zh-cn_topic_0225568896_p9716001"></a><a name="zh-cn_topic_0225568896_p9716001"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p48798580"><a name="zh-cn_topic_0225568896_p48798580"></a><a name="zh-cn_topic_0225568896_p48798580"></a>本次查询返回的API个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row36534044"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p6467596"><a name="zh-cn_topic_0225568896_p6467596"></a><a name="zh-cn_topic_0225568896_p6467596"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p54113248"><a name="zh-cn_topic_0225568896_p54113248"></a><a name="zh-cn_topic_0225568896_p54113248"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p21096961"><a name="zh-cn_topic_0225568896_p21096961"></a><a name="zh-cn_topic_0225568896_p21096961"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="zh-cn_topic_0225568896_table55654921"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568896_row66950944"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568896_p54317399"><a name="zh-cn_topic_0225568896_p54317399"></a><a name="zh-cn_topic_0225568896_p54317399"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568896_p37633227"><a name="zh-cn_topic_0225568896_p37633227"></a><a name="zh-cn_topic_0225568896_p37633227"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568896_p28392547"><a name="zh-cn_topic_0225568896_p28392547"></a><a name="zh-cn_topic_0225568896_p28392547"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568896_row18094984"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p56407585"><a name="zh-cn_topic_0225568896_p56407585"></a><a name="zh-cn_topic_0225568896_p56407585"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p5611671"><a name="zh-cn_topic_0225568896_p5611671"></a><a name="zh-cn_topic_0225568896_p5611671"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p51892177"><a name="zh-cn_topic_0225568896_p51892177"></a><a name="zh-cn_topic_0225568896_p51892177"></a>API的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row64376411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p47106807"><a name="zh-cn_topic_0225568896_p47106807"></a><a name="zh-cn_topic_0225568896_p47106807"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p57555019"><a name="zh-cn_topic_0225568896_p57555019"></a><a name="zh-cn_topic_0225568896_p57555019"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p31444992"><a name="zh-cn_topic_0225568896_p31444992"></a><a name="zh-cn_topic_0225568896_p31444992"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row14569478"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p39277103"><a name="zh-cn_topic_0225568896_p39277103"></a><a name="zh-cn_topic_0225568896_p39277103"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p27328780"><a name="zh-cn_topic_0225568896_p27328780"></a><a name="zh-cn_topic_0225568896_p27328780"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p66147590"><a name="zh-cn_topic_0225568896_p66147590"></a><a name="zh-cn_topic_0225568896_p66147590"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row58457401"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p37429032"><a name="zh-cn_topic_0225568896_p37429032"></a><a name="zh-cn_topic_0225568896_p37429032"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p11852776"><a name="zh-cn_topic_0225568896_p11852776"></a><a name="zh-cn_topic_0225568896_p11852776"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p20550817"><a name="zh-cn_topic_0225568896_p20550817"></a><a name="zh-cn_topic_0225568896_p20550817"></a>API所属分组的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row4920279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p62998338"><a name="zh-cn_topic_0225568896_p62998338"></a><a name="zh-cn_topic_0225568896_p62998338"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p2591766"><a name="zh-cn_topic_0225568896_p2591766"></a><a name="zh-cn_topic_0225568896_p2591766"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p8606457"><a name="zh-cn_topic_0225568896_p8606457"></a><a name="zh-cn_topic_0225568896_p8606457"></a>API开放状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row57391748"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p18220050"><a name="zh-cn_topic_0225568896_p18220050"></a><a name="zh-cn_topic_0225568896_p18220050"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p66537956"><a name="zh-cn_topic_0225568896_p66537956"></a><a name="zh-cn_topic_0225568896_p66537956"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p20865379"><a name="zh-cn_topic_0225568896_p20865379"></a><a name="zh-cn_topic_0225568896_p20865379"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row57771451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p48975920"><a name="zh-cn_topic_0225568896_p48975920"></a><a name="zh-cn_topic_0225568896_p48975920"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p7626561"><a name="zh-cn_topic_0225568896_p7626561"></a><a name="zh-cn_topic_0225568896_p7626561"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p13771736"><a name="zh-cn_topic_0225568896_p13771736"></a><a name="zh-cn_topic_0225568896_p13771736"></a>发布的环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row56836760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p40374832"><a name="zh-cn_topic_0225568896_p40374832"></a><a name="zh-cn_topic_0225568896_p40374832"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p49135936"><a name="zh-cn_topic_0225568896_p49135936"></a><a name="zh-cn_topic_0225568896_p49135936"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p20587889"><a name="zh-cn_topic_0225568896_p20587889"></a><a name="zh-cn_topic_0225568896_p20587889"></a>发布的环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row51073277"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p43294786"><a name="zh-cn_topic_0225568896_p43294786"></a><a name="zh-cn_topic_0225568896_p43294786"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p17216763"><a name="zh-cn_topic_0225568896_p17216763"></a><a name="zh-cn_topic_0225568896_p17216763"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p52380561"><a name="zh-cn_topic_0225568896_p52380561"></a><a name="zh-cn_topic_0225568896_p52380561"></a>API发布记录编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row1663002"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p485445"><a name="zh-cn_topic_0225568896_p485445"></a><a name="zh-cn_topic_0225568896_p485445"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p39321089"><a name="zh-cn_topic_0225568896_p39321089"></a><a name="zh-cn_topic_0225568896_p39321089"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p30891637"><a name="zh-cn_topic_0225568896_p30891637"></a><a name="zh-cn_topic_0225568896_p30891637"></a>绑定的其他同类型的ACL策略名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row76812386461"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p169163811462"><a name="zh-cn_topic_0225568896_p169163811462"></a><a name="zh-cn_topic_0225568896_p169163811462"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p146983804611"><a name="zh-cn_topic_0225568896_p146983804611"></a><a name="zh-cn_topic_0225568896_p146983804611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p469123819465"><a name="zh-cn_topic_0225568896_p469123819465"></a><a name="zh-cn_topic_0225568896_p469123819465"></a>API的访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row1937684294618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568896_p5376144210461"><a name="zh-cn_topic_0225568896_p5376144210461"></a><a name="zh-cn_topic_0225568896_p5376144210461"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568896_p13376134215468"><a name="zh-cn_topic_0225568896_p13376134215468"></a><a name="zh-cn_topic_0225568896_p13376134215468"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568896_p73761442124614"><a name="zh-cn_topic_0225568896_p73761442124614"></a><a name="zh-cn_topic_0225568896_p73761442124614"></a>API的认证方式</p>
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
      "publish_id": "a6e06a00c382436eb524fa2dd343cb6d",
      "req_uri": "/test",
      "auth_type": "NONE"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0225568896_section56037015"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568896_table28132847"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568896_row3719443"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568896_p32839460"><a name="zh-cn_topic_0225568896_p32839460"></a><a name="zh-cn_topic_0225568896_p32839460"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568896_p42750569"><a name="zh-cn_topic_0225568896_p42750569"></a><a name="zh-cn_topic_0225568896_p42750569"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568896_row40244042"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568896_p38542001"><a name="zh-cn_topic_0225568896_p38542001"></a><a name="zh-cn_topic_0225568896_p38542001"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568896_p34894339"><a name="zh-cn_topic_0225568896_p34894339"></a><a name="zh-cn_topic_0225568896_p34894339"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row45613601"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568896_p3714177"><a name="zh-cn_topic_0225568896_p3714177"></a><a name="zh-cn_topic_0225568896_p3714177"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568896_p32412930"><a name="zh-cn_topic_0225568896_p32412930"></a><a name="zh-cn_topic_0225568896_p32412930"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row23280918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568896_p6706219"><a name="zh-cn_topic_0225568896_p6706219"></a><a name="zh-cn_topic_0225568896_p6706219"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568896_p6332852"><a name="zh-cn_topic_0225568896_p6332852"></a><a name="zh-cn_topic_0225568896_p6332852"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row56995672"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568896_p53246699"><a name="zh-cn_topic_0225568896_p53246699"></a><a name="zh-cn_topic_0225568896_p53246699"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568896_p18015334"><a name="zh-cn_topic_0225568896_p18015334"></a><a name="zh-cn_topic_0225568896_p18015334"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568896_row27920282"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568896_p46950406"><a name="zh-cn_topic_0225568896_p46950406"></a><a name="zh-cn_topic_0225568896_p46950406"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568896_p44886509"><a name="zh-cn_topic_0225568896_p44886509"></a><a name="zh-cn_topic_0225568896_p44886509"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

