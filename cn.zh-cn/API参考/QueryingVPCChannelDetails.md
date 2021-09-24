# 查看VPC通道详情<a name="ZH-CN_TOPIC_0000001081837319"></a>

## 功能介绍<a name="zh-cn_topic_0118924576_section173482301428"></a>

查看指定的VPC通道详情。

## URI<a name="zh-cn_topic_0118924576_section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924576_table1439319294431"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924576_row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924576_p14361448204314"><a name="zh-cn_topic_0118924576_p14361448204314"></a><a name="zh-cn_topic_0118924576_p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924576_p1936174864316"><a name="zh-cn_topic_0118924576_p1936174864316"></a><a name="zh-cn_topic_0118924576_p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924576_row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924576_p1236111482435"><a name="zh-cn_topic_0118924576_p1236111482435"></a><a name="zh-cn_topic_0118924576_p1236111482435"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924576_p11361848184318"><a name="zh-cn_topic_0118924576_p11361848184318"></a><a name="zh-cn_topic_0118924576_p11361848184318"></a>/v1.0/apigw/vpc-channels/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924576_table18784710"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924576_row37287554"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924576_p393051"><a name="zh-cn_topic_0118924576_p393051"></a><a name="zh-cn_topic_0118924576_p393051"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924576_p31837140"><a name="zh-cn_topic_0118924576_p31837140"></a><a name="zh-cn_topic_0118924576_p31837140"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924576_p28671509"><a name="zh-cn_topic_0118924576_p28671509"></a><a name="zh-cn_topic_0118924576_p28671509"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924576_p40690887"><a name="zh-cn_topic_0118924576_p40690887"></a><a name="zh-cn_topic_0118924576_p40690887"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924576_row7627537"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924576_p13850780"><a name="zh-cn_topic_0118924576_p13850780"></a><a name="zh-cn_topic_0118924576_p13850780"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924576_p48171408"><a name="zh-cn_topic_0118924576_p48171408"></a><a name="zh-cn_topic_0118924576_p48171408"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924576_p9569939"><a name="zh-cn_topic_0118924576_p9569939"></a><a name="zh-cn_topic_0118924576_p9569939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924576_p36967632"><a name="zh-cn_topic_0118924576_p36967632"></a><a name="zh-cn_topic_0118924576_p36967632"></a>VPC通道的编号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924576_section73637302425"></a>

无

## 响应消息<a name="zh-cn_topic_0118924576_section9395153012420"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924576_table7395123013420"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924576_row114881330104215"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924576_p19488153019429"><a name="zh-cn_topic_0118924576_p19488153019429"></a><a name="zh-cn_topic_0118924576_p19488153019429"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924576_p248853014422"><a name="zh-cn_topic_0118924576_p248853014422"></a><a name="zh-cn_topic_0118924576_p248853014422"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924576_p64882308421"><a name="zh-cn_topic_0118924576_p64882308421"></a><a name="zh-cn_topic_0118924576_p64882308421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924576_row12488203074215"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p1448813305421"><a name="zh-cn_topic_0118924576_p1448813305421"></a><a name="zh-cn_topic_0118924576_p1448813305421"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p18488163024218"><a name="zh-cn_topic_0118924576_p18488163024218"></a><a name="zh-cn_topic_0118924576_p18488163024218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p25696563"><a name="zh-cn_topic_0118924576_p25696563"></a><a name="zh-cn_topic_0118924576_p25696563"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row17488133012421"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p1585685914587"><a name="zh-cn_topic_0118924576_p1585685914587"></a><a name="zh-cn_topic_0118924576_p1585685914587"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p4488183013424"><a name="zh-cn_topic_0118924576_p4488183013424"></a><a name="zh-cn_topic_0118924576_p4488183013424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p60351493"><a name="zh-cn_topic_0118924576_p60351493"></a><a name="zh-cn_topic_0118924576_p60351493"></a>VPC通道的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row748812305426"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p02495197162"><a name="zh-cn_topic_0118924576_p02495197162"></a><a name="zh-cn_topic_0118924576_p02495197162"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p16251161941619"><a name="zh-cn_topic_0118924576_p16251161941619"></a><a name="zh-cn_topic_0118924576_p16251161941619"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p5748337181118"><a name="zh-cn_topic_0118924576_p5748337181118"></a><a name="zh-cn_topic_0118924576_p5748337181118"></a>VPC通道的类型。</p>
<a name="zh-cn_topic_0118924576_ul4748103711119"></a><a name="zh-cn_topic_0118924576_ul4748103711119"></a><ul id="zh-cn_topic_0118924576_ul4748103711119"><li>2：API网关内置支持负载均衡功能的快速通道类型</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1670172818199"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p3847512181119"><a name="zh-cn_topic_0118924576_p3847512181119"></a><a name="zh-cn_topic_0118924576_p3847512181119"></a>member_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p18847112191114"><a name="zh-cn_topic_0118924576_p18847112191114"></a><a name="zh-cn_topic_0118924576_p18847112191114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p1399195415116"><a name="zh-cn_topic_0118924576_p1399195415116"></a><a name="zh-cn_topic_0118924576_p1399195415116"></a>VPC通道的成员类型。</p>
<a name="zh-cn_topic_0118924576_ul10402654141119"></a><a name="zh-cn_topic_0118924576_ul10402654141119"></a><ul id="zh-cn_topic_0118924576_ul10402654141119"><li>ip（暂不支持）</li><li>instance</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row138095017017"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p14809406014"><a name="zh-cn_topic_0118924576_p14809406014"></a><a name="zh-cn_topic_0118924576_p14809406014"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p5809305016"><a name="zh-cn_topic_0118924576_p5809305016"></a><a name="zh-cn_topic_0118924576_p5809305016"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p12663581620"><a name="zh-cn_topic_0118924576_p12663581620"></a><a name="zh-cn_topic_0118924576_p12663581620"></a>VPC通道的状态。</p>
<a name="zh-cn_topic_0118924576_ul15791839184416"></a><a name="zh-cn_topic_0118924576_ul15791839184416"></a><ul id="zh-cn_topic_0118924576_ul15791839184416"><li>1：正常</li><li>2：异常</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row31998111201"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p151995112018"><a name="zh-cn_topic_0118924576_p151995112018"></a><a name="zh-cn_topic_0118924576_p151995112018"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p15199011306"><a name="zh-cn_topic_0118924576_p15199011306"></a><a name="zh-cn_topic_0118924576_p15199011306"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p16681305"><a name="zh-cn_topic_0118924576_p16681305"></a><a name="zh-cn_topic_0118924576_p16681305"></a>VPC通道中主机的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row05591488016"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p135594817016"><a name="zh-cn_topic_0118924576_p135594817016"></a><a name="zh-cn_topic_0118924576_p135594817016"></a>balance_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p14559178309"><a name="zh-cn_topic_0118924576_p14559178309"></a><a name="zh-cn_topic_0118924576_p14559178309"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p22981401418"><a name="zh-cn_topic_0118924576_p22981401418"></a><a name="zh-cn_topic_0118924576_p22981401418"></a>分发算法。</p>
<a name="zh-cn_topic_0118924576_ul31881612450"></a><a name="zh-cn_topic_0118924576_ul31881612450"></a><ul id="zh-cn_topic_0118924576_ul31881612450"><li>1：加权轮询（wrr）</li><li>2：加权最少连接（wleastconn）</li><li>3：源地址哈希（source）</li><li>4：URI哈希（uri）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row109961654185911"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p19996135415590"><a name="zh-cn_topic_0118924576_p19996135415590"></a><a name="zh-cn_topic_0118924576_p19996135415590"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p20996554195919"><a name="zh-cn_topic_0118924576_p20996554195919"></a><a name="zh-cn_topic_0118924576_p20996554195919"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p198451273146"><a name="zh-cn_topic_0118924576_p198451273146"></a><a name="zh-cn_topic_0118924576_p198451273146"></a>VPC通道的创建时间。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row466713393162"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p1866793911618"><a name="zh-cn_topic_0118924576_p1866793911618"></a><a name="zh-cn_topic_0118924576_p1866793911618"></a>vpc_health_config</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p066713911614"><a name="zh-cn_topic_0118924576_p066713911614"></a><a name="zh-cn_topic_0118924576_p066713911614"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p8946531183318"><a name="zh-cn_topic_0118924576_p8946531183318"></a><a name="zh-cn_topic_0118924576_p8946531183318"></a>健康检查详情。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row164631042101616"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p2046324281615"><a name="zh-cn_topic_0118924576_p2046324281615"></a><a name="zh-cn_topic_0118924576_p2046324281615"></a>vpc_instances</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p44631442171612"><a name="zh-cn_topic_0118924576_p44631442171612"></a><a name="zh-cn_topic_0118924576_p44631442171612"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p14959403387"><a name="zh-cn_topic_0118924576_p14959403387"></a><a name="zh-cn_topic_0118924576_p14959403387"></a>后端实例列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  健康检查详情

<a name="zh-cn_topic_0118924576_table1693634310233"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924576_row0936643182314"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924576_p193613431232"><a name="zh-cn_topic_0118924576_p193613431232"></a><a name="zh-cn_topic_0118924576_p193613431232"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924576_p69521043122316"><a name="zh-cn_topic_0118924576_p69521043122316"></a><a name="zh-cn_topic_0118924576_p69521043122316"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924576_p795220430230"><a name="zh-cn_topic_0118924576_p795220430230"></a><a name="zh-cn_topic_0118924576_p795220430230"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924576_row16952243112316"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p32331457162311"><a name="zh-cn_topic_0118924576_p32331457162311"></a><a name="zh-cn_topic_0118924576_p32331457162311"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p15233175712314"><a name="zh-cn_topic_0118924576_p15233175712314"></a><a name="zh-cn_topic_0118924576_p15233175712314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p192337574235"><a name="zh-cn_topic_0118924576_p192337574235"></a><a name="zh-cn_topic_0118924576_p192337574235"></a>健康检查的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row6967154315237"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p2248185752312"><a name="zh-cn_topic_0118924576_p2248185752312"></a><a name="zh-cn_topic_0118924576_p2248185752312"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p1248657142318"><a name="zh-cn_topic_0118924576_p1248657142318"></a><a name="zh-cn_topic_0118924576_p1248657142318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p524825714231"><a name="zh-cn_topic_0118924576_p524825714231"></a><a name="zh-cn_topic_0118924576_p524825714231"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1196764392318"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p524812574235"><a name="zh-cn_topic_0118924576_p524812574235"></a><a name="zh-cn_topic_0118924576_p524812574235"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p18264145715238"><a name="zh-cn_topic_0118924576_p18264145715238"></a><a name="zh-cn_topic_0118924576_p18264145715238"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><div class="p" id="zh-cn_topic_0118924576_p1568844412104"><a name="zh-cn_topic_0118924576_p1568844412104"></a><a name="zh-cn_topic_0118924576_p1568844412104"></a>使用以下协议，对VPC中主机执行健康检查。<a name="zh-cn_topic_0118924576_ul19904951155719"></a><a name="zh-cn_topic_0118924576_ul19904951155719"></a><ul id="zh-cn_topic_0118924576_ul19904951155719"><li>TCP</li><li>HTTP</li><li>HTTPS</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row19983843172310"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p52641257192319"><a name="zh-cn_topic_0118924576_p52641257192319"></a><a name="zh-cn_topic_0118924576_p52641257192319"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p1926415571235"><a name="zh-cn_topic_0118924576_p1926415571235"></a><a name="zh-cn_topic_0118924576_p1926415571235"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p15591010195011"><a name="zh-cn_topic_0118924576_p15591010195011"></a><a name="zh-cn_topic_0118924576_p15591010195011"></a>健康检查时的目标路径。</p>
<div class="note" id="zh-cn_topic_0118924576_note38431529153919"><a name="zh-cn_topic_0118924576_note38431529153919"></a><a name="zh-cn_topic_0118924576_note38431529153919"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0118924576_p18843122918398"><a name="zh-cn_topic_0118924576_p18843122918398"></a><a name="zh-cn_topic_0118924576_p18843122918398"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row2099894312237"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p1528035752319"><a name="zh-cn_topic_0118924576_p1528035752319"></a><a name="zh-cn_topic_0118924576_p1528035752319"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p142803577233"><a name="zh-cn_topic_0118924576_p142803577233"></a><a name="zh-cn_topic_0118924576_p142803577233"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p78214132565"><a name="zh-cn_topic_0118924576_p78214132565"></a><a name="zh-cn_topic_0118924576_p78214132565"></a>健康检查的目标端口，缺省时为VPC中主机的端口号。</p>
<p id="zh-cn_topic_0118924576_p2782317155411"><a name="zh-cn_topic_0118924576_p2782317155411"></a><a name="zh-cn_topic_0118924576_p2782317155411"></a>取值范围1 ~ 65535。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row121312449237"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p728013575239"><a name="zh-cn_topic_0118924576_p728013575239"></a><a name="zh-cn_topic_0118924576_p728013575239"></a>threshold_normal</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p3280115719236"><a name="zh-cn_topic_0118924576_p3280115719236"></a><a name="zh-cn_topic_0118924576_p3280115719236"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p1315411125313"><a name="zh-cn_topic_0118924576_p1315411125313"></a><a name="zh-cn_topic_0118924576_p1315411125313"></a>正常阈值。</p>
<p id="zh-cn_topic_0118924576_p1798813185617"><a name="zh-cn_topic_0118924576_p1798813185617"></a><a name="zh-cn_topic_0118924576_p1798813185617"></a>判定VPC通道中主机正常的依据为：连续检查<em id="zh-cn_topic_0118924576_i421224922811"><a name="zh-cn_topic_0118924576_i421224922811"></a><a name="zh-cn_topic_0118924576_i421224922811"></a>x</em>成功，x为您设置的正常阈值。</p>
<p id="zh-cn_topic_0118924576_p35225297513"><a name="zh-cn_topic_0118924576_p35225297513"></a><a name="zh-cn_topic_0118924576_p35225297513"></a>取值范围2 ~ 10</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row9291144102319"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p1329505742320"><a name="zh-cn_topic_0118924576_p1329505742320"></a><a name="zh-cn_topic_0118924576_p1329505742320"></a>threshold_abnormal</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p9295105772310"><a name="zh-cn_topic_0118924576_p9295105772310"></a><a name="zh-cn_topic_0118924576_p9295105772310"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p1898161316565"><a name="zh-cn_topic_0118924576_p1898161316565"></a><a name="zh-cn_topic_0118924576_p1898161316565"></a>异常阙值。</p>
<p id="zh-cn_topic_0118924576_p79167352531"><a name="zh-cn_topic_0118924576_p79167352531"></a><a name="zh-cn_topic_0118924576_p79167352531"></a>判定VPC通道中主机异常的依据为：连续检查<em id="zh-cn_topic_0118924576_i37296135294"><a name="zh-cn_topic_0118924576_i37296135294"></a><a name="zh-cn_topic_0118924576_i37296135294"></a>x失败</em>，x为您设置的异常阈值。</p>
<p id="zh-cn_topic_0118924576_p1865194916514"><a name="zh-cn_topic_0118924576_p1865194916514"></a><a name="zh-cn_topic_0118924576_p1865194916514"></a>取值范围2 ~ 10。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row10458441233"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p15311057172317"><a name="zh-cn_topic_0118924576_p15311057172317"></a><a name="zh-cn_topic_0118924576_p15311057172317"></a>time_out</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p1531120573239"><a name="zh-cn_topic_0118924576_p1531120573239"></a><a name="zh-cn_topic_0118924576_p1531120573239"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p1925695318164"><a name="zh-cn_topic_0118924576_p1925695318164"></a><a name="zh-cn_topic_0118924576_p1925695318164"></a>超时时间：检查期间，无响应的时间，单位为秒。必须小于time_interval字段取值。</p>
<p id="zh-cn_topic_0118924576_p1825605391614"><a name="zh-cn_topic_0118924576_p1825605391614"></a><a name="zh-cn_topic_0118924576_p1825605391614"></a>取值范围2 ~ 30。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row945184422320"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p113114574236"><a name="zh-cn_topic_0118924576_p113114574236"></a><a name="zh-cn_topic_0118924576_p113114574236"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p2327155752313"><a name="zh-cn_topic_0118924576_p2327155752313"></a><a name="zh-cn_topic_0118924576_p2327155752313"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p52561653131615"><a name="zh-cn_topic_0118924576_p52561653131615"></a><a name="zh-cn_topic_0118924576_p52561653131615"></a>间隔时间：连续两次检查的间隔时间，单位为秒。必须大于time_out字段取值。</p>
<p id="zh-cn_topic_0118924576_p42566532160"><a name="zh-cn_topic_0118924576_p42566532160"></a><a name="zh-cn_topic_0118924576_p42566532160"></a>取值范围5 ~ 300。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row86064410234"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p1732745719232"><a name="zh-cn_topic_0118924576_p1732745719232"></a><a name="zh-cn_topic_0118924576_p1732745719232"></a>http_code</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p232711579234"><a name="zh-cn_topic_0118924576_p232711579234"></a><a name="zh-cn_topic_0118924576_p232711579234"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p15281310185519"><a name="zh-cn_topic_0118924576_p15281310185519"></a><a name="zh-cn_topic_0118924576_p15281310185519"></a>检查目标HTTP响应时，判断成功使用的HTTP响应码。</p>
<p id="zh-cn_topic_0118924576_p1144417511111"><a name="zh-cn_topic_0118924576_p1144417511111"></a><a name="zh-cn_topic_0118924576_p1144417511111"></a>取值范围为100到599之前的任意整数值，支持如下三种格式：</p>
<a name="zh-cn_topic_0118924576_ul343965120114"></a><a name="zh-cn_topic_0118924576_ul343965120114"></a><ul id="zh-cn_topic_0118924576_ul343965120114"><li>多个值，如：200,201,202</li><li>一系列值，如：200-299</li><li>组合值，如：201,202,210-299</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1931011312412"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p13103312242"><a name="zh-cn_topic_0118924576_p13103312242"></a><a name="zh-cn_topic_0118924576_p13103312242"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p522641116250"><a name="zh-cn_topic_0118924576_p522641116250"></a><a name="zh-cn_topic_0118924576_p522641116250"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p18226211142518"><a name="zh-cn_topic_0118924576_p18226211142518"></a><a name="zh-cn_topic_0118924576_p18226211142518"></a>VPC通道的创建时间。</p>
</td>
</tr>
</tbody>
</table>

**表 5**  后端实例详情

<a name="zh-cn_topic_0118924576_table2346632182717"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924576_row13464323270"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924576_p93464324278"><a name="zh-cn_topic_0118924576_p93464324278"></a><a name="zh-cn_topic_0118924576_p93464324278"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924576_p4346193213278"><a name="zh-cn_topic_0118924576_p4346193213278"></a><a name="zh-cn_topic_0118924576_p4346193213278"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924576_p53611732172712"><a name="zh-cn_topic_0118924576_p53611732172712"></a><a name="zh-cn_topic_0118924576_p53611732172712"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924576_row8361932112712"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p63611832132717"><a name="zh-cn_topic_0118924576_p63611832132717"></a><a name="zh-cn_topic_0118924576_p63611832132717"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p173611832112714"><a name="zh-cn_topic_0118924576_p173611832112714"></a><a name="zh-cn_topic_0118924576_p173611832112714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p163616323277"><a name="zh-cn_topic_0118924576_p163616323277"></a><a name="zh-cn_topic_0118924576_p163616323277"></a>后端实例对象的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row193611732112718"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p6361133242711"><a name="zh-cn_topic_0118924576_p6361133242711"></a><a name="zh-cn_topic_0118924576_p6361133242711"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p13377532192716"><a name="zh-cn_topic_0118924576_p13377532192716"></a><a name="zh-cn_topic_0118924576_p13377532192716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p4377103242715"><a name="zh-cn_topic_0118924576_p4377103242715"></a><a name="zh-cn_topic_0118924576_p4377103242715"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1537715321276"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p1637783215276"><a name="zh-cn_topic_0118924576_p1637783215276"></a><a name="zh-cn_topic_0118924576_p1637783215276"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p037713328279"><a name="zh-cn_topic_0118924576_p037713328279"></a><a name="zh-cn_topic_0118924576_p037713328279"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p1620615311293"><a name="zh-cn_topic_0118924576_p1620615311293"></a><a name="zh-cn_topic_0118924576_p1620615311293"></a>后端实例对象的状态。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row11392163220272"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p6462652102914"><a name="zh-cn_topic_0118924576_p6462652102914"></a><a name="zh-cn_topic_0118924576_p6462652102914"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p15392113202710"><a name="zh-cn_topic_0118924576_p15392113202710"></a><a name="zh-cn_topic_0118924576_p15392113202710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p7643513300"><a name="zh-cn_topic_0118924576_p7643513300"></a><a name="zh-cn_topic_0118924576_p7643513300"></a>后端实例的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1339216325273"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p12462195214295"><a name="zh-cn_topic_0118924576_p12462195214295"></a><a name="zh-cn_topic_0118924576_p12462195214295"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p103921532112711"><a name="zh-cn_topic_0118924576_p103921532112711"></a><a name="zh-cn_topic_0118924576_p103921532112711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p13641554304"><a name="zh-cn_topic_0118924576_p13641554304"></a><a name="zh-cn_topic_0118924576_p13641554304"></a>后端实例的ID。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1727563495911"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p11276133405917"><a name="zh-cn_topic_0118924576_p11276133405917"></a><a name="zh-cn_topic_0118924576_p11276133405917"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p127653405913"><a name="zh-cn_topic_0118924576_p127653405913"></a><a name="zh-cn_topic_0118924576_p127653405913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p1027614347599"><a name="zh-cn_topic_0118924576_p1027614347599"></a><a name="zh-cn_topic_0118924576_p1027614347599"></a>后端实例的主机地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1940916329273"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p10462165210296"><a name="zh-cn_topic_0118924576_p10462165210296"></a><a name="zh-cn_topic_0118924576_p10462165210296"></a>weight</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p5409163242719"><a name="zh-cn_topic_0118924576_p5409163242719"></a><a name="zh-cn_topic_0118924576_p5409163242719"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p1133512255618"><a name="zh-cn_topic_0118924576_p1133512255618"></a><a name="zh-cn_topic_0118924576_p1133512255618"></a>权重值。</p>
<p id="zh-cn_topic_0118924576_p4191102016478"><a name="zh-cn_topic_0118924576_p4191102016478"></a><a name="zh-cn_topic_0118924576_p4191102016478"></a>权重值越大，转发到该后端实例的请求数量越多。</p>
<p id="zh-cn_topic_0118924576_p17922913115812"><a name="zh-cn_topic_0118924576_p17922913115812"></a><a name="zh-cn_topic_0118924576_p17922913115812"></a>取值范围1 ~ 100。</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row043993222711"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924576_p143917320276"><a name="zh-cn_topic_0118924576_p143917320276"></a><a name="zh-cn_topic_0118924576_p143917320276"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924576_p1043963216271"><a name="zh-cn_topic_0118924576_p1043963216271"></a><a name="zh-cn_topic_0118924576_p1043963216271"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924576_p124391632192720"><a name="zh-cn_topic_0118924576_p124391632192720"></a><a name="zh-cn_topic_0118924576_p124391632192720"></a>后端实例增加到VPC通道的时间。</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "name": "vpc_001",
  "type": 2,
  "member_type": "instance",
  "port": 15565,
  "balance_strategy": 1,
  "id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
  "create_time": "2018-07-27T12:30:48Z",
  "status": 1,
  "vpc_health_config": {
    "protocol": "http",
    "path": "/hc",
    "port": 15563,
    "threshold_normal": 5,
    "threshold_abnormal": 5,
    "time_out": 30,
    "time_interval": 200,
    "http_code": "205",
    "id": "f26c1b158f2e40f2b531cf5c1b5e05e5",
    "vpc_id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
    "create_time": "2018-07-27T12:30:48Z"
  },
  "vpc_instances": [
    {
      "instance_id": "instance01",
      "instance_name": "instance_name01",
      "host": "127.0.0.1",
      "weight": 10,
      "id": "c3bc73605a8b400793363c87574fbad7",
      "vpc_id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
      "status": 1,
      "create_time": "2018-07-27T12:30:48Z"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0118924576_section338043011426"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0118924576_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924576_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924576_p174881730194216"><a name="zh-cn_topic_0118924576_p174881730194216"></a><a name="zh-cn_topic_0118924576_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924576_p848863018429"><a name="zh-cn_topic_0118924576_p848863018429"></a><a name="zh-cn_topic_0118924576_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924576_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924576_p7488163084211"><a name="zh-cn_topic_0118924576_p7488163084211"></a><a name="zh-cn_topic_0118924576_p7488163084211"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924576_p948803015424"><a name="zh-cn_topic_0118924576_p948803015424"></a><a name="zh-cn_topic_0118924576_p948803015424"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924576_p14488113015426"><a name="zh-cn_topic_0118924576_p14488113015426"></a><a name="zh-cn_topic_0118924576_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924576_p164881130154211"><a name="zh-cn_topic_0118924576_p164881130154211"></a><a name="zh-cn_topic_0118924576_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924576_p24883304428"><a name="zh-cn_topic_0118924576_p24883304428"></a><a name="zh-cn_topic_0118924576_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924576_p1848810308429"><a name="zh-cn_topic_0118924576_p1848810308429"></a><a name="zh-cn_topic_0118924576_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924576_p6488133064210"><a name="zh-cn_topic_0118924576_p6488133064210"></a><a name="zh-cn_topic_0118924576_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924576_p10488193018426"><a name="zh-cn_topic_0118924576_p10488193018426"></a><a name="zh-cn_topic_0118924576_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924576_p144883304428"><a name="zh-cn_topic_0118924576_p144883304428"></a><a name="zh-cn_topic_0118924576_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924576_p4488103094212"><a name="zh-cn_topic_0118924576_p4488103094212"></a><a name="zh-cn_topic_0118924576_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924576_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924576_p17488163014423"><a name="zh-cn_topic_0118924576_p17488163014423"></a><a name="zh-cn_topic_0118924576_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924576_p048813014216"><a name="zh-cn_topic_0118924576_p048813014216"></a><a name="zh-cn_topic_0118924576_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

