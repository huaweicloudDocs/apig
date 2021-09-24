# 查看API详情<a name="ZH-CN_TOPIC_0000001081976095"></a>

## 功能介绍<a name="zh-cn_topic_0118921498_section56312882"></a>

查看指定的API的详细信息。

## URI<a name="zh-cn_topic_0118921498_section37053890"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921498_table61687544"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row6551303"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921498_p60893511"><a name="zh-cn_topic_0118921498_p60893511"></a><a name="zh-cn_topic_0118921498_p60893511"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921498_p33427368"><a name="zh-cn_topic_0118921498_p33427368"></a><a name="zh-cn_topic_0118921498_p33427368"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row23262289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921498_p5197291"><a name="zh-cn_topic_0118921498_p5197291"></a><a name="zh-cn_topic_0118921498_p5197291"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921498_p18327454"><a name="zh-cn_topic_0118921498_p18327454"></a><a name="zh-cn_topic_0118921498_p18327454"></a>/v1.0/apigw/apis/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921498_table8128785"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row50936577"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921498_p32222095"><a name="zh-cn_topic_0118921498_p32222095"></a><a name="zh-cn_topic_0118921498_p32222095"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921498_p59852877"><a name="zh-cn_topic_0118921498_p59852877"></a><a name="zh-cn_topic_0118921498_p59852877"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921498_p16244835"><a name="zh-cn_topic_0118921498_p16244835"></a><a name="zh-cn_topic_0118921498_p16244835"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921498_p40763258"><a name="zh-cn_topic_0118921498_p40763258"></a><a name="zh-cn_topic_0118921498_p40763258"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row13489593"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921498_p18915273"><a name="zh-cn_topic_0118921498_p18915273"></a><a name="zh-cn_topic_0118921498_p18915273"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921498_p55742162"><a name="zh-cn_topic_0118921498_p55742162"></a><a name="zh-cn_topic_0118921498_p55742162"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921498_p18821243"><a name="zh-cn_topic_0118921498_p18821243"></a><a name="zh-cn_topic_0118921498_p18821243"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921498_p48125676"><a name="zh-cn_topic_0118921498_p48125676"></a><a name="zh-cn_topic_0118921498_p48125676"></a>API的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921498_section65049557"></a>

无

## 响应消息<a name="zh-cn_topic_0118921498_section34522802"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921498_table11945837"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row18624964"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p32227090"><a name="zh-cn_topic_0118921498_p32227090"></a><a name="zh-cn_topic_0118921498_p32227090"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p60257464"><a name="zh-cn_topic_0118921498_p60257464"></a><a name="zh-cn_topic_0118921498_p60257464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p49016415"><a name="zh-cn_topic_0118921498_p49016415"></a><a name="zh-cn_topic_0118921498_p49016415"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row10906670"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p11025102"><a name="zh-cn_topic_0118921498_p11025102"></a><a name="zh-cn_topic_0118921498_p11025102"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p20618087"><a name="zh-cn_topic_0118921498_p20618087"></a><a name="zh-cn_topic_0118921498_p20618087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p59452320"><a name="zh-cn_topic_0118921498_p59452320"></a><a name="zh-cn_topic_0118921498_p59452320"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row65308832"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p55524012"><a name="zh-cn_topic_0118921498_p55524012"></a><a name="zh-cn_topic_0118921498_p55524012"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1151149"><a name="zh-cn_topic_0118921498_p1151149"></a><a name="zh-cn_topic_0118921498_p1151149"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p26134283"><a name="zh-cn_topic_0118921498_p26134283"></a><a name="zh-cn_topic_0118921498_p26134283"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row33881960"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p60084252"><a name="zh-cn_topic_0118921498_p60084252"></a><a name="zh-cn_topic_0118921498_p60084252"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p34986207"><a name="zh-cn_topic_0118921498_p34986207"></a><a name="zh-cn_topic_0118921498_p34986207"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p15310556"><a name="zh-cn_topic_0118921498_p15310556"></a><a name="zh-cn_topic_0118921498_p15310556"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row3577279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p21324163"><a name="zh-cn_topic_0118921498_p21324163"></a><a name="zh-cn_topic_0118921498_p21324163"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p49535636"><a name="zh-cn_topic_0118921498_p49535636"></a><a name="zh-cn_topic_0118921498_p49535636"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p52963545"><a name="zh-cn_topic_0118921498_p52963545"></a><a name="zh-cn_topic_0118921498_p52963545"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row6909858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p22827665"><a name="zh-cn_topic_0118921498_p22827665"></a><a name="zh-cn_topic_0118921498_p22827665"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p37101609"><a name="zh-cn_topic_0118921498_p37101609"></a><a name="zh-cn_topic_0118921498_p37101609"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p52440337"><a name="zh-cn_topic_0118921498_p52440337"></a><a name="zh-cn_topic_0118921498_p52440337"></a>API的状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row2200986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p44062206"><a name="zh-cn_topic_0118921498_p44062206"></a><a name="zh-cn_topic_0118921498_p44062206"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p12268934"><a name="zh-cn_topic_0118921498_p12268934"></a><a name="zh-cn_topic_0118921498_p12268934"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p54259611"><a name="zh-cn_topic_0118921498_p54259611"></a><a name="zh-cn_topic_0118921498_p54259611"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row18574453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p28135752"><a name="zh-cn_topic_0118921498_p28135752"></a><a name="zh-cn_topic_0118921498_p28135752"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p64403419"><a name="zh-cn_topic_0118921498_p64403419"></a><a name="zh-cn_topic_0118921498_p64403419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p49294422"><a name="zh-cn_topic_0118921498_p49294422"></a><a name="zh-cn_topic_0118921498_p49294422"></a>API版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row40996618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p32391798"><a name="zh-cn_topic_0118921498_p32391798"></a><a name="zh-cn_topic_0118921498_p32391798"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p6489949"><a name="zh-cn_topic_0118921498_p6489949"></a><a name="zh-cn_topic_0118921498_p6489949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p55923881"><a name="zh-cn_topic_0118921498_p55923881"></a><a name="zh-cn_topic_0118921498_p55923881"></a>API访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row33552889"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p33429463"><a name="zh-cn_topic_0118921498_p33429463"></a><a name="zh-cn_topic_0118921498_p33429463"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p23431949"><a name="zh-cn_topic_0118921498_p23431949"></a><a name="zh-cn_topic_0118921498_p23431949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p18939716"><a name="zh-cn_topic_0118921498_p18939716"></a><a name="zh-cn_topic_0118921498_p18939716"></a>API请求方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row36239719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p49736130"><a name="zh-cn_topic_0118921498_p49736130"></a><a name="zh-cn_topic_0118921498_p49736130"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p2094705"><a name="zh-cn_topic_0118921498_p2094705"></a><a name="zh-cn_topic_0118921498_p2094705"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p35453405"><a name="zh-cn_topic_0118921498_p35453405"></a><a name="zh-cn_topic_0118921498_p35453405"></a>API访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row50645189"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p8619606"><a name="zh-cn_topic_0118921498_p8619606"></a><a name="zh-cn_topic_0118921498_p8619606"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p27099480"><a name="zh-cn_topic_0118921498_p27099480"></a><a name="zh-cn_topic_0118921498_p27099480"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p47574258"><a name="zh-cn_topic_0118921498_p47574258"></a><a name="zh-cn_topic_0118921498_p47574258"></a>API认证方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row5263105615455"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p45549491969"><a name="zh-cn_topic_0118921498_p45549491969"></a><a name="zh-cn_topic_0118921498_p45549491969"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p19554194910611"><a name="zh-cn_topic_0118921498_p19554194910611"></a><a name="zh-cn_topic_0118921498_p19554194910611"></a>字段数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p155541490617"><a name="zh-cn_topic_0118921498_p155541490617"></a><a name="zh-cn_topic_0118921498_p155541490617"></a>API认证方式参数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1552723173315"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p4426105522114"><a name="zh-cn_topic_0118921498_p4426105522114"></a><a name="zh-cn_topic_0118921498_p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p51041119338"><a name="zh-cn_topic_0118921498_p51041119338"></a><a name="zh-cn_topic_0118921498_p51041119338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p116491557133012"><a name="zh-cn_topic_0118921498_p116491557133012"></a><a name="zh-cn_topic_0118921498_p116491557133012"></a>前端自定义认证对象的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row25515144"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p53460794"><a name="zh-cn_topic_0118921498_p53460794"></a><a name="zh-cn_topic_0118921498_p53460794"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p35357081"><a name="zh-cn_topic_0118921498_p35357081"></a><a name="zh-cn_topic_0118921498_p35357081"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p45351308"><a name="zh-cn_topic_0118921498_p45351308"></a><a name="zh-cn_topic_0118921498_p45351308"></a>API匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row5508593"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p43542878"><a name="zh-cn_topic_0118921498_p43542878"></a><a name="zh-cn_topic_0118921498_p43542878"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p37312211"><a name="zh-cn_topic_0118921498_p37312211"></a><a name="zh-cn_topic_0118921498_p37312211"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p2390265"><a name="zh-cn_topic_0118921498_p2390265"></a><a name="zh-cn_topic_0118921498_p2390265"></a>API注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row21512390"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p64782007"><a name="zh-cn_topic_0118921498_p64782007"></a><a name="zh-cn_topic_0118921498_p64782007"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p12851246"><a name="zh-cn_topic_0118921498_p12851246"></a><a name="zh-cn_topic_0118921498_p12851246"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p34317968"><a name="zh-cn_topic_0118921498_p34317968"></a><a name="zh-cn_topic_0118921498_p34317968"></a>API修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row40426262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p53301766"><a name="zh-cn_topic_0118921498_p53301766"></a><a name="zh-cn_topic_0118921498_p53301766"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p22475799"><a name="zh-cn_topic_0118921498_p22475799"></a><a name="zh-cn_topic_0118921498_p22475799"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p8600432"><a name="zh-cn_topic_0118921498_p8600432"></a><a name="zh-cn_topic_0118921498_p8600432"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row10295032"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p28591249"><a name="zh-cn_topic_0118921498_p28591249"></a><a name="zh-cn_topic_0118921498_p28591249"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p34189831"><a name="zh-cn_topic_0118921498_p34189831"></a><a name="zh-cn_topic_0118921498_p34189831"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p17912897"><a name="zh-cn_topic_0118921498_p17912897"></a><a name="zh-cn_topic_0118921498_p17912897"></a>后端类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row26998347"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p39382503"><a name="zh-cn_topic_0118921498_p39382503"></a><a name="zh-cn_topic_0118921498_p39382503"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p35866171"><a name="zh-cn_topic_0118921498_p35866171"></a><a name="zh-cn_topic_0118921498_p35866171"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p19478768"><a name="zh-cn_topic_0118921498_p19478768"></a><a name="zh-cn_topic_0118921498_p19478768"></a>发布的环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row41091190"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p40052127"><a name="zh-cn_topic_0118921498_p40052127"></a><a name="zh-cn_topic_0118921498_p40052127"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p22996860"><a name="zh-cn_topic_0118921498_p22996860"></a><a name="zh-cn_topic_0118921498_p22996860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p50806390"><a name="zh-cn_topic_0118921498_p50806390"></a><a name="zh-cn_topic_0118921498_p50806390"></a>发布的环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row54604329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p60874520"><a name="zh-cn_topic_0118921498_p60874520"></a><a name="zh-cn_topic_0118921498_p60874520"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p31889112"><a name="zh-cn_topic_0118921498_p31889112"></a><a name="zh-cn_topic_0118921498_p31889112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p32881297"><a name="zh-cn_topic_0118921498_p32881297"></a><a name="zh-cn_topic_0118921498_p32881297"></a>发布记录的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row50078910"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p29859916"><a name="zh-cn_topic_0118921498_p29859916"></a><a name="zh-cn_topic_0118921498_p29859916"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p2734171"><a name="zh-cn_topic_0118921498_p2734171"></a><a name="zh-cn_topic_0118921498_p2734171"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p20141331"><a name="zh-cn_topic_0118921498_p20141331"></a><a name="zh-cn_topic_0118921498_p20141331"></a>是否需要编排</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row660031719333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p82576192276"><a name="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p82576192276"></a><a name="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p82576192276"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p1625711193277"><a name="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p1625711193277"></a><a name="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p1625711193277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p6273141922718"><a name="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p6273141922718"></a><a name="zh-cn_topic_0118921498_zh-cn_topic_0118921493_p6273141922718"></a>服务名称标签，待废弃字段</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row16495132510422"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p5689175210267"><a name="zh-cn_topic_0118921498_p5689175210267"></a><a name="zh-cn_topic_0118921498_p5689175210267"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p969065252610"><a name="zh-cn_topic_0118921498_p969065252610"></a><a name="zh-cn_topic_0118921498_p969065252610"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p10599103122713"><a name="zh-cn_topic_0118921498_p10599103122713"></a><a name="zh-cn_topic_0118921498_p10599103122713"></a>标签</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row37247202339"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p172881819162714"><a name="zh-cn_topic_0118921498_p172881819162714"></a><a name="zh-cn_topic_0118921498_p172881819162714"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p163043196278"><a name="zh-cn_topic_0118921498_p163043196278"></a><a name="zh-cn_topic_0118921498_p163043196278"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p13320121932715"><a name="zh-cn_topic_0118921498_p13320121932715"></a><a name="zh-cn_topic_0118921498_p13320121932715"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1749718315379"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p105561154343"><a name="zh-cn_topic_0118921498_p105561154343"></a><a name="zh-cn_topic_0118921498_p105561154343"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p75719510345"><a name="zh-cn_topic_0118921498_p75719510345"></a><a name="zh-cn_topic_0118921498_p75719510345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1571450346"><a name="zh-cn_topic_0118921498_p1571450346"></a><a name="zh-cn_topic_0118921498_p1571450346"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row140423763710"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p106341354349"><a name="zh-cn_topic_0118921498_p106341354349"></a><a name="zh-cn_topic_0118921498_p106341354349"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1463416511341"><a name="zh-cn_topic_0118921498_p1463416511341"></a><a name="zh-cn_topic_0118921498_p1463416511341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p46509516343"><a name="zh-cn_topic_0118921498_p46509516343"></a><a name="zh-cn_topic_0118921498_p46509516343"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row19654193413373"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p19696185133419"><a name="zh-cn_topic_0118921498_p19696185133419"></a><a name="zh-cn_topic_0118921498_p19696185133419"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p369665183416"><a name="zh-cn_topic_0118921498_p369665183416"></a><a name="zh-cn_topic_0118921498_p369665183416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p77123514347"><a name="zh-cn_topic_0118921498_p77123514347"></a><a name="zh-cn_topic_0118921498_p77123514347"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row38876451599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1388814535919"><a name="zh-cn_topic_0118921498_p1388814535919"></a><a name="zh-cn_topic_0118921498_p1388814535919"></a>response_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p5888345115911"><a name="zh-cn_topic_0118921498_p5888345115911"></a><a name="zh-cn_topic_0118921498_p5888345115911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p14331422017"><a name="zh-cn_topic_0118921498_p14331422017"></a><a name="zh-cn_topic_0118921498_p14331422017"></a>分组自定义响应ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row47054253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p53298164"><a name="zh-cn_topic_0118921498_p53298164"></a><a name="zh-cn_topic_0118921498_p53298164"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p22184056"><a name="zh-cn_topic_0118921498_p22184056"></a><a name="zh-cn_topic_0118921498_p22184056"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p52078112"><a name="zh-cn_topic_0118921498_p52078112"></a><a name="zh-cn_topic_0118921498_p52078112"></a>后端服务：web后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row66049829"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p48435967"><a name="zh-cn_topic_0118921498_p48435967"></a><a name="zh-cn_topic_0118921498_p48435967"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p30999282"><a name="zh-cn_topic_0118921498_p30999282"></a><a name="zh-cn_topic_0118921498_p30999282"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p27913893"><a name="zh-cn_topic_0118921498_p27913893"></a><a name="zh-cn_topic_0118921498_p27913893"></a>后端服务：MOCK详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row49898446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p15242308"><a name="zh-cn_topic_0118921498_p15242308"></a><a name="zh-cn_topic_0118921498_p15242308"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p26667472"><a name="zh-cn_topic_0118921498_p26667472"></a><a name="zh-cn_topic_0118921498_p26667472"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p12581591"><a name="zh-cn_topic_0118921498_p12581591"></a><a name="zh-cn_topic_0118921498_p12581591"></a>后端服务：函数工作流后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row3996134219376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p13999938164017"><a name="zh-cn_topic_0118921498_p13999938164017"></a><a name="zh-cn_topic_0118921498_p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1999203815404"><a name="zh-cn_topic_0118921498_p1999203815404"></a><a name="zh-cn_topic_0118921498_p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p11999143884013"><a name="zh-cn_topic_0118921498_p11999143884013"></a><a name="zh-cn_topic_0118921498_p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1854312455375"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p420294234017"><a name="zh-cn_topic_0118921498_p420294234017"></a><a name="zh-cn_topic_0118921498_p420294234017"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p17202184217401"><a name="zh-cn_topic_0118921498_p17202184217401"></a><a name="zh-cn_topic_0118921498_p17202184217401"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p112025421400"><a name="zh-cn_topic_0118921498_p112025421400"></a><a name="zh-cn_topic_0118921498_p112025421400"></a>API的后端参数列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row191941552203319"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p09691119194418"><a name="zh-cn_topic_0118921498_p09691119194418"></a><a name="zh-cn_topic_0118921498_p09691119194418"></a>policy_https</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p698531944420"><a name="zh-cn_topic_0118921498_p698531944420"></a><a name="zh-cn_topic_0118921498_p698531944420"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p142392054413"><a name="zh-cn_topic_0118921498_p142392054413"></a><a name="zh-cn_topic_0118921498_p142392054413"></a>web策略后端列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row172881855193313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p450102034414"><a name="zh-cn_topic_0118921498_p450102034414"></a><a name="zh-cn_topic_0118921498_p450102034414"></a>policy_mocks</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p966720104412"><a name="zh-cn_topic_0118921498_p966720104412"></a><a name="zh-cn_topic_0118921498_p966720104412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p01071207449"><a name="zh-cn_topic_0118921498_p01071207449"></a><a name="zh-cn_topic_0118921498_p01071207449"></a>mock策略后端列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row145517589338"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p18136122016449"><a name="zh-cn_topic_0118921498_p18136122016449"></a><a name="zh-cn_topic_0118921498_p18136122016449"></a>policy_functions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p715582011444"><a name="zh-cn_topic_0118921498_p715582011444"></a><a name="zh-cn_topic_0118921498_p715582011444"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p819162074416"><a name="zh-cn_topic_0118921498_p819162074416"></a><a name="zh-cn_topic_0118921498_p819162074416"></a>函数工作流策略后端列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  backend\_api参数说明

<a name="zh-cn_topic_0118921498_table46125461"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row21441395"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p59031425"><a name="zh-cn_topic_0118921498_p59031425"></a><a name="zh-cn_topic_0118921498_p59031425"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p16816124"><a name="zh-cn_topic_0118921498_p16816124"></a><a name="zh-cn_topic_0118921498_p16816124"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p19928779"><a name="zh-cn_topic_0118921498_p19928779"></a><a name="zh-cn_topic_0118921498_p19928779"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row3618391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p24654215"><a name="zh-cn_topic_0118921498_p24654215"></a><a name="zh-cn_topic_0118921498_p24654215"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p50834371"><a name="zh-cn_topic_0118921498_p50834371"></a><a name="zh-cn_topic_0118921498_p50834371"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p23943412"><a name="zh-cn_topic_0118921498_p23943412"></a><a name="zh-cn_topic_0118921498_p23943412"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row14164124"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p6443415"><a name="zh-cn_topic_0118921498_p6443415"></a><a name="zh-cn_topic_0118921498_p6443415"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p52154619"><a name="zh-cn_topic_0118921498_p52154619"></a><a name="zh-cn_topic_0118921498_p52154619"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p63774574"><a name="zh-cn_topic_0118921498_p63774574"></a><a name="zh-cn_topic_0118921498_p63774574"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row37100262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p52331254"><a name="zh-cn_topic_0118921498_p52331254"></a><a name="zh-cn_topic_0118921498_p52331254"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p10973162"><a name="zh-cn_topic_0118921498_p10973162"></a><a name="zh-cn_topic_0118921498_p10973162"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p15120014693"><a name="zh-cn_topic_0118921498_p15120014693"></a><a name="zh-cn_topic_0118921498_p15120014693"></a>后端endpoint</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row13480579"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p18185121"><a name="zh-cn_topic_0118921498_p18185121"></a><a name="zh-cn_topic_0118921498_p18185121"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p63708736"><a name="zh-cn_topic_0118921498_p63708736"></a><a name="zh-cn_topic_0118921498_p63708736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p60134024"><a name="zh-cn_topic_0118921498_p60134024"></a><a name="zh-cn_topic_0118921498_p60134024"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row4335306"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p15615521"><a name="zh-cn_topic_0118921498_p15615521"></a><a name="zh-cn_topic_0118921498_p15615521"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p56897717"><a name="zh-cn_topic_0118921498_p56897717"></a><a name="zh-cn_topic_0118921498_p56897717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p45312365"><a name="zh-cn_topic_0118921498_p45312365"></a><a name="zh-cn_topic_0118921498_p45312365"></a>访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row5158106"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p15153476"><a name="zh-cn_topic_0118921498_p15153476"></a><a name="zh-cn_topic_0118921498_p15153476"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p19472071"><a name="zh-cn_topic_0118921498_p19472071"></a><a name="zh-cn_topic_0118921498_p19472071"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p33733898"><a name="zh-cn_topic_0118921498_p33733898"></a><a name="zh-cn_topic_0118921498_p33733898"></a>访问方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row35169627"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p30167521"><a name="zh-cn_topic_0118921498_p30167521"></a><a name="zh-cn_topic_0118921498_p30167521"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p27650173"><a name="zh-cn_topic_0118921498_p27650173"></a><a name="zh-cn_topic_0118921498_p27650173"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p25071508"><a name="zh-cn_topic_0118921498_p25071508"></a><a name="zh-cn_topic_0118921498_p25071508"></a>访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row24316986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p23518872"><a name="zh-cn_topic_0118921498_p23518872"></a><a name="zh-cn_topic_0118921498_p23518872"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p25980454"><a name="zh-cn_topic_0118921498_p25980454"></a><a name="zh-cn_topic_0118921498_p25980454"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p24041996"><a name="zh-cn_topic_0118921498_p24041996"></a><a name="zh-cn_topic_0118921498_p24041996"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row15051376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p11201934"><a name="zh-cn_topic_0118921498_p11201934"></a><a name="zh-cn_topic_0118921498_p11201934"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p34941465"><a name="zh-cn_topic_0118921498_p34941465"></a><a name="zh-cn_topic_0118921498_p34941465"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p11686392"><a name="zh-cn_topic_0118921498_p11686392"></a><a name="zh-cn_topic_0118921498_p11686392"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row38068667"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p63663156"><a name="zh-cn_topic_0118921498_p63663156"></a><a name="zh-cn_topic_0118921498_p63663156"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p56441973"><a name="zh-cn_topic_0118921498_p56441973"></a><a name="zh-cn_topic_0118921498_p56441973"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p8397095"><a name="zh-cn_topic_0118921498_p8397095"></a><a name="zh-cn_topic_0118921498_p8397095"></a>修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row8464993"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p14575871"><a name="zh-cn_topic_0118921498_p14575871"></a><a name="zh-cn_topic_0118921498_p14575871"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p39794913"><a name="zh-cn_topic_0118921498_p39794913"></a><a name="zh-cn_topic_0118921498_p39794913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p2162544"><a name="zh-cn_topic_0118921498_p2162544"></a><a name="zh-cn_topic_0118921498_p2162544"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row19462899"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p32991024"><a name="zh-cn_topic_0118921498_p32991024"></a><a name="zh-cn_topic_0118921498_p32991024"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p55027277"><a name="zh-cn_topic_0118921498_p55027277"></a><a name="zh-cn_topic_0118921498_p55027277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p28024434"><a name="zh-cn_topic_0118921498_p28024434"></a><a name="zh-cn_topic_0118921498_p28024434"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row50893320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p28718221"><a name="zh-cn_topic_0118921498_p28718221"></a><a name="zh-cn_topic_0118921498_p28718221"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p44474542"><a name="zh-cn_topic_0118921498_p44474542"></a><a name="zh-cn_topic_0118921498_p44474542"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p45668181"><a name="zh-cn_topic_0118921498_p45668181"></a><a name="zh-cn_topic_0118921498_p45668181"></a>VPC通道信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row96871627153314"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p8505203193315"><a name="zh-cn_topic_0118921498_p8505203193315"></a><a name="zh-cn_topic_0118921498_p8505203193315"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p2585332331"><a name="zh-cn_topic_0118921498_p2585332331"></a><a name="zh-cn_topic_0118921498_p2585332331"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p9477136123312"><a name="zh-cn_topic_0118921498_p9477136123312"></a><a name="zh-cn_topic_0118921498_p9477136123312"></a>后端自定义认证对象的ID</p>
</td>
</tr>
</tbody>
</table>

**表 5**  mock\_info参数说明

<a name="zh-cn_topic_0118921498_table8360445"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row61660858"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p28473615"><a name="zh-cn_topic_0118921498_p28473615"></a><a name="zh-cn_topic_0118921498_p28473615"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p24661464"><a name="zh-cn_topic_0118921498_p24661464"></a><a name="zh-cn_topic_0118921498_p24661464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p51421566"><a name="zh-cn_topic_0118921498_p51421566"></a><a name="zh-cn_topic_0118921498_p51421566"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row4397288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p20636030"><a name="zh-cn_topic_0118921498_p20636030"></a><a name="zh-cn_topic_0118921498_p20636030"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p60905770"><a name="zh-cn_topic_0118921498_p60905770"></a><a name="zh-cn_topic_0118921498_p60905770"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p34420305"><a name="zh-cn_topic_0118921498_p34420305"></a><a name="zh-cn_topic_0118921498_p34420305"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row41347295"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p60796621"><a name="zh-cn_topic_0118921498_p60796621"></a><a name="zh-cn_topic_0118921498_p60796621"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p25579243"><a name="zh-cn_topic_0118921498_p25579243"></a><a name="zh-cn_topic_0118921498_p25579243"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p58652769"><a name="zh-cn_topic_0118921498_p58652769"></a><a name="zh-cn_topic_0118921498_p58652769"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row58112877"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p9522587"><a name="zh-cn_topic_0118921498_p9522587"></a><a name="zh-cn_topic_0118921498_p9522587"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p33132086"><a name="zh-cn_topic_0118921498_p33132086"></a><a name="zh-cn_topic_0118921498_p33132086"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p66453285"><a name="zh-cn_topic_0118921498_p66453285"></a><a name="zh-cn_topic_0118921498_p66453285"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row61208656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p58954073"><a name="zh-cn_topic_0118921498_p58954073"></a><a name="zh-cn_topic_0118921498_p58954073"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p10550570"><a name="zh-cn_topic_0118921498_p10550570"></a><a name="zh-cn_topic_0118921498_p10550570"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p49289836"><a name="zh-cn_topic_0118921498_p49289836"></a><a name="zh-cn_topic_0118921498_p49289836"></a>返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row40955342"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p29048444"><a name="zh-cn_topic_0118921498_p29048444"></a><a name="zh-cn_topic_0118921498_p29048444"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p4113774"><a name="zh-cn_topic_0118921498_p4113774"></a><a name="zh-cn_topic_0118921498_p4113774"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p64780301"><a name="zh-cn_topic_0118921498_p64780301"></a><a name="zh-cn_topic_0118921498_p64780301"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row46151800"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p47308357"><a name="zh-cn_topic_0118921498_p47308357"></a><a name="zh-cn_topic_0118921498_p47308357"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p6771698"><a name="zh-cn_topic_0118921498_p6771698"></a><a name="zh-cn_topic_0118921498_p6771698"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p11636647"><a name="zh-cn_topic_0118921498_p11636647"></a><a name="zh-cn_topic_0118921498_p11636647"></a>修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row37620965"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p27399290"><a name="zh-cn_topic_0118921498_p27399290"></a><a name="zh-cn_topic_0118921498_p27399290"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p4749995"><a name="zh-cn_topic_0118921498_p4749995"></a><a name="zh-cn_topic_0118921498_p4749995"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p49205346"><a name="zh-cn_topic_0118921498_p49205346"></a><a name="zh-cn_topic_0118921498_p49205346"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 6**  func\_info参数说明

<a name="zh-cn_topic_0118921498_table40194930"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row47908359"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p55371884"><a name="zh-cn_topic_0118921498_p55371884"></a><a name="zh-cn_topic_0118921498_p55371884"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p55937605"><a name="zh-cn_topic_0118921498_p55937605"></a><a name="zh-cn_topic_0118921498_p55937605"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p34652155"><a name="zh-cn_topic_0118921498_p34652155"></a><a name="zh-cn_topic_0118921498_p34652155"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row55361141"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p55067419"><a name="zh-cn_topic_0118921498_p55067419"></a><a name="zh-cn_topic_0118921498_p55067419"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p31275991"><a name="zh-cn_topic_0118921498_p31275991"></a><a name="zh-cn_topic_0118921498_p31275991"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p50327310"><a name="zh-cn_topic_0118921498_p50327310"></a><a name="zh-cn_topic_0118921498_p50327310"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row50292612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p47169794"><a name="zh-cn_topic_0118921498_p47169794"></a><a name="zh-cn_topic_0118921498_p47169794"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p62656944"><a name="zh-cn_topic_0118921498_p62656944"></a><a name="zh-cn_topic_0118921498_p62656944"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p42047670"><a name="zh-cn_topic_0118921498_p42047670"></a><a name="zh-cn_topic_0118921498_p42047670"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row42884714"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p51109800"><a name="zh-cn_topic_0118921498_p51109800"></a><a name="zh-cn_topic_0118921498_p51109800"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p46253139"><a name="zh-cn_topic_0118921498_p46253139"></a><a name="zh-cn_topic_0118921498_p46253139"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p55516754"><a name="zh-cn_topic_0118921498_p55516754"></a><a name="zh-cn_topic_0118921498_p55516754"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row29888741"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p5068926"><a name="zh-cn_topic_0118921498_p5068926"></a><a name="zh-cn_topic_0118921498_p5068926"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p7929823"><a name="zh-cn_topic_0118921498_p7929823"></a><a name="zh-cn_topic_0118921498_p7929823"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p38335921"><a name="zh-cn_topic_0118921498_p38335921"></a><a name="zh-cn_topic_0118921498_p38335921"></a>函数URN</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row9478971"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p29599225"><a name="zh-cn_topic_0118921498_p29599225"></a><a name="zh-cn_topic_0118921498_p29599225"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p48727035"><a name="zh-cn_topic_0118921498_p48727035"></a><a name="zh-cn_topic_0118921498_p48727035"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p54575786"><a name="zh-cn_topic_0118921498_p54575786"></a><a name="zh-cn_topic_0118921498_p54575786"></a>调用类型：async|sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row21420029"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p57300826"><a name="zh-cn_topic_0118921498_p57300826"></a><a name="zh-cn_topic_0118921498_p57300826"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p10855319"><a name="zh-cn_topic_0118921498_p10855319"></a><a name="zh-cn_topic_0118921498_p10855319"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p6865628"><a name="zh-cn_topic_0118921498_p6865628"></a><a name="zh-cn_topic_0118921498_p6865628"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row61790658"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p38987367"><a name="zh-cn_topic_0118921498_p38987367"></a><a name="zh-cn_topic_0118921498_p38987367"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p3860136"><a name="zh-cn_topic_0118921498_p3860136"></a><a name="zh-cn_topic_0118921498_p3860136"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p44235631"><a name="zh-cn_topic_0118921498_p44235631"></a><a name="zh-cn_topic_0118921498_p44235631"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row62576359"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p35520303"><a name="zh-cn_topic_0118921498_p35520303"></a><a name="zh-cn_topic_0118921498_p35520303"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p58572271"><a name="zh-cn_topic_0118921498_p58572271"></a><a name="zh-cn_topic_0118921498_p58572271"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p46733520"><a name="zh-cn_topic_0118921498_p46733520"></a><a name="zh-cn_topic_0118921498_p46733520"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row17948500"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p44542409"><a name="zh-cn_topic_0118921498_p44542409"></a><a name="zh-cn_topic_0118921498_p44542409"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p51165362"><a name="zh-cn_topic_0118921498_p51165362"></a><a name="zh-cn_topic_0118921498_p51165362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p50753656"><a name="zh-cn_topic_0118921498_p50753656"></a><a name="zh-cn_topic_0118921498_p50753656"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 7**  req\_params参数说明

<a name="zh-cn_topic_0118921498_table197251634194412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row2075603420446"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p11756234184411"><a name="zh-cn_topic_0118921498_p11756234184411"></a><a name="zh-cn_topic_0118921498_p11756234184411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p777143420447"><a name="zh-cn_topic_0118921498_p777143420447"></a><a name="zh-cn_topic_0118921498_p777143420447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p5771193415446"><a name="zh-cn_topic_0118921498_p5771193415446"></a><a name="zh-cn_topic_0118921498_p5771193415446"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row85313200454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1753320144511"><a name="zh-cn_topic_0118921498_p1753320144511"></a><a name="zh-cn_topic_0118921498_p1753320144511"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p75302015450"><a name="zh-cn_topic_0118921498_p75302015450"></a><a name="zh-cn_topic_0118921498_p75302015450"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p653162014451"><a name="zh-cn_topic_0118921498_p653162014451"></a><a name="zh-cn_topic_0118921498_p653162014451"></a>参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row8786123464413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p578618344445"><a name="zh-cn_topic_0118921498_p578618344445"></a><a name="zh-cn_topic_0118921498_p578618344445"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1480313412443"><a name="zh-cn_topic_0118921498_p1480313412443"></a><a name="zh-cn_topic_0118921498_p1480313412443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p48033344445"><a name="zh-cn_topic_0118921498_p48033344445"></a><a name="zh-cn_topic_0118921498_p48033344445"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row13818193434411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p781810341448"><a name="zh-cn_topic_0118921498_p781810341448"></a><a name="zh-cn_topic_0118921498_p781810341448"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p18342034114419"><a name="zh-cn_topic_0118921498_p18342034114419"></a><a name="zh-cn_topic_0118921498_p18342034114419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p083493413441"><a name="zh-cn_topic_0118921498_p083493413441"></a><a name="zh-cn_topic_0118921498_p083493413441"></a>参数类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row17850234124414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p18865203414418"><a name="zh-cn_topic_0118921498_p18865203414418"></a><a name="zh-cn_topic_0118921498_p18865203414418"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p16881203415443"><a name="zh-cn_topic_0118921498_p16881203415443"></a><a name="zh-cn_topic_0118921498_p16881203415443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p788120340445"><a name="zh-cn_topic_0118921498_p788120340445"></a><a name="zh-cn_topic_0118921498_p788120340445"></a>参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row99121534134414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p18912934114419"><a name="zh-cn_topic_0118921498_p18912934114419"></a><a name="zh-cn_topic_0118921498_p18912934114419"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p139281534104415"><a name="zh-cn_topic_0118921498_p139281534104415"></a><a name="zh-cn_topic_0118921498_p139281534104415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1592853454412"><a name="zh-cn_topic_0118921498_p1592853454412"></a><a name="zh-cn_topic_0118921498_p1592853454412"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1594315349446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p994311348442"><a name="zh-cn_topic_0118921498_p994311348442"></a><a name="zh-cn_topic_0118921498_p994311348442"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1495973414419"><a name="zh-cn_topic_0118921498_p1495973414419"></a><a name="zh-cn_topic_0118921498_p1495973414419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1695953413449"><a name="zh-cn_topic_0118921498_p1695953413449"></a><a name="zh-cn_topic_0118921498_p1695953413449"></a>参数示例值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1959173474410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p2974183417445"><a name="zh-cn_topic_0118921498_p2974183417445"></a><a name="zh-cn_topic_0118921498_p2974183417445"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p13974143417443"><a name="zh-cn_topic_0118921498_p13974143417443"></a><a name="zh-cn_topic_0118921498_p13974143417443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p699053414444"><a name="zh-cn_topic_0118921498_p699053414444"></a><a name="zh-cn_topic_0118921498_p699053414444"></a>是否必须：</p>
<a name="zh-cn_topic_0118921498_ul158441432194613"></a><a name="zh-cn_topic_0118921498_ul158441432194613"></a><ul id="zh-cn_topic_0118921498_ul158441432194613"><li>1：必须</li><li>2：非必须</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row662354446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p66183524412"><a name="zh-cn_topic_0118921498_p66183524412"></a><a name="zh-cn_topic_0118921498_p66183524412"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p32133519447"><a name="zh-cn_topic_0118921498_p32133519447"></a><a name="zh-cn_topic_0118921498_p32133519447"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p18371535124417"><a name="zh-cn_topic_0118921498_p18371535124417"></a><a name="zh-cn_topic_0118921498_p18371535124417"></a>是否开启校验</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1053435144414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p653133513441"><a name="zh-cn_topic_0118921498_p653133513441"></a><a name="zh-cn_topic_0118921498_p653133513441"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1867183512446"><a name="zh-cn_topic_0118921498_p1867183512446"></a><a name="zh-cn_topic_0118921498_p1867183512446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p567123584420"><a name="zh-cn_topic_0118921498_p567123584420"></a><a name="zh-cn_topic_0118921498_p567123584420"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row7100203515443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p181002035154415"><a name="zh-cn_topic_0118921498_p181002035154415"></a><a name="zh-cn_topic_0118921498_p181002035154415"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p161151635164413"><a name="zh-cn_topic_0118921498_p161151635164413"></a><a name="zh-cn_topic_0118921498_p161151635164413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p2559522184412"><a name="zh-cn_topic_0118921498_p2559522184412"></a><a name="zh-cn_topic_0118921498_p2559522184412"></a>参数枚举值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p151311235144415"><a name="zh-cn_topic_0118921498_p151311235144415"></a><a name="zh-cn_topic_0118921498_p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p713112353443"><a name="zh-cn_topic_0118921498_p713112353443"></a><a name="zh-cn_topic_0118921498_p713112353443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p95973228446"><a name="zh-cn_topic_0118921498_p95973228446"></a><a name="zh-cn_topic_0118921498_p95973228446"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p8146203564415"><a name="zh-cn_topic_0118921498_p8146203564415"></a><a name="zh-cn_topic_0118921498_p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p31627353442"><a name="zh-cn_topic_0118921498_p31627353442"></a><a name="zh-cn_topic_0118921498_p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p2631222104413"><a name="zh-cn_topic_0118921498_p2631222104413"></a><a name="zh-cn_topic_0118921498_p2631222104413"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p61782355443"><a name="zh-cn_topic_0118921498_p61782355443"></a><a name="zh-cn_topic_0118921498_p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p201932035194417"><a name="zh-cn_topic_0118921498_p201932035194417"></a><a name="zh-cn_topic_0118921498_p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p2668152294420"><a name="zh-cn_topic_0118921498_p2668152294420"></a><a name="zh-cn_topic_0118921498_p2668152294420"></a>参数最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p12209535144412"><a name="zh-cn_topic_0118921498_p12209535144412"></a><a name="zh-cn_topic_0118921498_p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p12251035164419"><a name="zh-cn_topic_0118921498_p12251035164419"></a><a name="zh-cn_topic_0118921498_p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p3702522184416"><a name="zh-cn_topic_0118921498_p3702522184416"></a><a name="zh-cn_topic_0118921498_p3702522184416"></a>参数最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p52401735134413"><a name="zh-cn_topic_0118921498_p52401735134413"></a><a name="zh-cn_topic_0118921498_p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p12240153510443"><a name="zh-cn_topic_0118921498_p12240153510443"></a><a name="zh-cn_topic_0118921498_p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p12731822184412"><a name="zh-cn_topic_0118921498_p12731822184412"></a><a name="zh-cn_topic_0118921498_p12731822184412"></a>正则校验规则（暂不支持）</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p202561335114413"><a name="zh-cn_topic_0118921498_p202561335114413"></a><a name="zh-cn_topic_0118921498_p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p16271035114412"><a name="zh-cn_topic_0118921498_p16271035114412"></a><a name="zh-cn_topic_0118921498_p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p57661222144411"><a name="zh-cn_topic_0118921498_p57661222144411"></a><a name="zh-cn_topic_0118921498_p57661222144411"></a>JSON校验规则（暂不支持）</p>
</td>
</tr>
</tbody>
</table>

**表 8**  backend\_params参数说明

<a name="zh-cn_topic_0118921498_table9287113513446"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row4302173564419"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p33182355443"><a name="zh-cn_topic_0118921498_p33182355443"></a><a name="zh-cn_topic_0118921498_p33182355443"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p14334103544415"><a name="zh-cn_topic_0118921498_p14334103544415"></a><a name="zh-cn_topic_0118921498_p14334103544415"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p19334153517444"><a name="zh-cn_topic_0118921498_p19334153517444"></a><a name="zh-cn_topic_0118921498_p19334153517444"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row17142774611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p47152713464"><a name="zh-cn_topic_0118921498_p47152713464"></a><a name="zh-cn_topic_0118921498_p47152713464"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1717279463"><a name="zh-cn_topic_0118921498_p1717279463"></a><a name="zh-cn_topic_0118921498_p1717279463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p27122714620"><a name="zh-cn_topic_0118921498_p27122714620"></a><a name="zh-cn_topic_0118921498_p27122714620"></a>参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row2936129114713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p199361729154717"><a name="zh-cn_topic_0118921498_p199361729154717"></a><a name="zh-cn_topic_0118921498_p199361729154717"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1693652934715"><a name="zh-cn_topic_0118921498_p1693652934715"></a><a name="zh-cn_topic_0118921498_p1693652934715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1093614294475"><a name="zh-cn_topic_0118921498_p1093614294475"></a><a name="zh-cn_topic_0118921498_p1093614294475"></a>对应的请求参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row833403514441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p13350143554413"><a name="zh-cn_topic_0118921498_p13350143554413"></a><a name="zh-cn_topic_0118921498_p13350143554413"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p6365163554417"><a name="zh-cn_topic_0118921498_p6365163554417"></a><a name="zh-cn_topic_0118921498_p6365163554417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p036516356445"><a name="zh-cn_topic_0118921498_p036516356445"></a><a name="zh-cn_topic_0118921498_p036516356445"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row203656353443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p4381103534420"><a name="zh-cn_topic_0118921498_p4381103534420"></a><a name="zh-cn_topic_0118921498_p4381103534420"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p838193504410"><a name="zh-cn_topic_0118921498_p838193504410"></a><a name="zh-cn_topic_0118921498_p838193504410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p10396123516442"><a name="zh-cn_topic_0118921498_p10396123516442"></a><a name="zh-cn_topic_0118921498_p10396123516442"></a>参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row7412103554417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p14271535144413"><a name="zh-cn_topic_0118921498_p14271535144413"></a><a name="zh-cn_topic_0118921498_p14271535144413"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1525155534613"><a name="zh-cn_topic_0118921498_p1525155534613"></a><a name="zh-cn_topic_0118921498_p1525155534613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1044312351449"><a name="zh-cn_topic_0118921498_p1044312351449"></a><a name="zh-cn_topic_0118921498_p1044312351449"></a>参数类别</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row445983511447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p5475203519440"><a name="zh-cn_topic_0118921498_p5475203519440"></a><a name="zh-cn_topic_0118921498_p5475203519440"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p8536145516465"><a name="zh-cn_topic_0118921498_p8536145516465"></a><a name="zh-cn_topic_0118921498_p8536145516465"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p9490435144419"><a name="zh-cn_topic_0118921498_p9490435144419"></a><a name="zh-cn_topic_0118921498_p9490435144419"></a>参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row7506335184410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p3506935104410"><a name="zh-cn_topic_0118921498_p3506935104410"></a><a name="zh-cn_topic_0118921498_p3506935104410"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p05217356442"><a name="zh-cn_topic_0118921498_p05217356442"></a><a name="zh-cn_topic_0118921498_p05217356442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p11521123517447"><a name="zh-cn_topic_0118921498_p11521123517447"></a><a name="zh-cn_topic_0118921498_p11521123517447"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 9**  policy\_https参数说明

<a name="zh-cn_topic_0118921498_table1883393417451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row12893173494517"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p1491393413454"><a name="zh-cn_topic_0118921498_p1491393413454"></a><a name="zh-cn_topic_0118921498_p1491393413454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p3930134144518"><a name="zh-cn_topic_0118921498_p3930134144518"></a><a name="zh-cn_topic_0118921498_p3930134144518"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p1394693410456"><a name="zh-cn_topic_0118921498_p1394693410456"></a><a name="zh-cn_topic_0118921498_p1394693410456"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row129661334174520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1997923418453"><a name="zh-cn_topic_0118921498_p1997923418453"></a><a name="zh-cn_topic_0118921498_p1997923418453"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p699316349457"><a name="zh-cn_topic_0118921498_p699316349457"></a><a name="zh-cn_topic_0118921498_p699316349457"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1176354455"><a name="zh-cn_topic_0118921498_p1176354455"></a><a name="zh-cn_topic_0118921498_p1176354455"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row191173534519"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p729183516457"><a name="zh-cn_topic_0118921498_p729183516457"></a><a name="zh-cn_topic_0118921498_p729183516457"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p5442035114515"><a name="zh-cn_topic_0118921498_p5442035114515"></a><a name="zh-cn_topic_0118921498_p5442035114515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p105673584520"><a name="zh-cn_topic_0118921498_p105673584520"></a><a name="zh-cn_topic_0118921498_p105673584520"></a>策略后端名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row19611535114513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p20805354452"><a name="zh-cn_topic_0118921498_p20805354452"></a><a name="zh-cn_topic_0118921498_p20805354452"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p09323564519"><a name="zh-cn_topic_0118921498_p09323564519"></a><a name="zh-cn_topic_0118921498_p09323564519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p131089355454"><a name="zh-cn_topic_0118921498_p131089355454"></a><a name="zh-cn_topic_0118921498_p131089355454"></a>策略后端endpoint</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row141732035194520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p11921135124512"><a name="zh-cn_topic_0118921498_p11921135124512"></a><a name="zh-cn_topic_0118921498_p11921135124512"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p2209173510459"><a name="zh-cn_topic_0118921498_p2209173510459"></a><a name="zh-cn_topic_0118921498_p2209173510459"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p2223153513453"><a name="zh-cn_topic_0118921498_p2223153513453"></a><a name="zh-cn_topic_0118921498_p2223153513453"></a>访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row102311835144513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p142451635144514"><a name="zh-cn_topic_0118921498_p142451635144514"></a><a name="zh-cn_topic_0118921498_p142451635144514"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p926153519453"><a name="zh-cn_topic_0118921498_p926153519453"></a><a name="zh-cn_topic_0118921498_p926153519453"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p0276135124514"><a name="zh-cn_topic_0118921498_p0276135124514"></a><a name="zh-cn_topic_0118921498_p0276135124514"></a>访问方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row9284735204514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1629817356452"><a name="zh-cn_topic_0118921498_p1629817356452"></a><a name="zh-cn_topic_0118921498_p1629817356452"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p2313183554516"><a name="zh-cn_topic_0118921498_p2313183554516"></a><a name="zh-cn_topic_0118921498_p2313183554516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p123341135134516"><a name="zh-cn_topic_0118921498_p123341135134516"></a><a name="zh-cn_topic_0118921498_p123341135134516"></a>访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row20342535194519"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p8362535154510"><a name="zh-cn_topic_0118921498_p8362535154510"></a><a name="zh-cn_topic_0118921498_p8362535154510"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p12378193514459"><a name="zh-cn_topic_0118921498_p12378193514459"></a><a name="zh-cn_topic_0118921498_p12378193514459"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p123951235114514"><a name="zh-cn_topic_0118921498_p123951235114514"></a><a name="zh-cn_topic_0118921498_p123951235114514"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1159233518458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p20614163564511"><a name="zh-cn_topic_0118921498_p20614163564511"></a><a name="zh-cn_topic_0118921498_p20614163564511"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p9632143519451"><a name="zh-cn_topic_0118921498_p9632143519451"></a><a name="zh-cn_topic_0118921498_p9632143519451"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p56481835124516"><a name="zh-cn_topic_0118921498_p56481835124516"></a><a name="zh-cn_topic_0118921498_p56481835124516"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row765613353459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p19673193519458"><a name="zh-cn_topic_0118921498_p19673193519458"></a><a name="zh-cn_topic_0118921498_p19673193519458"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p0690203524511"><a name="zh-cn_topic_0118921498_p0690203524511"></a><a name="zh-cn_topic_0118921498_p0690203524511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p20706143594518"><a name="zh-cn_topic_0118921498_p20706143594518"></a><a name="zh-cn_topic_0118921498_p20706143594518"></a>VPC通道信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row33971122125919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p7397722115911"><a name="zh-cn_topic_0118921498_p7397722115911"></a><a name="zh-cn_topic_0118921498_p7397722115911"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p14397142235915"><a name="zh-cn_topic_0118921498_p14397142235915"></a><a name="zh-cn_topic_0118921498_p14397142235915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p143978228592"><a name="zh-cn_topic_0118921498_p143978228592"></a><a name="zh-cn_topic_0118921498_p143978228592"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row17521289599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p181451844918"><a name="zh-cn_topic_0118921498_p181451844918"></a><a name="zh-cn_topic_0118921498_p181451844918"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p178501852715"><a name="zh-cn_topic_0118921498_p178501852715"></a><a name="zh-cn_topic_0118921498_p178501852715"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1091214598110"><a name="zh-cn_topic_0118921498_p1091214598110"></a><a name="zh-cn_topic_0118921498_p1091214598110"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row62321736195919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p131741744219"><a name="zh-cn_topic_0118921498_p131741744219"></a><a name="zh-cn_topic_0118921498_p131741744219"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1487855214114"><a name="zh-cn_topic_0118921498_p1487855214114"></a><a name="zh-cn_topic_0118921498_p1487855214114"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p3947175912116"><a name="zh-cn_topic_0118921498_p3947175912116"></a><a name="zh-cn_topic_0118921498_p3947175912116"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 10**  policy\_mocks参数说明

<a name="zh-cn_topic_0118921498_table12725183513454"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row15764635144513"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p378211357456"><a name="zh-cn_topic_0118921498_p378211357456"></a><a name="zh-cn_topic_0118921498_p378211357456"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p58001135104513"><a name="zh-cn_topic_0118921498_p58001135104513"></a><a name="zh-cn_topic_0118921498_p58001135104513"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p981853512455"><a name="zh-cn_topic_0118921498_p981853512455"></a><a name="zh-cn_topic_0118921498_p981853512455"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row2835103534513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p6852143510458"><a name="zh-cn_topic_0118921498_p6852143510458"></a><a name="zh-cn_topic_0118921498_p6852143510458"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p2866103524515"><a name="zh-cn_topic_0118921498_p2866103524515"></a><a name="zh-cn_topic_0118921498_p2866103524515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1587913519457"><a name="zh-cn_topic_0118921498_p1587913519457"></a><a name="zh-cn_topic_0118921498_p1587913519457"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row8887123534513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p15538921331"><a name="zh-cn_topic_0118921498_p15538921331"></a><a name="zh-cn_topic_0118921498_p15538921331"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p135591025311"><a name="zh-cn_topic_0118921498_p135591025311"></a><a name="zh-cn_topic_0118921498_p135591025311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p105814212311"><a name="zh-cn_topic_0118921498_p105814212311"></a><a name="zh-cn_topic_0118921498_p105814212311"></a>策略后端名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row119183644517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1737133612459"><a name="zh-cn_topic_0118921498_p1737133612459"></a><a name="zh-cn_topic_0118921498_p1737133612459"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p13522036104518"><a name="zh-cn_topic_0118921498_p13522036104518"></a><a name="zh-cn_topic_0118921498_p13522036104518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p116953674519"><a name="zh-cn_topic_0118921498_p116953674519"></a><a name="zh-cn_topic_0118921498_p116953674519"></a>返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1780193618456"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p129375499320"><a name="zh-cn_topic_0118921498_p129375499320"></a><a name="zh-cn_topic_0118921498_p129375499320"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p20959149733"><a name="zh-cn_topic_0118921498_p20959149733"></a><a name="zh-cn_topic_0118921498_p20959149733"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p49808491431"><a name="zh-cn_topic_0118921498_p49808491431"></a><a name="zh-cn_topic_0118921498_p49808491431"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row914193684515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p21155015317"><a name="zh-cn_topic_0118921498_p21155015317"></a><a name="zh-cn_topic_0118921498_p21155015317"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1631135010319"><a name="zh-cn_topic_0118921498_p1631135010319"></a><a name="zh-cn_topic_0118921498_p1631135010319"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p95105016320"><a name="zh-cn_topic_0118921498_p95105016320"></a><a name="zh-cn_topic_0118921498_p95105016320"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row220083616456"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p19851150935"><a name="zh-cn_topic_0118921498_p19851150935"></a><a name="zh-cn_topic_0118921498_p19851150935"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p191021350934"><a name="zh-cn_topic_0118921498_p191021350934"></a><a name="zh-cn_topic_0118921498_p191021350934"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p21240503312"><a name="zh-cn_topic_0118921498_p21240503312"></a><a name="zh-cn_topic_0118921498_p21240503312"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 11**  policy\_functions参数说明

<a name="zh-cn_topic_0118921498_table11274103664518"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row14323123615458"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p12336163614453"><a name="zh-cn_topic_0118921498_p12336163614453"></a><a name="zh-cn_topic_0118921498_p12336163614453"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p3348163613458"><a name="zh-cn_topic_0118921498_p3348163613458"></a><a name="zh-cn_topic_0118921498_p3348163613458"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p136353684510"><a name="zh-cn_topic_0118921498_p136353684510"></a><a name="zh-cn_topic_0118921498_p136353684510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row438373613454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p193981361454"><a name="zh-cn_topic_0118921498_p193981361454"></a><a name="zh-cn_topic_0118921498_p193981361454"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p10414336164515"><a name="zh-cn_topic_0118921498_p10414336164515"></a><a name="zh-cn_topic_0118921498_p10414336164515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1543203615456"><a name="zh-cn_topic_0118921498_p1543203615456"></a><a name="zh-cn_topic_0118921498_p1543203615456"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1844443611451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p145173216411"><a name="zh-cn_topic_0118921498_p145173216411"></a><a name="zh-cn_topic_0118921498_p145173216411"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p125371217420"><a name="zh-cn_topic_0118921498_p125371217420"></a><a name="zh-cn_topic_0118921498_p125371217420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p15581212410"><a name="zh-cn_topic_0118921498_p15581212410"></a><a name="zh-cn_topic_0118921498_p15581212410"></a>策略后端名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row450233644511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p25201036164517"><a name="zh-cn_topic_0118921498_p25201036164517"></a><a name="zh-cn_topic_0118921498_p25201036164517"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p16541736164516"><a name="zh-cn_topic_0118921498_p16541736164516"></a><a name="zh-cn_topic_0118921498_p16541736164516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p16558133684511"><a name="zh-cn_topic_0118921498_p16558133684511"></a><a name="zh-cn_topic_0118921498_p16558133684511"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row45685369453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p45841936134516"><a name="zh-cn_topic_0118921498_p45841936134516"></a><a name="zh-cn_topic_0118921498_p45841936134516"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p25991036114518"><a name="zh-cn_topic_0118921498_p25991036114518"></a><a name="zh-cn_topic_0118921498_p25991036114518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p6618133614456"><a name="zh-cn_topic_0118921498_p6618133614456"></a><a name="zh-cn_topic_0118921498_p6618133614456"></a>函数URN</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row56281362452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1364419365459"><a name="zh-cn_topic_0118921498_p1364419365459"></a><a name="zh-cn_topic_0118921498_p1364419365459"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p19665236114517"><a name="zh-cn_topic_0118921498_p19665236114517"></a><a name="zh-cn_topic_0118921498_p19665236114517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1968233654519"><a name="zh-cn_topic_0118921498_p1968233654519"></a><a name="zh-cn_topic_0118921498_p1968233654519"></a>调用类型:async|sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row108137365458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1183073613455"><a name="zh-cn_topic_0118921498_p1183073613455"></a><a name="zh-cn_topic_0118921498_p1183073613455"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1484712366457"><a name="zh-cn_topic_0118921498_p1484712366457"></a><a name="zh-cn_topic_0118921498_p1484712366457"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1687010368458"><a name="zh-cn_topic_0118921498_p1687010368458"></a><a name="zh-cn_topic_0118921498_p1687010368458"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1288018362459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p125311657249"><a name="zh-cn_topic_0118921498_p125311657249"></a><a name="zh-cn_topic_0118921498_p125311657249"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p165491576420"><a name="zh-cn_topic_0118921498_p165491576420"></a><a name="zh-cn_topic_0118921498_p165491576420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p556795712420"><a name="zh-cn_topic_0118921498_p556795712420"></a><a name="zh-cn_topic_0118921498_p556795712420"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row14199172719419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p259219571446"><a name="zh-cn_topic_0118921498_p259219571446"></a><a name="zh-cn_topic_0118921498_p259219571446"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p160916576412"><a name="zh-cn_topic_0118921498_p160916576412"></a><a name="zh-cn_topic_0118921498_p160916576412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p17627257149"><a name="zh-cn_topic_0118921498_p17627257149"></a><a name="zh-cn_topic_0118921498_p17627257149"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row107283241048"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p66684572045"><a name="zh-cn_topic_0118921498_p66684572045"></a><a name="zh-cn_topic_0118921498_p66684572045"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p126865574411"><a name="zh-cn_topic_0118921498_p126865574411"></a><a name="zh-cn_topic_0118921498_p126865574411"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p17025579410"><a name="zh-cn_topic_0118921498_p17025579410"></a><a name="zh-cn_topic_0118921498_p17025579410"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 12**  conditions参数说明

<a name="zh-cn_topic_0118921498_table54445157"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row01061051953"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p121240513510"><a name="zh-cn_topic_0118921498_p121240513510"></a><a name="zh-cn_topic_0118921498_p121240513510"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p0145557515"><a name="zh-cn_topic_0118921498_p0145557515"></a><a name="zh-cn_topic_0118921498_p0145557515"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p4166752511"><a name="zh-cn_topic_0118921498_p4166752511"></a><a name="zh-cn_topic_0118921498_p4166752511"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row1618417512511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p719835852"><a name="zh-cn_topic_0118921498_p719835852"></a><a name="zh-cn_topic_0118921498_p719835852"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p16224185456"><a name="zh-cn_topic_0118921498_p16224185456"></a><a name="zh-cn_topic_0118921498_p16224185456"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p102391557519"><a name="zh-cn_topic_0118921498_p102391557519"></a><a name="zh-cn_topic_0118921498_p102391557519"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row82501551858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1796083474"><a name="zh-cn_topic_0118921498_p1796083474"></a><a name="zh-cn_topic_0118921498_p1796083474"></a>condition_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p18804202017712"><a name="zh-cn_topic_0118921498_p18804202017712"></a><a name="zh-cn_topic_0118921498_p18804202017712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p382342012717"><a name="zh-cn_topic_0118921498_p382342012717"></a><a name="zh-cn_topic_0118921498_p382342012717"></a>策略条件</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row123301257513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p181491444714"><a name="zh-cn_topic_0118921498_p181491444714"></a><a name="zh-cn_topic_0118921498_p181491444714"></a>condition_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1492819201073"><a name="zh-cn_topic_0118921498_p1492819201073"></a><a name="zh-cn_topic_0118921498_p1492819201073"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1994462016716"><a name="zh-cn_topic_0118921498_p1994462016716"></a><a name="zh-cn_topic_0118921498_p1994462016716"></a>策略值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1040955655"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p12230841573"><a name="zh-cn_topic_0118921498_p12230841573"></a><a name="zh-cn_topic_0118921498_p12230841573"></a>condition_origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p197610207714"><a name="zh-cn_topic_0118921498_p197610207714"></a><a name="zh-cn_topic_0118921498_p197610207714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1999642015720"><a name="zh-cn_topic_0118921498_p1999642015720"></a><a name="zh-cn_topic_0118921498_p1999642015720"></a>策略类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1247645451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p193881741373"><a name="zh-cn_topic_0118921498_p193881741373"></a><a name="zh-cn_topic_0118921498_p193881741373"></a>req_param_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p1575921679"><a name="zh-cn_topic_0118921498_p1575921679"></a><a name="zh-cn_topic_0118921498_p1575921679"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1396172120712"><a name="zh-cn_topic_0118921498_p1396172120712"></a><a name="zh-cn_topic_0118921498_p1396172120712"></a>关联的请求参数对象名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row455495755"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p15751853519"><a name="zh-cn_topic_0118921498_p15751853519"></a><a name="zh-cn_topic_0118921498_p15751853519"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p10599451451"><a name="zh-cn_topic_0118921498_p10599451451"></a><a name="zh-cn_topic_0118921498_p10599451451"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p5617455515"><a name="zh-cn_topic_0118921498_p5617455515"></a><a name="zh-cn_topic_0118921498_p5617455515"></a>关联的请求参数对象编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row1862912512520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p176461751659"><a name="zh-cn_topic_0118921498_p176461751659"></a><a name="zh-cn_topic_0118921498_p176461751659"></a>req_param_location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p146711652057"><a name="zh-cn_topic_0118921498_p146711652057"></a><a name="zh-cn_topic_0118921498_p146711652057"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p869795651"><a name="zh-cn_topic_0118921498_p869795651"></a><a name="zh-cn_topic_0118921498_p869795651"></a>关联的请求参数对象位置</p>
</td>
</tr>
</tbody>
</table>

**表 13**  auth\_opt参数说明

<a name="zh-cn_topic_0118921498_table3296221173715"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row829715213377"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921498_p17297192173718"><a name="zh-cn_topic_0118921498_p17297192173718"></a><a name="zh-cn_topic_0118921498_p17297192173718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921498_p9297821143718"><a name="zh-cn_topic_0118921498_p9297821143718"></a><a name="zh-cn_topic_0118921498_p9297821143718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921498_p4297152163717"><a name="zh-cn_topic_0118921498_p4297152163717"></a><a name="zh-cn_topic_0118921498_p4297152163717"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row4297421123717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921498_p1848964315375"><a name="zh-cn_topic_0118921498_p1848964315375"></a><a name="zh-cn_topic_0118921498_p1848964315375"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921498_p4489164310372"><a name="zh-cn_topic_0118921498_p4489164310372"></a><a name="zh-cn_topic_0118921498_p4489164310372"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921498_p1948934316376"><a name="zh-cn_topic_0118921498_p1948934316376"></a><a name="zh-cn_topic_0118921498_p1948934316376"></a>AppCode简易认证类型</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "name": "test",
  "type": 1,
  "version": "V0.0.1",
  "req_protocol": "HTTPS",
  "req_method": "GET",
  "req_uri": "/test/{tenant_id}",
  "auth_type": "APP",
  "auth_opt": {
    "app_code_auth_type": "DISABLE"
  },
  "tags": ["APIG-SN-test", "test"],
  "cors": false,
  "match_mode": "NORMAL",
  "backend_type": "HTTP",
  "group_id": "f71f69876f90456ca6fd18ed012fdc11",
  "result_normal_sample": "hello world!",
  "id": "81efcfd94b8747a0b21e8c04144a4e8c",
  "status": 1,
  "arrange_necessary": 2,
  "register_time": "2018-08-15T03:41:11.0239936Z",
  "update_time": "2018-08-15T03:41:11.0239936Z",
  "group_name": "group0002",
  "backend_api": {
    "url_domain": "xxxxxxxxxxx",
    "req_protocol": "HTTP",
    "req_method": "GET",
    "req_uri": "/test",
    "timeout": 1000,
    "vpc_status": 2,
    "id": "3442ffd031814e3a8f133a9f1ea08453",
    "status": 1,
    "register_time": "2018-08-15T03:41:11.1019236Z",
    "update_time": "2018-08-15T03:41:11.1019236Z"
  },
  "req_params": [
    {
      "name": "tenant_id",
      "type": "STRING",
      "location": "PATH",
      "required": 1,
      "valid_enable": 2,
      "id": "593c5560e0924e00af08fb458f850ecb"
    },
    {
      "name": "city",
      "type": "STRING",
      "location": "QUERY",
      "required": 2,
      "valid_enable": 2,
      "id": "e0b91bc81ae54f8ea850848d782d6e1e"
    }
  ],
  "backend_params": [
    {
      "name": "tenant_id",
      "location": "QUERY",
      "origin": "REQUEST",
      "value": "tenant_id",
      "id": "44e03de2351e43a8b18ba9ec1e71d2e9",
      "req_param_id": "593c5560e0924e00af08fb458f850ecb"
    },
    {
      "name": "city",
      "location": "QUERY",
      "origin": "REQUEST",
      "value": "city",
      "id": "b60fbcb5b86f4f5c8705c445b9bd6325",
      "req_param_id": "e0b91bc81ae54f8ea850848d782d6e1e"
    }
  ],
  "policy_https": [{
    "conditions": [{
      "id": "44e03de2351e43a8b18ba9ec1e71d2e9",
      "condition_type": "pattern",
      "condition_value": "^[0-9]$",
      "condition_origin": "param",
      "req_param_name": "project_id",
      "req_param_id": "b60fbcb5b86f4f5c8705c445b9sda325",
      "req_param_location": "PATH"
    }],
    "backend_params": [{
      "name": "project_id",
      "value": "bbbb",
      "location": "QUERY",
      "origin": "REQUEST",
      "id": "44e03de2351e43a8b18ba9ec1e71d2e8",
      "req_param_id": "593c5560e0924e00af08fb458f850ecb"
    }],
    "effect_mode": "ANY",
    "id": "44e03de2351e43a8b18ba9ec1e71d2e8",
    "name": "policy001",
    "req_method": "GET",
    "req_protocol": "http",
    "req_uri": "/test/policy",
    "timeout": 10000,
    "url_domain": "xxxxxxxxxxx",
    "vpc_status": 2
  }]
}
```

## 状态码<a name="zh-cn_topic_0118921498_section48575109"></a>

**表 14**  返回消息说明

<a name="zh-cn_topic_0118921498_table5357896"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921498_row27259487"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921498_p60534834"><a name="zh-cn_topic_0118921498_p60534834"></a><a name="zh-cn_topic_0118921498_p60534834"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921498_p4374530"><a name="zh-cn_topic_0118921498_p4374530"></a><a name="zh-cn_topic_0118921498_p4374530"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921498_row18792630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921498_p45808055"><a name="zh-cn_topic_0118921498_p45808055"></a><a name="zh-cn_topic_0118921498_p45808055"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921498_p50988816"><a name="zh-cn_topic_0118921498_p50988816"></a><a name="zh-cn_topic_0118921498_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row40966733"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921498_p29971116"><a name="zh-cn_topic_0118921498_p29971116"></a><a name="zh-cn_topic_0118921498_p29971116"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921498_p29757115610"><a name="zh-cn_topic_0118921498_p29757115610"></a><a name="zh-cn_topic_0118921498_p29757115610"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row38563414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921498_p36628845"><a name="zh-cn_topic_0118921498_p36628845"></a><a name="zh-cn_topic_0118921498_p36628845"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921498_p9203142078"><a name="zh-cn_topic_0118921498_p9203142078"></a><a name="zh-cn_topic_0118921498_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row60209613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921498_p45140486"><a name="zh-cn_topic_0118921498_p45140486"></a><a name="zh-cn_topic_0118921498_p45140486"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921498_p13949586"><a name="zh-cn_topic_0118921498_p13949586"></a><a name="zh-cn_topic_0118921498_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921498_row24071607"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921498_p3643149"><a name="zh-cn_topic_0118921498_p3643149"></a><a name="zh-cn_topic_0118921498_p3643149"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921498_p26659623"><a name="zh-cn_topic_0118921498_p26659623"></a><a name="zh-cn_topic_0118921498_p26659623"></a>Not Found</p>
</td>
</tr>
</tbody>
</table>

