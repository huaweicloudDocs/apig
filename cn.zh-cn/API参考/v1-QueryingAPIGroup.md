# 查看分组详情<a name="ZH-CN_TOPIC_0000001082135159"></a>

## 功能介绍<a name="zh-cn_topic_0225568811_section1735744"></a>

查询指定分组的详细信息。

## URI<a name="zh-cn_topic_0225568811_section15621702"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568811_table32113079"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568811_row20115923"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568811_p18777034"><a name="zh-cn_topic_0225568811_p18777034"></a><a name="zh-cn_topic_0225568811_p18777034"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568811_p44544806"><a name="zh-cn_topic_0225568811_p44544806"></a><a name="zh-cn_topic_0225568811_p44544806"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568811_row51359567"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568811_p66484268"><a name="zh-cn_topic_0225568811_p66484268"></a><a name="zh-cn_topic_0225568811_p66484268"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568811_p16516646"><a name="zh-cn_topic_0225568811_p16516646"></a><a name="zh-cn_topic_0225568811_p16516646"></a>/v1/{project_id}/apigw/instances/{instance_id}/api-groups/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568811_table62779940"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568811_row53801450"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568811_p62950166"><a name="zh-cn_topic_0225568811_p62950166"></a><a name="zh-cn_topic_0225568811_p62950166"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568811_p65798711"><a name="zh-cn_topic_0225568811_p65798711"></a><a name="zh-cn_topic_0225568811_p65798711"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568811_p28095413"><a name="zh-cn_topic_0225568811_p28095413"></a><a name="zh-cn_topic_0225568811_p28095413"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568811_p61135991"><a name="zh-cn_topic_0225568811_p61135991"></a><a name="zh-cn_topic_0225568811_p61135991"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568811_row1394513141411"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568811_p55878963"><a name="zh-cn_topic_0225568811_p55878963"></a><a name="zh-cn_topic_0225568811_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568811_p29902160"><a name="zh-cn_topic_0225568811_p29902160"></a><a name="zh-cn_topic_0225568811_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568811_p6155914"><a name="zh-cn_topic_0225568811_p6155914"></a><a name="zh-cn_topic_0225568811_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568811_p28867016"><a name="zh-cn_topic_0225568811_p28867016"></a><a name="zh-cn_topic_0225568811_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row11154153116141"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568811_p1780913159538"><a name="zh-cn_topic_0225568811_p1780913159538"></a><a name="zh-cn_topic_0225568811_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568811_p9809215115310"><a name="zh-cn_topic_0225568811_p9809215115310"></a><a name="zh-cn_topic_0225568811_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568811_p1280914152538"><a name="zh-cn_topic_0225568811_p1280914152538"></a><a name="zh-cn_topic_0225568811_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568811_p1880914157537"><a name="zh-cn_topic_0225568811_p1880914157537"></a><a name="zh-cn_topic_0225568811_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row53068262"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568811_p3561961"><a name="zh-cn_topic_0225568811_p3561961"></a><a name="zh-cn_topic_0225568811_p3561961"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568811_p20083433"><a name="zh-cn_topic_0225568811_p20083433"></a><a name="zh-cn_topic_0225568811_p20083433"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568811_p16145357"><a name="zh-cn_topic_0225568811_p16145357"></a><a name="zh-cn_topic_0225568811_p16145357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568811_p32705534"><a name="zh-cn_topic_0225568811_p32705534"></a><a name="zh-cn_topic_0225568811_p32705534"></a>分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568811_section6377591"></a>

无

## 响应消息<a name="zh-cn_topic_0225568811_section46822891"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568811_table23378999"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568811_row11169479"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568811_p32312619"><a name="zh-cn_topic_0225568811_p32312619"></a><a name="zh-cn_topic_0225568811_p32312619"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568811_p76446"><a name="zh-cn_topic_0225568811_p76446"></a><a name="zh-cn_topic_0225568811_p76446"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568811_p6192203"><a name="zh-cn_topic_0225568811_p6192203"></a><a name="zh-cn_topic_0225568811_p6192203"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568811_row31806424"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p26183533"><a name="zh-cn_topic_0225568811_p26183533"></a><a name="zh-cn_topic_0225568811_p26183533"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p40491443"><a name="zh-cn_topic_0225568811_p40491443"></a><a name="zh-cn_topic_0225568811_p40491443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p58581457"><a name="zh-cn_topic_0225568811_p58581457"></a><a name="zh-cn_topic_0225568811_p58581457"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row57471073"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p24645368"><a name="zh-cn_topic_0225568811_p24645368"></a><a name="zh-cn_topic_0225568811_p24645368"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p50117754"><a name="zh-cn_topic_0225568811_p50117754"></a><a name="zh-cn_topic_0225568811_p50117754"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p33006289"><a name="zh-cn_topic_0225568811_p33006289"></a><a name="zh-cn_topic_0225568811_p33006289"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row28621152"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p36611985"><a name="zh-cn_topic_0225568811_p36611985"></a><a name="zh-cn_topic_0225568811_p36611985"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p12780810"><a name="zh-cn_topic_0225568811_p12780810"></a><a name="zh-cn_topic_0225568811_p12780810"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p28612724"><a name="zh-cn_topic_0225568811_p28612724"></a><a name="zh-cn_topic_0225568811_p28612724"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row56187931"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p54928561"><a name="zh-cn_topic_0225568811_p54928561"></a><a name="zh-cn_topic_0225568811_p54928561"></a>sl_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p20028427"><a name="zh-cn_topic_0225568811_p20028427"></a><a name="zh-cn_topic_0225568811_p20028427"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p11689873"><a name="zh-cn_topic_0225568811_p11689873"></a><a name="zh-cn_topic_0225568811_p11689873"></a>系统默认分配的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row38100001"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p66201237"><a name="zh-cn_topic_0225568811_p66201237"></a><a name="zh-cn_topic_0225568811_p66201237"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p60700010"><a name="zh-cn_topic_0225568811_p60700010"></a><a name="zh-cn_topic_0225568811_p60700010"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p17753800"><a name="zh-cn_topic_0225568811_p17753800"></a><a name="zh-cn_topic_0225568811_p17753800"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row25566473"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p57618438"><a name="zh-cn_topic_0225568811_p57618438"></a><a name="zh-cn_topic_0225568811_p57618438"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p36581920"><a name="zh-cn_topic_0225568811_p36581920"></a><a name="zh-cn_topic_0225568811_p36581920"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p10345534"><a name="zh-cn_topic_0225568811_p10345534"></a><a name="zh-cn_topic_0225568811_p10345534"></a>最近修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row26000946"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p25701906"><a name="zh-cn_topic_0225568811_p25701906"></a><a name="zh-cn_topic_0225568811_p25701906"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p1479659"><a name="zh-cn_topic_0225568811_p1479659"></a><a name="zh-cn_topic_0225568811_p1479659"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p52743524"><a name="zh-cn_topic_0225568811_p52743524"></a><a name="zh-cn_topic_0225568811_p52743524"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row4929668"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p63758800"><a name="zh-cn_topic_0225568811_p63758800"></a><a name="zh-cn_topic_0225568811_p63758800"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p64189201"><a name="zh-cn_topic_0225568811_p64189201"></a><a name="zh-cn_topic_0225568811_p64189201"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p31942831"><a name="zh-cn_topic_0225568811_p31942831"></a><a name="zh-cn_topic_0225568811_p31942831"></a>流控时长内分组下的API的总访问次数限制，默认不限，请根据服务的负载能力自行设置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row19050028"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p66657312"><a name="zh-cn_topic_0225568811_p66657312"></a><a name="zh-cn_topic_0225568811_p66657312"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p30533155"><a name="zh-cn_topic_0225568811_p30533155"></a><a name="zh-cn_topic_0225568811_p30533155"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p57266528"><a name="zh-cn_topic_0225568811_p57266528"></a><a name="zh-cn_topic_0225568811_p57266528"></a>流控时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row45636707"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p5585767"><a name="zh-cn_topic_0225568811_p5585767"></a><a name="zh-cn_topic_0225568811_p5585767"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p49793976"><a name="zh-cn_topic_0225568811_p49793976"></a><a name="zh-cn_topic_0225568811_p49793976"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p6780221"><a name="zh-cn_topic_0225568811_p6780221"></a><a name="zh-cn_topic_0225568811_p6780221"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row61021990"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p43834197"><a name="zh-cn_topic_0225568811_p43834197"></a><a name="zh-cn_topic_0225568811_p43834197"></a>url_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p60909101"><a name="zh-cn_topic_0225568811_p60909101"></a><a name="zh-cn_topic_0225568811_p60909101"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p34690133"><a name="zh-cn_topic_0225568811_p34690133"></a><a name="zh-cn_topic_0225568811_p34690133"></a>分组上绑定的独立域名列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row43775742"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p56174242"><a name="zh-cn_topic_0225568811_p56174242"></a><a name="zh-cn_topic_0225568811_p56174242"></a>on_sell_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p53819754"><a name="zh-cn_topic_0225568811_p53819754"></a><a name="zh-cn_topic_0225568811_p53819754"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p64432831"><a name="zh-cn_topic_0225568811_p64432831"></a><a name="zh-cn_topic_0225568811_p64432831"></a>是否已上架云市场：</p>
<a name="zh-cn_topic_0225568811_ul43024569"></a><a name="zh-cn_topic_0225568811_ul43024569"></a><ul id="zh-cn_topic_0225568811_ul43024569"><li>1：已上架</li><li>2：未上架</li><li>3：审核中</li></ul>
</td>
</tr>
</tbody>
</table>

**表 4**  url\_domains参数说明

<a name="zh-cn_topic_0225568811_table24320671"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568811_row54780417"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568811_p8028813"><a name="zh-cn_topic_0225568811_p8028813"></a><a name="zh-cn_topic_0225568811_p8028813"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568811_p46354150"><a name="zh-cn_topic_0225568811_p46354150"></a><a name="zh-cn_topic_0225568811_p46354150"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568811_p63698675"><a name="zh-cn_topic_0225568811_p63698675"></a><a name="zh-cn_topic_0225568811_p63698675"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568811_row59319069"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p40115275"><a name="zh-cn_topic_0225568811_p40115275"></a><a name="zh-cn_topic_0225568811_p40115275"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p28111846"><a name="zh-cn_topic_0225568811_p28111846"></a><a name="zh-cn_topic_0225568811_p28111846"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p62467029"><a name="zh-cn_topic_0225568811_p62467029"></a><a name="zh-cn_topic_0225568811_p62467029"></a>域名编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row25332352"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p38654601"><a name="zh-cn_topic_0225568811_p38654601"></a><a name="zh-cn_topic_0225568811_p38654601"></a>domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p44014938"><a name="zh-cn_topic_0225568811_p44014938"></a><a name="zh-cn_topic_0225568811_p44014938"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p8440220"><a name="zh-cn_topic_0225568811_p8440220"></a><a name="zh-cn_topic_0225568811_p8440220"></a>访问域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row8853118"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p46013996"><a name="zh-cn_topic_0225568811_p46013996"></a><a name="zh-cn_topic_0225568811_p46013996"></a>cname_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p36146206"><a name="zh-cn_topic_0225568811_p36146206"></a><a name="zh-cn_topic_0225568811_p36146206"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p42161597"><a name="zh-cn_topic_0225568811_p42161597"></a><a name="zh-cn_topic_0225568811_p42161597"></a>域名cname状态：</p>
<a name="zh-cn_topic_0225568811_ul43910056"></a><a name="zh-cn_topic_0225568811_ul43910056"></a><ul id="zh-cn_topic_0225568811_ul43910056"><li>1：未解析</li><li>2：解析中</li><li>3：解析成功</li><li>4：解析失败</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row26883636"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p30090901"><a name="zh-cn_topic_0225568811_p30090901"></a><a name="zh-cn_topic_0225568811_p30090901"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p21443882"><a name="zh-cn_topic_0225568811_p21443882"></a><a name="zh-cn_topic_0225568811_p21443882"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p59232859"><a name="zh-cn_topic_0225568811_p59232859"></a><a name="zh-cn_topic_0225568811_p59232859"></a>SSL证书编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row14816368320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568811_p1481696133213"><a name="zh-cn_topic_0225568811_p1481696133213"></a><a name="zh-cn_topic_0225568811_p1481696133213"></a>ssl_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568811_p188160643214"><a name="zh-cn_topic_0225568811_p188160643214"></a><a name="zh-cn_topic_0225568811_p188160643214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568811_p13816176133212"><a name="zh-cn_topic_0225568811_p13816176133212"></a><a name="zh-cn_topic_0225568811_p13816176133212"></a>SSL证书名称</p>
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
	"remark": "分组001",
	"register_time": "2017-12-28T11:44:53Z",
	"update_time": "2017-12-28T11:49:01.048601Z",
	"call_limits": 1000,
	"time_interval": 1,
	"time_unit": "SECOND",
	"on_sell_status": 2
}
```

## 状态码<a name="zh-cn_topic_0225568811_section57398326"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568811_table33970788"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568811_row57167435"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568811_p50635"><a name="zh-cn_topic_0225568811_p50635"></a><a name="zh-cn_topic_0225568811_p50635"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568811_p4101484"><a name="zh-cn_topic_0225568811_p4101484"></a><a name="zh-cn_topic_0225568811_p4101484"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568811_row63784789"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568811_p66294319"><a name="zh-cn_topic_0225568811_p66294319"></a><a name="zh-cn_topic_0225568811_p66294319"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568811_p50988816"><a name="zh-cn_topic_0225568811_p50988816"></a><a name="zh-cn_topic_0225568811_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row10177076"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568811_p19036798"><a name="zh-cn_topic_0225568811_p19036798"></a><a name="zh-cn_topic_0225568811_p19036798"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568811_p65585652"><a name="zh-cn_topic_0225568811_p65585652"></a><a name="zh-cn_topic_0225568811_p65585652"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row53399964"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568811_p30429824"><a name="zh-cn_topic_0225568811_p30429824"></a><a name="zh-cn_topic_0225568811_p30429824"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568811_p9203142078"><a name="zh-cn_topic_0225568811_p9203142078"></a><a name="zh-cn_topic_0225568811_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row37417203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568811_p10894636"><a name="zh-cn_topic_0225568811_p10894636"></a><a name="zh-cn_topic_0225568811_p10894636"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568811_p13949586"><a name="zh-cn_topic_0225568811_p13949586"></a><a name="zh-cn_topic_0225568811_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row23344103"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568811_p11824190"><a name="zh-cn_topic_0225568811_p11824190"></a><a name="zh-cn_topic_0225568811_p11824190"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568811_p18235325"><a name="zh-cn_topic_0225568811_p18235325"></a><a name="zh-cn_topic_0225568811_p18235325"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568811_row29900204"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568811_p5997435"><a name="zh-cn_topic_0225568811_p5997435"></a><a name="zh-cn_topic_0225568811_p5997435"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568811_p16030215"><a name="zh-cn_topic_0225568811_p16030215"></a><a name="zh-cn_topic_0225568811_p16030215"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

