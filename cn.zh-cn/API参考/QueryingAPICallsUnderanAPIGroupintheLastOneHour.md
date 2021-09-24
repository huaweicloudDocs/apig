# 分组统计信息查询-最近一小时<a name="ZH-CN_TOPIC_0000001082135149"></a>

## 功能介绍<a name="zh-cn_topic_0118924585_section40237157"></a>

根据API的id和最近的一段时间查询API被调用的次数，统计周期为1分钟。查询范围一小时以内，一分钟一个样本，其样本值为一分钟内的累计值。

>![](public_sys-resources/icon-note.gif) **说明：** 
>为了安全起见，在服务器上使用curl命令调用接口查询信息后，需要清理历史操作记录，包括但不限于“\~/.bash\_history”、“/var/log/messages”（如有）。

## URI<a name="zh-cn_topic_0118924585_section26590094"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924585_table5803581"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924585_row4909618"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924585_p62134781"><a name="zh-cn_topic_0118924585_p62134781"></a><a name="zh-cn_topic_0118924585_p62134781"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="84.85000000000001%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924585_p66861340"><a name="zh-cn_topic_0118924585_p66861340"></a><a name="zh-cn_topic_0118924585_p66861340"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924585_row47059448"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924585_p53718904"><a name="zh-cn_topic_0118924585_p53718904"></a><a name="zh-cn_topic_0118924585_p53718904"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="84.85000000000001%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924585_p56263940"><a name="zh-cn_topic_0118924585_p56263940"></a><a name="zh-cn_topic_0118924585_p56263940"></a>/v1.0/apigw/statistics/group/latest?group_id=[group_id]</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924585_section37984255"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118924585_table61085317"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924585_row48300983"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924585_p20065559"><a name="zh-cn_topic_0118924585_p20065559"></a><a name="zh-cn_topic_0118924585_p20065559"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924585_p14697563"><a name="zh-cn_topic_0118924585_p14697563"></a><a name="zh-cn_topic_0118924585_p14697563"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924585_p49651948"><a name="zh-cn_topic_0118924585_p49651948"></a><a name="zh-cn_topic_0118924585_p49651948"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924585_p62384817"><a name="zh-cn_topic_0118924585_p62384817"></a><a name="zh-cn_topic_0118924585_p62384817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924585_row20005394"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p9824249"><a name="zh-cn_topic_0118924585_p9824249"></a><a name="zh-cn_topic_0118924585_p9824249"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p57566667"><a name="zh-cn_topic_0118924585_p57566667"></a><a name="zh-cn_topic_0118924585_p57566667"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p32388466"><a name="zh-cn_topic_0118924585_p32388466"></a><a name="zh-cn_topic_0118924585_p32388466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p6220118"><a name="zh-cn_topic_0118924585_p6220118"></a><a name="zh-cn_topic_0118924585_p6220118"></a>分组的id</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0118924585_section56825797"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924585_table15405159"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924585_row4132425"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924585_p66290997"><a name="zh-cn_topic_0118924585_p66290997"></a><a name="zh-cn_topic_0118924585_p66290997"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924585_p861637"><a name="zh-cn_topic_0118924585_p861637"></a><a name="zh-cn_topic_0118924585_p861637"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924585_p2683745"><a name="zh-cn_topic_0118924585_p2683745"></a><a name="zh-cn_topic_0118924585_p2683745"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924585_p16056818"><a name="zh-cn_topic_0118924585_p16056818"></a><a name="zh-cn_topic_0118924585_p16056818"></a>操作类型</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924585_row25533920"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p54981650"><a name="zh-cn_topic_0118924585_p54981650"></a><a name="zh-cn_topic_0118924585_p54981650"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p24328689"><a name="zh-cn_topic_0118924585_p24328689"></a><a name="zh-cn_topic_0118924585_p24328689"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p24466788"><a name="zh-cn_topic_0118924585_p24466788"></a><a name="zh-cn_topic_0118924585_p24466788"></a>响应码</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p35652820"><a name="zh-cn_topic_0118924585_p35652820"></a><a name="zh-cn_topic_0118924585_p35652820"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row52439926"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p19775595"><a name="zh-cn_topic_0118924585_p19775595"></a><a name="zh-cn_topic_0118924585_p19775595"></a>msg</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p58319377"><a name="zh-cn_topic_0118924585_p58319377"></a><a name="zh-cn_topic_0118924585_p58319377"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p26249103"><a name="zh-cn_topic_0118924585_p26249103"></a><a name="zh-cn_topic_0118924585_p26249103"></a>返回消息</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p45802638"><a name="zh-cn_topic_0118924585_p45802638"></a><a name="zh-cn_topic_0118924585_p45802638"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row9570566"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p37018344"><a name="zh-cn_topic_0118924585_p37018344"></a><a name="zh-cn_topic_0118924585_p37018344"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p45695903"><a name="zh-cn_topic_0118924585_p45695903"></a><a name="zh-cn_topic_0118924585_p45695903"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p10380691"><a name="zh-cn_topic_0118924585_p10380691"></a><a name="zh-cn_topic_0118924585_p10380691"></a>开始时间的UTC时间戳</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p35529643"><a name="zh-cn_topic_0118924585_p35529643"></a><a name="zh-cn_topic_0118924585_p35529643"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row51331336"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p64197586"><a name="zh-cn_topic_0118924585_p64197586"></a><a name="zh-cn_topic_0118924585_p64197586"></a>end_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p32622005"><a name="zh-cn_topic_0118924585_p32622005"></a><a name="zh-cn_topic_0118924585_p32622005"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p25136728"><a name="zh-cn_topic_0118924585_p25136728"></a><a name="zh-cn_topic_0118924585_p25136728"></a>截止时间的UTC时间戳</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p22809059"><a name="zh-cn_topic_0118924585_p22809059"></a><a name="zh-cn_topic_0118924585_p22809059"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row3954943"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p51915003"><a name="zh-cn_topic_0118924585_p51915003"></a><a name="zh-cn_topic_0118924585_p51915003"></a>list</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p44365682"><a name="zh-cn_topic_0118924585_p44365682"></a><a name="zh-cn_topic_0118924585_p44365682"></a>结构体数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p36850510"><a name="zh-cn_topic_0118924585_p36850510"></a><a name="zh-cn_topic_0118924585_p36850510"></a>统计指标的数据结构结构体</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p32101367"><a name="zh-cn_topic_0118924585_p32101367"></a><a name="zh-cn_topic_0118924585_p32101367"></a>R</p>
</td>
</tr>
</tbody>
</table>

**表 4**  参数说明

<a name="zh-cn_topic_0118924585_table20476852"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924585_row32908784"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924585_p48365865"><a name="zh-cn_topic_0118924585_p48365865"></a><a name="zh-cn_topic_0118924585_p48365865"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924585_p25320962"><a name="zh-cn_topic_0118924585_p25320962"></a><a name="zh-cn_topic_0118924585_p25320962"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924585_p37732003"><a name="zh-cn_topic_0118924585_p37732003"></a><a name="zh-cn_topic_0118924585_p37732003"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924585_p36393397"><a name="zh-cn_topic_0118924585_p36393397"></a><a name="zh-cn_topic_0118924585_p36393397"></a>操作类型</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924585_row62184031"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p3741770"><a name="zh-cn_topic_0118924585_p3741770"></a><a name="zh-cn_topic_0118924585_p3741770"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p34647966"><a name="zh-cn_topic_0118924585_p34647966"></a><a name="zh-cn_topic_0118924585_p34647966"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p55021825"><a name="zh-cn_topic_0118924585_p55021825"></a><a name="zh-cn_topic_0118924585_p55021825"></a>分组的id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p27582878"><a name="zh-cn_topic_0118924585_p27582878"></a><a name="zh-cn_topic_0118924585_p27582878"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row46919313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p42367989"><a name="zh-cn_topic_0118924585_p42367989"></a><a name="zh-cn_topic_0118924585_p42367989"></a>current_minute</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p9255078"><a name="zh-cn_topic_0118924585_p9255078"></a><a name="zh-cn_topic_0118924585_p9255078"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p11463819"><a name="zh-cn_topic_0118924585_p11463819"></a><a name="zh-cn_topic_0118924585_p11463819"></a>utc的timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p56154124"><a name="zh-cn_topic_0118924585_p56154124"></a><a name="zh-cn_topic_0118924585_p56154124"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row35625075"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p67058859"><a name="zh-cn_topic_0118924585_p67058859"></a><a name="zh-cn_topic_0118924585_p67058859"></a>provider</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p63058483"><a name="zh-cn_topic_0118924585_p63058483"></a><a name="zh-cn_topic_0118924585_p63058483"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p7463475"><a name="zh-cn_topic_0118924585_p7463475"></a><a name="zh-cn_topic_0118924585_p7463475"></a>API拥有者</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p561748"><a name="zh-cn_topic_0118924585_p561748"></a><a name="zh-cn_topic_0118924585_p561748"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row5055736"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p6861485"><a name="zh-cn_topic_0118924585_p6861485"></a><a name="zh-cn_topic_0118924585_p6861485"></a>req_count</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p18909398"><a name="zh-cn_topic_0118924585_p18909398"></a><a name="zh-cn_topic_0118924585_p18909398"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p55266268"><a name="zh-cn_topic_0118924585_p55266268"></a><a name="zh-cn_topic_0118924585_p55266268"></a>请求总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p47382694"><a name="zh-cn_topic_0118924585_p47382694"></a><a name="zh-cn_topic_0118924585_p47382694"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row23791064"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p48028036"><a name="zh-cn_topic_0118924585_p48028036"></a><a name="zh-cn_topic_0118924585_p48028036"></a>max_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p65065704"><a name="zh-cn_topic_0118924585_p65065704"></a><a name="zh-cn_topic_0118924585_p65065704"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p35830701"><a name="zh-cn_topic_0118924585_p35830701"></a><a name="zh-cn_topic_0118924585_p35830701"></a>最大延时(ms)</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p16605691"><a name="zh-cn_topic_0118924585_p16605691"></a><a name="zh-cn_topic_0118924585_p16605691"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row15233492"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p25953345"><a name="zh-cn_topic_0118924585_p25953345"></a><a name="zh-cn_topic_0118924585_p25953345"></a>avg_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p21846219"><a name="zh-cn_topic_0118924585_p21846219"></a><a name="zh-cn_topic_0118924585_p21846219"></a>Double</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p24713305"><a name="zh-cn_topic_0118924585_p24713305"></a><a name="zh-cn_topic_0118924585_p24713305"></a>平均耗时（ms）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p55620692"><a name="zh-cn_topic_0118924585_p55620692"></a><a name="zh-cn_topic_0118924585_p55620692"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row30824181"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p13730750"><a name="zh-cn_topic_0118924585_p13730750"></a><a name="zh-cn_topic_0118924585_p13730750"></a>output_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p38448935"><a name="zh-cn_topic_0118924585_p38448935"></a><a name="zh-cn_topic_0118924585_p38448935"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p27355992"><a name="zh-cn_topic_0118924585_p27355992"></a><a name="zh-cn_topic_0118924585_p27355992"></a>下行吞吐量（byte）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p1242874"><a name="zh-cn_topic_0118924585_p1242874"></a><a name="zh-cn_topic_0118924585_p1242874"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row11185868"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p33640154"><a name="zh-cn_topic_0118924585_p33640154"></a><a name="zh-cn_topic_0118924585_p33640154"></a>input_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p40497964"><a name="zh-cn_topic_0118924585_p40497964"></a><a name="zh-cn_topic_0118924585_p40497964"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p59109675"><a name="zh-cn_topic_0118924585_p59109675"></a><a name="zh-cn_topic_0118924585_p59109675"></a>上行吞吐量（byte）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p23154366"><a name="zh-cn_topic_0118924585_p23154366"></a><a name="zh-cn_topic_0118924585_p23154366"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row7062707"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p35208384"><a name="zh-cn_topic_0118924585_p35208384"></a><a name="zh-cn_topic_0118924585_p35208384"></a>req_count4xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p33306837"><a name="zh-cn_topic_0118924585_p33306837"></a><a name="zh-cn_topic_0118924585_p33306837"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p13499291"><a name="zh-cn_topic_0118924585_p13499291"></a><a name="zh-cn_topic_0118924585_p13499291"></a>4xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p19700793"><a name="zh-cn_topic_0118924585_p19700793"></a><a name="zh-cn_topic_0118924585_p19700793"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row43089417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p581920"><a name="zh-cn_topic_0118924585_p581920"></a><a name="zh-cn_topic_0118924585_p581920"></a>req_count5xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p47135522"><a name="zh-cn_topic_0118924585_p47135522"></a><a name="zh-cn_topic_0118924585_p47135522"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p59880953"><a name="zh-cn_topic_0118924585_p59880953"></a><a name="zh-cn_topic_0118924585_p59880953"></a>5xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p18519053"><a name="zh-cn_topic_0118924585_p18519053"></a><a name="zh-cn_topic_0118924585_p18519053"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row32453753"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p11508338"><a name="zh-cn_topic_0118924585_p11508338"></a><a name="zh-cn_topic_0118924585_p11508338"></a>req_count2xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p59760220"><a name="zh-cn_topic_0118924585_p59760220"></a><a name="zh-cn_topic_0118924585_p59760220"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p8739679"><a name="zh-cn_topic_0118924585_p8739679"></a><a name="zh-cn_topic_0118924585_p8739679"></a>2xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p36825378"><a name="zh-cn_topic_0118924585_p36825378"></a><a name="zh-cn_topic_0118924585_p36825378"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row62992947"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p2155065"><a name="zh-cn_topic_0118924585_p2155065"></a><a name="zh-cn_topic_0118924585_p2155065"></a>req_count_error</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p40342613"><a name="zh-cn_topic_0118924585_p40342613"></a><a name="zh-cn_topic_0118924585_p40342613"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p46526188"><a name="zh-cn_topic_0118924585_p46526188"></a><a name="zh-cn_topic_0118924585_p46526188"></a>错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p10524904"><a name="zh-cn_topic_0118924585_p10524904"></a><a name="zh-cn_topic_0118924585_p10524904"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row27615280"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p22245182"><a name="zh-cn_topic_0118924585_p22245182"></a><a name="zh-cn_topic_0118924585_p22245182"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p57029284"><a name="zh-cn_topic_0118924585_p57029284"></a><a name="zh-cn_topic_0118924585_p57029284"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p55969291"><a name="zh-cn_topic_0118924585_p55969291"></a><a name="zh-cn_topic_0118924585_p55969291"></a>记录时间（格式为：yyyy-MM-dd HH:mm:ss）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p37218714"><a name="zh-cn_topic_0118924585_p37218714"></a><a name="zh-cn_topic_0118924585_p37218714"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924585_row66532977"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924585_p20462032"><a name="zh-cn_topic_0118924585_p20462032"></a><a name="zh-cn_topic_0118924585_p20462032"></a>req_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924585_p46811884"><a name="zh-cn_topic_0118924585_p46811884"></a><a name="zh-cn_topic_0118924585_p46811884"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924585_p33666220"><a name="zh-cn_topic_0118924585_p33666220"></a><a name="zh-cn_topic_0118924585_p33666220"></a>请求时间（格式为：yyyy-MM-dd HH:mm:ss）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924585_p42609272"><a name="zh-cn_topic_0118924585_p42609272"></a><a name="zh-cn_topic_0118924585_p42609272"></a>R</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"code": "000000",
	"msg": "",
	"list": [{
		"group_id": "d7b52683-341b-4234-8261-66b4cfbfbda5",
		"current_minute": 1516849440,
		"provider": "205fa874817a4dcfae9222a3be4725e8",
		"req_count": 1981,
		"max_latency": 199,
		"avg_latency": 98.17,
		"output_throughput": 694483,
		"input_throughput": 694483,
		"req_count4xx": 669,
		"req_count5xx": 312,
		"req_count2xx": 327,
		"req_count_error": 981,
		"register_time": "2018-01-25 11:04:09",
		"req_time": "2018-01-25 11:04:00"
	}],
	"start_time": 1516845900,
	"end_time": 1516849440
}
```

## 状态码<a name="zh-cn_topic_0118924585_section6313977"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924585_table8008179"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924585_row31994764"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924585_p41439074"><a name="zh-cn_topic_0118924585_p41439074"></a><a name="zh-cn_topic_0118924585_p41439074"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924585_p1121870"><a name="zh-cn_topic_0118924585_p1121870"></a><a name="zh-cn_topic_0118924585_p1121870"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924585_row23762613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924585_p45723521"><a name="zh-cn_topic_0118924585_p45723521"></a><a name="zh-cn_topic_0118924585_p45723521"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924585_p12617754"><a name="zh-cn_topic_0118924585_p12617754"></a><a name="zh-cn_topic_0118924585_p12617754"></a>Query Success</p>
</td>
</tr>
</tbody>
</table>

