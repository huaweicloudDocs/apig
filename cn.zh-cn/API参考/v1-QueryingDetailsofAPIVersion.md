# 查看版本详情<a name="ZH-CN_TOPIC_0000001081976169"></a>

## 功能介绍<a name="zh-cn_topic_0225568827_section56312882"></a>

查询某个指定的版本详情。

## URI<a name="zh-cn_topic_0225568827_section37053890"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568827_table61687544"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row6551303"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568827_p60893511"><a name="zh-cn_topic_0225568827_p60893511"></a><a name="zh-cn_topic_0225568827_p60893511"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568827_p33427368"><a name="zh-cn_topic_0225568827_p33427368"></a><a name="zh-cn_topic_0225568827_p33427368"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row23262289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568827_p5197291"><a name="zh-cn_topic_0225568827_p5197291"></a><a name="zh-cn_topic_0225568827_p5197291"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568827_p18327454"><a name="zh-cn_topic_0225568827_p18327454"></a><a name="zh-cn_topic_0225568827_p18327454"></a>/v1/{project_id}/apigw/instances/{instance_id}/apis/versions/{version_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568827_table14319067"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row47200048"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568827_p65107550"><a name="zh-cn_topic_0225568827_p65107550"></a><a name="zh-cn_topic_0225568827_p65107550"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568827_p39220237"><a name="zh-cn_topic_0225568827_p39220237"></a><a name="zh-cn_topic_0225568827_p39220237"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.46%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568827_p22722661"><a name="zh-cn_topic_0225568827_p22722661"></a><a name="zh-cn_topic_0225568827_p22722661"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="40.19%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568827_p28596237"><a name="zh-cn_topic_0225568827_p28596237"></a><a name="zh-cn_topic_0225568827_p28596237"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row1577314596193"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568827_p55878963"><a name="zh-cn_topic_0225568827_p55878963"></a><a name="zh-cn_topic_0225568827_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568827_p29902160"><a name="zh-cn_topic_0225568827_p29902160"></a><a name="zh-cn_topic_0225568827_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568827_p6155914"><a name="zh-cn_topic_0225568827_p6155914"></a><a name="zh-cn_topic_0225568827_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.19%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568827_p28867016"><a name="zh-cn_topic_0225568827_p28867016"></a><a name="zh-cn_topic_0225568827_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row75691259101913"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568827_p1780913159538"><a name="zh-cn_topic_0225568827_p1780913159538"></a><a name="zh-cn_topic_0225568827_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568827_p9809215115310"><a name="zh-cn_topic_0225568827_p9809215115310"></a><a name="zh-cn_topic_0225568827_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568827_p1280914152538"><a name="zh-cn_topic_0225568827_p1280914152538"></a><a name="zh-cn_topic_0225568827_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.19%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568827_p1880914157537"><a name="zh-cn_topic_0225568827_p1880914157537"></a><a name="zh-cn_topic_0225568827_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row34593837"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568827_p50637422"><a name="zh-cn_topic_0225568827_p50637422"></a><a name="zh-cn_topic_0225568827_p50637422"></a>version_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568827_p7990519"><a name="zh-cn_topic_0225568827_p7990519"></a><a name="zh-cn_topic_0225568827_p7990519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568827_p43252337"><a name="zh-cn_topic_0225568827_p43252337"></a><a name="zh-cn_topic_0225568827_p43252337"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="40.19%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568827_p13778436"><a name="zh-cn_topic_0225568827_p13778436"></a><a name="zh-cn_topic_0225568827_p13778436"></a>API版本的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568827_section65049557"></a>

无

## 响应消息<a name="zh-cn_topic_0225568827_section34522802"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568827_table11945837"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row18624964"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568827_p32227090"><a name="zh-cn_topic_0225568827_p32227090"></a><a name="zh-cn_topic_0225568827_p32227090"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568827_p60257464"><a name="zh-cn_topic_0225568827_p60257464"></a><a name="zh-cn_topic_0225568827_p60257464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568827_p49016415"><a name="zh-cn_topic_0225568827_p49016415"></a><a name="zh-cn_topic_0225568827_p49016415"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row10906670"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p11025102"><a name="zh-cn_topic_0225568827_p11025102"></a><a name="zh-cn_topic_0225568827_p11025102"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p20618087"><a name="zh-cn_topic_0225568827_p20618087"></a><a name="zh-cn_topic_0225568827_p20618087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p59452320"><a name="zh-cn_topic_0225568827_p59452320"></a><a name="zh-cn_topic_0225568827_p59452320"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row65308832"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p55524012"><a name="zh-cn_topic_0225568827_p55524012"></a><a name="zh-cn_topic_0225568827_p55524012"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1151149"><a name="zh-cn_topic_0225568827_p1151149"></a><a name="zh-cn_topic_0225568827_p1151149"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p26134283"><a name="zh-cn_topic_0225568827_p26134283"></a><a name="zh-cn_topic_0225568827_p26134283"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row33881960"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p60084252"><a name="zh-cn_topic_0225568827_p60084252"></a><a name="zh-cn_topic_0225568827_p60084252"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p34986207"><a name="zh-cn_topic_0225568827_p34986207"></a><a name="zh-cn_topic_0225568827_p34986207"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p15310556"><a name="zh-cn_topic_0225568827_p15310556"></a><a name="zh-cn_topic_0225568827_p15310556"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row3577279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p21324163"><a name="zh-cn_topic_0225568827_p21324163"></a><a name="zh-cn_topic_0225568827_p21324163"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p49535636"><a name="zh-cn_topic_0225568827_p49535636"></a><a name="zh-cn_topic_0225568827_p49535636"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p52963545"><a name="zh-cn_topic_0225568827_p52963545"></a><a name="zh-cn_topic_0225568827_p52963545"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row6909858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p22827665"><a name="zh-cn_topic_0225568827_p22827665"></a><a name="zh-cn_topic_0225568827_p22827665"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p37101609"><a name="zh-cn_topic_0225568827_p37101609"></a><a name="zh-cn_topic_0225568827_p37101609"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p52440337"><a name="zh-cn_topic_0225568827_p52440337"></a><a name="zh-cn_topic_0225568827_p52440337"></a>API的状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row2200986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p44062206"><a name="zh-cn_topic_0225568827_p44062206"></a><a name="zh-cn_topic_0225568827_p44062206"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p12268934"><a name="zh-cn_topic_0225568827_p12268934"></a><a name="zh-cn_topic_0225568827_p12268934"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p54259611"><a name="zh-cn_topic_0225568827_p54259611"></a><a name="zh-cn_topic_0225568827_p54259611"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row18574453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p28135752"><a name="zh-cn_topic_0225568827_p28135752"></a><a name="zh-cn_topic_0225568827_p28135752"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p64403419"><a name="zh-cn_topic_0225568827_p64403419"></a><a name="zh-cn_topic_0225568827_p64403419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p49294422"><a name="zh-cn_topic_0225568827_p49294422"></a><a name="zh-cn_topic_0225568827_p49294422"></a>API版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row40996618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p32391798"><a name="zh-cn_topic_0225568827_p32391798"></a><a name="zh-cn_topic_0225568827_p32391798"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p6489949"><a name="zh-cn_topic_0225568827_p6489949"></a><a name="zh-cn_topic_0225568827_p6489949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p55923881"><a name="zh-cn_topic_0225568827_p55923881"></a><a name="zh-cn_topic_0225568827_p55923881"></a>API访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row33552889"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p33429463"><a name="zh-cn_topic_0225568827_p33429463"></a><a name="zh-cn_topic_0225568827_p33429463"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p23431949"><a name="zh-cn_topic_0225568827_p23431949"></a><a name="zh-cn_topic_0225568827_p23431949"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p18939716"><a name="zh-cn_topic_0225568827_p18939716"></a><a name="zh-cn_topic_0225568827_p18939716"></a>API请求方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row36239719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p49736130"><a name="zh-cn_topic_0225568827_p49736130"></a><a name="zh-cn_topic_0225568827_p49736130"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p2094705"><a name="zh-cn_topic_0225568827_p2094705"></a><a name="zh-cn_topic_0225568827_p2094705"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p35453405"><a name="zh-cn_topic_0225568827_p35453405"></a><a name="zh-cn_topic_0225568827_p35453405"></a>API访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row50645189"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p8619606"><a name="zh-cn_topic_0225568827_p8619606"></a><a name="zh-cn_topic_0225568827_p8619606"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p27099480"><a name="zh-cn_topic_0225568827_p27099480"></a><a name="zh-cn_topic_0225568827_p27099480"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p47574258"><a name="zh-cn_topic_0225568827_p47574258"></a><a name="zh-cn_topic_0225568827_p47574258"></a>API认证方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row7122194222210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p45549491969"><a name="zh-cn_topic_0225568827_p45549491969"></a><a name="zh-cn_topic_0225568827_p45549491969"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p19554194910611"><a name="zh-cn_topic_0225568827_p19554194910611"></a><a name="zh-cn_topic_0225568827_p19554194910611"></a>字段数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p155541490617"><a name="zh-cn_topic_0225568827_p155541490617"></a><a name="zh-cn_topic_0225568827_p155541490617"></a>API认证方式参数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row16771143923415"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p4426105522114"><a name="zh-cn_topic_0225568827_p4426105522114"></a><a name="zh-cn_topic_0225568827_p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p6293346133419"><a name="zh-cn_topic_0225568827_p6293346133419"></a><a name="zh-cn_topic_0225568827_p6293346133419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p116491557133012"><a name="zh-cn_topic_0225568827_p116491557133012"></a><a name="zh-cn_topic_0225568827_p116491557133012"></a>前端自定义认证对象的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row25515144"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p53460794"><a name="zh-cn_topic_0225568827_p53460794"></a><a name="zh-cn_topic_0225568827_p53460794"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p35357081"><a name="zh-cn_topic_0225568827_p35357081"></a><a name="zh-cn_topic_0225568827_p35357081"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p45351308"><a name="zh-cn_topic_0225568827_p45351308"></a><a name="zh-cn_topic_0225568827_p45351308"></a>API匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row5508593"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p43542878"><a name="zh-cn_topic_0225568827_p43542878"></a><a name="zh-cn_topic_0225568827_p43542878"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p37312211"><a name="zh-cn_topic_0225568827_p37312211"></a><a name="zh-cn_topic_0225568827_p37312211"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p2390265"><a name="zh-cn_topic_0225568827_p2390265"></a><a name="zh-cn_topic_0225568827_p2390265"></a>API注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row21512390"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p64782007"><a name="zh-cn_topic_0225568827_p64782007"></a><a name="zh-cn_topic_0225568827_p64782007"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p12851246"><a name="zh-cn_topic_0225568827_p12851246"></a><a name="zh-cn_topic_0225568827_p12851246"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p34317968"><a name="zh-cn_topic_0225568827_p34317968"></a><a name="zh-cn_topic_0225568827_p34317968"></a>API修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row40426262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p53301766"><a name="zh-cn_topic_0225568827_p53301766"></a><a name="zh-cn_topic_0225568827_p53301766"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p22475799"><a name="zh-cn_topic_0225568827_p22475799"></a><a name="zh-cn_topic_0225568827_p22475799"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p8600432"><a name="zh-cn_topic_0225568827_p8600432"></a><a name="zh-cn_topic_0225568827_p8600432"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row10295032"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p28591249"><a name="zh-cn_topic_0225568827_p28591249"></a><a name="zh-cn_topic_0225568827_p28591249"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p34189831"><a name="zh-cn_topic_0225568827_p34189831"></a><a name="zh-cn_topic_0225568827_p34189831"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p17912897"><a name="zh-cn_topic_0225568827_p17912897"></a><a name="zh-cn_topic_0225568827_p17912897"></a>后端类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row26998347"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p39382503"><a name="zh-cn_topic_0225568827_p39382503"></a><a name="zh-cn_topic_0225568827_p39382503"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p35866171"><a name="zh-cn_topic_0225568827_p35866171"></a><a name="zh-cn_topic_0225568827_p35866171"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p19478768"><a name="zh-cn_topic_0225568827_p19478768"></a><a name="zh-cn_topic_0225568827_p19478768"></a>发布的环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row41091190"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p40052127"><a name="zh-cn_topic_0225568827_p40052127"></a><a name="zh-cn_topic_0225568827_p40052127"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p22996860"><a name="zh-cn_topic_0225568827_p22996860"></a><a name="zh-cn_topic_0225568827_p22996860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p50806390"><a name="zh-cn_topic_0225568827_p50806390"></a><a name="zh-cn_topic_0225568827_p50806390"></a>发布的环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row54604329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p60874520"><a name="zh-cn_topic_0225568827_p60874520"></a><a name="zh-cn_topic_0225568827_p60874520"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p31889112"><a name="zh-cn_topic_0225568827_p31889112"></a><a name="zh-cn_topic_0225568827_p31889112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p32881297"><a name="zh-cn_topic_0225568827_p32881297"></a><a name="zh-cn_topic_0225568827_p32881297"></a>发布记录的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row50078910"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p29859916"><a name="zh-cn_topic_0225568827_p29859916"></a><a name="zh-cn_topic_0225568827_p29859916"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p2734171"><a name="zh-cn_topic_0225568827_p2734171"></a><a name="zh-cn_topic_0225568827_p2734171"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p20141331"><a name="zh-cn_topic_0225568827_p20141331"></a><a name="zh-cn_topic_0225568827_p20141331"></a>是否需要编排</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row660031719333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p7679321181114"><a name="zh-cn_topic_0225568827_p7679321181114"></a><a name="zh-cn_topic_0225568827_p7679321181114"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p166791021161110"><a name="zh-cn_topic_0225568827_p166791021161110"></a><a name="zh-cn_topic_0225568827_p166791021161110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1167913211111"><a name="zh-cn_topic_0225568827_p1167913211111"></a><a name="zh-cn_topic_0225568827_p1167913211111"></a>服务名称标签，待废弃字段</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row136915684418"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p5689175210267"><a name="zh-cn_topic_0225568827_p5689175210267"></a><a name="zh-cn_topic_0225568827_p5689175210267"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p969065252610"><a name="zh-cn_topic_0225568827_p969065252610"></a><a name="zh-cn_topic_0225568827_p969065252610"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p10599103122713"><a name="zh-cn_topic_0225568827_p10599103122713"></a><a name="zh-cn_topic_0225568827_p10599103122713"></a>标签</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row37247202339"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p172881819162714"><a name="zh-cn_topic_0225568827_p172881819162714"></a><a name="zh-cn_topic_0225568827_p172881819162714"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p163043196278"><a name="zh-cn_topic_0225568827_p163043196278"></a><a name="zh-cn_topic_0225568827_p163043196278"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p13320121932715"><a name="zh-cn_topic_0225568827_p13320121932715"></a><a name="zh-cn_topic_0225568827_p13320121932715"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1749718315379"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p105561154343"><a name="zh-cn_topic_0225568827_p105561154343"></a><a name="zh-cn_topic_0225568827_p105561154343"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p75719510345"><a name="zh-cn_topic_0225568827_p75719510345"></a><a name="zh-cn_topic_0225568827_p75719510345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1571450346"><a name="zh-cn_topic_0225568827_p1571450346"></a><a name="zh-cn_topic_0225568827_p1571450346"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row140423763710"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p106341354349"><a name="zh-cn_topic_0225568827_p106341354349"></a><a name="zh-cn_topic_0225568827_p106341354349"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1463416511341"><a name="zh-cn_topic_0225568827_p1463416511341"></a><a name="zh-cn_topic_0225568827_p1463416511341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p46509516343"><a name="zh-cn_topic_0225568827_p46509516343"></a><a name="zh-cn_topic_0225568827_p46509516343"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row19654193413373"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p19696185133419"><a name="zh-cn_topic_0225568827_p19696185133419"></a><a name="zh-cn_topic_0225568827_p19696185133419"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p369665183416"><a name="zh-cn_topic_0225568827_p369665183416"></a><a name="zh-cn_topic_0225568827_p369665183416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p77123514347"><a name="zh-cn_topic_0225568827_p77123514347"></a><a name="zh-cn_topic_0225568827_p77123514347"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row310212653315"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p31023265331"><a name="zh-cn_topic_0225568827_p31023265331"></a><a name="zh-cn_topic_0225568827_p31023265331"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p810252612338"><a name="zh-cn_topic_0225568827_p810252612338"></a><a name="zh-cn_topic_0225568827_p810252612338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p141028264336"><a name="zh-cn_topic_0225568827_p141028264336"></a><a name="zh-cn_topic_0225568827_p141028264336"></a>分组的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row7851535153310"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p5859351331"><a name="zh-cn_topic_0225568827_p5859351331"></a><a name="zh-cn_topic_0225568827_p5859351331"></a>version_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p11857358338"><a name="zh-cn_topic_0225568827_p11857358338"></a><a name="zh-cn_topic_0225568827_p11857358338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p28512352339"><a name="zh-cn_topic_0225568827_p28512352339"></a><a name="zh-cn_topic_0225568827_p28512352339"></a>版本编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row19788230203313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p13788103073318"><a name="zh-cn_topic_0225568827_p13788103073318"></a><a name="zh-cn_topic_0225568827_p13788103073318"></a>publish_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p14788203013335"><a name="zh-cn_topic_0225568827_p14788203013335"></a><a name="zh-cn_topic_0225568827_p14788203013335"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1478815302335"><a name="zh-cn_topic_0225568827_p1478815302335"></a><a name="zh-cn_topic_0225568827_p1478815302335"></a>版本发布时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row47054253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p53298164"><a name="zh-cn_topic_0225568827_p53298164"></a><a name="zh-cn_topic_0225568827_p53298164"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p22184056"><a name="zh-cn_topic_0225568827_p22184056"></a><a name="zh-cn_topic_0225568827_p22184056"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p52078112"><a name="zh-cn_topic_0225568827_p52078112"></a><a name="zh-cn_topic_0225568827_p52078112"></a>后端服务：web后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row66049829"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p48435967"><a name="zh-cn_topic_0225568827_p48435967"></a><a name="zh-cn_topic_0225568827_p48435967"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p30999282"><a name="zh-cn_topic_0225568827_p30999282"></a><a name="zh-cn_topic_0225568827_p30999282"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p27913893"><a name="zh-cn_topic_0225568827_p27913893"></a><a name="zh-cn_topic_0225568827_p27913893"></a>后端服务：MOCK详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row49898446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p15242308"><a name="zh-cn_topic_0225568827_p15242308"></a><a name="zh-cn_topic_0225568827_p15242308"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p26667472"><a name="zh-cn_topic_0225568827_p26667472"></a><a name="zh-cn_topic_0225568827_p26667472"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p12581591"><a name="zh-cn_topic_0225568827_p12581591"></a><a name="zh-cn_topic_0225568827_p12581591"></a>后端服务：函数工作流后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row3996134219376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p13999938164017"><a name="zh-cn_topic_0225568827_p13999938164017"></a><a name="zh-cn_topic_0225568827_p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1999203815404"><a name="zh-cn_topic_0225568827_p1999203815404"></a><a name="zh-cn_topic_0225568827_p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p11999143884013"><a name="zh-cn_topic_0225568827_p11999143884013"></a><a name="zh-cn_topic_0225568827_p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1854312455375"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p420294234017"><a name="zh-cn_topic_0225568827_p420294234017"></a><a name="zh-cn_topic_0225568827_p420294234017"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p17202184217401"><a name="zh-cn_topic_0225568827_p17202184217401"></a><a name="zh-cn_topic_0225568827_p17202184217401"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p112025421400"><a name="zh-cn_topic_0225568827_p112025421400"></a><a name="zh-cn_topic_0225568827_p112025421400"></a>API的后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  backend\_api参数说明

<a name="zh-cn_topic_0225568827_table46125461"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row21441395"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568827_p59031425"><a name="zh-cn_topic_0225568827_p59031425"></a><a name="zh-cn_topic_0225568827_p59031425"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568827_p16816124"><a name="zh-cn_topic_0225568827_p16816124"></a><a name="zh-cn_topic_0225568827_p16816124"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568827_p19928779"><a name="zh-cn_topic_0225568827_p19928779"></a><a name="zh-cn_topic_0225568827_p19928779"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row3618391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p24654215"><a name="zh-cn_topic_0225568827_p24654215"></a><a name="zh-cn_topic_0225568827_p24654215"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p50834371"><a name="zh-cn_topic_0225568827_p50834371"></a><a name="zh-cn_topic_0225568827_p50834371"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p23943412"><a name="zh-cn_topic_0225568827_p23943412"></a><a name="zh-cn_topic_0225568827_p23943412"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row14164124"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p6443415"><a name="zh-cn_topic_0225568827_p6443415"></a><a name="zh-cn_topic_0225568827_p6443415"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p52154619"><a name="zh-cn_topic_0225568827_p52154619"></a><a name="zh-cn_topic_0225568827_p52154619"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p63774574"><a name="zh-cn_topic_0225568827_p63774574"></a><a name="zh-cn_topic_0225568827_p63774574"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row37100262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p52331254"><a name="zh-cn_topic_0225568827_p52331254"></a><a name="zh-cn_topic_0225568827_p52331254"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p10973162"><a name="zh-cn_topic_0225568827_p10973162"></a><a name="zh-cn_topic_0225568827_p10973162"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p15120014693"><a name="zh-cn_topic_0225568827_p15120014693"></a><a name="zh-cn_topic_0225568827_p15120014693"></a>后端endpoint</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row13480579"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p18185121"><a name="zh-cn_topic_0225568827_p18185121"></a><a name="zh-cn_topic_0225568827_p18185121"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p63708736"><a name="zh-cn_topic_0225568827_p63708736"></a><a name="zh-cn_topic_0225568827_p63708736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p60134024"><a name="zh-cn_topic_0225568827_p60134024"></a><a name="zh-cn_topic_0225568827_p60134024"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row4335306"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p15615521"><a name="zh-cn_topic_0225568827_p15615521"></a><a name="zh-cn_topic_0225568827_p15615521"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p56897717"><a name="zh-cn_topic_0225568827_p56897717"></a><a name="zh-cn_topic_0225568827_p56897717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p45312365"><a name="zh-cn_topic_0225568827_p45312365"></a><a name="zh-cn_topic_0225568827_p45312365"></a>访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row5158106"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p15153476"><a name="zh-cn_topic_0225568827_p15153476"></a><a name="zh-cn_topic_0225568827_p15153476"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p19472071"><a name="zh-cn_topic_0225568827_p19472071"></a><a name="zh-cn_topic_0225568827_p19472071"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p33733898"><a name="zh-cn_topic_0225568827_p33733898"></a><a name="zh-cn_topic_0225568827_p33733898"></a>访问方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row35169627"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p30167521"><a name="zh-cn_topic_0225568827_p30167521"></a><a name="zh-cn_topic_0225568827_p30167521"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p27650173"><a name="zh-cn_topic_0225568827_p27650173"></a><a name="zh-cn_topic_0225568827_p27650173"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p25071508"><a name="zh-cn_topic_0225568827_p25071508"></a><a name="zh-cn_topic_0225568827_p25071508"></a>访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row24316986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p23518872"><a name="zh-cn_topic_0225568827_p23518872"></a><a name="zh-cn_topic_0225568827_p23518872"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p25980454"><a name="zh-cn_topic_0225568827_p25980454"></a><a name="zh-cn_topic_0225568827_p25980454"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p24041996"><a name="zh-cn_topic_0225568827_p24041996"></a><a name="zh-cn_topic_0225568827_p24041996"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row15051376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p11201934"><a name="zh-cn_topic_0225568827_p11201934"></a><a name="zh-cn_topic_0225568827_p11201934"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p34941465"><a name="zh-cn_topic_0225568827_p34941465"></a><a name="zh-cn_topic_0225568827_p34941465"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p11686392"><a name="zh-cn_topic_0225568827_p11686392"></a><a name="zh-cn_topic_0225568827_p11686392"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row38068667"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p63663156"><a name="zh-cn_topic_0225568827_p63663156"></a><a name="zh-cn_topic_0225568827_p63663156"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p56441973"><a name="zh-cn_topic_0225568827_p56441973"></a><a name="zh-cn_topic_0225568827_p56441973"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p8397095"><a name="zh-cn_topic_0225568827_p8397095"></a><a name="zh-cn_topic_0225568827_p8397095"></a>修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row8464993"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p14575871"><a name="zh-cn_topic_0225568827_p14575871"></a><a name="zh-cn_topic_0225568827_p14575871"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p39794913"><a name="zh-cn_topic_0225568827_p39794913"></a><a name="zh-cn_topic_0225568827_p39794913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p2162544"><a name="zh-cn_topic_0225568827_p2162544"></a><a name="zh-cn_topic_0225568827_p2162544"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row19462899"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p32991024"><a name="zh-cn_topic_0225568827_p32991024"></a><a name="zh-cn_topic_0225568827_p32991024"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p55027277"><a name="zh-cn_topic_0225568827_p55027277"></a><a name="zh-cn_topic_0225568827_p55027277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p28024434"><a name="zh-cn_topic_0225568827_p28024434"></a><a name="zh-cn_topic_0225568827_p28024434"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row50893320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p28718221"><a name="zh-cn_topic_0225568827_p28718221"></a><a name="zh-cn_topic_0225568827_p28718221"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p44474542"><a name="zh-cn_topic_0225568827_p44474542"></a><a name="zh-cn_topic_0225568827_p44474542"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p45668181"><a name="zh-cn_topic_0225568827_p45668181"></a><a name="zh-cn_topic_0225568827_p45668181"></a>VPC通道信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row2093663014370"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p194723346378"><a name="zh-cn_topic_0225568827_p194723346378"></a><a name="zh-cn_topic_0225568827_p194723346378"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p146116361378"><a name="zh-cn_topic_0225568827_p146116361378"></a><a name="zh-cn_topic_0225568827_p146116361378"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p710015394375"><a name="zh-cn_topic_0225568827_p710015394375"></a><a name="zh-cn_topic_0225568827_p710015394375"></a>后端自定义认证对象的ID</p>
</td>
</tr>
</tbody>
</table>

**表 5**  mock\_info参数说明

<a name="zh-cn_topic_0225568827_table8360445"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row61660858"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568827_p28473615"><a name="zh-cn_topic_0225568827_p28473615"></a><a name="zh-cn_topic_0225568827_p28473615"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568827_p24661464"><a name="zh-cn_topic_0225568827_p24661464"></a><a name="zh-cn_topic_0225568827_p24661464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568827_p51421566"><a name="zh-cn_topic_0225568827_p51421566"></a><a name="zh-cn_topic_0225568827_p51421566"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row4397288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p20636030"><a name="zh-cn_topic_0225568827_p20636030"></a><a name="zh-cn_topic_0225568827_p20636030"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p60905770"><a name="zh-cn_topic_0225568827_p60905770"></a><a name="zh-cn_topic_0225568827_p60905770"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p34420305"><a name="zh-cn_topic_0225568827_p34420305"></a><a name="zh-cn_topic_0225568827_p34420305"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row41347295"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p60796621"><a name="zh-cn_topic_0225568827_p60796621"></a><a name="zh-cn_topic_0225568827_p60796621"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p25579243"><a name="zh-cn_topic_0225568827_p25579243"></a><a name="zh-cn_topic_0225568827_p25579243"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p58652769"><a name="zh-cn_topic_0225568827_p58652769"></a><a name="zh-cn_topic_0225568827_p58652769"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row58112877"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p9522587"><a name="zh-cn_topic_0225568827_p9522587"></a><a name="zh-cn_topic_0225568827_p9522587"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p33132086"><a name="zh-cn_topic_0225568827_p33132086"></a><a name="zh-cn_topic_0225568827_p33132086"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p66453285"><a name="zh-cn_topic_0225568827_p66453285"></a><a name="zh-cn_topic_0225568827_p66453285"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row61208656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p58954073"><a name="zh-cn_topic_0225568827_p58954073"></a><a name="zh-cn_topic_0225568827_p58954073"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p10550570"><a name="zh-cn_topic_0225568827_p10550570"></a><a name="zh-cn_topic_0225568827_p10550570"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p49289836"><a name="zh-cn_topic_0225568827_p49289836"></a><a name="zh-cn_topic_0225568827_p49289836"></a>返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row40955342"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p29048444"><a name="zh-cn_topic_0225568827_p29048444"></a><a name="zh-cn_topic_0225568827_p29048444"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p4113774"><a name="zh-cn_topic_0225568827_p4113774"></a><a name="zh-cn_topic_0225568827_p4113774"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p64780301"><a name="zh-cn_topic_0225568827_p64780301"></a><a name="zh-cn_topic_0225568827_p64780301"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row46151800"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p47308357"><a name="zh-cn_topic_0225568827_p47308357"></a><a name="zh-cn_topic_0225568827_p47308357"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p6771698"><a name="zh-cn_topic_0225568827_p6771698"></a><a name="zh-cn_topic_0225568827_p6771698"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p11636647"><a name="zh-cn_topic_0225568827_p11636647"></a><a name="zh-cn_topic_0225568827_p11636647"></a>修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row37620965"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p27399290"><a name="zh-cn_topic_0225568827_p27399290"></a><a name="zh-cn_topic_0225568827_p27399290"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p4749995"><a name="zh-cn_topic_0225568827_p4749995"></a><a name="zh-cn_topic_0225568827_p4749995"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p49205346"><a name="zh-cn_topic_0225568827_p49205346"></a><a name="zh-cn_topic_0225568827_p49205346"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 6**  func\_info参数说明

<a name="zh-cn_topic_0225568827_table40194930"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row47908359"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568827_p55371884"><a name="zh-cn_topic_0225568827_p55371884"></a><a name="zh-cn_topic_0225568827_p55371884"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568827_p55937605"><a name="zh-cn_topic_0225568827_p55937605"></a><a name="zh-cn_topic_0225568827_p55937605"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568827_p34652155"><a name="zh-cn_topic_0225568827_p34652155"></a><a name="zh-cn_topic_0225568827_p34652155"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row55361141"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p55067419"><a name="zh-cn_topic_0225568827_p55067419"></a><a name="zh-cn_topic_0225568827_p55067419"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p31275991"><a name="zh-cn_topic_0225568827_p31275991"></a><a name="zh-cn_topic_0225568827_p31275991"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p50327310"><a name="zh-cn_topic_0225568827_p50327310"></a><a name="zh-cn_topic_0225568827_p50327310"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row50292612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p47169794"><a name="zh-cn_topic_0225568827_p47169794"></a><a name="zh-cn_topic_0225568827_p47169794"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p62656944"><a name="zh-cn_topic_0225568827_p62656944"></a><a name="zh-cn_topic_0225568827_p62656944"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p42047670"><a name="zh-cn_topic_0225568827_p42047670"></a><a name="zh-cn_topic_0225568827_p42047670"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row42884714"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p51109800"><a name="zh-cn_topic_0225568827_p51109800"></a><a name="zh-cn_topic_0225568827_p51109800"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p46253139"><a name="zh-cn_topic_0225568827_p46253139"></a><a name="zh-cn_topic_0225568827_p46253139"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p55516754"><a name="zh-cn_topic_0225568827_p55516754"></a><a name="zh-cn_topic_0225568827_p55516754"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row29888741"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p5068926"><a name="zh-cn_topic_0225568827_p5068926"></a><a name="zh-cn_topic_0225568827_p5068926"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p7929823"><a name="zh-cn_topic_0225568827_p7929823"></a><a name="zh-cn_topic_0225568827_p7929823"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p38335921"><a name="zh-cn_topic_0225568827_p38335921"></a><a name="zh-cn_topic_0225568827_p38335921"></a>函数URN</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row9478971"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p29599225"><a name="zh-cn_topic_0225568827_p29599225"></a><a name="zh-cn_topic_0225568827_p29599225"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p48727035"><a name="zh-cn_topic_0225568827_p48727035"></a><a name="zh-cn_topic_0225568827_p48727035"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p54575786"><a name="zh-cn_topic_0225568827_p54575786"></a><a name="zh-cn_topic_0225568827_p54575786"></a>调用类型：async|sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row21420029"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p57300826"><a name="zh-cn_topic_0225568827_p57300826"></a><a name="zh-cn_topic_0225568827_p57300826"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p10855319"><a name="zh-cn_topic_0225568827_p10855319"></a><a name="zh-cn_topic_0225568827_p10855319"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p6865628"><a name="zh-cn_topic_0225568827_p6865628"></a><a name="zh-cn_topic_0225568827_p6865628"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row61790658"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p38987367"><a name="zh-cn_topic_0225568827_p38987367"></a><a name="zh-cn_topic_0225568827_p38987367"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p3860136"><a name="zh-cn_topic_0225568827_p3860136"></a><a name="zh-cn_topic_0225568827_p3860136"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p44235631"><a name="zh-cn_topic_0225568827_p44235631"></a><a name="zh-cn_topic_0225568827_p44235631"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row62576359"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p35520303"><a name="zh-cn_topic_0225568827_p35520303"></a><a name="zh-cn_topic_0225568827_p35520303"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p58572271"><a name="zh-cn_topic_0225568827_p58572271"></a><a name="zh-cn_topic_0225568827_p58572271"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p46733520"><a name="zh-cn_topic_0225568827_p46733520"></a><a name="zh-cn_topic_0225568827_p46733520"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row17948500"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p44542409"><a name="zh-cn_topic_0225568827_p44542409"></a><a name="zh-cn_topic_0225568827_p44542409"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p51165362"><a name="zh-cn_topic_0225568827_p51165362"></a><a name="zh-cn_topic_0225568827_p51165362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p50753656"><a name="zh-cn_topic_0225568827_p50753656"></a><a name="zh-cn_topic_0225568827_p50753656"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 7**  req\_params参数说明

<a name="zh-cn_topic_0225568827_table197251634194412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row2075603420446"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568827_p11756234184411"><a name="zh-cn_topic_0225568827_p11756234184411"></a><a name="zh-cn_topic_0225568827_p11756234184411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568827_p777143420447"><a name="zh-cn_topic_0225568827_p777143420447"></a><a name="zh-cn_topic_0225568827_p777143420447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568827_p5771193415446"><a name="zh-cn_topic_0225568827_p5771193415446"></a><a name="zh-cn_topic_0225568827_p5771193415446"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row85313200454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p1753320144511"><a name="zh-cn_topic_0225568827_p1753320144511"></a><a name="zh-cn_topic_0225568827_p1753320144511"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p75302015450"><a name="zh-cn_topic_0225568827_p75302015450"></a><a name="zh-cn_topic_0225568827_p75302015450"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p653162014451"><a name="zh-cn_topic_0225568827_p653162014451"></a><a name="zh-cn_topic_0225568827_p653162014451"></a>参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row8786123464413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p578618344445"><a name="zh-cn_topic_0225568827_p578618344445"></a><a name="zh-cn_topic_0225568827_p578618344445"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1480313412443"><a name="zh-cn_topic_0225568827_p1480313412443"></a><a name="zh-cn_topic_0225568827_p1480313412443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p48033344445"><a name="zh-cn_topic_0225568827_p48033344445"></a><a name="zh-cn_topic_0225568827_p48033344445"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row13818193434411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p781810341448"><a name="zh-cn_topic_0225568827_p781810341448"></a><a name="zh-cn_topic_0225568827_p781810341448"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p18342034114419"><a name="zh-cn_topic_0225568827_p18342034114419"></a><a name="zh-cn_topic_0225568827_p18342034114419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p083493413441"><a name="zh-cn_topic_0225568827_p083493413441"></a><a name="zh-cn_topic_0225568827_p083493413441"></a>参数类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row17850234124414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p18865203414418"><a name="zh-cn_topic_0225568827_p18865203414418"></a><a name="zh-cn_topic_0225568827_p18865203414418"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p16881203415443"><a name="zh-cn_topic_0225568827_p16881203415443"></a><a name="zh-cn_topic_0225568827_p16881203415443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p788120340445"><a name="zh-cn_topic_0225568827_p788120340445"></a><a name="zh-cn_topic_0225568827_p788120340445"></a>参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row99121534134414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p18912934114419"><a name="zh-cn_topic_0225568827_p18912934114419"></a><a name="zh-cn_topic_0225568827_p18912934114419"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p139281534104415"><a name="zh-cn_topic_0225568827_p139281534104415"></a><a name="zh-cn_topic_0225568827_p139281534104415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1592853454412"><a name="zh-cn_topic_0225568827_p1592853454412"></a><a name="zh-cn_topic_0225568827_p1592853454412"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1594315349446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p994311348442"><a name="zh-cn_topic_0225568827_p994311348442"></a><a name="zh-cn_topic_0225568827_p994311348442"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1495973414419"><a name="zh-cn_topic_0225568827_p1495973414419"></a><a name="zh-cn_topic_0225568827_p1495973414419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1695953413449"><a name="zh-cn_topic_0225568827_p1695953413449"></a><a name="zh-cn_topic_0225568827_p1695953413449"></a>参数示例值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1959173474410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p2974183417445"><a name="zh-cn_topic_0225568827_p2974183417445"></a><a name="zh-cn_topic_0225568827_p2974183417445"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p13974143417443"><a name="zh-cn_topic_0225568827_p13974143417443"></a><a name="zh-cn_topic_0225568827_p13974143417443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p699053414444"><a name="zh-cn_topic_0225568827_p699053414444"></a><a name="zh-cn_topic_0225568827_p699053414444"></a>是否必须</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row662354446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p66183524412"><a name="zh-cn_topic_0225568827_p66183524412"></a><a name="zh-cn_topic_0225568827_p66183524412"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p32133519447"><a name="zh-cn_topic_0225568827_p32133519447"></a><a name="zh-cn_topic_0225568827_p32133519447"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p18371535124417"><a name="zh-cn_topic_0225568827_p18371535124417"></a><a name="zh-cn_topic_0225568827_p18371535124417"></a>是否开启校验</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1053435144414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p653133513441"><a name="zh-cn_topic_0225568827_p653133513441"></a><a name="zh-cn_topic_0225568827_p653133513441"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1867183512446"><a name="zh-cn_topic_0225568827_p1867183512446"></a><a name="zh-cn_topic_0225568827_p1867183512446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p567123584420"><a name="zh-cn_topic_0225568827_p567123584420"></a><a name="zh-cn_topic_0225568827_p567123584420"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row7100203515443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p181002035154415"><a name="zh-cn_topic_0225568827_p181002035154415"></a><a name="zh-cn_topic_0225568827_p181002035154415"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p161151635164413"><a name="zh-cn_topic_0225568827_p161151635164413"></a><a name="zh-cn_topic_0225568827_p161151635164413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p9115133544413"><a name="zh-cn_topic_0225568827_p9115133544413"></a><a name="zh-cn_topic_0225568827_p9115133544413"></a>参数枚举值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p151311235144415"><a name="zh-cn_topic_0225568827_p151311235144415"></a><a name="zh-cn_topic_0225568827_p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p713112353443"><a name="zh-cn_topic_0225568827_p713112353443"></a><a name="zh-cn_topic_0225568827_p713112353443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p01464350441"><a name="zh-cn_topic_0225568827_p01464350441"></a><a name="zh-cn_topic_0225568827_p01464350441"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p8146203564415"><a name="zh-cn_topic_0225568827_p8146203564415"></a><a name="zh-cn_topic_0225568827_p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p31627353442"><a name="zh-cn_topic_0225568827_p31627353442"></a><a name="zh-cn_topic_0225568827_p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p117823511445"><a name="zh-cn_topic_0225568827_p117823511445"></a><a name="zh-cn_topic_0225568827_p117823511445"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p61782355443"><a name="zh-cn_topic_0225568827_p61782355443"></a><a name="zh-cn_topic_0225568827_p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p201932035194417"><a name="zh-cn_topic_0225568827_p201932035194417"></a><a name="zh-cn_topic_0225568827_p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1119312351443"><a name="zh-cn_topic_0225568827_p1119312351443"></a><a name="zh-cn_topic_0225568827_p1119312351443"></a>参数最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p12209535144412"><a name="zh-cn_topic_0225568827_p12209535144412"></a><a name="zh-cn_topic_0225568827_p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p12251035164419"><a name="zh-cn_topic_0225568827_p12251035164419"></a><a name="zh-cn_topic_0225568827_p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p13225335194419"><a name="zh-cn_topic_0225568827_p13225335194419"></a><a name="zh-cn_topic_0225568827_p13225335194419"></a>参数最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p52401735134413"><a name="zh-cn_topic_0225568827_p52401735134413"></a><a name="zh-cn_topic_0225568827_p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p12240153510443"><a name="zh-cn_topic_0225568827_p12240153510443"></a><a name="zh-cn_topic_0225568827_p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1256035204417"><a name="zh-cn_topic_0225568827_p1256035204417"></a><a name="zh-cn_topic_0225568827_p1256035204417"></a>正则校验规则</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p202561335114413"><a name="zh-cn_topic_0225568827_p202561335114413"></a><a name="zh-cn_topic_0225568827_p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p16271035114412"><a name="zh-cn_topic_0225568827_p16271035114412"></a><a name="zh-cn_topic_0225568827_p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1628793511445"><a name="zh-cn_topic_0225568827_p1628793511445"></a><a name="zh-cn_topic_0225568827_p1628793511445"></a>JSON校验规则</p>
</td>
</tr>
</tbody>
</table>

**表 8**  backend\_params参数说明

<a name="zh-cn_topic_0225568827_table9287113513446"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row4302173564419"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568827_p33182355443"><a name="zh-cn_topic_0225568827_p33182355443"></a><a name="zh-cn_topic_0225568827_p33182355443"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568827_p14334103544415"><a name="zh-cn_topic_0225568827_p14334103544415"></a><a name="zh-cn_topic_0225568827_p14334103544415"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568827_p19334153517444"><a name="zh-cn_topic_0225568827_p19334153517444"></a><a name="zh-cn_topic_0225568827_p19334153517444"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row17142774611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p47152713464"><a name="zh-cn_topic_0225568827_p47152713464"></a><a name="zh-cn_topic_0225568827_p47152713464"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1717279463"><a name="zh-cn_topic_0225568827_p1717279463"></a><a name="zh-cn_topic_0225568827_p1717279463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p27122714620"><a name="zh-cn_topic_0225568827_p27122714620"></a><a name="zh-cn_topic_0225568827_p27122714620"></a>参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row2936129114713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p199361729154717"><a name="zh-cn_topic_0225568827_p199361729154717"></a><a name="zh-cn_topic_0225568827_p199361729154717"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1693652934715"><a name="zh-cn_topic_0225568827_p1693652934715"></a><a name="zh-cn_topic_0225568827_p1693652934715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1093614294475"><a name="zh-cn_topic_0225568827_p1093614294475"></a><a name="zh-cn_topic_0225568827_p1093614294475"></a>对应的请求参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row833403514441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p13350143554413"><a name="zh-cn_topic_0225568827_p13350143554413"></a><a name="zh-cn_topic_0225568827_p13350143554413"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p6365163554417"><a name="zh-cn_topic_0225568827_p6365163554417"></a><a name="zh-cn_topic_0225568827_p6365163554417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p036516356445"><a name="zh-cn_topic_0225568827_p036516356445"></a><a name="zh-cn_topic_0225568827_p036516356445"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row203656353443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p4381103534420"><a name="zh-cn_topic_0225568827_p4381103534420"></a><a name="zh-cn_topic_0225568827_p4381103534420"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p838193504410"><a name="zh-cn_topic_0225568827_p838193504410"></a><a name="zh-cn_topic_0225568827_p838193504410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p10396123516442"><a name="zh-cn_topic_0225568827_p10396123516442"></a><a name="zh-cn_topic_0225568827_p10396123516442"></a>参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row7412103554417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p14271535144413"><a name="zh-cn_topic_0225568827_p14271535144413"></a><a name="zh-cn_topic_0225568827_p14271535144413"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p34431235184418"><a name="zh-cn_topic_0225568827_p34431235184418"></a><a name="zh-cn_topic_0225568827_p34431235184418"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1044312351449"><a name="zh-cn_topic_0225568827_p1044312351449"></a><a name="zh-cn_topic_0225568827_p1044312351449"></a>参数类别</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row445983511447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p5475203519440"><a name="zh-cn_topic_0225568827_p5475203519440"></a><a name="zh-cn_topic_0225568827_p5475203519440"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p1449053524417"><a name="zh-cn_topic_0225568827_p1449053524417"></a><a name="zh-cn_topic_0225568827_p1449053524417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p9490435144419"><a name="zh-cn_topic_0225568827_p9490435144419"></a><a name="zh-cn_topic_0225568827_p9490435144419"></a>参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row7506335184410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p3506935104410"><a name="zh-cn_topic_0225568827_p3506935104410"></a><a name="zh-cn_topic_0225568827_p3506935104410"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p05217356442"><a name="zh-cn_topic_0225568827_p05217356442"></a><a name="zh-cn_topic_0225568827_p05217356442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p11521123517447"><a name="zh-cn_topic_0225568827_p11521123517447"></a><a name="zh-cn_topic_0225568827_p11521123517447"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 9**  auth\_opt参数说明

<a name="zh-cn_topic_0225568827_table3296221173715"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row829715213377"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568827_p17297192173718"><a name="zh-cn_topic_0225568827_p17297192173718"></a><a name="zh-cn_topic_0225568827_p17297192173718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568827_p9297821143718"><a name="zh-cn_topic_0225568827_p9297821143718"></a><a name="zh-cn_topic_0225568827_p9297821143718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568827_p4297152163717"><a name="zh-cn_topic_0225568827_p4297152163717"></a><a name="zh-cn_topic_0225568827_p4297152163717"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row4297421123717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568827_p1848964315375"><a name="zh-cn_topic_0225568827_p1848964315375"></a><a name="zh-cn_topic_0225568827_p1848964315375"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568827_p4489164310372"><a name="zh-cn_topic_0225568827_p4489164310372"></a><a name="zh-cn_topic_0225568827_p4489164310372"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568827_p1948934316376"><a name="zh-cn_topic_0225568827_p1948934316376"></a><a name="zh-cn_topic_0225568827_p1948934316376"></a>AppCode简易认证类型</p>
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
  "req_uri": "/test/{project_id}",
  "auth_type": "APP",
  "auth_opt": {
    "app_code_auth_type": "HEADER"
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
  "sl_domain": "a8be0e466f0e4d8bb18ebd15402cdd66.apigw.southchina.example.com",
  "version_id": "69b7492e2855487398d45733b9d6147a",
  "publish_time": "2018-08-24T03:10:14Z",
  "backend_api": {
    "url_domain": "xxxxxxxxx",
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
      "name": "project_id",
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
      "name": "project_id",
      "location": "QUERY",
      "origin": "REQUEST",
      "value": "project_id",
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
  ]
}
```

## 状态码<a name="zh-cn_topic_0225568827_section48575109"></a>

**表 10**  返回消息说明

<a name="zh-cn_topic_0225568827_table5357896"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568827_row27259487"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568827_p60534834"><a name="zh-cn_topic_0225568827_p60534834"></a><a name="zh-cn_topic_0225568827_p60534834"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568827_p4374530"><a name="zh-cn_topic_0225568827_p4374530"></a><a name="zh-cn_topic_0225568827_p4374530"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568827_row18792630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568827_p45808055"><a name="zh-cn_topic_0225568827_p45808055"></a><a name="zh-cn_topic_0225568827_p45808055"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568827_p50988816"><a name="zh-cn_topic_0225568827_p50988816"></a><a name="zh-cn_topic_0225568827_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row40966733"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568827_p29971116"><a name="zh-cn_topic_0225568827_p29971116"></a><a name="zh-cn_topic_0225568827_p29971116"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568827_p29757115610"><a name="zh-cn_topic_0225568827_p29757115610"></a><a name="zh-cn_topic_0225568827_p29757115610"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row38563414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568827_p36628845"><a name="zh-cn_topic_0225568827_p36628845"></a><a name="zh-cn_topic_0225568827_p36628845"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568827_p9203142078"><a name="zh-cn_topic_0225568827_p9203142078"></a><a name="zh-cn_topic_0225568827_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row60209613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568827_p45140486"><a name="zh-cn_topic_0225568827_p45140486"></a><a name="zh-cn_topic_0225568827_p45140486"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568827_p13949586"><a name="zh-cn_topic_0225568827_p13949586"></a><a name="zh-cn_topic_0225568827_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row24071607"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568827_p3643149"><a name="zh-cn_topic_0225568827_p3643149"></a><a name="zh-cn_topic_0225568827_p3643149"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568827_p26659623"><a name="zh-cn_topic_0225568827_p26659623"></a><a name="zh-cn_topic_0225568827_p26659623"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568827_row95308112592"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568827_p51472750"><a name="zh-cn_topic_0225568827_p51472750"></a><a name="zh-cn_topic_0225568827_p51472750"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568827_p8543194"><a name="zh-cn_topic_0225568827_p8543194"></a><a name="zh-cn_topic_0225568827_p8543194"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

