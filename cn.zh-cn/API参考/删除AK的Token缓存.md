# 删除AK的Token缓存<a name="apig-phapi-180713147"></a>

## 功能介绍<a name="section2242913143410"></a>

删除缓存的Token，需要指明哪些AK的Token需要被删除。

该接口为面向IAM开放的接口。

>![](public_sys-resources/icon-note.gif) **说明：**   
>为了安全起见，在服务器上使用curl命令调用接口查询信息后，需要清理历史操作记录，包括但不限于“\~/.bash\_history”、“/var/log/messages”（如有）。  

## URI<a name="section924281319348"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table7871154393511"></a>
<table><thead align="left"><tr id="row17871154343512"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p143670131345"><a name="p143670131345"></a><a name="p143670131345"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p63671913183410"><a name="p63671913183410"></a><a name="p63671913183410"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row1987114343515"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p636712137348"><a name="p636712137348"></a><a name="p636712137348"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p536701353414"><a name="p536701353414"></a><a name="p536701353414"></a>/native/token/{domain_id}/{user_id}/aks/{time}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table4851459153818"></a>
<table><thead align="left"><tr id="row1985259143813"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p12367713193420"><a name="p12367713193420"></a><a name="p12367713193420"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.689999999999998%" id="mcps1.2.5.1.2"><p id="p7367161316343"><a name="p7367161316343"></a><a name="p7367161316343"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.44%" id="mcps1.2.5.1.3"><p id="p93675133347"><a name="p93675133347"></a><a name="p93675133347"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.870000000000005%" id="mcps1.2.5.1.4"><p id="p836761317349"><a name="p836761317349"></a><a name="p836761317349"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7507182425213"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.870000000000005%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row11991182375212"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.870000000000005%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row18555915383"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p336731316340"><a name="p336731316340"></a><a name="p336731316340"></a>domain_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.2.5.1.2 "><p id="p736718137343"><a name="p736718137343"></a><a name="p736718137343"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.5.1.3 "><p id="p6367713143414"><a name="p6367713143414"></a><a name="p6367713143414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.870000000000005%" headers="mcps1.2.5.1.4 "><p id="p4367813143416"><a name="p4367813143416"></a><a name="p4367813143416"></a>租户ID。</p>
</td>
</tr>
<tr id="row985145963819"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p63679133340"><a name="p63679133340"></a><a name="p63679133340"></a>user_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.2.5.1.2 "><p id="p10367913203417"><a name="p10367913203417"></a><a name="p10367913203417"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.5.1.3 "><p id="p5367131312342"><a name="p5367131312342"></a><a name="p5367131312342"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.870000000000005%" headers="mcps1.2.5.1.4 "><p id="p15367121314345"><a name="p15367121314345"></a><a name="p15367121314345"></a>用户ID。</p>
</td>
</tr>
<tr id="row18511592389"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p11367151393413"><a name="p11367151393413"></a><a name="p11367151393413"></a>time</p>
</td>
<td class="cellrowborder" valign="top" width="19.689999999999998%" headers="mcps1.2.5.1.2 "><p id="p436716137342"><a name="p436716137342"></a><a name="p436716137342"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.44%" headers="mcps1.2.5.1.3 "><p id="p73671013193410"><a name="p73671013193410"></a><a name="p73671013193410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.870000000000005%" headers="mcps1.2.5.1.4 "><p id="p2367191333420"><a name="p2367191333420"></a><a name="p2367191333420"></a>过期时间，毫秒级别的UTC的时间戳。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section14272513203411"></a>

**表 3**  参数说明

<a name="table129205343371"></a>
<table><thead align="left"><tr id="row11920183410372"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p036741363412"><a name="p036741363412"></a><a name="p036741363412"></a><strong id="b10367713203415"><a name="b10367713203415"></a><a name="b10367713203415"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p12367171393414"><a name="p12367171393414"></a><a name="p12367171393414"></a><strong id="b13531125105610"><a name="b13531125105610"></a><a name="b13531125105610"></a>是否必选</strong></p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p7383513193413"><a name="p7383513193413"></a><a name="p7383513193413"></a><strong id="b53837136348"><a name="b53837136348"></a><a name="b53837136348"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p1338351318345"><a name="p1338351318345"></a><a name="p1338351318345"></a><strong id="b113833139349"><a name="b113833139349"></a><a name="b113833139349"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row149208347376"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1538361317348"><a name="p1538361317348"></a><a name="p1538361317348"></a>remove_aks</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p11383171319349"><a name="p11383171319349"></a><a name="p11383171319349"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p12383161318349"><a name="p12383161318349"></a><a name="p12383161318349"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p138381393410"><a name="p138381393410"></a><a name="p138381393410"></a>需要清除缓存的token的ak清单。</p>
</td>
</tr>
<tr id="row199201934113717"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p8383131333419"><a name="p8383131333419"></a><a name="p8383131333419"></a>available_aks</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p93831113183413"><a name="p93831113183413"></a><a name="p93831113183413"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p15383113113419"><a name="p15383113113419"></a><a name="p15383113113419"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1338391316349"><a name="p1338391316349"></a><a name="p1338391316349"></a>可以保留缓存的token的ak清单。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
curl -X DELETE --header 'Content-Type: application/json' --header 'Accept: application/json' --header 'X-Auth-Token: +VMXCx******7NK7Vw8=' -d '{"remove_aks":["FGDLYZHRLBJS0U7OH8FB","WI3VKVW0YJ1KZDPSQJED"],"available_aks":["IDGAP7TUF8Y43AEDJJNN"]}' 'https://localhost:8443/native/token/f4f4e49e1a6d4a3396073112576fac79/5e74d6c12fa54bdda519a7235eacf7b7/aks/1521771388684
```

## 响应消息<a name="section5289513183412"></a>

无

## 状态码<a name="section428919136345"></a>

**表 4**  返回消息说明

<a name="table16289101310345"></a>
<table><thead align="left"><tr id="row16383141315342"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p63835132342"><a name="p63835132342"></a><a name="p63835132342"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p93834136347"><a name="p93834136347"></a><a name="p93834136347"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row143831313153418"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3383713203410"><a name="p3383713203410"></a><a name="p3383713203410"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1038312131345"><a name="p1038312131345"></a><a name="p1038312131345"></a>No Content</p>
</td>
</tr>
<tr id="row183831813123410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p63836134346"><a name="p63836134346"></a><a name="p63836134346"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p7383131314342"><a name="p7383131314342"></a><a name="p7383131314342"></a>Bad Request</p>
</td>
</tr>
<tr id="row17383131310345"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p73831213143413"><a name="p73831213143413"></a><a name="p73831213143413"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p10383513163414"><a name="p10383513163414"></a><a name="p10383513163414"></a>Unauthorized</p>
</td>
</tr>
<tr id="row6383713103410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1938321319342"><a name="p1938321319342"></a><a name="p1938321319342"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1438361313340"><a name="p1438361313340"></a><a name="p1438361313340"></a>Forbidden</p>
</td>
</tr>
<tr id="row11383151333417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1383111316342"><a name="p1383111316342"></a><a name="p1383111316342"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

