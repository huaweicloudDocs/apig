# 查询API运行时定义<a name="ZH-CN_TOPIC_0000001082221177"></a>

## 功能介绍<a name="zh-cn_topic_0127584628_section56312882"></a>

查看指定的API在指定的环境上的运行时定义，默认查询RELEASE环境上的运行时定义。

API的定义分为临时定义和运行时定义，分别代表如下含义：

-   临时定义：API在编辑中的定义，表示用户最后一次编辑后的API的状态
-   运行时定义：API在发布到某个环境时，对发布时的API的临时定义进行快照，固化出来的API的状态。

访问某个环境上的API，其实访问的就是其运行时的定义

## URI<a name="zh-cn_topic_0127584628_section37053890"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0127584628_table61687544"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127584628_row6551303"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127584628_p60893511"><a name="zh-cn_topic_0127584628_p60893511"></a><a name="zh-cn_topic_0127584628_p60893511"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127584628_p33427368"><a name="zh-cn_topic_0127584628_p33427368"></a><a name="zh-cn_topic_0127584628_p33427368"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127584628_row23262289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127584628_p5197291"><a name="zh-cn_topic_0127584628_p5197291"></a><a name="zh-cn_topic_0127584628_p5197291"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127584628_p18327454"><a name="zh-cn_topic_0127584628_p18327454"></a><a name="zh-cn_topic_0127584628_p18327454"></a>/v1.0/apigw/apis/runtime/{id}[?env_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：env\_id。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0127584628_table8128785"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127584628_row50936577"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0127584628_p32222095"><a name="zh-cn_topic_0127584628_p32222095"></a><a name="zh-cn_topic_0127584628_p32222095"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0127584628_p59852877"><a name="zh-cn_topic_0127584628_p59852877"></a><a name="zh-cn_topic_0127584628_p59852877"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0127584628_p16244835"><a name="zh-cn_topic_0127584628_p16244835"></a><a name="zh-cn_topic_0127584628_p16244835"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0127584628_p40763258"><a name="zh-cn_topic_0127584628_p40763258"></a><a name="zh-cn_topic_0127584628_p40763258"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127584628_row13489593"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127584628_p18915273"><a name="zh-cn_topic_0127584628_p18915273"></a><a name="zh-cn_topic_0127584628_p18915273"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127584628_p55742162"><a name="zh-cn_topic_0127584628_p55742162"></a><a name="zh-cn_topic_0127584628_p55742162"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127584628_p18821243"><a name="zh-cn_topic_0127584628_p18821243"></a><a name="zh-cn_topic_0127584628_p18821243"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127584628_p48125676"><a name="zh-cn_topic_0127584628_p48125676"></a><a name="zh-cn_topic_0127584628_p48125676"></a>API的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0127584628_section65049557"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0127584628_table309072"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127584628_row29526596"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0127584628_p42844056"><a name="zh-cn_topic_0127584628_p42844056"></a><a name="zh-cn_topic_0127584628_p42844056"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0127584628_p47816505"><a name="zh-cn_topic_0127584628_p47816505"></a><a name="zh-cn_topic_0127584628_p47816505"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0127584628_p47931662"><a name="zh-cn_topic_0127584628_p47931662"></a><a name="zh-cn_topic_0127584628_p47931662"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0127584628_p57259391"><a name="zh-cn_topic_0127584628_p57259391"></a><a name="zh-cn_topic_0127584628_p57259391"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127584628_row7499126"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127584628_p3449432"><a name="zh-cn_topic_0127584628_p3449432"></a><a name="zh-cn_topic_0127584628_p3449432"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127584628_p10968591"><a name="zh-cn_topic_0127584628_p10968591"></a><a name="zh-cn_topic_0127584628_p10968591"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127584628_p16040707"><a name="zh-cn_topic_0127584628_p16040707"></a><a name="zh-cn_topic_0127584628_p16040707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127584628_p24228891"><a name="zh-cn_topic_0127584628_p24228891"></a><a name="zh-cn_topic_0127584628_p24228891"></a>API的发布环境编号</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0127584628_section34522802"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0127584628_table11945837"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127584628_row18624964"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0127584628_p32227090"><a name="zh-cn_topic_0127584628_p32227090"></a><a name="zh-cn_topic_0127584628_p32227090"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0127584628_p60257464"><a name="zh-cn_topic_0127584628_p60257464"></a><a name="zh-cn_topic_0127584628_p60257464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0127584628_p49016415"><a name="zh-cn_topic_0127584628_p49016415"></a><a name="zh-cn_topic_0127584628_p49016415"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127584628_row10906670"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p11025102"><a name="zh-cn_topic_0127584628_p11025102"></a><a name="zh-cn_topic_0127584628_p11025102"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p20618087"><a name="zh-cn_topic_0127584628_p20618087"></a><a name="zh-cn_topic_0127584628_p20618087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p59452320"><a name="zh-cn_topic_0127584628_p59452320"></a><a name="zh-cn_topic_0127584628_p59452320"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row65308832"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p55524012"><a name="zh-cn_topic_0127584628_p55524012"></a><a name="zh-cn_topic_0127584628_p55524012"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p1151149"><a name="zh-cn_topic_0127584628_p1151149"></a><a name="zh-cn_topic_0127584628_p1151149"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p26134283"><a name="zh-cn_topic_0127584628_p26134283"></a><a name="zh-cn_topic_0127584628_p26134283"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row33881960"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p60084252"><a name="zh-cn_topic_0127584628_p60084252"></a><a name="zh-cn_topic_0127584628_p60084252"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p34986207"><a name="zh-cn_topic_0127584628_p34986207"></a><a name="zh-cn_topic_0127584628_p34986207"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p15310556"><a name="zh-cn_topic_0127584628_p15310556"></a><a name="zh-cn_topic_0127584628_p15310556"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row3577279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p21324163"><a name="zh-cn_topic_0127584628_p21324163"></a><a name="zh-cn_topic_0127584628_p21324163"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p49535636"><a name="zh-cn_topic_0127584628_p49535636"></a><a name="zh-cn_topic_0127584628_p49535636"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p52963545"><a name="zh-cn_topic_0127584628_p52963545"></a><a name="zh-cn_topic_0127584628_p52963545"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row2200986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p44062206"><a name="zh-cn_topic_0127584628_p44062206"></a><a name="zh-cn_topic_0127584628_p44062206"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p12268934"><a name="zh-cn_topic_0127584628_p12268934"></a><a name="zh-cn_topic_0127584628_p12268934"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p54259611"><a name="zh-cn_topic_0127584628_p54259611"></a><a name="zh-cn_topic_0127584628_p54259611"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row18574453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p28135752"><a name="zh-cn_topic_0127584628_p28135752"></a><a name="zh-cn_topic_0127584628_p28135752"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p64403419"><a name="zh-cn_topic_0127584628_p64403419"></a><a name="zh-cn_topic_0127584628_p64403419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p49294422"><a name="zh-cn_topic_0127584628_p49294422"></a><a name="zh-cn_topic_0127584628_p49294422"></a>API版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row40996618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p32391798"><a name="zh-cn_topic_0127584628_p32391798"></a><a name="zh-cn_topic_0127584628_p32391798"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p6489949"><a name="zh-cn_topic_0127584628_p6489949"></a><a name="zh-cn_topic_0127584628_p6489949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p55923881"><a name="zh-cn_topic_0127584628_p55923881"></a><a name="zh-cn_topic_0127584628_p55923881"></a>API访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row33552889"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p33429463"><a name="zh-cn_topic_0127584628_p33429463"></a><a name="zh-cn_topic_0127584628_p33429463"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p23431949"><a name="zh-cn_topic_0127584628_p23431949"></a><a name="zh-cn_topic_0127584628_p23431949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p18939716"><a name="zh-cn_topic_0127584628_p18939716"></a><a name="zh-cn_topic_0127584628_p18939716"></a>API请求方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row36239719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p49736130"><a name="zh-cn_topic_0127584628_p49736130"></a><a name="zh-cn_topic_0127584628_p49736130"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p2094705"><a name="zh-cn_topic_0127584628_p2094705"></a><a name="zh-cn_topic_0127584628_p2094705"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p35453405"><a name="zh-cn_topic_0127584628_p35453405"></a><a name="zh-cn_topic_0127584628_p35453405"></a>API访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row50645189"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p8619606"><a name="zh-cn_topic_0127584628_p8619606"></a><a name="zh-cn_topic_0127584628_p8619606"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p27099480"><a name="zh-cn_topic_0127584628_p27099480"></a><a name="zh-cn_topic_0127584628_p27099480"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p47574258"><a name="zh-cn_topic_0127584628_p47574258"></a><a name="zh-cn_topic_0127584628_p47574258"></a>API认证方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row62411685519"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p45549491969"><a name="zh-cn_topic_0127584628_p45549491969"></a><a name="zh-cn_topic_0127584628_p45549491969"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p19554194910611"><a name="zh-cn_topic_0127584628_p19554194910611"></a><a name="zh-cn_topic_0127584628_p19554194910611"></a>字段数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p155541490617"><a name="zh-cn_topic_0127584628_p155541490617"></a><a name="zh-cn_topic_0127584628_p155541490617"></a>API认证方式参数</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row3470115593817"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p4426105522114"><a name="zh-cn_topic_0127584628_p4426105522114"></a><a name="zh-cn_topic_0127584628_p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p118419143911"><a name="zh-cn_topic_0127584628_p118419143911"></a><a name="zh-cn_topic_0127584628_p118419143911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p11470115583820"><a name="zh-cn_topic_0127584628_p11470115583820"></a><a name="zh-cn_topic_0127584628_p11470115583820"></a>前端自定义认证对象的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row25515144"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p53460794"><a name="zh-cn_topic_0127584628_p53460794"></a><a name="zh-cn_topic_0127584628_p53460794"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p35357081"><a name="zh-cn_topic_0127584628_p35357081"></a><a name="zh-cn_topic_0127584628_p35357081"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p45351308"><a name="zh-cn_topic_0127584628_p45351308"></a><a name="zh-cn_topic_0127584628_p45351308"></a>API匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row40426262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p53301766"><a name="zh-cn_topic_0127584628_p53301766"></a><a name="zh-cn_topic_0127584628_p53301766"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p22475799"><a name="zh-cn_topic_0127584628_p22475799"></a><a name="zh-cn_topic_0127584628_p22475799"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p8600432"><a name="zh-cn_topic_0127584628_p8600432"></a><a name="zh-cn_topic_0127584628_p8600432"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row10295032"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p28591249"><a name="zh-cn_topic_0127584628_p28591249"></a><a name="zh-cn_topic_0127584628_p28591249"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p34189831"><a name="zh-cn_topic_0127584628_p34189831"></a><a name="zh-cn_topic_0127584628_p34189831"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p17912897"><a name="zh-cn_topic_0127584628_p17912897"></a><a name="zh-cn_topic_0127584628_p17912897"></a>后端类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row26998347"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p39382503"><a name="zh-cn_topic_0127584628_p39382503"></a><a name="zh-cn_topic_0127584628_p39382503"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p35866171"><a name="zh-cn_topic_0127584628_p35866171"></a><a name="zh-cn_topic_0127584628_p35866171"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p19478768"><a name="zh-cn_topic_0127584628_p19478768"></a><a name="zh-cn_topic_0127584628_p19478768"></a>发布的环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row41091190"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p40052127"><a name="zh-cn_topic_0127584628_p40052127"></a><a name="zh-cn_topic_0127584628_p40052127"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p22996860"><a name="zh-cn_topic_0127584628_p22996860"></a><a name="zh-cn_topic_0127584628_p22996860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p50806390"><a name="zh-cn_topic_0127584628_p50806390"></a><a name="zh-cn_topic_0127584628_p50806390"></a>发布的环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row54604329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p60874520"><a name="zh-cn_topic_0127584628_p60874520"></a><a name="zh-cn_topic_0127584628_p60874520"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p31889112"><a name="zh-cn_topic_0127584628_p31889112"></a><a name="zh-cn_topic_0127584628_p31889112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p32881297"><a name="zh-cn_topic_0127584628_p32881297"></a><a name="zh-cn_topic_0127584628_p32881297"></a>发布记录的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row660031719333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p7679321181114"><a name="zh-cn_topic_0127584628_p7679321181114"></a><a name="zh-cn_topic_0127584628_p7679321181114"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p166791021161110"><a name="zh-cn_topic_0127584628_p166791021161110"></a><a name="zh-cn_topic_0127584628_p166791021161110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1167913211111"><a name="zh-cn_topic_0127584628_p1167913211111"></a><a name="zh-cn_topic_0127584628_p1167913211111"></a>服务名称标签，待废弃字段</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row12222174304613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p5689175210267"><a name="zh-cn_topic_0127584628_p5689175210267"></a><a name="zh-cn_topic_0127584628_p5689175210267"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p969065252610"><a name="zh-cn_topic_0127584628_p969065252610"></a><a name="zh-cn_topic_0127584628_p969065252610"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p10599103122713"><a name="zh-cn_topic_0127584628_p10599103122713"></a><a name="zh-cn_topic_0127584628_p10599103122713"></a>标签</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row37247202339"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p172881819162714"><a name="zh-cn_topic_0127584628_p172881819162714"></a><a name="zh-cn_topic_0127584628_p172881819162714"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p163043196278"><a name="zh-cn_topic_0127584628_p163043196278"></a><a name="zh-cn_topic_0127584628_p163043196278"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p13320121932715"><a name="zh-cn_topic_0127584628_p13320121932715"></a><a name="zh-cn_topic_0127584628_p13320121932715"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row1749718315379"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p105561154343"><a name="zh-cn_topic_0127584628_p105561154343"></a><a name="zh-cn_topic_0127584628_p105561154343"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p75719510345"><a name="zh-cn_topic_0127584628_p75719510345"></a><a name="zh-cn_topic_0127584628_p75719510345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1571450346"><a name="zh-cn_topic_0127584628_p1571450346"></a><a name="zh-cn_topic_0127584628_p1571450346"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row140423763710"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p106341354349"><a name="zh-cn_topic_0127584628_p106341354349"></a><a name="zh-cn_topic_0127584628_p106341354349"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p1463416511341"><a name="zh-cn_topic_0127584628_p1463416511341"></a><a name="zh-cn_topic_0127584628_p1463416511341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p46509516343"><a name="zh-cn_topic_0127584628_p46509516343"></a><a name="zh-cn_topic_0127584628_p46509516343"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row19654193413373"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p19696185133419"><a name="zh-cn_topic_0127584628_p19696185133419"></a><a name="zh-cn_topic_0127584628_p19696185133419"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p369665183416"><a name="zh-cn_topic_0127584628_p369665183416"></a><a name="zh-cn_topic_0127584628_p369665183416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p77123514347"><a name="zh-cn_topic_0127584628_p77123514347"></a><a name="zh-cn_topic_0127584628_p77123514347"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row145818161028"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p1388814535919"><a name="zh-cn_topic_0127584628_p1388814535919"></a><a name="zh-cn_topic_0127584628_p1388814535919"></a>response_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p5888345115911"><a name="zh-cn_topic_0127584628_p5888345115911"></a><a name="zh-cn_topic_0127584628_p5888345115911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p14331422017"><a name="zh-cn_topic_0127584628_p14331422017"></a><a name="zh-cn_topic_0127584628_p14331422017"></a>分组自定义响应ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row19308181115391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p193081111183920"><a name="zh-cn_topic_0127584628_p193081111183920"></a><a name="zh-cn_topic_0127584628_p193081111183920"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p1330871173912"><a name="zh-cn_topic_0127584628_p1330871173912"></a><a name="zh-cn_topic_0127584628_p1330871173912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p7308111123910"><a name="zh-cn_topic_0127584628_p7308111123910"></a><a name="zh-cn_topic_0127584628_p7308111123910"></a>分组的二级域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row178881548184514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p148891448174511"><a name="zh-cn_topic_0127584628_p148891448174511"></a><a name="zh-cn_topic_0127584628_p148891448174511"></a>sl_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p0889114813459"><a name="zh-cn_topic_0127584628_p0889114813459"></a><a name="zh-cn_topic_0127584628_p0889114813459"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p18960185694515"><a name="zh-cn_topic_0127584628_p18960185694515"></a><a name="zh-cn_topic_0127584628_p18960185694515"></a>分组的二级域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row3996134219376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p13999938164017"><a name="zh-cn_topic_0127584628_p13999938164017"></a><a name="zh-cn_topic_0127584628_p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p1999203815404"><a name="zh-cn_topic_0127584628_p1999203815404"></a><a name="zh-cn_topic_0127584628_p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p11999143884013"><a name="zh-cn_topic_0127584628_p11999143884013"></a><a name="zh-cn_topic_0127584628_p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  req\_params参数说明

<a name="zh-cn_topic_0127584628_table197251634194412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127584628_row2075603420446"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0127584628_p11756234184411"><a name="zh-cn_topic_0127584628_p11756234184411"></a><a name="zh-cn_topic_0127584628_p11756234184411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0127584628_p777143420447"><a name="zh-cn_topic_0127584628_p777143420447"></a><a name="zh-cn_topic_0127584628_p777143420447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0127584628_p5771193415446"><a name="zh-cn_topic_0127584628_p5771193415446"></a><a name="zh-cn_topic_0127584628_p5771193415446"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127584628_row85313200454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p1753320144511"><a name="zh-cn_topic_0127584628_p1753320144511"></a><a name="zh-cn_topic_0127584628_p1753320144511"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p75302015450"><a name="zh-cn_topic_0127584628_p75302015450"></a><a name="zh-cn_topic_0127584628_p75302015450"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p653162014451"><a name="zh-cn_topic_0127584628_p653162014451"></a><a name="zh-cn_topic_0127584628_p653162014451"></a>参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row8786123464413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p578618344445"><a name="zh-cn_topic_0127584628_p578618344445"></a><a name="zh-cn_topic_0127584628_p578618344445"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p1480313412443"><a name="zh-cn_topic_0127584628_p1480313412443"></a><a name="zh-cn_topic_0127584628_p1480313412443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p48033344445"><a name="zh-cn_topic_0127584628_p48033344445"></a><a name="zh-cn_topic_0127584628_p48033344445"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row13818193434411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p781810341448"><a name="zh-cn_topic_0127584628_p781810341448"></a><a name="zh-cn_topic_0127584628_p781810341448"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p18342034114419"><a name="zh-cn_topic_0127584628_p18342034114419"></a><a name="zh-cn_topic_0127584628_p18342034114419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p083493413441"><a name="zh-cn_topic_0127584628_p083493413441"></a><a name="zh-cn_topic_0127584628_p083493413441"></a>参数类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row17850234124414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p18865203414418"><a name="zh-cn_topic_0127584628_p18865203414418"></a><a name="zh-cn_topic_0127584628_p18865203414418"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p16881203415443"><a name="zh-cn_topic_0127584628_p16881203415443"></a><a name="zh-cn_topic_0127584628_p16881203415443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p788120340445"><a name="zh-cn_topic_0127584628_p788120340445"></a><a name="zh-cn_topic_0127584628_p788120340445"></a>参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row99121534134414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p18912934114419"><a name="zh-cn_topic_0127584628_p18912934114419"></a><a name="zh-cn_topic_0127584628_p18912934114419"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p139281534104415"><a name="zh-cn_topic_0127584628_p139281534104415"></a><a name="zh-cn_topic_0127584628_p139281534104415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1592853454412"><a name="zh-cn_topic_0127584628_p1592853454412"></a><a name="zh-cn_topic_0127584628_p1592853454412"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row1594315349446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p994311348442"><a name="zh-cn_topic_0127584628_p994311348442"></a><a name="zh-cn_topic_0127584628_p994311348442"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p1495973414419"><a name="zh-cn_topic_0127584628_p1495973414419"></a><a name="zh-cn_topic_0127584628_p1495973414419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1695953413449"><a name="zh-cn_topic_0127584628_p1695953413449"></a><a name="zh-cn_topic_0127584628_p1695953413449"></a>参数示例值</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row1959173474410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p2974183417445"><a name="zh-cn_topic_0127584628_p2974183417445"></a><a name="zh-cn_topic_0127584628_p2974183417445"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p13974143417443"><a name="zh-cn_topic_0127584628_p13974143417443"></a><a name="zh-cn_topic_0127584628_p13974143417443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p699053414444"><a name="zh-cn_topic_0127584628_p699053414444"></a><a name="zh-cn_topic_0127584628_p699053414444"></a>是否必须</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row662354446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p66183524412"><a name="zh-cn_topic_0127584628_p66183524412"></a><a name="zh-cn_topic_0127584628_p66183524412"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p32133519447"><a name="zh-cn_topic_0127584628_p32133519447"></a><a name="zh-cn_topic_0127584628_p32133519447"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p18371535124417"><a name="zh-cn_topic_0127584628_p18371535124417"></a><a name="zh-cn_topic_0127584628_p18371535124417"></a>是否开启校验</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row1053435144414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p653133513441"><a name="zh-cn_topic_0127584628_p653133513441"></a><a name="zh-cn_topic_0127584628_p653133513441"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p1867183512446"><a name="zh-cn_topic_0127584628_p1867183512446"></a><a name="zh-cn_topic_0127584628_p1867183512446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p567123584420"><a name="zh-cn_topic_0127584628_p567123584420"></a><a name="zh-cn_topic_0127584628_p567123584420"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row7100203515443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p181002035154415"><a name="zh-cn_topic_0127584628_p181002035154415"></a><a name="zh-cn_topic_0127584628_p181002035154415"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p161151635164413"><a name="zh-cn_topic_0127584628_p161151635164413"></a><a name="zh-cn_topic_0127584628_p161151635164413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p9115133544413"><a name="zh-cn_topic_0127584628_p9115133544413"></a><a name="zh-cn_topic_0127584628_p9115133544413"></a>参数枚举值</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p151311235144415"><a name="zh-cn_topic_0127584628_p151311235144415"></a><a name="zh-cn_topic_0127584628_p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p713112353443"><a name="zh-cn_topic_0127584628_p713112353443"></a><a name="zh-cn_topic_0127584628_p713112353443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p01464350441"><a name="zh-cn_topic_0127584628_p01464350441"></a><a name="zh-cn_topic_0127584628_p01464350441"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p8146203564415"><a name="zh-cn_topic_0127584628_p8146203564415"></a><a name="zh-cn_topic_0127584628_p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p31627353442"><a name="zh-cn_topic_0127584628_p31627353442"></a><a name="zh-cn_topic_0127584628_p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p117823511445"><a name="zh-cn_topic_0127584628_p117823511445"></a><a name="zh-cn_topic_0127584628_p117823511445"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p61782355443"><a name="zh-cn_topic_0127584628_p61782355443"></a><a name="zh-cn_topic_0127584628_p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p201932035194417"><a name="zh-cn_topic_0127584628_p201932035194417"></a><a name="zh-cn_topic_0127584628_p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1119312351443"><a name="zh-cn_topic_0127584628_p1119312351443"></a><a name="zh-cn_topic_0127584628_p1119312351443"></a>参数最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p12209535144412"><a name="zh-cn_topic_0127584628_p12209535144412"></a><a name="zh-cn_topic_0127584628_p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p12251035164419"><a name="zh-cn_topic_0127584628_p12251035164419"></a><a name="zh-cn_topic_0127584628_p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p13225335194419"><a name="zh-cn_topic_0127584628_p13225335194419"></a><a name="zh-cn_topic_0127584628_p13225335194419"></a>参数最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p52401735134413"><a name="zh-cn_topic_0127584628_p52401735134413"></a><a name="zh-cn_topic_0127584628_p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p12240153510443"><a name="zh-cn_topic_0127584628_p12240153510443"></a><a name="zh-cn_topic_0127584628_p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1256035204417"><a name="zh-cn_topic_0127584628_p1256035204417"></a><a name="zh-cn_topic_0127584628_p1256035204417"></a>正则校验规则</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p202561335114413"><a name="zh-cn_topic_0127584628_p202561335114413"></a><a name="zh-cn_topic_0127584628_p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p16271035114412"><a name="zh-cn_topic_0127584628_p16271035114412"></a><a name="zh-cn_topic_0127584628_p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1628793511445"><a name="zh-cn_topic_0127584628_p1628793511445"></a><a name="zh-cn_topic_0127584628_p1628793511445"></a>JSON校验规则</p>
</td>
</tr>
</tbody>
</table>

**表 6**  auth\_opt参数说明

<a name="zh-cn_topic_0127584628_table3296221173715"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127584628_row829715213377"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0127584628_p17297192173718"><a name="zh-cn_topic_0127584628_p17297192173718"></a><a name="zh-cn_topic_0127584628_p17297192173718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0127584628_p9297821143718"><a name="zh-cn_topic_0127584628_p9297821143718"></a><a name="zh-cn_topic_0127584628_p9297821143718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0127584628_p4297152163717"><a name="zh-cn_topic_0127584628_p4297152163717"></a><a name="zh-cn_topic_0127584628_p4297152163717"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127584628_row4297421123717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127584628_p1848964315375"><a name="zh-cn_topic_0127584628_p1848964315375"></a><a name="zh-cn_topic_0127584628_p1848964315375"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127584628_p4489164310372"><a name="zh-cn_topic_0127584628_p4489164310372"></a><a name="zh-cn_topic_0127584628_p4489164310372"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127584628_p1948934316376"><a name="zh-cn_topic_0127584628_p1948934316376"></a><a name="zh-cn_topic_0127584628_p1948934316376"></a>AppCode简易认证类型</p>
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
  "sl_domains": ["61297835ff1e4905b6f635dbcdf1777e.apigw.example.com", "61297835ff1e4905b6f635dbcdf1777e.apigw.example.cn"],
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

## 状态码<a name="zh-cn_topic_0127584628_section48575109"></a>

**表 7**  返回消息说明

<a name="zh-cn_topic_0127584628_table5357896"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127584628_row27259487"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127584628_p60534834"><a name="zh-cn_topic_0127584628_p60534834"></a><a name="zh-cn_topic_0127584628_p60534834"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127584628_p4374530"><a name="zh-cn_topic_0127584628_p4374530"></a><a name="zh-cn_topic_0127584628_p4374530"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127584628_row18792630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127584628_p45808055"><a name="zh-cn_topic_0127584628_p45808055"></a><a name="zh-cn_topic_0127584628_p45808055"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127584628_p50988816"><a name="zh-cn_topic_0127584628_p50988816"></a><a name="zh-cn_topic_0127584628_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row40966733"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127584628_p29971116"><a name="zh-cn_topic_0127584628_p29971116"></a><a name="zh-cn_topic_0127584628_p29971116"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127584628_p29757115610"><a name="zh-cn_topic_0127584628_p29757115610"></a><a name="zh-cn_topic_0127584628_p29757115610"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row38563414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127584628_p36628845"><a name="zh-cn_topic_0127584628_p36628845"></a><a name="zh-cn_topic_0127584628_p36628845"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127584628_p9203142078"><a name="zh-cn_topic_0127584628_p9203142078"></a><a name="zh-cn_topic_0127584628_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row60209613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127584628_p45140486"><a name="zh-cn_topic_0127584628_p45140486"></a><a name="zh-cn_topic_0127584628_p45140486"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127584628_p13949586"><a name="zh-cn_topic_0127584628_p13949586"></a><a name="zh-cn_topic_0127584628_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0127584628_row24071607"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127584628_p3643149"><a name="zh-cn_topic_0127584628_p3643149"></a><a name="zh-cn_topic_0127584628_p3643149"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127584628_p26659623"><a name="zh-cn_topic_0127584628_p26659623"></a><a name="zh-cn_topic_0127584628_p26659623"></a>Not Found</p>
</td>
</tr>
</tbody>
</table>

