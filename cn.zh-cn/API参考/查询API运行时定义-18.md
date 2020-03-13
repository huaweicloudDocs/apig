# 查询API运行时定义<a name="apig-phapi-180911219"></a>

## 功能介绍<a name="section56312882"></a>

查看指定的API在指定的环境上的运行时定义，默认查询RELEASE环境上的运行时定义。

API的定义分为临时定义和运行时定义，分别代表如下含义：

-   临时定义：API在编辑中的定义，表示用户最后一次编辑后的API的状态
-   运行时定义：API在发布到某个环境时，对发布时的API的临时定义进行快照，固化出来的API的状态。

访问某个环境上的API，其实访问的就是其运行时的定义

## URI<a name="section37053890"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table61687544"></a>
<table><thead align="left"><tr id="row6551303"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p60893511"><a name="p60893511"></a><a name="p60893511"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p33427368"><a name="p33427368"></a><a name="p33427368"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row23262289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p5197291"><a name="p5197291"></a><a name="p5197291"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p18327454"><a name="p18327454"></a><a name="p18327454"></a><span id="ph4785655184120"><a name="ph4785655184120"></a><a name="ph4785655184120"></a>/v1/{project_id}/apigw/instances/{instance_id}</span>/apis/runtime/{id}[?env_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：env\_id。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table8128785"></a>
<table><thead align="left"><tr id="row50936577"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p32222095"><a name="p32222095"></a><a name="p32222095"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.07%" id="mcps1.2.5.1.2"><p id="p59852877"><a name="p59852877"></a><a name="p59852877"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.46%" id="mcps1.2.5.1.3"><p id="p16244835"><a name="p16244835"></a><a name="p16244835"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.47%" id="mcps1.2.5.1.4"><p id="p40763258"><a name="p40763258"></a><a name="p40763258"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19690162212206"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.46%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.47%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row213672212203"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.46%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.47%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row13489593"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p18915273"><a name="p18915273"></a><a name="p18915273"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.07%" headers="mcps1.2.5.1.2 "><p id="p55742162"><a name="p55742162"></a><a name="p55742162"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.46%" headers="mcps1.2.5.1.3 "><p id="p18821243"><a name="p18821243"></a><a name="p18821243"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.47%" headers="mcps1.2.5.1.4 "><p id="p48125676"><a name="p48125676"></a><a name="p48125676"></a>API的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section65049557"></a>

**表 3**  参数说明

<a name="table309072"></a>
<table><thead align="left"><tr id="row29526596"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p42844056"><a name="p42844056"></a><a name="p42844056"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p47816505"><a name="p47816505"></a><a name="p47816505"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p47931662"><a name="p47931662"></a><a name="p47931662"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p57259391"><a name="p57259391"></a><a name="p57259391"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7499126"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p3449432"><a name="p3449432"></a><a name="p3449432"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p10968591"><a name="p10968591"></a><a name="p10968591"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p16040707"><a name="p16040707"></a><a name="p16040707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p24228891"><a name="p24228891"></a><a name="p24228891"></a>API的发布环境编号</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section34522802"></a>

**表 4**  参数说明

<a name="table11945837"></a>
<table><thead align="left"><tr id="row18624964"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p32227090"><a name="p32227090"></a><a name="p32227090"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p60257464"><a name="p60257464"></a><a name="p60257464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p49016415"><a name="p49016415"></a><a name="p49016415"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10906670"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11025102"><a name="p11025102"></a><a name="p11025102"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20618087"><a name="p20618087"></a><a name="p20618087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p59452320"><a name="p59452320"></a><a name="p59452320"></a>API编号</p>
</td>
</tr>
<tr id="row65308832"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55524012"><a name="p55524012"></a><a name="p55524012"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1151149"><a name="p1151149"></a><a name="p1151149"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p26134283"><a name="p26134283"></a><a name="p26134283"></a>API名称</p>
</td>
</tr>
<tr id="row33881960"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p60084252"><a name="p60084252"></a><a name="p60084252"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34986207"><a name="p34986207"></a><a name="p34986207"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15310556"><a name="p15310556"></a><a name="p15310556"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row3577279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p21324163"><a name="p21324163"></a><a name="p21324163"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p49535636"><a name="p49535636"></a><a name="p49535636"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52963545"><a name="p52963545"></a><a name="p52963545"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row2200986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44062206"><a name="p44062206"></a><a name="p44062206"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12268934"><a name="p12268934"></a><a name="p12268934"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54259611"><a name="p54259611"></a><a name="p54259611"></a>API类型</p>
</td>
</tr>
<tr id="row18574453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28135752"><a name="p28135752"></a><a name="p28135752"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64403419"><a name="p64403419"></a><a name="p64403419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p49294422"><a name="p49294422"></a><a name="p49294422"></a>API版本</p>
</td>
</tr>
<tr id="row40996618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p32391798"><a name="p32391798"></a><a name="p32391798"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6489949"><a name="p6489949"></a><a name="p6489949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p55923881"><a name="p55923881"></a><a name="p55923881"></a>API访问协议</p>
</td>
</tr>
<tr id="row33552889"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p33429463"><a name="p33429463"></a><a name="p33429463"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23431949"><a name="p23431949"></a><a name="p23431949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18939716"><a name="p18939716"></a><a name="p18939716"></a>API请求方式</p>
</td>
</tr>
<tr id="row36239719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p49736130"><a name="p49736130"></a><a name="p49736130"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2094705"><a name="p2094705"></a><a name="p2094705"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p35453405"><a name="p35453405"></a><a name="p35453405"></a>API访问地址</p>
</td>
</tr>
<tr id="row50645189"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8619606"><a name="p8619606"></a><a name="p8619606"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p27099480"><a name="p27099480"></a><a name="p27099480"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p47574258"><a name="p47574258"></a><a name="p47574258"></a>API认证方式</p>
</td>
</tr>
<tr id="row1856191962514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p45549491969"><a name="p45549491969"></a><a name="p45549491969"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19554194910611"><a name="p19554194910611"></a><a name="p19554194910611"></a>字段数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p155541490617"><a name="p155541490617"></a><a name="p155541490617"></a>API认证方式参数</p>
</td>
</tr>
<tr id="row3470115593817"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4426105522114"><a name="p4426105522114"></a><a name="p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p118419143911"><a name="p118419143911"></a><a name="p118419143911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11470115583820"><a name="p11470115583820"></a><a name="p11470115583820"></a>前端自定义认证对象的ID</p>
</td>
</tr>
<tr id="row25515144"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53460794"><a name="p53460794"></a><a name="p53460794"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35357081"><a name="p35357081"></a><a name="p35357081"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p45351308"><a name="p45351308"></a><a name="p45351308"></a>API匹配方式</p>
</td>
</tr>
<tr id="row40426262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53301766"><a name="p53301766"></a><a name="p53301766"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22475799"><a name="p22475799"></a><a name="p22475799"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8600432"><a name="p8600432"></a><a name="p8600432"></a>API描述</p>
</td>
</tr>
<tr id="row10295032"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28591249"><a name="p28591249"></a><a name="p28591249"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34189831"><a name="p34189831"></a><a name="p34189831"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17912897"><a name="p17912897"></a><a name="p17912897"></a>后端类型</p>
</td>
</tr>
<tr id="row26998347"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39382503"><a name="p39382503"></a><a name="p39382503"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35866171"><a name="p35866171"></a><a name="p35866171"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19478768"><a name="p19478768"></a><a name="p19478768"></a>发布的环境名</p>
</td>
</tr>
<tr id="row41091190"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40052127"><a name="p40052127"></a><a name="p40052127"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22996860"><a name="p22996860"></a><a name="p22996860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p50806390"><a name="p50806390"></a><a name="p50806390"></a>发布的环境id</p>
</td>
</tr>
<tr id="row54604329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p60874520"><a name="p60874520"></a><a name="p60874520"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31889112"><a name="p31889112"></a><a name="p31889112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p32881297"><a name="p32881297"></a><a name="p32881297"></a>发布记录的编号</p>
</td>
</tr>
<tr id="row660031719333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7679321181114"><a name="p7679321181114"></a><a name="p7679321181114"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p166791021161110"><a name="p166791021161110"></a><a name="p166791021161110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1167913211111"><a name="p1167913211111"></a><a name="p1167913211111"></a>服务名称标签，待废弃字段</p>
</td>
</tr>
<tr id="row12222174304613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5689175210267"><a name="p5689175210267"></a><a name="p5689175210267"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p969065252610"><a name="p969065252610"></a><a name="p969065252610"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10599103122713"><a name="p10599103122713"></a><a name="p10599103122713"></a>标签</p>
</td>
</tr>
<tr id="row37247202339"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p172881819162714"><a name="p172881819162714"></a><a name="p172881819162714"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p163043196278"><a name="p163043196278"></a><a name="p163043196278"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13320121932715"><a name="p13320121932715"></a><a name="p13320121932715"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="row1749718315379"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p105561154343"><a name="p105561154343"></a><a name="p105561154343"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p75719510345"><a name="p75719510345"></a><a name="p75719510345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1571450346"><a name="p1571450346"></a><a name="p1571450346"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
</td>
</tr>
<tr id="row140423763710"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p106341354349"><a name="p106341354349"></a><a name="p106341354349"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1463416511341"><a name="p1463416511341"></a><a name="p1463416511341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46509516343"><a name="p46509516343"></a><a name="p46509516343"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
<tr id="row19654193413373"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19696185133419"><a name="p19696185133419"></a><a name="p19696185133419"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p369665183416"><a name="p369665183416"></a><a name="p369665183416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p77123514347"><a name="p77123514347"></a><a name="p77123514347"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="row19308181115391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p193081111183920"><a name="p193081111183920"></a><a name="p193081111183920"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1330871173912"><a name="p1330871173912"></a><a name="p1330871173912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7308111123910"><a name="p7308111123910"></a><a name="p7308111123910"></a>分组的二级域名</p>
</td>
</tr>
<tr id="row3996134219376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13999938164017"><a name="p13999938164017"></a><a name="p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1999203815404"><a name="p1999203815404"></a><a name="p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11999143884013"><a name="p11999143884013"></a><a name="p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  req\_params参数说明

<a name="table197251634194412"></a>
<table><thead align="left"><tr id="row2075603420446"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p11756234184411"><a name="p11756234184411"></a><a name="p11756234184411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p777143420447"><a name="p777143420447"></a><a name="p777143420447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p5771193415446"><a name="p5771193415446"></a><a name="p5771193415446"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row85313200454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1753320144511"><a name="p1753320144511"></a><a name="p1753320144511"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p75302015450"><a name="p75302015450"></a><a name="p75302015450"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p653162014451"><a name="p653162014451"></a><a name="p653162014451"></a>参数编号</p>
</td>
</tr>
<tr id="row8786123464413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p578618344445"><a name="p578618344445"></a><a name="p578618344445"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1480313412443"><a name="p1480313412443"></a><a name="p1480313412443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48033344445"><a name="p48033344445"></a><a name="p48033344445"></a>参数名称</p>
</td>
</tr>
<tr id="row13818193434411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p781810341448"><a name="p781810341448"></a><a name="p781810341448"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18342034114419"><a name="p18342034114419"></a><a name="p18342034114419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p083493413441"><a name="p083493413441"></a><a name="p083493413441"></a>参数类型</p>
</td>
</tr>
<tr id="row17850234124414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18865203414418"><a name="p18865203414418"></a><a name="p18865203414418"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16881203415443"><a name="p16881203415443"></a><a name="p16881203415443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p788120340445"><a name="p788120340445"></a><a name="p788120340445"></a>参数位置</p>
</td>
</tr>
<tr id="row99121534134414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18912934114419"><a name="p18912934114419"></a><a name="p18912934114419"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p139281534104415"><a name="p139281534104415"></a><a name="p139281534104415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1592853454412"><a name="p1592853454412"></a><a name="p1592853454412"></a>参数默认值</p>
</td>
</tr>
<tr id="row1594315349446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p994311348442"><a name="p994311348442"></a><a name="p994311348442"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1495973414419"><a name="p1495973414419"></a><a name="p1495973414419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1695953413449"><a name="p1695953413449"></a><a name="p1695953413449"></a>参数示例值</p>
</td>
</tr>
<tr id="row1959173474410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2974183417445"><a name="p2974183417445"></a><a name="p2974183417445"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13974143417443"><a name="p13974143417443"></a><a name="p13974143417443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p699053414444"><a name="p699053414444"></a><a name="p699053414444"></a>是否必须</p>
</td>
</tr>
<tr id="row662354446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p66183524412"><a name="p66183524412"></a><a name="p66183524412"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p32133519447"><a name="p32133519447"></a><a name="p32133519447"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18371535124417"><a name="p18371535124417"></a><a name="p18371535124417"></a>是否开启校验</p>
</td>
</tr>
<tr id="row1053435144414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p653133513441"><a name="p653133513441"></a><a name="p653133513441"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1867183512446"><a name="p1867183512446"></a><a name="p1867183512446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p567123584420"><a name="p567123584420"></a><a name="p567123584420"></a>描述</p>
</td>
</tr>
<tr id="row7100203515443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p181002035154415"><a name="p181002035154415"></a><a name="p181002035154415"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p161151635164413"><a name="p161151635164413"></a><a name="p161151635164413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9115133544413"><a name="p9115133544413"></a><a name="p9115133544413"></a>参数枚举值</p>
</td>
</tr>
<tr id="row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p151311235144415"><a name="p151311235144415"></a><a name="p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p713112353443"><a name="p713112353443"></a><a name="p713112353443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p01464350441"><a name="p01464350441"></a><a name="p01464350441"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8146203564415"><a name="p8146203564415"></a><a name="p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31627353442"><a name="p31627353442"></a><a name="p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p117823511445"><a name="p117823511445"></a><a name="p117823511445"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p61782355443"><a name="p61782355443"></a><a name="p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p201932035194417"><a name="p201932035194417"></a><a name="p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1119312351443"><a name="p1119312351443"></a><a name="p1119312351443"></a>参数最小长度</p>
</td>
</tr>
<tr id="row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12209535144412"><a name="p12209535144412"></a><a name="p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12251035164419"><a name="p12251035164419"></a><a name="p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13225335194419"><a name="p13225335194419"></a><a name="p13225335194419"></a>参数最大长度</p>
</td>
</tr>
<tr id="row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52401735134413"><a name="p52401735134413"></a><a name="p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12240153510443"><a name="p12240153510443"></a><a name="p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1256035204417"><a name="p1256035204417"></a><a name="p1256035204417"></a>正则校验规则</p>
</td>
</tr>
<tr id="row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p202561335114413"><a name="p202561335114413"></a><a name="p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16271035114412"><a name="p16271035114412"></a><a name="p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1628793511445"><a name="p1628793511445"></a><a name="p1628793511445"></a>JSON校验规则</p>
</td>
</tr>
</tbody>
</table>

**表 6**  auth\_opt参数说明

<a name="table3296221173715"></a>
<table><thead align="left"><tr id="row829715213377"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p17297192173718"><a name="p17297192173718"></a><a name="p17297192173718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p9297821143718"><a name="p9297821143718"></a><a name="p9297821143718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p4297152163717"><a name="p4297152163717"></a><a name="p4297152163717"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4297421123717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1848964315375"><a name="p1848964315375"></a><a name="p1848964315375"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4489164310372"><a name="p4489164310372"></a><a name="p4489164310372"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1948934316376"><a name="p1948934316376"></a><a name="p1948934316376"></a>AppCode简易认证类型</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "name": "market_api01",
  "type": 1,
  "version": "V0.0.1",
  "req_protocol": "HTTPS",
  "req_method": "GET",
  "req_uri": "/test01",
  "auth_type": "APP",
  "auth_opt": {
    "app_code_auth_type": "HEADER"
  },
  "tags": ["APIG-SN-test", "test"],
  "cors": true,
  "match_mode": "NORMAL",
  "backend_type": "MOCK",
  "remark": "market_api01",
  "group_id": "7f848adc971749cda9c6aff3877cfc3e",
  "body_remark": "market_api01",
  "result_normal_sample": "success",
  "result_failure_sample": "",
  "id": "0e51b689e0784bc884f43756bbf34fa5",
  "group_name": "market_group01",
  "run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
  "run_env_name": "RELEASE",
  "publish_id": "f07eb9f5e5ba4bbfbe89326f5cae99c7",
  "sl_domain": "61297835ff1e4905b6f635dbcdf1777e.apigw.example.com",
  "req_params": [
    {
      "name": "project_id",
      "type": "STRING",
      "location": "PATH",
      "default_value": "",
      "sample_value": "",
      "required": 1,
      "valid_enable": 2,
      "remark": "",
      "enumerations": "",
      "min_num": 0,
      "max_num": 0,
      "min_size": 0,
      "max_size": 0,
      "regular": "",
      "json_schema": "",
      "id": "2a61905ea2304186a9422faba2940735"
    }
  ]
}
```

## 状态码<a name="section48575109"></a>

**表 7**  返回消息说明

<a name="table5357896"></a>
<table><thead align="left"><tr id="row27259487"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p60534834"><a name="p60534834"></a><a name="p60534834"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p4374530"><a name="p4374530"></a><a name="p4374530"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18792630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p45808055"><a name="p45808055"></a><a name="p45808055"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row40966733"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p29971116"><a name="p29971116"></a><a name="p29971116"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p29757115610"><a name="p29757115610"></a><a name="p29757115610"></a>Bad Request</p>
</td>
</tr>
<tr id="row38563414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p36628845"><a name="p36628845"></a><a name="p36628845"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row60209613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p45140486"><a name="p45140486"></a><a name="p45140486"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row24071607"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3643149"><a name="p3643149"></a><a name="p3643149"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p26659623"><a name="p26659623"></a><a name="p26659623"></a>Not Found</p>
</td>
</tr>
</tbody>
</table>

