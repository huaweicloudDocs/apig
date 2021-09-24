# 查询变量列表<a name="ZH-CN_TOPIC_0000001081976187"></a>

## 功能介绍<a name="zh-cn_topic_0225568858_section38838407"></a>

查询分组下的所有环境变量的列表。

## URI<a name="zh-cn_topic_0225568858_section14001345"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568858_table24301087"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568858_row30079465"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568858_p20517635"><a name="zh-cn_topic_0225568858_p20517635"></a><a name="zh-cn_topic_0225568858_p20517635"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568858_p51315766"><a name="zh-cn_topic_0225568858_p51315766"></a><a name="zh-cn_topic_0225568858_p51315766"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568858_row62936361"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568858_p64680452"><a name="zh-cn_topic_0225568858_p64680452"></a><a name="zh-cn_topic_0225568858_p64680452"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568858_p4625264"><a name="zh-cn_topic_0225568858_p4625264"></a><a name="zh-cn_topic_0225568858_p4625264"></a>/v1/{project_id}/apigw/instances/{instance_id}/env-variables[?page_size, page_no, env_id, group_id, variable_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：env\_id、group\_id、variable\_name、page\_size、page\_no

**表 2**  参数说明

<a name="zh-cn_topic_0225568858_table51273191"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568858_row29844517"><th class="cellrowborder" valign="top" width="22.932293229322934%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568858_p1486816"><a name="zh-cn_topic_0225568858_p1486816"></a><a name="zh-cn_topic_0225568858_p1486816"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.55195519551955%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568858_p53323247"><a name="zh-cn_topic_0225568858_p53323247"></a><a name="zh-cn_topic_0225568858_p53323247"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.461746174617463%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568858_p24215739"><a name="zh-cn_topic_0225568858_p24215739"></a><a name="zh-cn_topic_0225568858_p24215739"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.054005400540056%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568858_p15317803"><a name="zh-cn_topic_0225568858_p15317803"></a><a name="zh-cn_topic_0225568858_p15317803"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568858_row1348816172493"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p55878963"><a name="zh-cn_topic_0225568858_p55878963"></a><a name="zh-cn_topic_0225568858_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p29902160"><a name="zh-cn_topic_0225568858_p29902160"></a><a name="zh-cn_topic_0225568858_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p6155914"><a name="zh-cn_topic_0225568858_p6155914"></a><a name="zh-cn_topic_0225568858_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p28867016"><a name="zh-cn_topic_0225568858_p28867016"></a><a name="zh-cn_topic_0225568858_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row33059171496"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p1780913159538"><a name="zh-cn_topic_0225568858_p1780913159538"></a><a name="zh-cn_topic_0225568858_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p9809215115310"><a name="zh-cn_topic_0225568858_p9809215115310"></a><a name="zh-cn_topic_0225568858_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p1280914152538"><a name="zh-cn_topic_0225568858_p1280914152538"></a><a name="zh-cn_topic_0225568858_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p1880914157537"><a name="zh-cn_topic_0225568858_p1880914157537"></a><a name="zh-cn_topic_0225568858_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row32782503"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p38137112"><a name="zh-cn_topic_0225568858_p38137112"></a><a name="zh-cn_topic_0225568858_p38137112"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p2098406"><a name="zh-cn_topic_0225568858_p2098406"></a><a name="zh-cn_topic_0225568858_p2098406"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p35753208"><a name="zh-cn_topic_0225568858_p35753208"></a><a name="zh-cn_topic_0225568858_p35753208"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p10328759"><a name="zh-cn_topic_0225568858_p10328759"></a><a name="zh-cn_topic_0225568858_p10328759"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row25849970"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p13472863"><a name="zh-cn_topic_0225568858_p13472863"></a><a name="zh-cn_topic_0225568858_p13472863"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p17560108"><a name="zh-cn_topic_0225568858_p17560108"></a><a name="zh-cn_topic_0225568858_p17560108"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p13082625"><a name="zh-cn_topic_0225568858_p13082625"></a><a name="zh-cn_topic_0225568858_p13082625"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p53059719"><a name="zh-cn_topic_0225568858_p53059719"></a><a name="zh-cn_topic_0225568858_p53059719"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row7775428"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p25829909"><a name="zh-cn_topic_0225568858_p25829909"></a><a name="zh-cn_topic_0225568858_p25829909"></a>variable_name</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p11847916"><a name="zh-cn_topic_0225568858_p11847916"></a><a name="zh-cn_topic_0225568858_p11847916"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p20157102"><a name="zh-cn_topic_0225568858_p20157102"></a><a name="zh-cn_topic_0225568858_p20157102"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p22112581"><a name="zh-cn_topic_0225568858_p22112581"></a><a name="zh-cn_topic_0225568858_p22112581"></a>变量名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row64795508"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p36230260"><a name="zh-cn_topic_0225568858_p36230260"></a><a name="zh-cn_topic_0225568858_p36230260"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p55787422"><a name="zh-cn_topic_0225568858_p55787422"></a><a name="zh-cn_topic_0225568858_p55787422"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p22487368"><a name="zh-cn_topic_0225568858_p22487368"></a><a name="zh-cn_topic_0225568858_p22487368"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p9537547"><a name="zh-cn_topic_0225568858_p9537547"></a><a name="zh-cn_topic_0225568858_p9537547"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row18729061"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p40658943"><a name="zh-cn_topic_0225568858_p40658943"></a><a name="zh-cn_topic_0225568858_p40658943"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p5040069"><a name="zh-cn_topic_0225568858_p5040069"></a><a name="zh-cn_topic_0225568858_p5040069"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p5592481"><a name="zh-cn_topic_0225568858_p5592481"></a><a name="zh-cn_topic_0225568858_p5592481"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p50337784"><a name="zh-cn_topic_0225568858_p50337784"></a><a name="zh-cn_topic_0225568858_p50337784"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row1121020705418"><td class="cellrowborder" valign="top" width="22.932293229322934%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568858_p297092819498"><a name="zh-cn_topic_0225568858_p297092819498"></a><a name="zh-cn_topic_0225568858_p297092819498"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="19.55195519551955%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568858_p397092812491"><a name="zh-cn_topic_0225568858_p397092812491"></a><a name="zh-cn_topic_0225568858_p397092812491"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.461746174617463%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568858_p49701728194913"><a name="zh-cn_topic_0225568858_p49701728194913"></a><a name="zh-cn_topic_0225568858_p49701728194913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.054005400540056%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568858_p19970928194911"><a name="zh-cn_topic_0225568858_p19970928194911"></a><a name="zh-cn_topic_0225568858_p19970928194911"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568858_section58903244"></a>

无

## 响应消息<a name="zh-cn_topic_0225568858_section6433474"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568858_table54592882"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568858_row39850381"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568858_p6655456"><a name="zh-cn_topic_0225568858_p6655456"></a><a name="zh-cn_topic_0225568858_p6655456"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568858_p2221043"><a name="zh-cn_topic_0225568858_p2221043"></a><a name="zh-cn_topic_0225568858_p2221043"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568858_p45686766"><a name="zh-cn_topic_0225568858_p45686766"></a><a name="zh-cn_topic_0225568858_p45686766"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568858_row9640570"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p42688702"><a name="zh-cn_topic_0225568858_p42688702"></a><a name="zh-cn_topic_0225568858_p42688702"></a>variables</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p35232867"><a name="zh-cn_topic_0225568858_p35232867"></a><a name="zh-cn_topic_0225568858_p35232867"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p35290001"><a name="zh-cn_topic_0225568858_p35290001"></a><a name="zh-cn_topic_0225568858_p35290001"></a>本次返回的环境变量列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row49174554"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p23715943"><a name="zh-cn_topic_0225568858_p23715943"></a><a name="zh-cn_topic_0225568858_p23715943"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p41943249"><a name="zh-cn_topic_0225568858_p41943249"></a><a name="zh-cn_topic_0225568858_p41943249"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p41959999"><a name="zh-cn_topic_0225568858_p41959999"></a><a name="zh-cn_topic_0225568858_p41959999"></a>满足条件的环境变量总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row42095675"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p54306539"><a name="zh-cn_topic_0225568858_p54306539"></a><a name="zh-cn_topic_0225568858_p54306539"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p36753556"><a name="zh-cn_topic_0225568858_p36753556"></a><a name="zh-cn_topic_0225568858_p36753556"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p24248029"><a name="zh-cn_topic_0225568858_p24248029"></a><a name="zh-cn_topic_0225568858_p24248029"></a>本次返回的列表长度</p>
</td>
</tr>
</tbody>
</table>

**表 4**  variables参数说明

<a name="zh-cn_topic_0225568858_table16905669"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568858_row22600933"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568858_p18736297"><a name="zh-cn_topic_0225568858_p18736297"></a><a name="zh-cn_topic_0225568858_p18736297"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568858_p41245052"><a name="zh-cn_topic_0225568858_p41245052"></a><a name="zh-cn_topic_0225568858_p41245052"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568858_p52514953"><a name="zh-cn_topic_0225568858_p52514953"></a><a name="zh-cn_topic_0225568858_p52514953"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568858_row25852790"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p13701227"><a name="zh-cn_topic_0225568858_p13701227"></a><a name="zh-cn_topic_0225568858_p13701227"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p36057617"><a name="zh-cn_topic_0225568858_p36057617"></a><a name="zh-cn_topic_0225568858_p36057617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p34985871"><a name="zh-cn_topic_0225568858_p34985871"></a><a name="zh-cn_topic_0225568858_p34985871"></a>环境变量编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row46437391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p3332358"><a name="zh-cn_topic_0225568858_p3332358"></a><a name="zh-cn_topic_0225568858_p3332358"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p1485544"><a name="zh-cn_topic_0225568858_p1485544"></a><a name="zh-cn_topic_0225568858_p1485544"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p53220255"><a name="zh-cn_topic_0225568858_p53220255"></a><a name="zh-cn_topic_0225568858_p53220255"></a>环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row9220254"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p8643119"><a name="zh-cn_topic_0225568858_p8643119"></a><a name="zh-cn_topic_0225568858_p8643119"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p29004040"><a name="zh-cn_topic_0225568858_p29004040"></a><a name="zh-cn_topic_0225568858_p29004040"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p517074"><a name="zh-cn_topic_0225568858_p517074"></a><a name="zh-cn_topic_0225568858_p517074"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row4653673"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p41403231"><a name="zh-cn_topic_0225568858_p41403231"></a><a name="zh-cn_topic_0225568858_p41403231"></a>variable_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p65327385"><a name="zh-cn_topic_0225568858_p65327385"></a><a name="zh-cn_topic_0225568858_p65327385"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p57026815"><a name="zh-cn_topic_0225568858_p57026815"></a><a name="zh-cn_topic_0225568858_p57026815"></a>变量名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row43479295"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568858_p32162003"><a name="zh-cn_topic_0225568858_p32162003"></a><a name="zh-cn_topic_0225568858_p32162003"></a>variable_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568858_p54985480"><a name="zh-cn_topic_0225568858_p54985480"></a><a name="zh-cn_topic_0225568858_p54985480"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568858_p24638918"><a name="zh-cn_topic_0225568858_p24638918"></a><a name="zh-cn_topic_0225568858_p24638918"></a>变量值</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"variables": [{
		"id": "09ab8135-7224-40b9-bf5d-107f2a09d409",
		"env_id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"variable_name": "port",
		"variable_value": "8080"
	},
	{
		"id": "104185e5-3e8f-4c63-a7e5-ef4117bf870c",
		"env_id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"variable_name": "address",
		"variable_value": "192.168.1.5"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568858_section60367154"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568858_table23486013"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568858_row20940407"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568858_p18451398"><a name="zh-cn_topic_0225568858_p18451398"></a><a name="zh-cn_topic_0225568858_p18451398"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568858_p18168294"><a name="zh-cn_topic_0225568858_p18168294"></a><a name="zh-cn_topic_0225568858_p18168294"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568858_row62345727"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568858_p16839096"><a name="zh-cn_topic_0225568858_p16839096"></a><a name="zh-cn_topic_0225568858_p16839096"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568858_p21789497"><a name="zh-cn_topic_0225568858_p21789497"></a><a name="zh-cn_topic_0225568858_p21789497"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row61887748"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568858_p46851717"><a name="zh-cn_topic_0225568858_p46851717"></a><a name="zh-cn_topic_0225568858_p46851717"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568858_p14446173764116"><a name="zh-cn_topic_0225568858_p14446173764116"></a><a name="zh-cn_topic_0225568858_p14446173764116"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row63599488"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568858_p51284916"><a name="zh-cn_topic_0225568858_p51284916"></a><a name="zh-cn_topic_0225568858_p51284916"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568858_p60437495"><a name="zh-cn_topic_0225568858_p60437495"></a><a name="zh-cn_topic_0225568858_p60437495"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row7066551"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568858_p35519767"><a name="zh-cn_topic_0225568858_p35519767"></a><a name="zh-cn_topic_0225568858_p35519767"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568858_p58528859"><a name="zh-cn_topic_0225568858_p58528859"></a><a name="zh-cn_topic_0225568858_p58528859"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row56997686"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568858_p53409868"><a name="zh-cn_topic_0225568858_p53409868"></a><a name="zh-cn_topic_0225568858_p53409868"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568858_p31232058"><a name="zh-cn_topic_0225568858_p31232058"></a><a name="zh-cn_topic_0225568858_p31232058"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568858_row12653074"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568858_p18266105"><a name="zh-cn_topic_0225568858_p18266105"></a><a name="zh-cn_topic_0225568858_p18266105"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568858_p14947689"><a name="zh-cn_topic_0225568858_p14947689"></a><a name="zh-cn_topic_0225568858_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

