# API统计信息查询<a name="apig-phapi-180713170"></a>

## 功能介绍<a name="section32025744"></a>

根据API的id和开始、截止时间查询API被调用的次数，统计周期可选分钟、小时和天。

>![](public_sys-resources/icon-note.gif) **说明：**   
>为了安全起见，在服务器上使用curl命令调用接口查询信息后，需要清理历史操作记录，包括但不限于“\~/.bash\_history”、“/var/log/messages”（如有）。  

## URI<a name="section19796243"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table808683"></a>
<table><thead align="left"><tr id="row2329171"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.3.1.1"><p id="p54445169"><a name="p54445169"></a><a name="p54445169"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="84.85000000000001%" id="mcps1.2.3.1.2"><p id="p47982608"><a name="p47982608"></a><a name="p47982608"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row61386072"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.3.1.1 "><p id="p6215920"><a name="p6215920"></a><a name="p6215920"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="84.85000000000001%" headers="mcps1.2.3.1.2 "><p id="p33727488"><a name="p33727488"></a><a name="p33727488"></a>/v1/{project_id}/apigw/instances/{instance_id}/statistics/api?api_id=[api_id]&amp;start_time=[start_time]&amp;end_time=[start_time]&amp;cycle=[cycle]</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section43948466"></a>

**表 2**  参数说明

<a name="table47572017"></a>
<table><thead align="left"><tr id="row30936794"><th class="cellrowborder" valign="top" width="16.491649164916492%" id="mcps1.2.5.1.1"><p id="p22852357"><a name="p22852357"></a><a name="p22852357"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="16.491649164916492%" id="mcps1.2.5.1.2"><p id="p39101633"><a name="p39101633"></a><a name="p39101633"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.491649164916492%" id="mcps1.2.5.1.3"><p id="p13115701"><a name="p13115701"></a><a name="p13115701"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.52505250525052%" id="mcps1.2.5.1.4"><p id="p55738890"><a name="p55738890"></a><a name="p55738890"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1643422019011"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.52505250525052%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row88160193019"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.52505250525052%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row18556264"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.1 "><p id="p26662390"><a name="p26662390"></a><a name="p26662390"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.2 "><p id="p12169948"><a name="p12169948"></a><a name="p12169948"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.3 "><p id="p46241731"><a name="p46241731"></a><a name="p46241731"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.52505250525052%" headers="mcps1.2.5.1.4 "><p id="p54592722"><a name="p54592722"></a><a name="p54592722"></a>API的id</p>
</td>
</tr>
<tr id="row21572457"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.1 "><p id="p2538568"><a name="p2538568"></a><a name="p2538568"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.2 "><p id="p4297444"><a name="p4297444"></a><a name="p4297444"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.3 "><p id="p12548644"><a name="p12548644"></a><a name="p12548644"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.52505250525052%" headers="mcps1.2.5.1.4 "><p id="p9807216"><a name="p9807216"></a><a name="p9807216"></a>查询的开始时间，格式为：yyyy-MM-dd HH:mm:ss</p>
</td>
</tr>
<tr id="row21156087"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.1 "><p id="p35921473"><a name="p35921473"></a><a name="p35921473"></a>end_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.2 "><p id="p23958220"><a name="p23958220"></a><a name="p23958220"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.3 "><p id="p61567680"><a name="p61567680"></a><a name="p61567680"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.52505250525052%" headers="mcps1.2.5.1.4 "><p id="p20926147"><a name="p20926147"></a><a name="p20926147"></a>查询的截止时间，格式为：yyyy-MM-dd HH:mm:ss</p>
</td>
</tr>
<tr id="row54117603"><td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.1 "><p id="p21449731"><a name="p21449731"></a><a name="p21449731"></a>cycle</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.2 "><p id="p59706631"><a name="p59706631"></a><a name="p59706631"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.491649164916492%" headers="mcps1.2.5.1.3 "><p id="p4398936"><a name="p4398936"></a><a name="p4398936"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.52505250525052%" headers="mcps1.2.5.1.4 "><p id="p20769501"><a name="p20769501"></a><a name="p20769501"></a>统计周期，包括分钟、小时、天。分别为：MINUTE、HOUR和DAY，默认为MINUTE。默认1小时内会返回分钟周期的数据、72小时内会返回统计周期为小时的数据、其他返回周期为天的数据</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
curl -X GET --header 'Accept: application/json'  --header 'X-Auth-Token: +VMXCx******7NK7Vw8=' 'https://localhost:8443/v1/{project_id}/apigw/instances/{instance_id}/statistics/api?api_id=dd954099-c6b7-484f-83a0-39928f4110e7&start_time=2017-10-19%2012%3A12%3A00&end_time=2017-12-19%2012%3A12%3A00'
```

## 响应消息<a name="section3055980"></a>

**表 3**  参数说明

<a name="table6355662"></a>
<table><thead align="left"><tr id="row25936518"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p20483219"><a name="p20483219"></a><a name="p20483219"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.2"><p id="p48528061"><a name="p48528061"></a><a name="p48528061"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.3"><p id="p38458859"><a name="p38458859"></a><a name="p38458859"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.4"><p id="p28159878"><a name="p28159878"></a><a name="p28159878"></a>操作类型</p>
</th>
</tr>
</thead>
<tbody><tr id="row66357621"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p6258209"><a name="p6258209"></a><a name="p6258209"></a>code</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p37152881"><a name="p37152881"></a><a name="p37152881"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p56593357"><a name="p56593357"></a><a name="p56593357"></a>响应码</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p20659230"><a name="p20659230"></a><a name="p20659230"></a>R</p>
</td>
</tr>
<tr id="row51715350"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p28193841"><a name="p28193841"></a><a name="p28193841"></a>msg</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p1999797"><a name="p1999797"></a><a name="p1999797"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p27765832"><a name="p27765832"></a><a name="p27765832"></a>返回消息</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p34439957"><a name="p34439957"></a><a name="p34439957"></a>R</p>
</td>
</tr>
<tr id="row41524160"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8013780"><a name="p8013780"></a><a name="p8013780"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p45136437"><a name="p45136437"></a><a name="p45136437"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p32172746"><a name="p32172746"></a><a name="p32172746"></a>开始时间的UTC的时间戳（预留）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p55855611"><a name="p55855611"></a><a name="p55855611"></a>R</p>
</td>
</tr>
<tr id="row32938458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p50769474"><a name="p50769474"></a><a name="p50769474"></a>end_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p18686714"><a name="p18686714"></a><a name="p18686714"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p37228842"><a name="p37228842"></a><a name="p37228842"></a>截止时间的UTC的时间戳（预留）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p62746235"><a name="p62746235"></a><a name="p62746235"></a>R</p>
</td>
</tr>
<tr id="row27845207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p40869308"><a name="p40869308"></a><a name="p40869308"></a>list</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p22079637"><a name="p22079637"></a><a name="p22079637"></a>结构体数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p43620171"><a name="p43620171"></a><a name="p43620171"></a>统计指标的数据结构结构体</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p43572933"><a name="p43572933"></a><a name="p43572933"></a>R</p>
</td>
</tr>
</tbody>
</table>

**表 4**  参数说明

<a name="table56612079"></a>
<table><thead align="left"><tr id="row16926674"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p28883328"><a name="p28883328"></a><a name="p28883328"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.2"><p id="p57848198"><a name="p57848198"></a><a name="p57848198"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="30%" id="mcps1.2.5.1.3"><p id="p55192461"><a name="p55192461"></a><a name="p55192461"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.4"><p id="p41404348"><a name="p41404348"></a><a name="p41404348"></a>操作类型</p>
</th>
</tr>
</thead>
<tbody><tr id="row65417916"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p64359861"><a name="p64359861"></a><a name="p64359861"></a>cycle</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p45766222"><a name="p45766222"></a><a name="p45766222"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p16076463"><a name="p16076463"></a><a name="p16076463"></a>统计周期（预留）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p27125121"><a name="p27125121"></a><a name="p27125121"></a>R</p>
</td>
</tr>
<tr id="row42799499"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p44207433"><a name="p44207433"></a><a name="p44207433"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p24032331"><a name="p24032331"></a><a name="p24032331"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p461818"><a name="p461818"></a><a name="p461818"></a>api的id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p37407293"><a name="p37407293"></a><a name="p37407293"></a>R</p>
</td>
</tr>
<tr id="row1121322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p23718247"><a name="p23718247"></a><a name="p23718247"></a>current_minute</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p42129836"><a name="p42129836"></a><a name="p42129836"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p57073570"><a name="p57073570"></a><a name="p57073570"></a>API访问的UTC时间戳</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p59556464"><a name="p59556464"></a><a name="p59556464"></a>R</p>
</td>
</tr>
<tr id="row66246136"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p64336831"><a name="p64336831"></a><a name="p64336831"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p43900785"><a name="p43900785"></a><a name="p43900785"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p66302712"><a name="p66302712"></a><a name="p66302712"></a>API的分组ID</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p1810620"><a name="p1810620"></a><a name="p1810620"></a>R</p>
</td>
</tr>
<tr id="row16295584"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p44873929"><a name="p44873929"></a><a name="p44873929"></a>provider</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p10909667"><a name="p10909667"></a><a name="p10909667"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p11267862"><a name="p11267862"></a><a name="p11267862"></a>API拥有者</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p40281609"><a name="p40281609"></a><a name="p40281609"></a>R</p>
</td>
</tr>
<tr id="row26990162"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p38719496"><a name="p38719496"></a><a name="p38719496"></a>req_count</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p49271508"><a name="p49271508"></a><a name="p49271508"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p31569179"><a name="p31569179"></a><a name="p31569179"></a>请求总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p6966727"><a name="p6966727"></a><a name="p6966727"></a>R</p>
</td>
</tr>
<tr id="row62700551"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p45579845"><a name="p45579845"></a><a name="p45579845"></a>max_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p979931"><a name="p979931"></a><a name="p979931"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p12265586"><a name="p12265586"></a><a name="p12265586"></a>最大延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p53988401"><a name="p53988401"></a><a name="p53988401"></a>R</p>
</td>
</tr>
<tr id="row16133568"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p31750607"><a name="p31750607"></a><a name="p31750607"></a>avg_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p21662363"><a name="p21662363"></a><a name="p21662363"></a>Double</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p9820939"><a name="p9820939"></a><a name="p9820939"></a>平均耗时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p57298567"><a name="p57298567"></a><a name="p57298567"></a>R</p>
</td>
</tr>
<tr id="row45925062"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p28942528"><a name="p28942528"></a><a name="p28942528"></a>max_backend_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p62643451"><a name="p62643451"></a><a name="p62643451"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p40954783"><a name="p40954783"></a><a name="p40954783"></a>最大后端延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p29003090"><a name="p29003090"></a><a name="p29003090"></a>R</p>
</td>
</tr>
<tr id="row59701226"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3961146"><a name="p3961146"></a><a name="p3961146"></a>avg_backend_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p52417390"><a name="p52417390"></a><a name="p52417390"></a>double</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p17950191"><a name="p17950191"></a><a name="p17950191"></a>平均后端延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p44679332"><a name="p44679332"></a><a name="p44679332"></a>R</p>
</td>
</tr>
<tr id="row66569669"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p23434148"><a name="p23434148"></a><a name="p23434148"></a>max_inner_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p19117868"><a name="p19117868"></a><a name="p19117868"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p5043460"><a name="p5043460"></a><a name="p5043460"></a>最大网关内部延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p5867092"><a name="p5867092"></a><a name="p5867092"></a>R</p>
</td>
</tr>
<tr id="row52803833"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p49252081"><a name="p49252081"></a><a name="p49252081"></a>avg_inner_latency</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p29995638"><a name="p29995638"></a><a name="p29995638"></a>Double</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p13727599"><a name="p13727599"></a><a name="p13727599"></a>平均网关内部延时</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p38193733"><a name="p38193733"></a><a name="p38193733"></a>R</p>
</td>
</tr>
<tr id="row8199278"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p60161753"><a name="p60161753"></a><a name="p60161753"></a>output_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p41263829"><a name="p41263829"></a><a name="p41263829"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p54035849"><a name="p54035849"></a><a name="p54035849"></a>下行吞吐量（byte）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p14827678"><a name="p14827678"></a><a name="p14827678"></a>R</p>
</td>
</tr>
<tr id="row66340244"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p4850717"><a name="p4850717"></a><a name="p4850717"></a>input_throughput</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p57363802"><a name="p57363802"></a><a name="p57363802"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p15956404"><a name="p15956404"></a><a name="p15956404"></a>上行吞吐量（byte）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p17400338"><a name="p17400338"></a><a name="p17400338"></a>R</p>
</td>
</tr>
<tr id="row22385318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1271494"><a name="p1271494"></a><a name="p1271494"></a>req_count4xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p35882207"><a name="p35882207"></a><a name="p35882207"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p20777624"><a name="p20777624"></a><a name="p20777624"></a>4xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p5265945"><a name="p5265945"></a><a name="p5265945"></a>R</p>
</td>
</tr>
<tr id="row47393508"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13668965"><a name="p13668965"></a><a name="p13668965"></a>req_count5xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p33444419"><a name="p33444419"></a><a name="p33444419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p24643429"><a name="p24643429"></a><a name="p24643429"></a>5xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p49960756"><a name="p49960756"></a><a name="p49960756"></a>R</p>
</td>
</tr>
<tr id="row46993623"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p48387156"><a name="p48387156"></a><a name="p48387156"></a>req_count2xx</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p27045553"><a name="p27045553"></a><a name="p27045553"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p43206166"><a name="p43206166"></a><a name="p43206166"></a>2xx响应码总次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p10038572"><a name="p10038572"></a><a name="p10038572"></a>R</p>
</td>
</tr>
<tr id="row23238289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3253234"><a name="p3253234"></a><a name="p3253234"></a>req_count_error</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p62185433"><a name="p62185433"></a><a name="p62185433"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p3855275"><a name="p3855275"></a><a name="p3855275"></a>错误次数</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p43841874"><a name="p43841874"></a><a name="p43841874"></a>R</p>
</td>
</tr>
<tr id="row59032553"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p16907498"><a name="p16907498"></a><a name="p16907498"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p27330099"><a name="p27330099"></a><a name="p27330099"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p66254445"><a name="p66254445"></a><a name="p66254445"></a>记录时间（yyy-MM-dd HH:mm:ss）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p65009856"><a name="p65009856"></a><a name="p65009856"></a>R</p>
</td>
</tr>
<tr id="row48217794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13327212"><a name="p13327212"></a><a name="p13327212"></a>req_time</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p5762370"><a name="p5762370"></a><a name="p5762370"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p64098862"><a name="p64098862"></a><a name="p64098862"></a>API请求时间（yyy-MM-dd HH:mm:ss）</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p24625301"><a name="p24625301"></a><a name="p24625301"></a>R</p>
</td>
</tr>
<tr id="row20301123"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p33778289"><a name="p33778289"></a><a name="p33778289"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.2 "><p id="p51686863"><a name="p51686863"></a><a name="p51686863"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30%" headers="mcps1.2.5.1.3 "><p id="p25886341"><a name="p25886341"></a><a name="p25886341"></a>状态-预留</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.4 "><p id="p16418876"><a name="p16418876"></a><a name="p16418876"></a>R</p>
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

## 状态码<a name="section59991876"></a>

**表 5**  返回消息说明

<a name="table37703589"></a>
<table><thead align="left"><tr id="row2664002"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p14457610"><a name="p14457610"></a><a name="p14457610"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p30215775"><a name="p30215775"></a><a name="p30215775"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row31558696"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6117582"><a name="p6117582"></a><a name="p6117582"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p25762104"><a name="p25762104"></a><a name="p25762104"></a>Query Success</p>
</td>
</tr>
</tbody>
</table>

