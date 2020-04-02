# 查看API详情<a name="apig-zh-api-180713030"></a>

## 功能介绍<a name="section56312882"></a>

查看指定的API的详细信息。

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
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p18327454"><a name="p18327454"></a><a name="p18327454"></a>/v1.0/apigw/apis/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table8128785"></a>
<table><thead align="left"><tr id="row50936577"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p32222095"><a name="p32222095"></a><a name="p32222095"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p59852877"><a name="p59852877"></a><a name="p59852877"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p16244835"><a name="p16244835"></a><a name="p16244835"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p40763258"><a name="p40763258"></a><a name="p40763258"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13489593"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p18915273"><a name="p18915273"></a><a name="p18915273"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p55742162"><a name="p55742162"></a><a name="p55742162"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p18821243"><a name="p18821243"></a><a name="p18821243"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p48125676"><a name="p48125676"></a><a name="p48125676"></a>API的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section65049557"></a>

无

## 响应消息<a name="section34522802"></a>

**表 3**  参数说明

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
<tr id="row6909858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p22827665"><a name="p22827665"></a><a name="p22827665"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p37101609"><a name="p37101609"></a><a name="p37101609"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52440337"><a name="p52440337"></a><a name="p52440337"></a>API的状态</p>
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
<tr id="row5263105615455"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p45549491969"><a name="p45549491969"></a><a name="p45549491969"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19554194910611"><a name="p19554194910611"></a><a name="p19554194910611"></a>字段数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p155541490617"><a name="p155541490617"></a><a name="p155541490617"></a>API认证方式参数</p>
</td>
</tr>
<tr id="row1552723173315"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4426105522114"><a name="p4426105522114"></a><a name="p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51041119338"><a name="p51041119338"></a><a name="p51041119338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p116491557133012"><a name="p116491557133012"></a><a name="p116491557133012"></a>前端自定义认证对象的ID</p>
</td>
</tr>
<tr id="row25515144"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53460794"><a name="p53460794"></a><a name="p53460794"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35357081"><a name="p35357081"></a><a name="p35357081"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p45351308"><a name="p45351308"></a><a name="p45351308"></a>API匹配方式</p>
</td>
</tr>
<tr id="row5508593"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p43542878"><a name="p43542878"></a><a name="p43542878"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p37312211"><a name="p37312211"></a><a name="p37312211"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2390265"><a name="p2390265"></a><a name="p2390265"></a>API注册时间</p>
</td>
</tr>
<tr id="row21512390"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p64782007"><a name="p64782007"></a><a name="p64782007"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12851246"><a name="p12851246"></a><a name="p12851246"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p34317968"><a name="p34317968"></a><a name="p34317968"></a>API修改时间</p>
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
<tr id="row50078910"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29859916"><a name="p29859916"></a><a name="p29859916"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2734171"><a name="p2734171"></a><a name="p2734171"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20141331"><a name="p20141331"></a><a name="p20141331"></a>是否需要编排</p>
</td>
</tr>
<tr id="row660031719333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921493_p82576192276"><a name="zh-cn_topic_0118921493_p82576192276"></a><a name="zh-cn_topic_0118921493_p82576192276"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921493_p1625711193277"><a name="zh-cn_topic_0118921493_p1625711193277"></a><a name="zh-cn_topic_0118921493_p1625711193277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921493_p6273141922718"><a name="zh-cn_topic_0118921493_p6273141922718"></a><a name="zh-cn_topic_0118921493_p6273141922718"></a>服务名称标签，待废弃字段</p>
</td>
</tr>
<tr id="row16495132510422"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5689175210267"><a name="p5689175210267"></a><a name="p5689175210267"></a>tags</p>
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
<tr id="row38876451599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1388814535919"><a name="p1388814535919"></a><a name="p1388814535919"></a>response_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5888345115911"><a name="p5888345115911"></a><a name="p5888345115911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14331422017"><a name="p14331422017"></a><a name="p14331422017"></a>分组自定义响应ID</p>
</td>
</tr>
<tr id="row47054253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53298164"><a name="p53298164"></a><a name="p53298164"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22184056"><a name="p22184056"></a><a name="p22184056"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52078112"><a name="p52078112"></a><a name="p52078112"></a>后端服务：web后端详情</p>
</td>
</tr>
<tr id="row66049829"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48435967"><a name="p48435967"></a><a name="p48435967"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p30999282"><a name="p30999282"></a><a name="p30999282"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27913893"><a name="p27913893"></a><a name="p27913893"></a>后端服务：MOCK详情</p>
</td>
</tr>
<tr id="row49898446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15242308"><a name="p15242308"></a><a name="p15242308"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p26667472"><a name="p26667472"></a><a name="p26667472"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12581591"><a name="p12581591"></a><a name="p12581591"></a>后端服务：函数工作流后端详情</p>
</td>
</tr>
<tr id="row3996134219376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13999938164017"><a name="p13999938164017"></a><a name="p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1999203815404"><a name="p1999203815404"></a><a name="p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11999143884013"><a name="p11999143884013"></a><a name="p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="row1854312455375"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p420294234017"><a name="p420294234017"></a><a name="p420294234017"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17202184217401"><a name="p17202184217401"></a><a name="p17202184217401"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p112025421400"><a name="p112025421400"></a><a name="p112025421400"></a>API的后端参数列表</p>
</td>
</tr>
<tr id="row191941552203319"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p09691119194418"><a name="p09691119194418"></a><a name="p09691119194418"></a>policy_https</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p698531944420"><a name="p698531944420"></a><a name="p698531944420"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p142392054413"><a name="p142392054413"></a><a name="p142392054413"></a>web策略后端列表</p>
</td>
</tr>
<tr id="row172881855193313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p450102034414"><a name="p450102034414"></a><a name="p450102034414"></a>policy_mocks</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p966720104412"><a name="p966720104412"></a><a name="p966720104412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p01071207449"><a name="p01071207449"></a><a name="p01071207449"></a>mock策略后端列表</p>
</td>
</tr>
<tr id="row145517589338"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18136122016449"><a name="p18136122016449"></a><a name="p18136122016449"></a>policy_functions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p715582011444"><a name="p715582011444"></a><a name="p715582011444"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p819162074416"><a name="p819162074416"></a><a name="p819162074416"></a>函数工作流策略后端列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  backend\_api参数说明

<a name="table46125461"></a>
<table><thead align="left"><tr id="row21441395"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p59031425"><a name="p59031425"></a><a name="p59031425"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p16816124"><a name="p16816124"></a><a name="p16816124"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p19928779"><a name="p19928779"></a><a name="p19928779"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3618391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24654215"><a name="p24654215"></a><a name="p24654215"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p50834371"><a name="p50834371"></a><a name="p50834371"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p23943412"><a name="p23943412"></a><a name="p23943412"></a>编号</p>
</td>
</tr>
<tr id="row14164124"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6443415"><a name="p6443415"></a><a name="p6443415"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p52154619"><a name="p52154619"></a><a name="p52154619"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p63774574"><a name="p63774574"></a><a name="p63774574"></a>状态</p>
</td>
</tr>
<tr id="row37100262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52331254"><a name="p52331254"></a><a name="p52331254"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10973162"><a name="p10973162"></a><a name="p10973162"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15120014693"><a name="p15120014693"></a><a name="p15120014693"></a>后端endpoint</p>
</td>
</tr>
<tr id="row13480579"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18185121"><a name="p18185121"></a><a name="p18185121"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p63708736"><a name="p63708736"></a><a name="p63708736"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60134024"><a name="p60134024"></a><a name="p60134024"></a>版本</p>
</td>
</tr>
<tr id="row4335306"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15615521"><a name="p15615521"></a><a name="p15615521"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56897717"><a name="p56897717"></a><a name="p56897717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p45312365"><a name="p45312365"></a><a name="p45312365"></a>访问协议</p>
</td>
</tr>
<tr id="row5158106"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15153476"><a name="p15153476"></a><a name="p15153476"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19472071"><a name="p19472071"></a><a name="p19472071"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p33733898"><a name="p33733898"></a><a name="p33733898"></a>访问方式</p>
</td>
</tr>
<tr id="row35169627"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p30167521"><a name="p30167521"></a><a name="p30167521"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p27650173"><a name="p27650173"></a><a name="p27650173"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p25071508"><a name="p25071508"></a><a name="p25071508"></a>访问地址</p>
</td>
</tr>
<tr id="row24316986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p23518872"><a name="p23518872"></a><a name="p23518872"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p25980454"><a name="p25980454"></a><a name="p25980454"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p24041996"><a name="p24041996"></a><a name="p24041996"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row15051376"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11201934"><a name="p11201934"></a><a name="p11201934"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34941465"><a name="p34941465"></a><a name="p34941465"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11686392"><a name="p11686392"></a><a name="p11686392"></a>注册时间</p>
</td>
</tr>
<tr id="row38068667"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63663156"><a name="p63663156"></a><a name="p63663156"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56441973"><a name="p56441973"></a><a name="p56441973"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8397095"><a name="p8397095"></a><a name="p8397095"></a>修改时间</p>
</td>
</tr>
<tr id="row8464993"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14575871"><a name="p14575871"></a><a name="p14575871"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p39794913"><a name="p39794913"></a><a name="p39794913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2162544"><a name="p2162544"></a><a name="p2162544"></a>描述</p>
</td>
</tr>
<tr id="row19462899"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p32991024"><a name="p32991024"></a><a name="p32991024"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p55027277"><a name="p55027277"></a><a name="p55027277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p28024434"><a name="p28024434"></a><a name="p28024434"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="row50893320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28718221"><a name="p28718221"></a><a name="p28718221"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44474542"><a name="p44474542"></a><a name="p44474542"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p45668181"><a name="p45668181"></a><a name="p45668181"></a>VPC通道信息</p>
</td>
</tr>
<tr id="row96871627153314"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8505203193315"><a name="p8505203193315"></a><a name="p8505203193315"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2585332331"><a name="p2585332331"></a><a name="p2585332331"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9477136123312"><a name="p9477136123312"></a><a name="p9477136123312"></a>后端自定义认证对象的ID</p>
</td>
</tr>
</tbody>
</table>

**表 5**  mock\_info参数说明

<a name="table8360445"></a>
<table><thead align="left"><tr id="row61660858"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p28473615"><a name="p28473615"></a><a name="p28473615"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p24661464"><a name="p24661464"></a><a name="p24661464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p51421566"><a name="p51421566"></a><a name="p51421566"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4397288"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20636030"><a name="p20636030"></a><a name="p20636030"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p60905770"><a name="p60905770"></a><a name="p60905770"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p34420305"><a name="p34420305"></a><a name="p34420305"></a>编号</p>
</td>
</tr>
<tr id="row41347295"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p60796621"><a name="p60796621"></a><a name="p60796621"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p25579243"><a name="p25579243"></a><a name="p25579243"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p58652769"><a name="p58652769"></a><a name="p58652769"></a>状态</p>
</td>
</tr>
<tr id="row58112877"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9522587"><a name="p9522587"></a><a name="p9522587"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p33132086"><a name="p33132086"></a><a name="p33132086"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66453285"><a name="p66453285"></a><a name="p66453285"></a>版本</p>
</td>
</tr>
<tr id="row61208656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p58954073"><a name="p58954073"></a><a name="p58954073"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10550570"><a name="p10550570"></a><a name="p10550570"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p49289836"><a name="p49289836"></a><a name="p49289836"></a>返回结果</p>
</td>
</tr>
<tr id="row40955342"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29048444"><a name="p29048444"></a><a name="p29048444"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4113774"><a name="p4113774"></a><a name="p4113774"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p64780301"><a name="p64780301"></a><a name="p64780301"></a>注册时间</p>
</td>
</tr>
<tr id="row46151800"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47308357"><a name="p47308357"></a><a name="p47308357"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6771698"><a name="p6771698"></a><a name="p6771698"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11636647"><a name="p11636647"></a><a name="p11636647"></a>修改时间</p>
</td>
</tr>
<tr id="row37620965"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p27399290"><a name="p27399290"></a><a name="p27399290"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4749995"><a name="p4749995"></a><a name="p4749995"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p49205346"><a name="p49205346"></a><a name="p49205346"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 6**  func\_info参数说明

<a name="table40194930"></a>
<table><thead align="left"><tr id="row47908359"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p55371884"><a name="p55371884"></a><a name="p55371884"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p55937605"><a name="p55937605"></a><a name="p55937605"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p34652155"><a name="p34652155"></a><a name="p34652155"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row55361141"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55067419"><a name="p55067419"></a><a name="p55067419"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31275991"><a name="p31275991"></a><a name="p31275991"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p50327310"><a name="p50327310"></a><a name="p50327310"></a>编号</p>
</td>
</tr>
<tr id="row50292612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47169794"><a name="p47169794"></a><a name="p47169794"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62656944"><a name="p62656944"></a><a name="p62656944"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p42047670"><a name="p42047670"></a><a name="p42047670"></a>状态</p>
</td>
</tr>
<tr id="row42884714"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51109800"><a name="p51109800"></a><a name="p51109800"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p46253139"><a name="p46253139"></a><a name="p46253139"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p55516754"><a name="p55516754"></a><a name="p55516754"></a>版本</p>
</td>
</tr>
<tr id="row29888741"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5068926"><a name="p5068926"></a><a name="p5068926"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7929823"><a name="p7929823"></a><a name="p7929823"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38335921"><a name="p38335921"></a><a name="p38335921"></a>函数URN</p>
</td>
</tr>
<tr id="row9478971"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29599225"><a name="p29599225"></a><a name="p29599225"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48727035"><a name="p48727035"></a><a name="p48727035"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54575786"><a name="p54575786"></a><a name="p54575786"></a>调用类型：async|sync</p>
</td>
</tr>
<tr id="row21420029"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57300826"><a name="p57300826"></a><a name="p57300826"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10855319"><a name="p10855319"></a><a name="p10855319"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6865628"><a name="p6865628"></a><a name="p6865628"></a>注册时间</p>
</td>
</tr>
<tr id="row61790658"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p38987367"><a name="p38987367"></a><a name="p38987367"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3860136"><a name="p3860136"></a><a name="p3860136"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p44235631"><a name="p44235631"></a><a name="p44235631"></a>更新时间</p>
</td>
</tr>
<tr id="row62576359"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p35520303"><a name="p35520303"></a><a name="p35520303"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p58572271"><a name="p58572271"></a><a name="p58572271"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46733520"><a name="p46733520"></a><a name="p46733520"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row17948500"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44542409"><a name="p44542409"></a><a name="p44542409"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51165362"><a name="p51165362"></a><a name="p51165362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p50753656"><a name="p50753656"></a><a name="p50753656"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 7**  req\_params参数说明

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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2559522184412"><a name="p2559522184412"></a><a name="p2559522184412"></a>参数枚举值</p>
</td>
</tr>
<tr id="row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p151311235144415"><a name="p151311235144415"></a><a name="p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p713112353443"><a name="p713112353443"></a><a name="p713112353443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p95973228446"><a name="p95973228446"></a><a name="p95973228446"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8146203564415"><a name="p8146203564415"></a><a name="p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31627353442"><a name="p31627353442"></a><a name="p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2631222104413"><a name="p2631222104413"></a><a name="p2631222104413"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p61782355443"><a name="p61782355443"></a><a name="p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p201932035194417"><a name="p201932035194417"></a><a name="p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2668152294420"><a name="p2668152294420"></a><a name="p2668152294420"></a>参数最小长度</p>
</td>
</tr>
<tr id="row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12209535144412"><a name="p12209535144412"></a><a name="p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12251035164419"><a name="p12251035164419"></a><a name="p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3702522184416"><a name="p3702522184416"></a><a name="p3702522184416"></a>参数最大长度</p>
</td>
</tr>
<tr id="row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52401735134413"><a name="p52401735134413"></a><a name="p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12240153510443"><a name="p12240153510443"></a><a name="p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12731822184412"><a name="p12731822184412"></a><a name="p12731822184412"></a>正则校验规则（暂不支持）</p>
</td>
</tr>
<tr id="row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p202561335114413"><a name="p202561335114413"></a><a name="p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16271035114412"><a name="p16271035114412"></a><a name="p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57661222144411"><a name="p57661222144411"></a><a name="p57661222144411"></a>JSON校验规则（暂不支持）</p>
</td>
</tr>
</tbody>
</table>

**表 8**  backend\_params参数说明

<a name="table9287113513446"></a>
<table><thead align="left"><tr id="row4302173564419"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p33182355443"><a name="p33182355443"></a><a name="p33182355443"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p14334103544415"><a name="p14334103544415"></a><a name="p14334103544415"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p19334153517444"><a name="p19334153517444"></a><a name="p19334153517444"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17142774611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47152713464"><a name="p47152713464"></a><a name="p47152713464"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1717279463"><a name="p1717279463"></a><a name="p1717279463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27122714620"><a name="p27122714620"></a><a name="p27122714620"></a>参数编号</p>
</td>
</tr>
<tr id="row2936129114713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p199361729154717"><a name="p199361729154717"></a><a name="p199361729154717"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1693652934715"><a name="p1693652934715"></a><a name="p1693652934715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1093614294475"><a name="p1093614294475"></a><a name="p1093614294475"></a>对应的请求参数编号</p>
</td>
</tr>
<tr id="row833403514441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13350143554413"><a name="p13350143554413"></a><a name="p13350143554413"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6365163554417"><a name="p6365163554417"></a><a name="p6365163554417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p036516356445"><a name="p036516356445"></a><a name="p036516356445"></a>参数名称</p>
</td>
</tr>
<tr id="row203656353443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4381103534420"><a name="p4381103534420"></a><a name="p4381103534420"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p838193504410"><a name="p838193504410"></a><a name="p838193504410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10396123516442"><a name="p10396123516442"></a><a name="p10396123516442"></a>参数位置</p>
</td>
</tr>
<tr id="row7412103554417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14271535144413"><a name="p14271535144413"></a><a name="p14271535144413"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1525155534613"><a name="p1525155534613"></a><a name="p1525155534613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1044312351449"><a name="p1044312351449"></a><a name="p1044312351449"></a>参数类别</p>
</td>
</tr>
<tr id="row445983511447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5475203519440"><a name="p5475203519440"></a><a name="p5475203519440"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8536145516465"><a name="p8536145516465"></a><a name="p8536145516465"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9490435144419"><a name="p9490435144419"></a><a name="p9490435144419"></a>参数值</p>
</td>
</tr>
<tr id="row7506335184410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3506935104410"><a name="p3506935104410"></a><a name="p3506935104410"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p05217356442"><a name="p05217356442"></a><a name="p05217356442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11521123517447"><a name="p11521123517447"></a><a name="p11521123517447"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 9**  policy\_https参数说明

<a name="table1883393417451"></a>
<table><thead align="left"><tr id="row12893173494517"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p1491393413454"><a name="p1491393413454"></a><a name="p1491393413454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p3930134144518"><a name="p3930134144518"></a><a name="p3930134144518"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1394693410456"><a name="p1394693410456"></a><a name="p1394693410456"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row129661334174520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1997923418453"><a name="p1997923418453"></a><a name="p1997923418453"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p699316349457"><a name="p699316349457"></a><a name="p699316349457"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1176354455"><a name="p1176354455"></a><a name="p1176354455"></a>编号</p>
</td>
</tr>
<tr id="row191173534519"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p729183516457"><a name="p729183516457"></a><a name="p729183516457"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5442035114515"><a name="p5442035114515"></a><a name="p5442035114515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p105673584520"><a name="p105673584520"></a><a name="p105673584520"></a>策略后端名称</p>
</td>
</tr>
<tr id="row19611535114513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20805354452"><a name="p20805354452"></a><a name="p20805354452"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p09323564519"><a name="p09323564519"></a><a name="p09323564519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p131089355454"><a name="p131089355454"></a><a name="p131089355454"></a>策略后端endpoint</p>
</td>
</tr>
<tr id="row141732035194520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11921135124512"><a name="p11921135124512"></a><a name="p11921135124512"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2209173510459"><a name="p2209173510459"></a><a name="p2209173510459"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2223153513453"><a name="p2223153513453"></a><a name="p2223153513453"></a>访问协议</p>
</td>
</tr>
<tr id="row102311835144513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p142451635144514"><a name="p142451635144514"></a><a name="p142451635144514"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p926153519453"><a name="p926153519453"></a><a name="p926153519453"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p0276135124514"><a name="p0276135124514"></a><a name="p0276135124514"></a>访问方式</p>
</td>
</tr>
<tr id="row9284735204514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1629817356452"><a name="p1629817356452"></a><a name="p1629817356452"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2313183554516"><a name="p2313183554516"></a><a name="p2313183554516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p123341135134516"><a name="p123341135134516"></a><a name="p123341135134516"></a>访问地址</p>
</td>
</tr>
<tr id="row20342535194519"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8362535154510"><a name="p8362535154510"></a><a name="p8362535154510"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12378193514459"><a name="p12378193514459"></a><a name="p12378193514459"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p123951235114514"><a name="p123951235114514"></a><a name="p123951235114514"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row1159233518458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20614163564511"><a name="p20614163564511"></a><a name="p20614163564511"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9632143519451"><a name="p9632143519451"></a><a name="p9632143519451"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56481835124516"><a name="p56481835124516"></a><a name="p56481835124516"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="row765613353459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19673193519458"><a name="p19673193519458"></a><a name="p19673193519458"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p0690203524511"><a name="p0690203524511"></a><a name="p0690203524511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20706143594518"><a name="p20706143594518"></a><a name="p20706143594518"></a>VPC通道信息</p>
</td>
</tr>
<tr id="row33971122125919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7397722115911"><a name="p7397722115911"></a><a name="p7397722115911"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14397142235915"><a name="p14397142235915"></a><a name="p14397142235915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p143978228592"><a name="p143978228592"></a><a name="p143978228592"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="row17521289599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p181451844918"><a name="p181451844918"></a><a name="p181451844918"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p178501852715"><a name="p178501852715"></a><a name="p178501852715"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1091214598110"><a name="p1091214598110"></a><a name="p1091214598110"></a>策略条件列表</p>
</td>
</tr>
<tr id="row62321736195919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p131741744219"><a name="p131741744219"></a><a name="p131741744219"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1487855214114"><a name="p1487855214114"></a><a name="p1487855214114"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3947175912116"><a name="p3947175912116"></a><a name="p3947175912116"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 10**  policy\_mocks参数说明

<a name="table12725183513454"></a>
<table><thead align="left"><tr id="row15764635144513"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p378211357456"><a name="p378211357456"></a><a name="p378211357456"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p58001135104513"><a name="p58001135104513"></a><a name="p58001135104513"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p981853512455"><a name="p981853512455"></a><a name="p981853512455"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2835103534513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6852143510458"><a name="p6852143510458"></a><a name="p6852143510458"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2866103524515"><a name="p2866103524515"></a><a name="p2866103524515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1587913519457"><a name="p1587913519457"></a><a name="p1587913519457"></a>编号</p>
</td>
</tr>
<tr id="row8887123534513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15538921331"><a name="p15538921331"></a><a name="p15538921331"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p135591025311"><a name="p135591025311"></a><a name="p135591025311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p105814212311"><a name="p105814212311"></a><a name="p105814212311"></a>策略后端名称</p>
</td>
</tr>
<tr id="row119183644517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1737133612459"><a name="p1737133612459"></a><a name="p1737133612459"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13522036104518"><a name="p13522036104518"></a><a name="p13522036104518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p116953674519"><a name="p116953674519"></a><a name="p116953674519"></a>返回结果</p>
</td>
</tr>
<tr id="row1780193618456"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p129375499320"><a name="p129375499320"></a><a name="p129375499320"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20959149733"><a name="p20959149733"></a><a name="p20959149733"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p49808491431"><a name="p49808491431"></a><a name="p49808491431"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="row914193684515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p21155015317"><a name="p21155015317"></a><a name="p21155015317"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1631135010319"><a name="p1631135010319"></a><a name="p1631135010319"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p95105016320"><a name="p95105016320"></a><a name="p95105016320"></a>策略条件列表</p>
</td>
</tr>
<tr id="row220083616456"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19851150935"><a name="p19851150935"></a><a name="p19851150935"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p191021350934"><a name="p191021350934"></a><a name="p191021350934"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p21240503312"><a name="p21240503312"></a><a name="p21240503312"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 11**  policy\_functions参数说明

<a name="table11274103664518"></a>
<table><thead align="left"><tr id="row14323123615458"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p12336163614453"><a name="p12336163614453"></a><a name="p12336163614453"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p3348163613458"><a name="p3348163613458"></a><a name="p3348163613458"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p136353684510"><a name="p136353684510"></a><a name="p136353684510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row438373613454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p193981361454"><a name="p193981361454"></a><a name="p193981361454"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10414336164515"><a name="p10414336164515"></a><a name="p10414336164515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1543203615456"><a name="p1543203615456"></a><a name="p1543203615456"></a>编号</p>
</td>
</tr>
<tr id="row1844443611451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p145173216411"><a name="p145173216411"></a><a name="p145173216411"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p125371217420"><a name="p125371217420"></a><a name="p125371217420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15581212410"><a name="p15581212410"></a><a name="p15581212410"></a>策略后端名称</p>
</td>
</tr>
<tr id="row450233644511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p25201036164517"><a name="p25201036164517"></a><a name="p25201036164517"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16541736164516"><a name="p16541736164516"></a><a name="p16541736164516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16558133684511"><a name="p16558133684511"></a><a name="p16558133684511"></a>版本</p>
</td>
</tr>
<tr id="row45685369453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p45841936134516"><a name="p45841936134516"></a><a name="p45841936134516"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p25991036114518"><a name="p25991036114518"></a><a name="p25991036114518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6618133614456"><a name="p6618133614456"></a><a name="p6618133614456"></a>函数URN</p>
</td>
</tr>
<tr id="row56281362452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1364419365459"><a name="p1364419365459"></a><a name="p1364419365459"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p19665236114517"><a name="p19665236114517"></a><a name="p19665236114517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1968233654519"><a name="p1968233654519"></a><a name="p1968233654519"></a>调用类型:async|sync</p>
</td>
</tr>
<tr id="row108137365458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1183073613455"><a name="p1183073613455"></a><a name="p1183073613455"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1484712366457"><a name="p1484712366457"></a><a name="p1484712366457"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1687010368458"><a name="p1687010368458"></a><a name="p1687010368458"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row1288018362459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p125311657249"><a name="p125311657249"></a><a name="p125311657249"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p165491576420"><a name="p165491576420"></a><a name="p165491576420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p556795712420"><a name="p556795712420"></a><a name="p556795712420"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="row14199172719419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p259219571446"><a name="p259219571446"></a><a name="p259219571446"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p160916576412"><a name="p160916576412"></a><a name="p160916576412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17627257149"><a name="p17627257149"></a><a name="p17627257149"></a>策略条件列表</p>
</td>
</tr>
<tr id="row107283241048"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p66684572045"><a name="p66684572045"></a><a name="p66684572045"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p126865574411"><a name="p126865574411"></a><a name="p126865574411"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17025579410"><a name="p17025579410"></a><a name="p17025579410"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 12**  conditions参数说明

<a name="table54445157"></a>
<table><thead align="left"><tr id="row01061051953"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p121240513510"><a name="p121240513510"></a><a name="p121240513510"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p0145557515"><a name="p0145557515"></a><a name="p0145557515"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p4166752511"><a name="p4166752511"></a><a name="p4166752511"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1618417512511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p719835852"><a name="p719835852"></a><a name="p719835852"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16224185456"><a name="p16224185456"></a><a name="p16224185456"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p102391557519"><a name="p102391557519"></a><a name="p102391557519"></a>编号</p>
</td>
</tr>
<tr id="row82501551858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1796083474"><a name="p1796083474"></a><a name="p1796083474"></a>condition_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18804202017712"><a name="p18804202017712"></a><a name="p18804202017712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p382342012717"><a name="p382342012717"></a><a name="p382342012717"></a>策略条件</p>
</td>
</tr>
<tr id="row123301257513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p181491444714"><a name="p181491444714"></a><a name="p181491444714"></a>condition_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1492819201073"><a name="p1492819201073"></a><a name="p1492819201073"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1994462016716"><a name="p1994462016716"></a><a name="p1994462016716"></a>策略值</p>
</td>
</tr>
<tr id="row1040955655"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12230841573"><a name="p12230841573"></a><a name="p12230841573"></a>condition_origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p197610207714"><a name="p197610207714"></a><a name="p197610207714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1999642015720"><a name="p1999642015720"></a><a name="p1999642015720"></a>策略类型</p>
</td>
</tr>
<tr id="row1247645451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p193881741373"><a name="p193881741373"></a><a name="p193881741373"></a>req_param_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1575921679"><a name="p1575921679"></a><a name="p1575921679"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1396172120712"><a name="p1396172120712"></a><a name="p1396172120712"></a>关联的请求参数对象名称</p>
</td>
</tr>
<tr id="row455495755"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15751853519"><a name="p15751853519"></a><a name="p15751853519"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10599451451"><a name="p10599451451"></a><a name="p10599451451"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5617455515"><a name="p5617455515"></a><a name="p5617455515"></a>关联的请求参数对象编号</p>
</td>
</tr>
<tr id="row1862912512520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p176461751659"><a name="p176461751659"></a><a name="p176461751659"></a>req_param_location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p146711652057"><a name="p146711652057"></a><a name="p146711652057"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p869795651"><a name="p869795651"></a><a name="p869795651"></a>关联的请求参数对象位置</p>
</td>
</tr>
</tbody>
</table>

**表 13**  auth\_opt参数说明

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

## 状态码<a name="section48575109"></a>

**表 14**  返回消息说明

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

