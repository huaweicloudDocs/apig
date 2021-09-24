# API统计信息查询-最近一段时间<a name="ZH-CN_TOPIC_0000001082221233"></a>

## 功能介绍<a name="zh-cn_topic_0118924584_section41694086"></a>

根据API的id和最近的一段时间查询API被调用的次数，统计周期为1分钟、小时、天。

-   查询范围一小时以内，一分钟一个样本，其样本值为一分钟内的累计值，服务器返回服务器的时间的上一分钟到往前推N分钟的数据；
-   查询范围一天以内，返回一小时一个样本，其样本值为一小时内的累计值，服务器会返回最近时长横跨统计周期的数据，比如时长为大于2小时，且小于3小时，那么会查询最近3个小时的数据；
-   查询超过一天以上，返回一天为一个样本，其样本值为一天内的累计值，服务器会返回最近时长横跨统计周期的数据。

>![](public_sys-resources/icon-note.gif) **说明：** 
>为了安全起见，在服务器上使用curl命令调用接口查询信息后，需要清理历史操作记录，包括但不限于“\~/.bash\_history”、“/var/log/messages”（如有）。

## URI<a name="zh-cn_topic_0118924584_section39702459"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924584_table50516043"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924584_row66861325"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924584_p47058244"><a name="zh-cn_topic_0118924584_p47058244"></a><a name="zh-cn_topic_0118924584_p47058244"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="84.85000000000001%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924584_p53621411"><a name="zh-cn_topic_0118924584_p53621411"></a><a name="zh-cn_topic_0118924584_p53621411"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924584_row48367059"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924584_p25417724"><a name="zh-cn_topic_0118924584_p25417724"></a><a name="zh-cn_topic_0118924584_p25417724"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="84.85000000000001%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924584_p45569733"><a name="zh-cn_topic_0118924584_p45569733"></a><a name="zh-cn_topic_0118924584_p45569733"></a>/v1.0/apigw/statistics/api/latest?api_id=[api_id]&amp;duration=[duration]</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924584_section21777819"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118924584_table160854"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924584_row30025489"><th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924584_p16145508"><a name="zh-cn_topic_0118924584_p16145508"></a><a name="zh-cn_topic_0118924584_p16145508"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924584_p32717809"><a name="zh-cn_topic_0118924584_p32717809"></a><a name="zh-cn_topic_0118924584_p32717809"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924584_p32896862"><a name="zh-cn_topic_0118924584_p32896862"></a><a name="zh-cn_topic_0118924584_p32896862"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924584_p47400147"><a name="zh-cn_topic_0118924584_p47400147"></a><a name="zh-cn_topic_0118924584_p47400147"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924584_row14206713"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p9893111"><a name="zh-cn_topic_0118924584_p9893111"></a><a name="zh-cn_topic_0118924584_p9893111"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p63144566"><a name="zh-cn_topic_0118924584_p63144566"></a><a name="zh-cn_topic_0118924584_p63144566"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p14436254"><a name="zh-cn_topic_0118924584_p14436254"></a><a name="zh-cn_topic_0118924584_p14436254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p28485910"><a name="zh-cn_topic_0118924584_p28485910"></a><a name="zh-cn_topic_0118924584_p28485910"></a>API的id</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row55046599"><td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p29589563"><a name="zh-cn_topic_0118924584_p29589563"></a><a name="zh-cn_topic_0118924584_p29589563"></a>duration</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p47944403"><a name="zh-cn_topic_0118924584_p47944403"></a><a name="zh-cn_topic_0118924584_p47944403"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p58291448"><a name="zh-cn_topic_0118924584_p58291448"></a><a name="zh-cn_topic_0118924584_p58291448"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p23986833"><a name="zh-cn_topic_0118924584_p23986833"></a><a name="zh-cn_topic_0118924584_p23986833"></a>最近统计时长，单位必须为h和m，比如1h和1m，分别代表最近1小时和最近1分钟</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0118924584_section19172900"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924584_table4240863"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924584_row18409318"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924584_p14759815"><a name="zh-cn_topic_0118924584_p14759815"></a><a name="zh-cn_topic_0118924584_p14759815"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924584_p54694405"><a name="zh-cn_topic_0118924584_p54694405"></a><a name="zh-cn_topic_0118924584_p54694405"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924584_p1061831"><a name="zh-cn_topic_0118924584_p1061831"></a><a name="zh-cn_topic_0118924584_p1061831"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924584_p18899510"><a name="zh-cn_topic_0118924584_p18899510"></a><a name="zh-cn_topic_0118924584_p18899510"></a>操作类型</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924584_row54465337"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p49616185"><a name="zh-cn_topic_0118924584_p49616185"></a><a name="zh-cn_topic_0118924584_p49616185"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p59488029"><a name="zh-cn_topic_0118924584_p59488029"></a><a name="zh-cn_topic_0118924584_p59488029"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p53801038"><a name="zh-cn_topic_0118924584_p53801038"></a><a name="zh-cn_topic_0118924584_p53801038"></a>响应码</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p62916787"><a name="zh-cn_topic_0118924584_p62916787"></a><a name="zh-cn_topic_0118924584_p62916787"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row29380172"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p30983771"><a name="zh-cn_topic_0118924584_p30983771"></a><a name="zh-cn_topic_0118924584_p30983771"></a>msg</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p26657555"><a name="zh-cn_topic_0118924584_p26657555"></a><a name="zh-cn_topic_0118924584_p26657555"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p11778331"><a name="zh-cn_topic_0118924584_p11778331"></a><a name="zh-cn_topic_0118924584_p11778331"></a>返回消息</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p14520731"><a name="zh-cn_topic_0118924584_p14520731"></a><a name="zh-cn_topic_0118924584_p14520731"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row63577720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p49521696"><a name="zh-cn_topic_0118924584_p49521696"></a><a name="zh-cn_topic_0118924584_p49521696"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p51834453"><a name="zh-cn_topic_0118924584_p51834453"></a><a name="zh-cn_topic_0118924584_p51834453"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p37841150"><a name="zh-cn_topic_0118924584_p37841150"></a><a name="zh-cn_topic_0118924584_p37841150"></a>开始时间的UTC的时间戳</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p45234308"><a name="zh-cn_topic_0118924584_p45234308"></a><a name="zh-cn_topic_0118924584_p45234308"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row4455589"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p25358400"><a name="zh-cn_topic_0118924584_p25358400"></a><a name="zh-cn_topic_0118924584_p25358400"></a>end_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p40764524"><a name="zh-cn_topic_0118924584_p40764524"></a><a name="zh-cn_topic_0118924584_p40764524"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p13592144"><a name="zh-cn_topic_0118924584_p13592144"></a><a name="zh-cn_topic_0118924584_p13592144"></a>截止时间的UTC的时间戳</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p27221909"><a name="zh-cn_topic_0118924584_p27221909"></a><a name="zh-cn_topic_0118924584_p27221909"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row43670595"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p47657340"><a name="zh-cn_topic_0118924584_p47657340"></a><a name="zh-cn_topic_0118924584_p47657340"></a>list</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p35039337"><a name="zh-cn_topic_0118924584_p35039337"></a><a name="zh-cn_topic_0118924584_p35039337"></a>结构体数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p19614067"><a name="zh-cn_topic_0118924584_p19614067"></a><a name="zh-cn_topic_0118924584_p19614067"></a>统计指标的数据结构结构体</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p45235585"><a name="zh-cn_topic_0118924584_p45235585"></a><a name="zh-cn_topic_0118924584_p45235585"></a>R</p>
</td>
</tr>
</tbody>
</table>

**表 4**  参数说明

<a name="zh-cn_topic_0118924584_table4467085"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924584_row59812800"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924584_p12998626"><a name="zh-cn_topic_0118924584_p12998626"></a><a name="zh-cn_topic_0118924584_p12998626"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924584_p46255772"><a name="zh-cn_topic_0118924584_p46255772"></a><a name="zh-cn_topic_0118924584_p46255772"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924584_p55730071"><a name="zh-cn_topic_0118924584_p55730071"></a><a name="zh-cn_topic_0118924584_p55730071"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924584_p17841915"><a name="zh-cn_topic_0118924584_p17841915"></a><a name="zh-cn_topic_0118924584_p17841915"></a>操作类型</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924584_row35908974"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p22945819"><a name="zh-cn_topic_0118924584_p22945819"></a><a name="zh-cn_topic_0118924584_p22945819"></a>cycle</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p46672040"><a name="zh-cn_topic_0118924584_p46672040"></a><a name="zh-cn_topic_0118924584_p46672040"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p22338877"><a name="zh-cn_topic_0118924584_p22338877"></a><a name="zh-cn_topic_0118924584_p22338877"></a>统计周期（预留）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p64618627"><a name="zh-cn_topic_0118924584_p64618627"></a><a name="zh-cn_topic_0118924584_p64618627"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row44696736"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p63665841"><a name="zh-cn_topic_0118924584_p63665841"></a><a name="zh-cn_topic_0118924584_p63665841"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p56659528"><a name="zh-cn_topic_0118924584_p56659528"></a><a name="zh-cn_topic_0118924584_p56659528"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p26019018"><a name="zh-cn_topic_0118924584_p26019018"></a><a name="zh-cn_topic_0118924584_p26019018"></a>API的id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p27165729"><a name="zh-cn_topic_0118924584_p27165729"></a><a name="zh-cn_topic_0118924584_p27165729"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row43164976"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p6702177"><a name="zh-cn_topic_0118924584_p6702177"></a><a name="zh-cn_topic_0118924584_p6702177"></a>current_minute</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p6005466"><a name="zh-cn_topic_0118924584_p6005466"></a><a name="zh-cn_topic_0118924584_p6005466"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p16680772"><a name="zh-cn_topic_0118924584_p16680772"></a><a name="zh-cn_topic_0118924584_p16680772"></a>API访问的UTC时间戳</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p8965319"><a name="zh-cn_topic_0118924584_p8965319"></a><a name="zh-cn_topic_0118924584_p8965319"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row13579009"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p26157915"><a name="zh-cn_topic_0118924584_p26157915"></a><a name="zh-cn_topic_0118924584_p26157915"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p38416353"><a name="zh-cn_topic_0118924584_p38416353"></a><a name="zh-cn_topic_0118924584_p38416353"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p24716925"><a name="zh-cn_topic_0118924584_p24716925"></a><a name="zh-cn_topic_0118924584_p24716925"></a>API的分组ID</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p55913876"><a name="zh-cn_topic_0118924584_p55913876"></a><a name="zh-cn_topic_0118924584_p55913876"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row33462842"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p26135704"><a name="zh-cn_topic_0118924584_p26135704"></a><a name="zh-cn_topic_0118924584_p26135704"></a>provider</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p36617254"><a name="zh-cn_topic_0118924584_p36617254"></a><a name="zh-cn_topic_0118924584_p36617254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p13207564"><a name="zh-cn_topic_0118924584_p13207564"></a><a name="zh-cn_topic_0118924584_p13207564"></a>API拥有者</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p63179763"><a name="zh-cn_topic_0118924584_p63179763"></a><a name="zh-cn_topic_0118924584_p63179763"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row31746958"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p21366809"><a name="zh-cn_topic_0118924584_p21366809"></a><a name="zh-cn_topic_0118924584_p21366809"></a>req_count</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p52989944"><a name="zh-cn_topic_0118924584_p52989944"></a><a name="zh-cn_topic_0118924584_p52989944"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p64327060"><a name="zh-cn_topic_0118924584_p64327060"></a><a name="zh-cn_topic_0118924584_p64327060"></a>请求总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p43109332"><a name="zh-cn_topic_0118924584_p43109332"></a><a name="zh-cn_topic_0118924584_p43109332"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row52439669"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p19754791"><a name="zh-cn_topic_0118924584_p19754791"></a><a name="zh-cn_topic_0118924584_p19754791"></a>max_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p56634225"><a name="zh-cn_topic_0118924584_p56634225"></a><a name="zh-cn_topic_0118924584_p56634225"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p23969532"><a name="zh-cn_topic_0118924584_p23969532"></a><a name="zh-cn_topic_0118924584_p23969532"></a>最大延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p62483952"><a name="zh-cn_topic_0118924584_p62483952"></a><a name="zh-cn_topic_0118924584_p62483952"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row25484656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p50991251"><a name="zh-cn_topic_0118924584_p50991251"></a><a name="zh-cn_topic_0118924584_p50991251"></a>avg_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p36650675"><a name="zh-cn_topic_0118924584_p36650675"></a><a name="zh-cn_topic_0118924584_p36650675"></a>Double</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p15914679"><a name="zh-cn_topic_0118924584_p15914679"></a><a name="zh-cn_topic_0118924584_p15914679"></a>平均耗时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p14020616"><a name="zh-cn_topic_0118924584_p14020616"></a><a name="zh-cn_topic_0118924584_p14020616"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row59076680"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p20481782"><a name="zh-cn_topic_0118924584_p20481782"></a><a name="zh-cn_topic_0118924584_p20481782"></a>max_backend_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p48411685"><a name="zh-cn_topic_0118924584_p48411685"></a><a name="zh-cn_topic_0118924584_p48411685"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p29032445"><a name="zh-cn_topic_0118924584_p29032445"></a><a name="zh-cn_topic_0118924584_p29032445"></a>最大后端延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p2817829"><a name="zh-cn_topic_0118924584_p2817829"></a><a name="zh-cn_topic_0118924584_p2817829"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row25360462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p40931570"><a name="zh-cn_topic_0118924584_p40931570"></a><a name="zh-cn_topic_0118924584_p40931570"></a>avg_backend_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p27122874"><a name="zh-cn_topic_0118924584_p27122874"></a><a name="zh-cn_topic_0118924584_p27122874"></a>Double</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p49469199"><a name="zh-cn_topic_0118924584_p49469199"></a><a name="zh-cn_topic_0118924584_p49469199"></a>平均后端延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p47582168"><a name="zh-cn_topic_0118924584_p47582168"></a><a name="zh-cn_topic_0118924584_p47582168"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row25586332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p59226991"><a name="zh-cn_topic_0118924584_p59226991"></a><a name="zh-cn_topic_0118924584_p59226991"></a>max_inner_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p32656938"><a name="zh-cn_topic_0118924584_p32656938"></a><a name="zh-cn_topic_0118924584_p32656938"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p27966326"><a name="zh-cn_topic_0118924584_p27966326"></a><a name="zh-cn_topic_0118924584_p27966326"></a>最大网关内部延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p50679930"><a name="zh-cn_topic_0118924584_p50679930"></a><a name="zh-cn_topic_0118924584_p50679930"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row53466193"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p35794397"><a name="zh-cn_topic_0118924584_p35794397"></a><a name="zh-cn_topic_0118924584_p35794397"></a>avg_inner_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p13665078"><a name="zh-cn_topic_0118924584_p13665078"></a><a name="zh-cn_topic_0118924584_p13665078"></a>Double</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p33129539"><a name="zh-cn_topic_0118924584_p33129539"></a><a name="zh-cn_topic_0118924584_p33129539"></a>平均网关内部延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p66247021"><a name="zh-cn_topic_0118924584_p66247021"></a><a name="zh-cn_topic_0118924584_p66247021"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row59352280"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p42805367"><a name="zh-cn_topic_0118924584_p42805367"></a><a name="zh-cn_topic_0118924584_p42805367"></a>output_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p44682727"><a name="zh-cn_topic_0118924584_p44682727"></a><a name="zh-cn_topic_0118924584_p44682727"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p62531152"><a name="zh-cn_topic_0118924584_p62531152"></a><a name="zh-cn_topic_0118924584_p62531152"></a>下行吞吐量（byte）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p31858521"><a name="zh-cn_topic_0118924584_p31858521"></a><a name="zh-cn_topic_0118924584_p31858521"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row18291233"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p5194877"><a name="zh-cn_topic_0118924584_p5194877"></a><a name="zh-cn_topic_0118924584_p5194877"></a>input_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p18131918"><a name="zh-cn_topic_0118924584_p18131918"></a><a name="zh-cn_topic_0118924584_p18131918"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p59399292"><a name="zh-cn_topic_0118924584_p59399292"></a><a name="zh-cn_topic_0118924584_p59399292"></a>上行吞吐量（byte）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p46613358"><a name="zh-cn_topic_0118924584_p46613358"></a><a name="zh-cn_topic_0118924584_p46613358"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row16867045"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p24053368"><a name="zh-cn_topic_0118924584_p24053368"></a><a name="zh-cn_topic_0118924584_p24053368"></a>req_count4xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p2165829"><a name="zh-cn_topic_0118924584_p2165829"></a><a name="zh-cn_topic_0118924584_p2165829"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p41214450"><a name="zh-cn_topic_0118924584_p41214450"></a><a name="zh-cn_topic_0118924584_p41214450"></a>4xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p50036135"><a name="zh-cn_topic_0118924584_p50036135"></a><a name="zh-cn_topic_0118924584_p50036135"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row47672037"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p36229754"><a name="zh-cn_topic_0118924584_p36229754"></a><a name="zh-cn_topic_0118924584_p36229754"></a>req_count5xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p48928939"><a name="zh-cn_topic_0118924584_p48928939"></a><a name="zh-cn_topic_0118924584_p48928939"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p3821154"><a name="zh-cn_topic_0118924584_p3821154"></a><a name="zh-cn_topic_0118924584_p3821154"></a>5xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p41078020"><a name="zh-cn_topic_0118924584_p41078020"></a><a name="zh-cn_topic_0118924584_p41078020"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row34157866"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p15323738"><a name="zh-cn_topic_0118924584_p15323738"></a><a name="zh-cn_topic_0118924584_p15323738"></a>req_count2xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p33263275"><a name="zh-cn_topic_0118924584_p33263275"></a><a name="zh-cn_topic_0118924584_p33263275"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p9970756"><a name="zh-cn_topic_0118924584_p9970756"></a><a name="zh-cn_topic_0118924584_p9970756"></a>2xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p2324942"><a name="zh-cn_topic_0118924584_p2324942"></a><a name="zh-cn_topic_0118924584_p2324942"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row20924485"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p17161723"><a name="zh-cn_topic_0118924584_p17161723"></a><a name="zh-cn_topic_0118924584_p17161723"></a>req_count_error</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p47922293"><a name="zh-cn_topic_0118924584_p47922293"></a><a name="zh-cn_topic_0118924584_p47922293"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p56500507"><a name="zh-cn_topic_0118924584_p56500507"></a><a name="zh-cn_topic_0118924584_p56500507"></a>错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p13138391"><a name="zh-cn_topic_0118924584_p13138391"></a><a name="zh-cn_topic_0118924584_p13138391"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row51136655"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p48428420"><a name="zh-cn_topic_0118924584_p48428420"></a><a name="zh-cn_topic_0118924584_p48428420"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p30387970"><a name="zh-cn_topic_0118924584_p30387970"></a><a name="zh-cn_topic_0118924584_p30387970"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p45506480"><a name="zh-cn_topic_0118924584_p45506480"></a><a name="zh-cn_topic_0118924584_p45506480"></a>记录时间（yyy-MM-dd HH:mm:ss）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p62146230"><a name="zh-cn_topic_0118924584_p62146230"></a><a name="zh-cn_topic_0118924584_p62146230"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row22445162"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p6118824"><a name="zh-cn_topic_0118924584_p6118824"></a><a name="zh-cn_topic_0118924584_p6118824"></a>req_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p25862739"><a name="zh-cn_topic_0118924584_p25862739"></a><a name="zh-cn_topic_0118924584_p25862739"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p14507090"><a name="zh-cn_topic_0118924584_p14507090"></a><a name="zh-cn_topic_0118924584_p14507090"></a>API请求时间（yyy-MM-dd HH:mm:ss）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p34223630"><a name="zh-cn_topic_0118924584_p34223630"></a><a name="zh-cn_topic_0118924584_p34223630"></a>R</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924584_row39577214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924584_p51637727"><a name="zh-cn_topic_0118924584_p51637727"></a><a name="zh-cn_topic_0118924584_p51637727"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924584_p21906353"><a name="zh-cn_topic_0118924584_p21906353"></a><a name="zh-cn_topic_0118924584_p21906353"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924584_p29584155"><a name="zh-cn_topic_0118924584_p29584155"></a><a name="zh-cn_topic_0118924584_p29584155"></a>状态-预留</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924584_p47506374"><a name="zh-cn_topic_0118924584_p47506374"></a><a name="zh-cn_topic_0118924584_p47506374"></a>R</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
    "code":"APIG.0000",
    "msg":"",
    "start_time":1524735000,
    "end_time":1524735000,
    "list":[
        {
            "api_id":"ae12b59fef2e4c6b8e01d44e98b738c0",
            "current_minute":1524735000,
            "group_id":"26463e4b2445415eabb55b2414012989",
            "provider":"d4ef919b31bd43d3927c5d46c71b68c4",
            "req_count":45,
            "max_latency":59,
            "avg_latency":2.53,
            "max_backend_latency":0,
            "avg_backend_latency":0,
            "max_inner_latency":59,
            "avg_inner_latency":2.53,
            "output_throughput":31815,
            "input_throughput":334474,
            "req_count4xx":0,
            "req_count5xx":0,
            "req_count2xx":45,
            "req_count_error":0,
            "register_time":"2018-04-26 17:30:48",
            "req_time":"2018-04-26 17:30:00",
            "status":1
        }
    ]
}

```

## 状态码<a name="zh-cn_topic_0118924584_section61782645"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924584_table7328321"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924584_row41686554"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924584_p21167734"><a name="zh-cn_topic_0118924584_p21167734"></a><a name="zh-cn_topic_0118924584_p21167734"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924584_p36864927"><a name="zh-cn_topic_0118924584_p36864927"></a><a name="zh-cn_topic_0118924584_p36864927"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924584_row33269116"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924584_p10443894"><a name="zh-cn_topic_0118924584_p10443894"></a><a name="zh-cn_topic_0118924584_p10443894"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924584_p40649076"><a name="zh-cn_topic_0118924584_p40649076"></a><a name="zh-cn_topic_0118924584_p40649076"></a>Query Success</p>
</td>
</tr>
</tbody>
</table>

