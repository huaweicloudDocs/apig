# 查看分组详情<a name="ZH-CN_TOPIC_0000001082135085"></a>

## 功能介绍<a name="zh-cn_topic_0118921489_section1735744"></a>

查询指定分组的详细信息。

## URI<a name="zh-cn_topic_0118921489_section15621702"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921489_table32113079"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921489_row20115923"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921489_p18777034"><a name="zh-cn_topic_0118921489_p18777034"></a><a name="zh-cn_topic_0118921489_p18777034"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921489_p44544806"><a name="zh-cn_topic_0118921489_p44544806"></a><a name="zh-cn_topic_0118921489_p44544806"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921489_row51359567"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921489_p66484268"><a name="zh-cn_topic_0118921489_p66484268"></a><a name="zh-cn_topic_0118921489_p66484268"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921489_p16516646"><a name="zh-cn_topic_0118921489_p16516646"></a><a name="zh-cn_topic_0118921489_p16516646"></a>/v1.0/apigw/api-groups/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921489_table62779940"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921489_row53801450"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921489_p62950166"><a name="zh-cn_topic_0118921489_p62950166"></a><a name="zh-cn_topic_0118921489_p62950166"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921489_p65798711"><a name="zh-cn_topic_0118921489_p65798711"></a><a name="zh-cn_topic_0118921489_p65798711"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921489_p28095413"><a name="zh-cn_topic_0118921489_p28095413"></a><a name="zh-cn_topic_0118921489_p28095413"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921489_p61135991"><a name="zh-cn_topic_0118921489_p61135991"></a><a name="zh-cn_topic_0118921489_p61135991"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921489_row53068262"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921489_p3561961"><a name="zh-cn_topic_0118921489_p3561961"></a><a name="zh-cn_topic_0118921489_p3561961"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921489_p20083433"><a name="zh-cn_topic_0118921489_p20083433"></a><a name="zh-cn_topic_0118921489_p20083433"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921489_p16145357"><a name="zh-cn_topic_0118921489_p16145357"></a><a name="zh-cn_topic_0118921489_p16145357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921489_p32705534"><a name="zh-cn_topic_0118921489_p32705534"></a><a name="zh-cn_topic_0118921489_p32705534"></a>分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921489_section6377591"></a>

无

## 响应消息<a name="zh-cn_topic_0118921489_section46822891"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921489_table23378999"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921489_row11169479"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921489_p32312619"><a name="zh-cn_topic_0118921489_p32312619"></a><a name="zh-cn_topic_0118921489_p32312619"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921489_p76446"><a name="zh-cn_topic_0118921489_p76446"></a><a name="zh-cn_topic_0118921489_p76446"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921489_p6192203"><a name="zh-cn_topic_0118921489_p6192203"></a><a name="zh-cn_topic_0118921489_p6192203"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921489_row31806424"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p26183533"><a name="zh-cn_topic_0118921489_p26183533"></a><a name="zh-cn_topic_0118921489_p26183533"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p40491443"><a name="zh-cn_topic_0118921489_p40491443"></a><a name="zh-cn_topic_0118921489_p40491443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p58581457"><a name="zh-cn_topic_0118921489_p58581457"></a><a name="zh-cn_topic_0118921489_p58581457"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row57471073"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p24645368"><a name="zh-cn_topic_0118921489_p24645368"></a><a name="zh-cn_topic_0118921489_p24645368"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p50117754"><a name="zh-cn_topic_0118921489_p50117754"></a><a name="zh-cn_topic_0118921489_p50117754"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p33006289"><a name="zh-cn_topic_0118921489_p33006289"></a><a name="zh-cn_topic_0118921489_p33006289"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row28621152"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p36611985"><a name="zh-cn_topic_0118921489_p36611985"></a><a name="zh-cn_topic_0118921489_p36611985"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p12780810"><a name="zh-cn_topic_0118921489_p12780810"></a><a name="zh-cn_topic_0118921489_p12780810"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p28612724"><a name="zh-cn_topic_0118921489_p28612724"></a><a name="zh-cn_topic_0118921489_p28612724"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row56187931"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p54928561"><a name="zh-cn_topic_0118921489_p54928561"></a><a name="zh-cn_topic_0118921489_p54928561"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p20028427"><a name="zh-cn_topic_0118921489_p20028427"></a><a name="zh-cn_topic_0118921489_p20028427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p11689873"><a name="zh-cn_topic_0118921489_p11689873"></a><a name="zh-cn_topic_0118921489_p11689873"></a>系统默认分配的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row14817853182912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p48182537297"><a name="zh-cn_topic_0118921489_p48182537297"></a><a name="zh-cn_topic_0118921489_p48182537297"></a>sl_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p152141058102913"><a name="zh-cn_topic_0118921489_p152141058102913"></a><a name="zh-cn_topic_0118921489_p152141058102913"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p51743143020"><a name="zh-cn_topic_0118921489_p51743143020"></a><a name="zh-cn_topic_0118921489_p51743143020"></a>系统默认分配的子域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row38100001"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p66201237"><a name="zh-cn_topic_0118921489_p66201237"></a><a name="zh-cn_topic_0118921489_p66201237"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p60700010"><a name="zh-cn_topic_0118921489_p60700010"></a><a name="zh-cn_topic_0118921489_p60700010"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p17753800"><a name="zh-cn_topic_0118921489_p17753800"></a><a name="zh-cn_topic_0118921489_p17753800"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row25566473"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p57618438"><a name="zh-cn_topic_0118921489_p57618438"></a><a name="zh-cn_topic_0118921489_p57618438"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p36581920"><a name="zh-cn_topic_0118921489_p36581920"></a><a name="zh-cn_topic_0118921489_p36581920"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p10345534"><a name="zh-cn_topic_0118921489_p10345534"></a><a name="zh-cn_topic_0118921489_p10345534"></a>最近修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row26000946"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p25701906"><a name="zh-cn_topic_0118921489_p25701906"></a><a name="zh-cn_topic_0118921489_p25701906"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p1479659"><a name="zh-cn_topic_0118921489_p1479659"></a><a name="zh-cn_topic_0118921489_p1479659"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p52743524"><a name="zh-cn_topic_0118921489_p52743524"></a><a name="zh-cn_topic_0118921489_p52743524"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row4929668"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p63758800"><a name="zh-cn_topic_0118921489_p63758800"></a><a name="zh-cn_topic_0118921489_p63758800"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p64189201"><a name="zh-cn_topic_0118921489_p64189201"></a><a name="zh-cn_topic_0118921489_p64189201"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p31942831"><a name="zh-cn_topic_0118921489_p31942831"></a><a name="zh-cn_topic_0118921489_p31942831"></a>流控时长内分组下的API的总访问次数限制，默认不限，请根据服务的负载能力自行设置</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row19050028"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p66657312"><a name="zh-cn_topic_0118921489_p66657312"></a><a name="zh-cn_topic_0118921489_p66657312"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p30533155"><a name="zh-cn_topic_0118921489_p30533155"></a><a name="zh-cn_topic_0118921489_p30533155"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p57266528"><a name="zh-cn_topic_0118921489_p57266528"></a><a name="zh-cn_topic_0118921489_p57266528"></a>流控时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row45636707"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p5585767"><a name="zh-cn_topic_0118921489_p5585767"></a><a name="zh-cn_topic_0118921489_p5585767"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p49793976"><a name="zh-cn_topic_0118921489_p49793976"></a><a name="zh-cn_topic_0118921489_p49793976"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p6780221"><a name="zh-cn_topic_0118921489_p6780221"></a><a name="zh-cn_topic_0118921489_p6780221"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row61021990"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p43834197"><a name="zh-cn_topic_0118921489_p43834197"></a><a name="zh-cn_topic_0118921489_p43834197"></a>url_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p60909101"><a name="zh-cn_topic_0118921489_p60909101"></a><a name="zh-cn_topic_0118921489_p60909101"></a>Array of <a href="#zh-cn_topic_0118921489_table9811220">UrlDomainsResp</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p34690133"><a name="zh-cn_topic_0118921489_p34690133"></a><a name="zh-cn_topic_0118921489_p34690133"></a>分组上绑定的独立域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row43775742"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p56174242"><a name="zh-cn_topic_0118921489_p56174242"></a><a name="zh-cn_topic_0118921489_p56174242"></a>on_sell_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p53819754"><a name="zh-cn_topic_0118921489_p53819754"></a><a name="zh-cn_topic_0118921489_p53819754"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p64432831"><a name="zh-cn_topic_0118921489_p64432831"></a><a name="zh-cn_topic_0118921489_p64432831"></a>是否已上架云市场：</p>
<a name="zh-cn_topic_0118921489_ul43024569"></a><a name="zh-cn_topic_0118921489_ul43024569"></a><ul id="zh-cn_topic_0118921489_ul43024569"><li>1：已上架</li><li>2：未上架</li><li>3：审核中</li></ul>
</td>
</tr>
</tbody>
</table>

**表 4**  UrlDomainsResp

<a name="zh-cn_topic_0118921489_table9811220"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921489_row18394177"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921489_p13533375"><a name="zh-cn_topic_0118921489_p13533375"></a><a name="zh-cn_topic_0118921489_p13533375"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921489_p22461630"><a name="zh-cn_topic_0118921489_p22461630"></a><a name="zh-cn_topic_0118921489_p22461630"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921489_p7452774"><a name="zh-cn_topic_0118921489_p7452774"></a><a name="zh-cn_topic_0118921489_p7452774"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921489_row66803806"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p42399182"><a name="zh-cn_topic_0118921489_p42399182"></a><a name="zh-cn_topic_0118921489_p42399182"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p11781727"><a name="zh-cn_topic_0118921489_p11781727"></a><a name="zh-cn_topic_0118921489_p11781727"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p14795832"><a name="zh-cn_topic_0118921489_p14795832"></a><a name="zh-cn_topic_0118921489_p14795832"></a>域名编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row66053632"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p48743961"><a name="zh-cn_topic_0118921489_p48743961"></a><a name="zh-cn_topic_0118921489_p48743961"></a>domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p55946767"><a name="zh-cn_topic_0118921489_p55946767"></a><a name="zh-cn_topic_0118921489_p55946767"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p35394249"><a name="zh-cn_topic_0118921489_p35394249"></a><a name="zh-cn_topic_0118921489_p35394249"></a>访问域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row50112787"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p32603951"><a name="zh-cn_topic_0118921489_p32603951"></a><a name="zh-cn_topic_0118921489_p32603951"></a>cname_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p23674371"><a name="zh-cn_topic_0118921489_p23674371"></a><a name="zh-cn_topic_0118921489_p23674371"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p38575928"><a name="zh-cn_topic_0118921489_p38575928"></a><a name="zh-cn_topic_0118921489_p38575928"></a>域名cname状态：</p>
<a name="zh-cn_topic_0118921489_ul11639038"></a><a name="zh-cn_topic_0118921489_ul11639038"></a><ul id="zh-cn_topic_0118921489_ul11639038"><li>1：未解析</li><li>2：解析中</li><li>3：解析成功</li><li>4：解析失败</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row11732266"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p10789489"><a name="zh-cn_topic_0118921489_p10789489"></a><a name="zh-cn_topic_0118921489_p10789489"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p1533408"><a name="zh-cn_topic_0118921489_p1533408"></a><a name="zh-cn_topic_0118921489_p1533408"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p57097248"><a name="zh-cn_topic_0118921489_p57097248"></a><a name="zh-cn_topic_0118921489_p57097248"></a>SSL证书编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row967016619319"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921489_p667011623113"><a name="zh-cn_topic_0118921489_p667011623113"></a><a name="zh-cn_topic_0118921489_p667011623113"></a>ssl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921489_p967017623110"><a name="zh-cn_topic_0118921489_p967017623110"></a><a name="zh-cn_topic_0118921489_p967017623110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921489_p76701261314"><a name="zh-cn_topic_0118921489_p76701261314"></a><a name="zh-cn_topic_0118921489_p76701261314"></a>SSL证书名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "7efb2b91-155a-4f6a-9f45-c5c95a6e4950",
	"name": "api_group_001",
	"status": 1,
	"sl_domain": "0e91b83b-0774-4e8e-b187-2d695ed4743b.apigw.example.com",
        "sl_domains": ["0e91b83b-0774-4e8e-b187-2d695ed4743b.apigw.example.com","0e91b83b-0774-4e8e-b187-2d695ed4743b.apigw.example.cn"],
	"remark": "分组001",
	"register_time": "2017-12-28T11:44:53Z",
	"update_time": "2017-12-28T11:49:01.048601Z",
	"call_limits": 1000,
	"time_interval": 1,
	"time_unit": "SECOND",
	"on_sell_status": 2
}
```

## 状态码<a name="zh-cn_topic_0118921489_section57398326"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118921489_table33970788"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921489_row57167435"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921489_p50635"><a name="zh-cn_topic_0118921489_p50635"></a><a name="zh-cn_topic_0118921489_p50635"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921489_p4101484"><a name="zh-cn_topic_0118921489_p4101484"></a><a name="zh-cn_topic_0118921489_p4101484"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921489_row63784789"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921489_p66294319"><a name="zh-cn_topic_0118921489_p66294319"></a><a name="zh-cn_topic_0118921489_p66294319"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921489_p50988816"><a name="zh-cn_topic_0118921489_p50988816"></a><a name="zh-cn_topic_0118921489_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row10177076"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921489_p19036798"><a name="zh-cn_topic_0118921489_p19036798"></a><a name="zh-cn_topic_0118921489_p19036798"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921489_p65585652"><a name="zh-cn_topic_0118921489_p65585652"></a><a name="zh-cn_topic_0118921489_p65585652"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row53399964"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921489_p30429824"><a name="zh-cn_topic_0118921489_p30429824"></a><a name="zh-cn_topic_0118921489_p30429824"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921489_p9203142078"><a name="zh-cn_topic_0118921489_p9203142078"></a><a name="zh-cn_topic_0118921489_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row37417203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921489_p10894636"><a name="zh-cn_topic_0118921489_p10894636"></a><a name="zh-cn_topic_0118921489_p10894636"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921489_p13949586"><a name="zh-cn_topic_0118921489_p13949586"></a><a name="zh-cn_topic_0118921489_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row23344103"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921489_p11824190"><a name="zh-cn_topic_0118921489_p11824190"></a><a name="zh-cn_topic_0118921489_p11824190"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921489_p18235325"><a name="zh-cn_topic_0118921489_p18235325"></a><a name="zh-cn_topic_0118921489_p18235325"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921489_row29900204"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921489_p5997435"><a name="zh-cn_topic_0118921489_p5997435"></a><a name="zh-cn_topic_0118921489_p5997435"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921489_p16030215"><a name="zh-cn_topic_0118921489_p16030215"></a><a name="zh-cn_topic_0118921489_p16030215"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

