# 查看API绑定的流控策略列表<a name="ZH-CN_TOPIC_0000001082221199"></a>

## 功能介绍<a name="zh-cn_topic_0118922266_section3787021"></a>

查询某个API绑定的流控策略列表。每个环境上应该最多只有一个流控策略。

## URI<a name="zh-cn_topic_0118922266_section34083192"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922266_table24918216"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922266_row36797024"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922266_p27768974"><a name="zh-cn_topic_0118922266_p27768974"></a><a name="zh-cn_topic_0118922266_p27768974"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922266_p34694461"><a name="zh-cn_topic_0118922266_p34694461"></a><a name="zh-cn_topic_0118922266_p34694461"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922266_row58787989"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922266_p64206653"><a name="zh-cn_topic_0118922266_p64206653"></a><a name="zh-cn_topic_0118922266_p64206653"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922266_p33356381"><a name="zh-cn_topic_0118922266_p33356381"></a><a name="zh-cn_topic_0118922266_p33356381"></a>/v1.0/apigw/throttle-bindings/binded-throttles[?page_no, page_size, api_id, throttle_id, throttle_name,env_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：api\_id 、throttle\_id、throttle\_name、env\_id、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922266_table15819367"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922266_row61671638"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922266_p29346818"><a name="zh-cn_topic_0118922266_p29346818"></a><a name="zh-cn_topic_0118922266_p29346818"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922266_p28282025"><a name="zh-cn_topic_0118922266_p28282025"></a><a name="zh-cn_topic_0118922266_p28282025"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922266_p9142709"><a name="zh-cn_topic_0118922266_p9142709"></a><a name="zh-cn_topic_0118922266_p9142709"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922266_p2361998"><a name="zh-cn_topic_0118922266_p2361998"></a><a name="zh-cn_topic_0118922266_p2361998"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922266_row57104155"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922266_p62033861"><a name="zh-cn_topic_0118922266_p62033861"></a><a name="zh-cn_topic_0118922266_p62033861"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922266_p58686835"><a name="zh-cn_topic_0118922266_p58686835"></a><a name="zh-cn_topic_0118922266_p58686835"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922266_p56013198"><a name="zh-cn_topic_0118922266_p56013198"></a><a name="zh-cn_topic_0118922266_p56013198"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922266_p40775165"><a name="zh-cn_topic_0118922266_p40775165"></a><a name="zh-cn_topic_0118922266_p40775165"></a>api的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row31432168"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922266_p62977649"><a name="zh-cn_topic_0118922266_p62977649"></a><a name="zh-cn_topic_0118922266_p62977649"></a>throttle_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922266_p915906"><a name="zh-cn_topic_0118922266_p915906"></a><a name="zh-cn_topic_0118922266_p915906"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922266_p7079556"><a name="zh-cn_topic_0118922266_p7079556"></a><a name="zh-cn_topic_0118922266_p7079556"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922266_p36573150"><a name="zh-cn_topic_0118922266_p36573150"></a><a name="zh-cn_topic_0118922266_p36573150"></a>流控策略的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row60722900"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922266_p19607878"><a name="zh-cn_topic_0118922266_p19607878"></a><a name="zh-cn_topic_0118922266_p19607878"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922266_p44734309"><a name="zh-cn_topic_0118922266_p44734309"></a><a name="zh-cn_topic_0118922266_p44734309"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922266_p66709272"><a name="zh-cn_topic_0118922266_p66709272"></a><a name="zh-cn_topic_0118922266_p66709272"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922266_p34741960"><a name="zh-cn_topic_0118922266_p34741960"></a><a name="zh-cn_topic_0118922266_p34741960"></a>流控策略的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row44242186"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922266_p26847295"><a name="zh-cn_topic_0118922266_p26847295"></a><a name="zh-cn_topic_0118922266_p26847295"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922266_p27147301"><a name="zh-cn_topic_0118922266_p27147301"></a><a name="zh-cn_topic_0118922266_p27147301"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922266_p51447779"><a name="zh-cn_topic_0118922266_p51447779"></a><a name="zh-cn_topic_0118922266_p51447779"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922266_p6520610"><a name="zh-cn_topic_0118922266_p6520610"></a><a name="zh-cn_topic_0118922266_p6520610"></a>绑定的环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row58685498"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922266_p55904860"><a name="zh-cn_topic_0118922266_p55904860"></a><a name="zh-cn_topic_0118922266_p55904860"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922266_p31999827"><a name="zh-cn_topic_0118922266_p31999827"></a><a name="zh-cn_topic_0118922266_p31999827"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922266_p41849223"><a name="zh-cn_topic_0118922266_p41849223"></a><a name="zh-cn_topic_0118922266_p41849223"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922266_p34343903"><a name="zh-cn_topic_0118922266_p34343903"></a><a name="zh-cn_topic_0118922266_p34343903"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row40659676"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922266_p5099494"><a name="zh-cn_topic_0118922266_p5099494"></a><a name="zh-cn_topic_0118922266_p5099494"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922266_p10405897"><a name="zh-cn_topic_0118922266_p10405897"></a><a name="zh-cn_topic_0118922266_p10405897"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922266_p37571308"><a name="zh-cn_topic_0118922266_p37571308"></a><a name="zh-cn_topic_0118922266_p37571308"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922266_p23377079"><a name="zh-cn_topic_0118922266_p23377079"></a><a name="zh-cn_topic_0118922266_p23377079"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922266_section38313279"></a>

无

## 响应消息<a name="zh-cn_topic_0118922266_section16367881"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118922266_table48937735"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922266_row9136068"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922266_p1824044"><a name="zh-cn_topic_0118922266_p1824044"></a><a name="zh-cn_topic_0118922266_p1824044"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922266_p13529889"><a name="zh-cn_topic_0118922266_p13529889"></a><a name="zh-cn_topic_0118922266_p13529889"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922266_p22179210"><a name="zh-cn_topic_0118922266_p22179210"></a><a name="zh-cn_topic_0118922266_p22179210"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922266_row51685584"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p25782746"><a name="zh-cn_topic_0118922266_p25782746"></a><a name="zh-cn_topic_0118922266_p25782746"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p8027664"><a name="zh-cn_topic_0118922266_p8027664"></a><a name="zh-cn_topic_0118922266_p8027664"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p46261084"><a name="zh-cn_topic_0118922266_p46261084"></a><a name="zh-cn_topic_0118922266_p46261084"></a>满足条件的流控策略总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row13696572"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p35680577"><a name="zh-cn_topic_0118922266_p35680577"></a><a name="zh-cn_topic_0118922266_p35680577"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p4445647"><a name="zh-cn_topic_0118922266_p4445647"></a><a name="zh-cn_topic_0118922266_p4445647"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p24553101"><a name="zh-cn_topic_0118922266_p24553101"></a><a name="zh-cn_topic_0118922266_p24553101"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row19651317"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p48252863"><a name="zh-cn_topic_0118922266_p48252863"></a><a name="zh-cn_topic_0118922266_p48252863"></a>throttles</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p16167821"><a name="zh-cn_topic_0118922266_p16167821"></a><a name="zh-cn_topic_0118922266_p16167821"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p34525128"><a name="zh-cn_topic_0118922266_p34525128"></a><a name="zh-cn_topic_0118922266_p34525128"></a>本次查询返回的流控策略列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  throttles参数说明

<a name="zh-cn_topic_0118922266_table42290697"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922266_row54536847"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118922266_p55408512"><a name="zh-cn_topic_0118922266_p55408512"></a><a name="zh-cn_topic_0118922266_p55408512"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118922266_p58904526"><a name="zh-cn_topic_0118922266_p58904526"></a><a name="zh-cn_topic_0118922266_p58904526"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118922266_p6537312"><a name="zh-cn_topic_0118922266_p6537312"></a><a name="zh-cn_topic_0118922266_p6537312"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922266_row59760287"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p8745074"><a name="zh-cn_topic_0118922266_p8745074"></a><a name="zh-cn_topic_0118922266_p8745074"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p37262402"><a name="zh-cn_topic_0118922266_p37262402"></a><a name="zh-cn_topic_0118922266_p37262402"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p65464566"><a name="zh-cn_topic_0118922266_p65464566"></a><a name="zh-cn_topic_0118922266_p65464566"></a>流控策略的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row52310185"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p9266607"><a name="zh-cn_topic_0118922266_p9266607"></a><a name="zh-cn_topic_0118922266_p9266607"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p12397709"><a name="zh-cn_topic_0118922266_p12397709"></a><a name="zh-cn_topic_0118922266_p12397709"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p64690412"><a name="zh-cn_topic_0118922266_p64690412"></a><a name="zh-cn_topic_0118922266_p64690412"></a>流控策略的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row45342804"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p48888470"><a name="zh-cn_topic_0118922266_p48888470"></a><a name="zh-cn_topic_0118922266_p48888470"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p543149"><a name="zh-cn_topic_0118922266_p543149"></a><a name="zh-cn_topic_0118922266_p543149"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p43995137"><a name="zh-cn_topic_0118922266_p43995137"></a><a name="zh-cn_topic_0118922266_p43995137"></a>单个API流控时间内能够被访问的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row60411917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p61527110"><a name="zh-cn_topic_0118922266_p61527110"></a><a name="zh-cn_topic_0118922266_p61527110"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p17640048"><a name="zh-cn_topic_0118922266_p17640048"></a><a name="zh-cn_topic_0118922266_p17640048"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p19557811"><a name="zh-cn_topic_0118922266_p19557811"></a><a name="zh-cn_topic_0118922266_p19557811"></a>单个用户流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row41802573"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p30565223"><a name="zh-cn_topic_0118922266_p30565223"></a><a name="zh-cn_topic_0118922266_p30565223"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p59863981"><a name="zh-cn_topic_0118922266_p59863981"></a><a name="zh-cn_topic_0118922266_p59863981"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p17144329"><a name="zh-cn_topic_0118922266_p17144329"></a><a name="zh-cn_topic_0118922266_p17144329"></a>单个APP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row1754915731214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p1055095713123"><a name="zh-cn_topic_0118922266_p1055095713123"></a><a name="zh-cn_topic_0118922266_p1055095713123"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p71091461318"><a name="zh-cn_topic_0118922266_p71091461318"></a><a name="zh-cn_topic_0118922266_p71091461318"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p15358518161319"><a name="zh-cn_topic_0118922266_p15358518161319"></a><a name="zh-cn_topic_0118922266_p15358518161319"></a>单个源IP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row20081233"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p15967206"><a name="zh-cn_topic_0118922266_p15967206"></a><a name="zh-cn_topic_0118922266_p15967206"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p18275332"><a name="zh-cn_topic_0118922266_p18275332"></a><a name="zh-cn_topic_0118922266_p18275332"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p3906898"><a name="zh-cn_topic_0118922266_p3906898"></a><a name="zh-cn_topic_0118922266_p3906898"></a>流控的时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row35162082"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p29556412"><a name="zh-cn_topic_0118922266_p29556412"></a><a name="zh-cn_topic_0118922266_p29556412"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p45259162"><a name="zh-cn_topic_0118922266_p45259162"></a><a name="zh-cn_topic_0118922266_p45259162"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p42113509"><a name="zh-cn_topic_0118922266_p42113509"></a><a name="zh-cn_topic_0118922266_p42113509"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row43477262"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p31997351"><a name="zh-cn_topic_0118922266_p31997351"></a><a name="zh-cn_topic_0118922266_p31997351"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p41648608"><a name="zh-cn_topic_0118922266_p41648608"></a><a name="zh-cn_topic_0118922266_p41648608"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p18094049"><a name="zh-cn_topic_0118922266_p18094049"></a><a name="zh-cn_topic_0118922266_p18094049"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row28628716"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p37224685"><a name="zh-cn_topic_0118922266_p37224685"></a><a name="zh-cn_topic_0118922266_p37224685"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p62409547"><a name="zh-cn_topic_0118922266_p62409547"></a><a name="zh-cn_topic_0118922266_p62409547"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p22008557"><a name="zh-cn_topic_0118922266_p22008557"></a><a name="zh-cn_topic_0118922266_p22008557"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row63859292"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p5220127"><a name="zh-cn_topic_0118922266_p5220127"></a><a name="zh-cn_topic_0118922266_p5220127"></a>is_include_special_throttle</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p20177180"><a name="zh-cn_topic_0118922266_p20177180"></a><a name="zh-cn_topic_0118922266_p20177180"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p23738873"><a name="zh-cn_topic_0118922266_p23738873"></a><a name="zh-cn_topic_0118922266_p23738873"></a>是否包含特殊流控：1、包含；2、不包含</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row12323267"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p58660564"><a name="zh-cn_topic_0118922266_p58660564"></a><a name="zh-cn_topic_0118922266_p58660564"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p53885209"><a name="zh-cn_topic_0118922266_p53885209"></a><a name="zh-cn_topic_0118922266_p53885209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p2625786"><a name="zh-cn_topic_0118922266_p2625786"></a><a name="zh-cn_topic_0118922266_p2625786"></a>流控策略生效的环境（即在哪个环境上有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row1032433881812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p113241238121816"><a name="zh-cn_topic_0118922266_p113241238121816"></a><a name="zh-cn_topic_0118922266_p113241238121816"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p13324193881813"><a name="zh-cn_topic_0118922266_p13324193881813"></a><a name="zh-cn_topic_0118922266_p13324193881813"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p532463851810"><a name="zh-cn_topic_0118922266_p532463851810"></a><a name="zh-cn_topic_0118922266_p532463851810"></a>流控策略的类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row103351101412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p183401111418"><a name="zh-cn_topic_0118922266_p183401111418"></a><a name="zh-cn_topic_0118922266_p183401111418"></a>bind_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p103420131412"><a name="zh-cn_topic_0118922266_p103420131412"></a><a name="zh-cn_topic_0118922266_p103420131412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p1349121416"><a name="zh-cn_topic_0118922266_p1349121416"></a><a name="zh-cn_topic_0118922266_p1349121416"></a>流控策略与API绑定关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row14618831149"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p46186321411"><a name="zh-cn_topic_0118922266_p46186321411"></a><a name="zh-cn_topic_0118922266_p46186321411"></a>bind_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p66187319145"><a name="zh-cn_topic_0118922266_p66187319145"></a><a name="zh-cn_topic_0118922266_p66187319145"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p196181132148"><a name="zh-cn_topic_0118922266_p196181132148"></a><a name="zh-cn_topic_0118922266_p196181132148"></a>流控策略与API绑定时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row24961721994"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p104961221996"><a name="zh-cn_topic_0118922266_p104961221996"></a><a name="zh-cn_topic_0118922266_p104961221996"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p54961121997"><a name="zh-cn_topic_0118922266_p54961121997"></a><a name="zh-cn_topic_0118922266_p54961121997"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p14969218913"><a name="zh-cn_topic_0118922266_p14969218913"></a><a name="zh-cn_topic_0118922266_p14969218913"></a>流控策略绑定的API数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row1912417351899"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118922266_p19770121614477"><a name="zh-cn_topic_0118922266_p19770121614477"></a><a name="zh-cn_topic_0118922266_p19770121614477"></a>enable_adaptive_control</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118922266_p27566352475"><a name="zh-cn_topic_0118922266_p27566352475"></a><a name="zh-cn_topic_0118922266_p27566352475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118922266_p13499124885712"><a name="zh-cn_topic_0118922266_p13499124885712"></a><a name="zh-cn_topic_0118922266_p13499124885712"></a>是否开启动态流控，暂不支持</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 1,
	"size": 1,
	"throttles": [{
		"id": "0325b671-2d50-4614-9868-22102262695d",
		"name": "每秒1000次",
		"api_call_limits": 1000,
		"user_call_limits": 500,
		"app_call_limits": 300,
		"ip_call_limits": 100,
		"time_interval": 1,
		"time_unit": "SECOND",
		"create_time": "2017-12-29T01:55:59Z",
		"remark": "API每秒1000次，用户500次，APP300次",
		"is_inclu_special_throttle": 2,
		"env_name": "RELEASE",
                "type":1,
                "bind_id":"359f5c1868f647b6ad0f0d285154a791",
                "bind_time":"2019-07-08T01:27:38Z",
                "bind_num":1,
                "enable_adaptive_control":"FALSE"
	}]
}
```

## 状态码<a name="zh-cn_topic_0118922266_section9275193"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118922266_table33264679"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922266_row36740715"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922266_p23207944"><a name="zh-cn_topic_0118922266_p23207944"></a><a name="zh-cn_topic_0118922266_p23207944"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922266_p795330"><a name="zh-cn_topic_0118922266_p795330"></a><a name="zh-cn_topic_0118922266_p795330"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922266_row64421760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922266_p50780075"><a name="zh-cn_topic_0118922266_p50780075"></a><a name="zh-cn_topic_0118922266_p50780075"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922266_p19545386"><a name="zh-cn_topic_0118922266_p19545386"></a><a name="zh-cn_topic_0118922266_p19545386"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row41690749"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922266_p21507478"><a name="zh-cn_topic_0118922266_p21507478"></a><a name="zh-cn_topic_0118922266_p21507478"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922266_p64384119"><a name="zh-cn_topic_0118922266_p64384119"></a><a name="zh-cn_topic_0118922266_p64384119"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row42586162"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922266_p26927123"><a name="zh-cn_topic_0118922266_p26927123"></a><a name="zh-cn_topic_0118922266_p26927123"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922266_p33613393"><a name="zh-cn_topic_0118922266_p33613393"></a><a name="zh-cn_topic_0118922266_p33613393"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row34085086"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922266_p9428594"><a name="zh-cn_topic_0118922266_p9428594"></a><a name="zh-cn_topic_0118922266_p9428594"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922266_p25518613"><a name="zh-cn_topic_0118922266_p25518613"></a><a name="zh-cn_topic_0118922266_p25518613"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row28340933"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922266_p13914245"><a name="zh-cn_topic_0118922266_p13914245"></a><a name="zh-cn_topic_0118922266_p13914245"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922266_p53312041"><a name="zh-cn_topic_0118922266_p53312041"></a><a name="zh-cn_topic_0118922266_p53312041"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922266_row10046324"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922266_p8445930"><a name="zh-cn_topic_0118922266_p8445930"></a><a name="zh-cn_topic_0118922266_p8445930"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922266_p13031736"><a name="zh-cn_topic_0118922266_p13031736"></a><a name="zh-cn_topic_0118922266_p13031736"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

