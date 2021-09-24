# 批量导出API<a name="ZH-CN_TOPIC_0000001082135225"></a>

## 功能介绍<a name="zh-cn_topic_0225569012_section39777523194"></a>

按API ID列表批量导出指定分组、指定环境中发布的API的基础/全量/扩展Swagger定义。

## URI<a name="zh-cn_topic_0225569012_section1199919551442"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1** 

<a name="zh-cn_topic_0225569012_table1030719520475"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row1130715217477"><th class="cellrowborder" valign="top" width="20.57%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569012_p130795213478"><a name="zh-cn_topic_0225569012_p130795213478"></a><a name="zh-cn_topic_0225569012_p130795213478"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="79.43%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569012_p13307135204712"><a name="zh-cn_topic_0225569012_p13307135204712"></a><a name="zh-cn_topic_0225569012_p13307135204712"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row15307252144718"><td class="cellrowborder" valign="top" width="20.57%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569012_p1930714525475"><a name="zh-cn_topic_0225569012_p1930714525475"></a><a name="zh-cn_topic_0225569012_p1930714525475"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="79.43%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569012_p19454226101515"><a name="zh-cn_topic_0225569012_p19454226101515"></a><a name="zh-cn_topic_0225569012_p19454226101515"></a>/v1/{project_id}/apigw/instances/{instance_id}/openapi/apis?env_id={0}&amp;define={2}&amp;version={3}&amp;type={4}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225569012_table871144945810"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row14734499589"><th class="cellrowborder" valign="top" width="18.13181318131813%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p1973174918589"><a name="zh-cn_topic_0225569012_p1973174918589"></a><a name="zh-cn_topic_0225569012_p1973174918589"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.511351135113511%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p4731749125817"><a name="zh-cn_topic_0225569012_p4731749125817"></a><a name="zh-cn_topic_0225569012_p4731749125817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.781778177817785%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p1730491589"><a name="zh-cn_topic_0225569012_p1730491589"></a><a name="zh-cn_topic_0225569012_p1730491589"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="50.57505750575058%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1073649175817"><a name="zh-cn_topic_0225569012_p1073649175817"></a><a name="zh-cn_topic_0225569012_p1073649175817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row4617113412519"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p55878963"><a name="zh-cn_topic_0225569012_p55878963"></a><a name="zh-cn_topic_0225569012_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.511351135113511%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p29902160"><a name="zh-cn_topic_0225569012_p29902160"></a><a name="zh-cn_topic_0225569012_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.781778177817785%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p6155914"><a name="zh-cn_topic_0225569012_p6155914"></a><a name="zh-cn_topic_0225569012_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.57505750575058%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p28867016"><a name="zh-cn_topic_0225569012_p28867016"></a><a name="zh-cn_topic_0225569012_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row56321031053"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1780913159538"><a name="zh-cn_topic_0225569012_p1780913159538"></a><a name="zh-cn_topic_0225569012_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.511351135113511%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p9809215115310"><a name="zh-cn_topic_0225569012_p9809215115310"></a><a name="zh-cn_topic_0225569012_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.781778177817785%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1280914152538"><a name="zh-cn_topic_0225569012_p1280914152538"></a><a name="zh-cn_topic_0225569012_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.57505750575058%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1880914157537"><a name="zh-cn_topic_0225569012_p1880914157537"></a><a name="zh-cn_topic_0225569012_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row87315493588"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p823317911818"><a name="zh-cn_topic_0225569012_p823317911818"></a><a name="zh-cn_topic_0225569012_p823317911818"></a>env_id/env</p>
</td>
<td class="cellrowborder" valign="top" width="13.511351135113511%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p52331931812"><a name="zh-cn_topic_0225569012_p52331931812"></a><a name="zh-cn_topic_0225569012_p52331931812"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.781778177817785%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8233696183"><a name="zh-cn_topic_0225569012_p8233696183"></a><a name="zh-cn_topic_0225569012_p8233696183"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.57505750575058%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p14233692182"><a name="zh-cn_topic_0225569012_p14233692182"></a><a name="zh-cn_topic_0225569012_p14233692182"></a>API分组发布的环境ID，目前支持env_id和env，两个均存在时以env_id为准，建议使用env_id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row67415491585"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p83064412117"><a name="zh-cn_topic_0225569012_p83064412117"></a><a name="zh-cn_topic_0225569012_p83064412117"></a>define</p>
</td>
<td class="cellrowborder" valign="top" width="13.511351135113511%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p3691511113"><a name="zh-cn_topic_0225569012_p3691511113"></a><a name="zh-cn_topic_0225569012_p3691511113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.781778177817785%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p6697511314"><a name="zh-cn_topic_0225569012_p6697511314"></a><a name="zh-cn_topic_0225569012_p6697511314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.57505750575058%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p294920378347"><a name="zh-cn_topic_0225569012_p294920378347"></a><a name="zh-cn_topic_0225569012_p294920378347"></a>导出API的定义范围：</p>
<a name="zh-cn_topic_0225569012_ul169331437173420"></a><a name="zh-cn_topic_0225569012_ul169331437173420"></a><ul id="zh-cn_topic_0225569012_ul169331437173420"><li>base：基础定义</li><li>full：全量定义</li><li>all：扩展定义</li></ul>
<p id="zh-cn_topic_0225569012_p184466500348"><a name="zh-cn_topic_0225569012_p184466500348"></a><a name="zh-cn_topic_0225569012_p184466500348"></a>默认为base</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row8723131211572"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p147231112105720"><a name="zh-cn_topic_0225569012_p147231112105720"></a><a name="zh-cn_topic_0225569012_p147231112105720"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.511351135113511%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p16723512135714"><a name="zh-cn_topic_0225569012_p16723512135714"></a><a name="zh-cn_topic_0225569012_p16723512135714"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.781778177817785%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8723712115711"><a name="zh-cn_topic_0225569012_p8723712115711"></a><a name="zh-cn_topic_0225569012_p8723712115711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.57505750575058%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1972317129578"><a name="zh-cn_topic_0225569012_p1972317129578"></a><a name="zh-cn_topic_0225569012_p1972317129578"></a>导出的API定义版本，默认为当前时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row14825155574"><td class="cellrowborder" valign="top" width="18.13181318131813%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p178210154576"><a name="zh-cn_topic_0225569012_p178210154576"></a><a name="zh-cn_topic_0225569012_p178210154576"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.511351135113511%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p68241555711"><a name="zh-cn_topic_0225569012_p68241555711"></a><a name="zh-cn_topic_0225569012_p68241555711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.781778177817785%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p4821315105719"><a name="zh-cn_topic_0225569012_p4821315105719"></a><a name="zh-cn_topic_0225569012_p4821315105719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="50.57505750575058%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p68281565719"><a name="zh-cn_topic_0225569012_p68281565719"></a><a name="zh-cn_topic_0225569012_p68281565719"></a>导出的API定义的格式：json/yaml，默认为json</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225569012_section178868115223"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225569012_table11428152"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row63593960"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p50837158"><a name="zh-cn_topic_0225569012_p50837158"></a><a name="zh-cn_topic_0225569012_p50837158"></a>参数位置</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p24169108"><a name="zh-cn_topic_0225569012_p24169108"></a><a name="zh-cn_topic_0225569012_p24169108"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p11540698"><a name="zh-cn_topic_0225569012_p11540698"></a><a name="zh-cn_topic_0225569012_p11540698"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p62381345"><a name="zh-cn_topic_0225569012_p62381345"></a><a name="zh-cn_topic_0225569012_p62381345"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row19724176"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p111152374516"><a name="zh-cn_topic_0225569012_p111152374516"></a><a name="zh-cn_topic_0225569012_p111152374516"></a>body</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p24434185"><a name="zh-cn_topic_0225569012_p24434185"></a><a name="zh-cn_topic_0225569012_p24434185"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p33011938"><a name="zh-cn_topic_0225569012_p33011938"></a><a name="zh-cn_topic_0225569012_p33011938"></a>String Array</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p56721283"><a name="zh-cn_topic_0225569012_p56721283"></a><a name="zh-cn_topic_0225569012_p56721283"></a>导出的API ID列表</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
["81efcfd94b8747a0b21e8c04144a4e8c","7addcd00cfab433984b1d8bf2fe08aaa"]
```

## 响应消息<a name="zh-cn_topic_0225569012_section526345615258"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225569012_table1572222154819"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row4722162124812"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p14494181014915"><a name="zh-cn_topic_0225569012_p14494181014915"></a><a name="zh-cn_topic_0225569012_p14494181014915"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p14257165012297"><a name="zh-cn_topic_0225569012_p14257165012297"></a><a name="zh-cn_topic_0225569012_p14257165012297"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p449481014494"><a name="zh-cn_topic_0225569012_p449481014494"></a><a name="zh-cn_topic_0225569012_p449481014494"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.44554455445545%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p0494191044917"><a name="zh-cn_topic_0225569012_p0494191044917"></a><a name="zh-cn_topic_0225569012_p0494191044917"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row5722921144812"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p74205913314"><a name="zh-cn_topic_0225569012_p74205913314"></a><a name="zh-cn_topic_0225569012_p74205913314"></a>swagger</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p10257175042917"><a name="zh-cn_topic_0225569012_p10257175042917"></a><a name="zh-cn_topic_0225569012_p10257175042917"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p042059436"><a name="zh-cn_topic_0225569012_p042059436"></a><a name="zh-cn_topic_0225569012_p042059436"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p242019919316"><a name="zh-cn_topic_0225569012_p242019919316"></a><a name="zh-cn_topic_0225569012_p242019919316"></a>固定值2.0</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row07221521144814"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p14201792310"><a name="zh-cn_topic_0225569012_p14201792310"></a><a name="zh-cn_topic_0225569012_p14201792310"></a>info</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1125735017292"><a name="zh-cn_topic_0225569012_p1125735017292"></a><a name="zh-cn_topic_0225569012_p1125735017292"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8420129035"><a name="zh-cn_topic_0225569012_p8420129035"></a><a name="zh-cn_topic_0225569012_p8420129035"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p5420591034"><a name="zh-cn_topic_0225569012_p5420591034"></a><a name="zh-cn_topic_0225569012_p5420591034"></a>参考<a href="#zh-cn_topic_0225569012_table17635735113614">表5</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row127225216483"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p154206914311"><a name="zh-cn_topic_0225569012_p154206914311"></a><a name="zh-cn_topic_0225569012_p154206914311"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p82576501291"><a name="zh-cn_topic_0225569012_p82576501291"></a><a name="zh-cn_topic_0225569012_p82576501291"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p242049934"><a name="zh-cn_topic_0225569012_p242049934"></a><a name="zh-cn_topic_0225569012_p242049934"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1542012918312"><a name="zh-cn_topic_0225569012_p1542012918312"></a><a name="zh-cn_topic_0225569012_p1542012918312"></a>API分组绑定的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row87221121164818"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p14420497317"><a name="zh-cn_topic_0225569012_p14420497317"></a><a name="zh-cn_topic_0225569012_p14420497317"></a>paths</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p4257175016290"><a name="zh-cn_topic_0225569012_p4257175016290"></a><a name="zh-cn_topic_0225569012_p4257175016290"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p13420596313"><a name="zh-cn_topic_0225569012_p13420596313"></a><a name="zh-cn_topic_0225569012_p13420596313"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p84201891538"><a name="zh-cn_topic_0225569012_p84201891538"></a><a name="zh-cn_topic_0225569012_p84201891538"></a>参考<a href="#zh-cn_topic_0225569012_table56661941123610">表 paths参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row572310210483"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p5420494312"><a name="zh-cn_topic_0225569012_p5420494312"></a><a name="zh-cn_topic_0225569012_p5420494312"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p425715505299"><a name="zh-cn_topic_0225569012_p425715505299"></a><a name="zh-cn_topic_0225569012_p425715505299"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p7420159639"><a name="zh-cn_topic_0225569012_p7420159639"></a><a name="zh-cn_topic_0225569012_p7420159639"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p16420990317"><a name="zh-cn_topic_0225569012_p16420990317"></a><a name="zh-cn_topic_0225569012_p16420990317"></a>公用响应定义，可以被引用在{method}的操作中，参考<a href="#zh-cn_topic_0225569012_table2199124914459">表10</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row10641458154212"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p176455814213"><a name="zh-cn_topic_0225569012_p176455814213"></a><a name="zh-cn_topic_0225569012_p176455814213"></a>securityDefinitions</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p116435813429"><a name="zh-cn_topic_0225569012_p116435813429"></a><a name="zh-cn_topic_0225569012_p116435813429"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1164145814216"><a name="zh-cn_topic_0225569012_p1164145814216"></a><a name="zh-cn_topic_0225569012_p1164145814216"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p146415586424"><a name="zh-cn_topic_0225569012_p146415586424"></a><a name="zh-cn_topic_0225569012_p146415586424"></a>定义鉴权方式，参考<a href="#zh-cn_topic_0225569012_table20400943104516">表14</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row263503512294"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p9635103514291"><a name="zh-cn_topic_0225569012_p9635103514291"></a><a name="zh-cn_topic_0225569012_p9635103514291"></a>x-apigateway-access-controls</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p16635935122917"><a name="zh-cn_topic_0225569012_p16635935122917"></a><a name="zh-cn_topic_0225569012_p16635935122917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1763513572916"><a name="zh-cn_topic_0225569012_p1763513572916"></a><a name="zh-cn_topic_0225569012_p1763513572916"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1635163582912"><a name="zh-cn_topic_0225569012_p1635163582912"></a><a name="zh-cn_topic_0225569012_p1635163582912"></a>访问控制信息，参考<a href="#zh-cn_topic_0225569012_table1621715417575">表 x-apigateway-access-controls参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row97293812293"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1772193872915"><a name="zh-cn_topic_0225569012_p1772193872915"></a><a name="zh-cn_topic_0225569012_p1772193872915"></a>x-apigateway-ratelimits</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1772203810299"><a name="zh-cn_topic_0225569012_p1772203810299"></a><a name="zh-cn_topic_0225569012_p1772203810299"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p12728382294"><a name="zh-cn_topic_0225569012_p12728382294"></a><a name="zh-cn_topic_0225569012_p12728382294"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p4721738182920"><a name="zh-cn_topic_0225569012_p4721738182920"></a><a name="zh-cn_topic_0225569012_p4721738182920"></a>流量空时信息，参考<a href="#zh-cn_topic_0225569012_table18116161025717">表 x-apigateway-ratelimits参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 5**  info参数说明

<a name="zh-cn_topic_0225569012_table17635735113614"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row9651163533614"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p136511035153614"><a name="zh-cn_topic_0225569012_p136511035153614"></a><a name="zh-cn_topic_0225569012_p136511035153614"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p1565133583617"><a name="zh-cn_topic_0225569012_p1565133583617"></a><a name="zh-cn_topic_0225569012_p1565133583617"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p5651173513362"><a name="zh-cn_topic_0225569012_p5651173513362"></a><a name="zh-cn_topic_0225569012_p5651173513362"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1765113543613"><a name="zh-cn_topic_0225569012_p1765113543613"></a><a name="zh-cn_topic_0225569012_p1765113543613"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row56668359364"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p106663354365"><a name="zh-cn_topic_0225569012_p106663354365"></a><a name="zh-cn_topic_0225569012_p106663354365"></a>title</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p7666153510362"><a name="zh-cn_topic_0225569012_p7666153510362"></a><a name="zh-cn_topic_0225569012_p7666153510362"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8666035123619"><a name="zh-cn_topic_0225569012_p8666035123619"></a><a name="zh-cn_topic_0225569012_p8666035123619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p136821357361"><a name="zh-cn_topic_0225569012_p136821357361"></a><a name="zh-cn_topic_0225569012_p136821357361"></a>API分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row8682103583613"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p268213563618"><a name="zh-cn_topic_0225569012_p268213563618"></a><a name="zh-cn_topic_0225569012_p268213563618"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p176821535183610"><a name="zh-cn_topic_0225569012_p176821535183610"></a><a name="zh-cn_topic_0225569012_p176821535183610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p168212359362"><a name="zh-cn_topic_0225569012_p168212359362"></a><a name="zh-cn_topic_0225569012_p168212359362"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p19682435173612"><a name="zh-cn_topic_0225569012_p19682435173612"></a><a name="zh-cn_topic_0225569012_p19682435173612"></a>版本号，用户输入自定义版本号或者使用默认的当前时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row179491349114015"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p5949849114012"><a name="zh-cn_topic_0225569012_p5949849114012"></a><a name="zh-cn_topic_0225569012_p5949849114012"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p494984944010"><a name="zh-cn_topic_0225569012_p494984944010"></a><a name="zh-cn_topic_0225569012_p494984944010"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p179495498402"><a name="zh-cn_topic_0225569012_p179495498402"></a><a name="zh-cn_topic_0225569012_p179495498402"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p209496493407"><a name="zh-cn_topic_0225569012_p209496493407"></a><a name="zh-cn_topic_0225569012_p209496493407"></a>分组描述信息</p>
</td>
</tr>
</tbody>
</table>

**表 6**  paths参数说明

<a name="zh-cn_topic_0225569012_table56661941123610"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row6682441163619"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p568214112369"><a name="zh-cn_topic_0225569012_p568214112369"></a><a name="zh-cn_topic_0225569012_p568214112369"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p2068214115369"><a name="zh-cn_topic_0225569012_p2068214115369"></a><a name="zh-cn_topic_0225569012_p2068214115369"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p5698144153619"><a name="zh-cn_topic_0225569012_p5698144153619"></a><a name="zh-cn_topic_0225569012_p5698144153619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p169834114367"><a name="zh-cn_topic_0225569012_p169834114367"></a><a name="zh-cn_topic_0225569012_p169834114367"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row1069854117364"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p126983416366"><a name="zh-cn_topic_0225569012_p126983416366"></a><a name="zh-cn_topic_0225569012_p126983416366"></a>uri</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p57123417365"><a name="zh-cn_topic_0225569012_p57123417365"></a><a name="zh-cn_topic_0225569012_p57123417365"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1271274123617"><a name="zh-cn_topic_0225569012_p1271274123617"></a><a name="zh-cn_topic_0225569012_p1271274123617"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p9712164143610"><a name="zh-cn_topic_0225569012_p9712164143610"></a><a name="zh-cn_topic_0225569012_p9712164143610"></a>API访问地址，参考<a href="#zh-cn_topic_0225569012_table683442044912">表7</a></p>
</td>
</tr>
</tbody>
</table>

**表 7**  uri参数说明

<a name="zh-cn_topic_0225569012_table683442044912"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row1586516201494"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p10865220114913"><a name="zh-cn_topic_0225569012_p10865220114913"></a><a name="zh-cn_topic_0225569012_p10865220114913"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p14865420134916"><a name="zh-cn_topic_0225569012_p14865420134916"></a><a name="zh-cn_topic_0225569012_p14865420134916"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p78811520104914"><a name="zh-cn_topic_0225569012_p78811520104914"></a><a name="zh-cn_topic_0225569012_p78811520104914"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p788132019493"><a name="zh-cn_topic_0225569012_p788132019493"></a><a name="zh-cn_topic_0225569012_p788132019493"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row19881520164910"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p17896420144917"><a name="zh-cn_topic_0225569012_p17896420144917"></a><a name="zh-cn_topic_0225569012_p17896420144917"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p108961520104914"><a name="zh-cn_topic_0225569012_p108961520104914"></a><a name="zh-cn_topic_0225569012_p108961520104914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p12896720104910"><a name="zh-cn_topic_0225569012_p12896720104910"></a><a name="zh-cn_topic_0225569012_p12896720104910"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p10912132034910"><a name="zh-cn_topic_0225569012_p10912132034910"></a><a name="zh-cn_topic_0225569012_p10912132034910"></a>API访问方法，参考<a href="#zh-cn_topic_0225569012_table9653181810518">表8</a></p>
</td>
</tr>
</tbody>
</table>

**表 8**  method参数说明

<a name="zh-cn_topic_0225569012_table9653181810518"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row3685201811512"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p1570071814519"><a name="zh-cn_topic_0225569012_p1570071814519"></a><a name="zh-cn_topic_0225569012_p1570071814519"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p11700101811516"><a name="zh-cn_topic_0225569012_p11700101811516"></a><a name="zh-cn_topic_0225569012_p11700101811516"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p20716121895111"><a name="zh-cn_topic_0225569012_p20716121895111"></a><a name="zh-cn_topic_0225569012_p20716121895111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p0716518105114"><a name="zh-cn_topic_0225569012_p0716518105114"></a><a name="zh-cn_topic_0225569012_p0716518105114"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row104190398180"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p16420163910182"><a name="zh-cn_topic_0225569012_p16420163910182"></a><a name="zh-cn_topic_0225569012_p16420163910182"></a>operationId</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p4420103951819"><a name="zh-cn_topic_0225569012_p4420103951819"></a><a name="zh-cn_topic_0225569012_p4420103951819"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1420113991815"><a name="zh-cn_topic_0225569012_p1420113991815"></a><a name="zh-cn_topic_0225569012_p1420113991815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p194201939111810"><a name="zh-cn_topic_0225569012_p194201939111810"></a><a name="zh-cn_topic_0225569012_p194201939111810"></a>API的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row107164181517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1473241845115"><a name="zh-cn_topic_0225569012_p1473241845115"></a><a name="zh-cn_topic_0225569012_p1473241845115"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p18732161810518"><a name="zh-cn_topic_0225569012_p18732161810518"></a><a name="zh-cn_topic_0225569012_p18732161810518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p18747618155114"><a name="zh-cn_topic_0225569012_p18747618155114"></a><a name="zh-cn_topic_0225569012_p18747618155114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p974719181516"><a name="zh-cn_topic_0225569012_p974719181516"></a><a name="zh-cn_topic_0225569012_p974719181516"></a>API的描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row745316124521"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p10453151215523"><a name="zh-cn_topic_0225569012_p10453151215523"></a><a name="zh-cn_topic_0225569012_p10453151215523"></a>schemes</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p154535126524"><a name="zh-cn_topic_0225569012_p154535126524"></a><a name="zh-cn_topic_0225569012_p154535126524"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p18453191210526"><a name="zh-cn_topic_0225569012_p18453191210526"></a><a name="zh-cn_topic_0225569012_p18453191210526"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p5453121220523"><a name="zh-cn_topic_0225569012_p5453121220523"></a><a name="zh-cn_topic_0225569012_p5453121220523"></a>API的请求协议对象数组定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row103226238486"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p9216125044912"><a name="zh-cn_topic_0225569012_p9216125044912"></a><a name="zh-cn_topic_0225569012_p9216125044912"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p13216135064915"><a name="zh-cn_topic_0225569012_p13216135064915"></a><a name="zh-cn_topic_0225569012_p13216135064915"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p221645017492"><a name="zh-cn_topic_0225569012_p221645017492"></a><a name="zh-cn_topic_0225569012_p221645017492"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p92161450174913"><a name="zh-cn_topic_0225569012_p92161450174913"></a><a name="zh-cn_topic_0225569012_p92161450174913"></a>API标签对象数组定义</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row3151319125712"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p101551913579"><a name="zh-cn_topic_0225569012_p101551913579"></a><a name="zh-cn_topic_0225569012_p101551913579"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p8151419125717"><a name="zh-cn_topic_0225569012_p8151419125717"></a><a name="zh-cn_topic_0225569012_p8151419125717"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p4150192574"><a name="zh-cn_topic_0225569012_p4150192574"></a><a name="zh-cn_topic_0225569012_p4150192574"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p61581995717"><a name="zh-cn_topic_0225569012_p61581995717"></a><a name="zh-cn_topic_0225569012_p61581995717"></a>请求参数对象数组定义，参考<a href="#zh-cn_topic_0225569012_table96841643204513">表 前端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row108121288529"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1181222885217"><a name="zh-cn_topic_0225569012_p1181222885217"></a><a name="zh-cn_topic_0225569012_p1181222885217"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1812102811520"><a name="zh-cn_topic_0225569012_p1812102811520"></a><a name="zh-cn_topic_0225569012_p1812102811520"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p158121828195215"><a name="zh-cn_topic_0225569012_p158121828195215"></a><a name="zh-cn_topic_0225569012_p158121828195215"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1681242885218"><a name="zh-cn_topic_0225569012_p1681242885218"></a><a name="zh-cn_topic_0225569012_p1681242885218"></a>响应定义，参考<a href="#zh-cn_topic_0225569012_table2199124914459">表10</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row07827715207"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p37827792016"><a name="zh-cn_topic_0225569012_p37827792016"></a><a name="zh-cn_topic_0225569012_p37827792016"></a>security</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1778316712011"><a name="zh-cn_topic_0225569012_p1778316712011"></a><a name="zh-cn_topic_0225569012_p1778316712011"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p17833720206"><a name="zh-cn_topic_0225569012_p17833720206"></a><a name="zh-cn_topic_0225569012_p17833720206"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1978311762017"><a name="zh-cn_topic_0225569012_p1978311762017"></a><a name="zh-cn_topic_0225569012_p1978311762017"></a>API的认证类型对象数组定义，参考<a href="#zh-cn_topic_0225569012_table5546275362">表 security参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row15485171610202"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1348518161208"><a name="zh-cn_topic_0225569012_p1348518161208"></a><a name="zh-cn_topic_0225569012_p1348518161208"></a>x-apigateway-access-control</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1248561618201"><a name="zh-cn_topic_0225569012_p1248561618201"></a><a name="zh-cn_topic_0225569012_p1248561618201"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1648551662018"><a name="zh-cn_topic_0225569012_p1648551662018"></a><a name="zh-cn_topic_0225569012_p1648551662018"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p15485111662013"><a name="zh-cn_topic_0225569012_p15485111662013"></a><a name="zh-cn_topic_0225569012_p15485111662013"></a>API绑定的访问控制对象数组定义</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row13552843123117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p355316435319"><a name="zh-cn_topic_0225569012_p355316435319"></a><a name="zh-cn_topic_0225569012_p355316435319"></a>x-apigateway-backend</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p7553204317316"><a name="zh-cn_topic_0225569012_p7553204317316"></a><a name="zh-cn_topic_0225569012_p7553204317316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p0553114318310"><a name="zh-cn_topic_0225569012_p0553114318310"></a><a name="zh-cn_topic_0225569012_p0553114318310"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1555384333113"><a name="zh-cn_topic_0225569012_p1555384333113"></a><a name="zh-cn_topic_0225569012_p1555384333113"></a>API的后端信息，参考<a href="#zh-cn_topic_0225569012_table1399375061810">表 x-apigateway-backend参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row13319311576"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p0341231277"><a name="zh-cn_topic_0225569012_p0341231277"></a><a name="zh-cn_topic_0225569012_p0341231277"></a>x-apigateway-backend-policies</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p12340311715"><a name="zh-cn_topic_0225569012_p12340311715"></a><a name="zh-cn_topic_0225569012_p12340311715"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p23423113714"><a name="zh-cn_topic_0225569012_p23423113714"></a><a name="zh-cn_topic_0225569012_p23423113714"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p143412311879"><a name="zh-cn_topic_0225569012_p143412311879"></a><a name="zh-cn_topic_0225569012_p143412311879"></a>API的策略后端信息，参考<a href="#zh-cn_topic_0225569012_table1531411471794">表 x-apigateway-backend-policies参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row192755417314"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p199271354113110"><a name="zh-cn_topic_0225569012_p199271354113110"></a><a name="zh-cn_topic_0225569012_p199271354113110"></a>x-apigateway-cors</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p14927115412311"><a name="zh-cn_topic_0225569012_p14927115412311"></a><a name="zh-cn_topic_0225569012_p14927115412311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p17927054183117"><a name="zh-cn_topic_0225569012_p17927054183117"></a><a name="zh-cn_topic_0225569012_p17927054183117"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p129278547312"><a name="zh-cn_topic_0225569012_p129278547312"></a><a name="zh-cn_topic_0225569012_p129278547312"></a>是否支持跨域</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1121618116329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p821681133220"><a name="zh-cn_topic_0225569012_p821681133220"></a><a name="zh-cn_topic_0225569012_p821681133220"></a>x-apigateway-match-mode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1621610143211"><a name="zh-cn_topic_0225569012_p1621610143211"></a><a name="zh-cn_topic_0225569012_p1621610143211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1821691103220"><a name="zh-cn_topic_0225569012_p1821691103220"></a><a name="zh-cn_topic_0225569012_p1821691103220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p12216914321"><a name="zh-cn_topic_0225569012_p12216914321"></a><a name="zh-cn_topic_0225569012_p12216914321"></a>API的匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row850353143219"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1450314319327"><a name="zh-cn_topic_0225569012_p1450314319327"></a><a name="zh-cn_topic_0225569012_p1450314319327"></a>x-apigateway-ratelimit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p75031939327"><a name="zh-cn_topic_0225569012_p75031939327"></a><a name="zh-cn_topic_0225569012_p75031939327"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p55039310321"><a name="zh-cn_topic_0225569012_p55039310321"></a><a name="zh-cn_topic_0225569012_p55039310321"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p195042353215"><a name="zh-cn_topic_0225569012_p195042353215"></a><a name="zh-cn_topic_0225569012_p195042353215"></a>API绑定的流量控制名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row257683483213"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p45771534113212"><a name="zh-cn_topic_0225569012_p45771534113212"></a><a name="zh-cn_topic_0225569012_p45771534113212"></a>x-apigateway-request-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1157716346325"><a name="zh-cn_topic_0225569012_p1157716346325"></a><a name="zh-cn_topic_0225569012_p1157716346325"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p17577434183217"><a name="zh-cn_topic_0225569012_p17577434183217"></a><a name="zh-cn_topic_0225569012_p17577434183217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p3577153423216"><a name="zh-cn_topic_0225569012_p3577153423216"></a><a name="zh-cn_topic_0225569012_p3577153423216"></a>API的类型</p>
</td>
</tr>
</tbody>
</table>

**表 9**  前端parameters参数说明

<a name="zh-cn_topic_0225569012_table96841643204513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row66992043194515"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p14699134344514"><a name="zh-cn_topic_0225569012_p14699134344514"></a><a name="zh-cn_topic_0225569012_p14699134344514"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p14699343114516"><a name="zh-cn_topic_0225569012_p14699343114516"></a><a name="zh-cn_topic_0225569012_p14699343114516"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p127151543194511"><a name="zh-cn_topic_0225569012_p127151543194511"></a><a name="zh-cn_topic_0225569012_p127151543194511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p07150438452"><a name="zh-cn_topic_0225569012_p07150438452"></a><a name="zh-cn_topic_0225569012_p07150438452"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row8715134315456"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p7715143104515"><a name="zh-cn_topic_0225569012_p7715143104515"></a><a name="zh-cn_topic_0225569012_p7715143104515"></a>maximum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p117301943184518"><a name="zh-cn_topic_0225569012_p117301943184518"></a><a name="zh-cn_topic_0225569012_p117301943184518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p197307437456"><a name="zh-cn_topic_0225569012_p197307437456"></a><a name="zh-cn_topic_0225569012_p197307437456"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p13730104310458"><a name="zh-cn_topic_0225569012_p13730104310458"></a><a name="zh-cn_topic_0225569012_p13730104310458"></a>参数为数值类型时，最大参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row13730134313451"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p67467431458"><a name="zh-cn_topic_0225569012_p67467431458"></a><a name="zh-cn_topic_0225569012_p67467431458"></a>minimum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p147461943124519"><a name="zh-cn_topic_0225569012_p147461943124519"></a><a name="zh-cn_topic_0225569012_p147461943124519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1774614374513"><a name="zh-cn_topic_0225569012_p1774614374513"></a><a name="zh-cn_topic_0225569012_p1774614374513"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p14746184312456"><a name="zh-cn_topic_0225569012_p14746184312456"></a><a name="zh-cn_topic_0225569012_p14746184312456"></a>参数为数值类型时，最小参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row14828193310413"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p082893311412"><a name="zh-cn_topic_0225569012_p082893311412"></a><a name="zh-cn_topic_0225569012_p082893311412"></a>maxLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1782812331542"><a name="zh-cn_topic_0225569012_p1782812331542"></a><a name="zh-cn_topic_0225569012_p1782812331542"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p482833317419"><a name="zh-cn_topic_0225569012_p482833317419"></a><a name="zh-cn_topic_0225569012_p482833317419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p11828633240"><a name="zh-cn_topic_0225569012_p11828633240"></a><a name="zh-cn_topic_0225569012_p11828633240"></a>参数为字符串类型时，参数的最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row7832187517"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p18321987513"><a name="zh-cn_topic_0225569012_p18321987513"></a><a name="zh-cn_topic_0225569012_p18321987513"></a>minLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p168327812514"><a name="zh-cn_topic_0225569012_p168327812514"></a><a name="zh-cn_topic_0225569012_p168327812514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p4832681152"><a name="zh-cn_topic_0225569012_p4832681152"></a><a name="zh-cn_topic_0225569012_p4832681152"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1283208859"><a name="zh-cn_topic_0225569012_p1283208859"></a><a name="zh-cn_topic_0225569012_p1283208859"></a>参数为字符串类型时，参数的最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row13193916520"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p4383919515"><a name="zh-cn_topic_0225569012_p4383919515"></a><a name="zh-cn_topic_0225569012_p4383919515"></a>pattern</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p9311391520"><a name="zh-cn_topic_0225569012_p9311391520"></a><a name="zh-cn_topic_0225569012_p9311391520"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p12363918512"><a name="zh-cn_topic_0225569012_p12363918512"></a><a name="zh-cn_topic_0225569012_p12363918512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p331139359"><a name="zh-cn_topic_0225569012_p331139359"></a><a name="zh-cn_topic_0225569012_p331139359"></a>参数值为正则匹配表达式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row8585345656"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p185859453519"><a name="zh-cn_topic_0225569012_p185859453519"></a><a name="zh-cn_topic_0225569012_p185859453519"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1558517451052"><a name="zh-cn_topic_0225569012_p1558517451052"></a><a name="zh-cn_topic_0225569012_p1558517451052"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p2585114516518"><a name="zh-cn_topic_0225569012_p2585114516518"></a><a name="zh-cn_topic_0225569012_p2585114516518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p165856451053"><a name="zh-cn_topic_0225569012_p165856451053"></a><a name="zh-cn_topic_0225569012_p165856451053"></a>参数类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1169574817514"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p26951482516"><a name="zh-cn_topic_0225569012_p26951482516"></a><a name="zh-cn_topic_0225569012_p26951482516"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1769584810510"><a name="zh-cn_topic_0225569012_p1769584810510"></a><a name="zh-cn_topic_0225569012_p1769584810510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1569524811513"><a name="zh-cn_topic_0225569012_p1569524811513"></a><a name="zh-cn_topic_0225569012_p1569524811513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p76951248650"><a name="zh-cn_topic_0225569012_p76951248650"></a><a name="zh-cn_topic_0225569012_p76951248650"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row82578561453"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p3257115620516"><a name="zh-cn_topic_0225569012_p3257115620516"></a><a name="zh-cn_topic_0225569012_p3257115620516"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p325714561153"><a name="zh-cn_topic_0225569012_p325714561153"></a><a name="zh-cn_topic_0225569012_p325714561153"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1225725612517"><a name="zh-cn_topic_0225569012_p1225725612517"></a><a name="zh-cn_topic_0225569012_p1225725612517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p172572561853"><a name="zh-cn_topic_0225569012_p172572561853"></a><a name="zh-cn_topic_0225569012_p172572561853"></a>参数描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row861611131466"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1861691314615"><a name="zh-cn_topic_0225569012_p1861691314615"></a><a name="zh-cn_topic_0225569012_p1861691314615"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p10616113260"><a name="zh-cn_topic_0225569012_p10616113260"></a><a name="zh-cn_topic_0225569012_p10616113260"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p96167132069"><a name="zh-cn_topic_0225569012_p96167132069"></a><a name="zh-cn_topic_0225569012_p96167132069"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p156162131463"><a name="zh-cn_topic_0225569012_p156162131463"></a><a name="zh-cn_topic_0225569012_p156162131463"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row425719201066"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p625792018611"><a name="zh-cn_topic_0225569012_p625792018611"></a><a name="zh-cn_topic_0225569012_p625792018611"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p192571204615"><a name="zh-cn_topic_0225569012_p192571204615"></a><a name="zh-cn_topic_0225569012_p192571204615"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p4257132014618"><a name="zh-cn_topic_0225569012_p4257132014618"></a><a name="zh-cn_topic_0225569012_p4257132014618"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p10257132019611"><a name="zh-cn_topic_0225569012_p10257132019611"></a><a name="zh-cn_topic_0225569012_p10257132019611"></a>参数位置，支持path、header、query、formData、body</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row94454221362"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p44451422761"><a name="zh-cn_topic_0225569012_p44451422761"></a><a name="zh-cn_topic_0225569012_p44451422761"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1644515221861"><a name="zh-cn_topic_0225569012_p1644515221861"></a><a name="zh-cn_topic_0225569012_p1644515221861"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p174451622061"><a name="zh-cn_topic_0225569012_p174451622061"></a><a name="zh-cn_topic_0225569012_p174451622061"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p7445422469"><a name="zh-cn_topic_0225569012_p7445422469"></a><a name="zh-cn_topic_0225569012_p7445422469"></a>参数是否必需，参数位置为path时必需</p>
</td>
</tr>
</tbody>
</table>

**表 10**  responses参数说明

<a name="zh-cn_topic_0225569012_table2199124914459"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row1823034918452"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p3230154911454"><a name="zh-cn_topic_0225569012_p3230154911454"></a><a name="zh-cn_topic_0225569012_p3230154911454"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p723020492454"><a name="zh-cn_topic_0225569012_p723020492454"></a><a name="zh-cn_topic_0225569012_p723020492454"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p1923034919458"><a name="zh-cn_topic_0225569012_p1923034919458"></a><a name="zh-cn_topic_0225569012_p1923034919458"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p15246144913454"><a name="zh-cn_topic_0225569012_p15246144913454"></a><a name="zh-cn_topic_0225569012_p15246144913454"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row6246204964515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p82464491455"><a name="zh-cn_topic_0225569012_p82464491455"></a><a name="zh-cn_topic_0225569012_p82464491455"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p20246194910459"><a name="zh-cn_topic_0225569012_p20246194910459"></a><a name="zh-cn_topic_0225569012_p20246194910459"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8262149124511"><a name="zh-cn_topic_0225569012_p8262149124511"></a><a name="zh-cn_topic_0225569012_p8262149124511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p5181165718115"><a name="zh-cn_topic_0225569012_p5181165718115"></a><a name="zh-cn_topic_0225569012_p5181165718115"></a>缺省响应，描述未定义的响应码</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row132620499454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p726214910458"><a name="zh-cn_topic_0225569012_p726214910458"></a><a name="zh-cn_topic_0225569012_p726214910458"></a>status_code</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p7262144916451"><a name="zh-cn_topic_0225569012_p7262144916451"></a><a name="zh-cn_topic_0225569012_p7262144916451"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p102621049114516"><a name="zh-cn_topic_0225569012_p102621049114516"></a><a name="zh-cn_topic_0225569012_p102621049114516"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1918110576113"><a name="zh-cn_topic_0225569012_p1918110576113"></a><a name="zh-cn_topic_0225569012_p1918110576113"></a>响应状态码，值为响应对象，参考<a href="#zh-cn_topic_0225569012_table19651114094519">表12</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1774720508918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p774812501894"><a name="zh-cn_topic_0225569012_p774812501894"></a><a name="zh-cn_topic_0225569012_p774812501894"></a>x-apigateway-result-failure-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p474815020916"><a name="zh-cn_topic_0225569012_p474815020916"></a><a name="zh-cn_topic_0225569012_p474815020916"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p11749105017914"><a name="zh-cn_topic_0225569012_p11749105017914"></a><a name="zh-cn_topic_0225569012_p11749105017914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p14749750398"><a name="zh-cn_topic_0225569012_p14749750398"></a><a name="zh-cn_topic_0225569012_p14749750398"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row71795541897"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1117913541917"><a name="zh-cn_topic_0225569012_p1117913541917"></a><a name="zh-cn_topic_0225569012_p1117913541917"></a>x-apigateway-result-normal-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p517914541191"><a name="zh-cn_topic_0225569012_p517914541191"></a><a name="zh-cn_topic_0225569012_p517914541191"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p171791554493"><a name="zh-cn_topic_0225569012_p171791554493"></a><a name="zh-cn_topic_0225569012_p171791554493"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p111791154598"><a name="zh-cn_topic_0225569012_p111791154598"></a><a name="zh-cn_topic_0225569012_p111791154598"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
</tbody>
</table>

**表 11**  security参数说明

<a name="zh-cn_topic_0225569012_table5546275362"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row95592719367"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p555327163610"><a name="zh-cn_topic_0225569012_p555327163610"></a><a name="zh-cn_topic_0225569012_p555327163610"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p1155182713613"><a name="zh-cn_topic_0225569012_p1155182713613"></a><a name="zh-cn_topic_0225569012_p1155182713613"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p7551127153619"><a name="zh-cn_topic_0225569012_p7551127153619"></a><a name="zh-cn_topic_0225569012_p7551127153619"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1655527153612"><a name="zh-cn_topic_0225569012_p1655527153612"></a><a name="zh-cn_topic_0225569012_p1655527153612"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row85552713617"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p95502723610"><a name="zh-cn_topic_0225569012_p95502723610"></a><a name="zh-cn_topic_0225569012_p95502723610"></a>apig-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p115552743618"><a name="zh-cn_topic_0225569012_p115552743618"></a><a name="zh-cn_topic_0225569012_p115552743618"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p255027123613"><a name="zh-cn_topic_0225569012_p255027123613"></a><a name="zh-cn_topic_0225569012_p255027123613"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p055162753612"><a name="zh-cn_topic_0225569012_p055162753612"></a><a name="zh-cn_topic_0225569012_p055162753612"></a>API的认证类型对象数组定义，为空数组</p>
<p id="zh-cn_topic_0225569012_p6722101419557"><a name="zh-cn_topic_0225569012_p6722101419557"></a><a name="zh-cn_topic_0225569012_p6722101419557"></a>apig-auth-type支持：</p>
<a name="zh-cn_topic_0225569012_ul3401225145518"></a><a name="zh-cn_topic_0225569012_ul3401225145518"></a><ul id="zh-cn_topic_0225569012_ul3401225145518"><li>APP认证： apig-auth-app</li><li>IAM认证：apig-auth-iam</li><li>NONE：不填写</li></ul>
</td>
</tr>
</tbody>
</table>

**表 12**  status code参数说明

<a name="zh-cn_topic_0225569012_table19651114094519"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row8666040184514"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p1682640114511"><a name="zh-cn_topic_0225569012_p1682640114511"></a><a name="zh-cn_topic_0225569012_p1682640114511"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p15682114019454"><a name="zh-cn_topic_0225569012_p15682114019454"></a><a name="zh-cn_topic_0225569012_p15682114019454"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p12682340164519"><a name="zh-cn_topic_0225569012_p12682340164519"></a><a name="zh-cn_topic_0225569012_p12682340164519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p16682144074512"><a name="zh-cn_topic_0225569012_p16682144074512"></a><a name="zh-cn_topic_0225569012_p16682144074512"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row176971403455"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p469714405452"><a name="zh-cn_topic_0225569012_p469714405452"></a><a name="zh-cn_topic_0225569012_p469714405452"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p069724034518"><a name="zh-cn_topic_0225569012_p069724034518"></a><a name="zh-cn_topic_0225569012_p069724034518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p2697174044516"><a name="zh-cn_topic_0225569012_p2697174044516"></a><a name="zh-cn_topic_0225569012_p2697174044516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1910319151215"><a name="zh-cn_topic_0225569012_p1910319151215"></a><a name="zh-cn_topic_0225569012_p1910319151215"></a>响应描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row15713194017458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1871312409458"><a name="zh-cn_topic_0225569012_p1871312409458"></a><a name="zh-cn_topic_0225569012_p1871312409458"></a>schema</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1871344024513"><a name="zh-cn_topic_0225569012_p1871344024513"></a><a name="zh-cn_topic_0225569012_p1871344024513"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p6713640144513"><a name="zh-cn_topic_0225569012_p6713640144513"></a><a name="zh-cn_topic_0225569012_p6713640144513"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p810313161213"><a name="zh-cn_topic_0225569012_p810313161213"></a><a name="zh-cn_topic_0225569012_p810313161213"></a>响应正文定义，参考<a href="#zh-cn_topic_0225569012_table1642164217453">表13</a></p>
</td>
</tr>
</tbody>
</table>

**表 13**  schema参数说明

<a name="zh-cn_topic_0225569012_table1642164217453"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row956942204511"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p55611427454"><a name="zh-cn_topic_0225569012_p55611427454"></a><a name="zh-cn_topic_0225569012_p55611427454"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p65624215455"><a name="zh-cn_topic_0225569012_p65624215455"></a><a name="zh-cn_topic_0225569012_p65624215455"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p1472164254519"><a name="zh-cn_topic_0225569012_p1472164254519"></a><a name="zh-cn_topic_0225569012_p1472164254519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1972174211456"><a name="zh-cn_topic_0225569012_p1972174211456"></a><a name="zh-cn_topic_0225569012_p1972174211456"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row472194212458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p15721042124520"><a name="zh-cn_topic_0225569012_p15721042124520"></a><a name="zh-cn_topic_0225569012_p15721042124520"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1888114213455"><a name="zh-cn_topic_0225569012_p1888114213455"></a><a name="zh-cn_topic_0225569012_p1888114213455"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p188804210453"><a name="zh-cn_topic_0225569012_p188804210453"></a><a name="zh-cn_topic_0225569012_p188804210453"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p7181193121210"><a name="zh-cn_topic_0225569012_p7181193121210"></a><a name="zh-cn_topic_0225569012_p7181193121210"></a>BODY体描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row10881742194515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p288184213458"><a name="zh-cn_topic_0225569012_p288184213458"></a><a name="zh-cn_topic_0225569012_p288184213458"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p210417426451"><a name="zh-cn_topic_0225569012_p210417426451"></a><a name="zh-cn_topic_0225569012_p210417426451"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1710410427459"><a name="zh-cn_topic_0225569012_p1710410427459"></a><a name="zh-cn_topic_0225569012_p1710410427459"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p318143141216"><a name="zh-cn_topic_0225569012_p318143141216"></a><a name="zh-cn_topic_0225569012_p318143141216"></a>BODY体类型：FORM/STREAM（表单/字节流）</p>
</td>
</tr>
</tbody>
</table>

**表 14**  securityDefinitions参数说明

<a name="zh-cn_topic_0225569012_table20400943104516"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row15416154311455"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p18432164316459"><a name="zh-cn_topic_0225569012_p18432164316459"></a><a name="zh-cn_topic_0225569012_p18432164316459"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p14432543104514"><a name="zh-cn_topic_0225569012_p14432543104514"></a><a name="zh-cn_topic_0225569012_p14432543104514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p34329432455"><a name="zh-cn_topic_0225569012_p34329432455"></a><a name="zh-cn_topic_0225569012_p34329432455"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.46534653465347%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p143274314515"><a name="zh-cn_topic_0225569012_p143274314515"></a><a name="zh-cn_topic_0225569012_p143274314515"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row144487431456"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p19448043104514"><a name="zh-cn_topic_0225569012_p19448043104514"></a><a name="zh-cn_topic_0225569012_p19448043104514"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p14448204304512"><a name="zh-cn_topic_0225569012_p14448204304512"></a><a name="zh-cn_topic_0225569012_p14448204304512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p2448194316457"><a name="zh-cn_topic_0225569012_p2448194316457"></a><a name="zh-cn_topic_0225569012_p2448194316457"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="53.46534653465347%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p83222641215"><a name="zh-cn_topic_0225569012_p83222641215"></a><a name="zh-cn_topic_0225569012_p83222641215"></a>自定义鉴权方式名称，参考<a href="#zh-cn_topic_0225569012_table868104464512">表15</a></p>
</td>
</tr>
</tbody>
</table>

**表 15**  name参数说明

<a name="zh-cn_topic_0225569012_table868104464512"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row9698134415451"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p14698944114515"><a name="zh-cn_topic_0225569012_p14698944114515"></a><a name="zh-cn_topic_0225569012_p14698944114515"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p1969864464518"><a name="zh-cn_topic_0225569012_p1969864464518"></a><a name="zh-cn_topic_0225569012_p1969864464518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p137141944184517"><a name="zh-cn_topic_0225569012_p137141944184517"></a><a name="zh-cn_topic_0225569012_p137141944184517"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p871416443459"><a name="zh-cn_topic_0225569012_p871416443459"></a><a name="zh-cn_topic_0225569012_p871416443459"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row5714124415455"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1972913440459"><a name="zh-cn_topic_0225569012_p1972913440459"></a><a name="zh-cn_topic_0225569012_p1972913440459"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p772984404520"><a name="zh-cn_topic_0225569012_p772984404520"></a><a name="zh-cn_topic_0225569012_p772984404520"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1572912448456"><a name="zh-cn_topic_0225569012_p1572912448456"></a><a name="zh-cn_topic_0225569012_p1572912448456"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p391615711217"><a name="zh-cn_topic_0225569012_p391615711217"></a><a name="zh-cn_topic_0225569012_p391615711217"></a>鉴权类型，支持apiKey</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row174417447455"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p137441344124516"><a name="zh-cn_topic_0225569012_p137441344124516"></a><a name="zh-cn_topic_0225569012_p137441344124516"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p5744194417451"><a name="zh-cn_topic_0225569012_p5744194417451"></a><a name="zh-cn_topic_0225569012_p5744194417451"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p17759844114514"><a name="zh-cn_topic_0225569012_p17759844114514"></a><a name="zh-cn_topic_0225569012_p17759844114514"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p79161875126"><a name="zh-cn_topic_0225569012_p79161875126"></a><a name="zh-cn_topic_0225569012_p79161875126"></a>apiKey参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row102624414498"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p6262154124918"><a name="zh-cn_topic_0225569012_p6262154124918"></a><a name="zh-cn_topic_0225569012_p6262154124918"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p726244115495"><a name="zh-cn_topic_0225569012_p726244115495"></a><a name="zh-cn_topic_0225569012_p726244115495"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1226214110494"><a name="zh-cn_topic_0225569012_p1226214110494"></a><a name="zh-cn_topic_0225569012_p1226214110494"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1226284194920"><a name="zh-cn_topic_0225569012_p1226284194920"></a><a name="zh-cn_topic_0225569012_p1226284194920"></a>apiKey参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row15495134319491"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p249515433492"><a name="zh-cn_topic_0225569012_p249515433492"></a><a name="zh-cn_topic_0225569012_p249515433492"></a>x-apigateway-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1495743154918"><a name="zh-cn_topic_0225569012_p1495743154918"></a><a name="zh-cn_topic_0225569012_p1495743154918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p19495194374913"><a name="zh-cn_topic_0225569012_p19495194374913"></a><a name="zh-cn_topic_0225569012_p19495194374913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p6495184315490"><a name="zh-cn_topic_0225569012_p6495184315490"></a><a name="zh-cn_topic_0225569012_p6495184315490"></a>扩展鉴权类型，基于apiKey鉴权方式的扩展，网关自定义的鉴权方式，支持AppSigv1、IAM、IAM_NONE</p>
</td>
</tr>
</tbody>
</table>

**表 16**  x-apigateway-backend参数说明

<a name="zh-cn_topic_0225569012_table1399375061810"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row1099445011810"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p399420504185"><a name="zh-cn_topic_0225569012_p399420504185"></a><a name="zh-cn_topic_0225569012_p399420504185"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p1599412506188"><a name="zh-cn_topic_0225569012_p1599412506188"></a><a name="zh-cn_topic_0225569012_p1599412506188"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p109941150191817"><a name="zh-cn_topic_0225569012_p109941150191817"></a><a name="zh-cn_topic_0225569012_p109941150191817"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p6994850121814"><a name="zh-cn_topic_0225569012_p6994850121814"></a><a name="zh-cn_topic_0225569012_p6994850121814"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row1099411501188"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p9994115041815"><a name="zh-cn_topic_0225569012_p9994115041815"></a><a name="zh-cn_topic_0225569012_p9994115041815"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p199405091810"><a name="zh-cn_topic_0225569012_p199405091810"></a><a name="zh-cn_topic_0225569012_p199405091810"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p149943505187"><a name="zh-cn_topic_0225569012_p149943505187"></a><a name="zh-cn_topic_0225569012_p149943505187"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p999485001810"><a name="zh-cn_topic_0225569012_p999485001810"></a><a name="zh-cn_topic_0225569012_p999485001810"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1899475091815"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p149942507183"><a name="zh-cn_topic_0225569012_p149942507183"></a><a name="zh-cn_topic_0225569012_p149942507183"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1099445091814"><a name="zh-cn_topic_0225569012_p1099445091814"></a><a name="zh-cn_topic_0225569012_p1099445091814"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p109949506186"><a name="zh-cn_topic_0225569012_p109949506186"></a><a name="zh-cn_topic_0225569012_p109949506186"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p899545041818"><a name="zh-cn_topic_0225569012_p899545041818"></a><a name="zh-cn_topic_0225569012_p899545041818"></a>后端参数对象数组定义，参考<a href="#zh-cn_topic_0225569012_table114356017274">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1399518509189"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1099510502182"><a name="zh-cn_topic_0225569012_p1099510502182"></a><a name="zh-cn_topic_0225569012_p1099510502182"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p139953502183"><a name="zh-cn_topic_0225569012_p139953502183"></a><a name="zh-cn_topic_0225569012_p139953502183"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p0995650141816"><a name="zh-cn_topic_0225569012_p0995650141816"></a><a name="zh-cn_topic_0225569012_p0995650141816"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p17995650121814"><a name="zh-cn_topic_0225569012_p17995650121814"></a><a name="zh-cn_topic_0225569012_p17995650121814"></a>API后端定义</p>
<p id="zh-cn_topic_0225569012_p1355171103619"><a name="zh-cn_topic_0225569012_p1355171103619"></a><a name="zh-cn_topic_0225569012_p1355171103619"></a>backend_define支持：</p>
<a name="zh-cn_topic_0225569012_ul6490161393619"></a><a name="zh-cn_topic_0225569012_ul6490161393619"></a><ul id="zh-cn_topic_0225569012_ul6490161393619"><li>httpEndpoints，参考<a href="#zh-cn_topic_0225569012_table1239533823112">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#zh-cn_topic_0225569012_table883265113385">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#zh-cn_topic_0225569012_table6690165310383">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#zh-cn_topic_0225569012_table2097855511388">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
</tbody>
</table>

**表 17**  x-apigateway-backend-policies参数说明

<a name="zh-cn_topic_0225569012_table1531411471794"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row173156479918"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p331564718911"><a name="zh-cn_topic_0225569012_p331564718911"></a><a name="zh-cn_topic_0225569012_p331564718911"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p63150471293"><a name="zh-cn_topic_0225569012_p63150471293"></a><a name="zh-cn_topic_0225569012_p63150471293"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p1031510475914"><a name="zh-cn_topic_0225569012_p1031510475914"></a><a name="zh-cn_topic_0225569012_p1031510475914"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p031616471799"><a name="zh-cn_topic_0225569012_p031616471799"></a><a name="zh-cn_topic_0225569012_p031616471799"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row4316104716920"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p123161547391"><a name="zh-cn_topic_0225569012_p123161547391"></a><a name="zh-cn_topic_0225569012_p123161547391"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p631619471996"><a name="zh-cn_topic_0225569012_p631619471996"></a><a name="zh-cn_topic_0225569012_p631619471996"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1731684716910"><a name="zh-cn_topic_0225569012_p1731684716910"></a><a name="zh-cn_topic_0225569012_p1731684716910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1231615471994"><a name="zh-cn_topic_0225569012_p1231615471994"></a><a name="zh-cn_topic_0225569012_p1231615471994"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1856112297106"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p6312143881016"><a name="zh-cn_topic_0225569012_p6312143881016"></a><a name="zh-cn_topic_0225569012_p6312143881016"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1831243814107"><a name="zh-cn_topic_0225569012_p1831243814107"></a><a name="zh-cn_topic_0225569012_p1831243814107"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8312183812106"><a name="zh-cn_topic_0225569012_p8312183812106"></a><a name="zh-cn_topic_0225569012_p8312183812106"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p15312173891013"><a name="zh-cn_topic_0225569012_p15312173891013"></a><a name="zh-cn_topic_0225569012_p15312173891013"></a>后端策略名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row431615474917"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p231654718912"><a name="zh-cn_topic_0225569012_p231654718912"></a><a name="zh-cn_topic_0225569012_p231654718912"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p19316124719914"><a name="zh-cn_topic_0225569012_p19316124719914"></a><a name="zh-cn_topic_0225569012_p19316124719914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p183161247292"><a name="zh-cn_topic_0225569012_p183161247292"></a><a name="zh-cn_topic_0225569012_p183161247292"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1931713471097"><a name="zh-cn_topic_0225569012_p1931713471097"></a><a name="zh-cn_topic_0225569012_p1931713471097"></a>后端参数对象数组定义，参考<a href="#zh-cn_topic_0225569012_table114356017274">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row19317174717912"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p131744718910"><a name="zh-cn_topic_0225569012_p131744718910"></a><a name="zh-cn_topic_0225569012_p131744718910"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p203179474919"><a name="zh-cn_topic_0225569012_p203179474919"></a><a name="zh-cn_topic_0225569012_p203179474919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8317247296"><a name="zh-cn_topic_0225569012_p8317247296"></a><a name="zh-cn_topic_0225569012_p8317247296"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1931710474910"><a name="zh-cn_topic_0225569012_p1931710474910"></a><a name="zh-cn_topic_0225569012_p1931710474910"></a>API后端定义</p>
<p id="zh-cn_topic_0225569012_p173171047995"><a name="zh-cn_topic_0225569012_p173171047995"></a><a name="zh-cn_topic_0225569012_p173171047995"></a>backend_define支持：</p>
<a name="zh-cn_topic_0225569012_ul13317104716917"></a><a name="zh-cn_topic_0225569012_ul13317104716917"></a><ul id="zh-cn_topic_0225569012_ul13317104716917"><li>httpEndpoints，参考<a href="#zh-cn_topic_0225569012_table1239533823112">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#zh-cn_topic_0225569012_table883265113385">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#zh-cn_topic_0225569012_table6690165310383">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#zh-cn_topic_0225569012_table2097855511388">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row11626194931016"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p0412355171010"><a name="zh-cn_topic_0225569012_p0412355171010"></a><a name="zh-cn_topic_0225569012_p0412355171010"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p18412185521017"><a name="zh-cn_topic_0225569012_p18412185521017"></a><a name="zh-cn_topic_0225569012_p18412185521017"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p9412105511015"><a name="zh-cn_topic_0225569012_p9412105511015"></a><a name="zh-cn_topic_0225569012_p9412105511015"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p154121455111020"><a name="zh-cn_topic_0225569012_p154121455111020"></a><a name="zh-cn_topic_0225569012_p154121455111020"></a>策略条件对象数组定义，参考<a href="#zh-cn_topic_0225569012_table2664522111210">表 conditions参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row8601019134513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p7826184743414"><a name="zh-cn_topic_0225569012_p7826184743414"></a><a name="zh-cn_topic_0225569012_p7826184743414"></a>effectMode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p15826134712343"><a name="zh-cn_topic_0225569012_p15826134712343"></a><a name="zh-cn_topic_0225569012_p15826134712343"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p58262047113410"><a name="zh-cn_topic_0225569012_p58262047113410"></a><a name="zh-cn_topic_0225569012_p58262047113410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p17355191291320"><a name="zh-cn_topic_0225569012_p17355191291320"></a><a name="zh-cn_topic_0225569012_p17355191291320"></a>关联的策略组合模式，支持ANY、ALL</p>
</td>
</tr>
</tbody>
</table>

**表 18**  后端parameters参数说明

<a name="zh-cn_topic_0225569012_table114356017274"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row443650112715"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p194361603275"><a name="zh-cn_topic_0225569012_p194361603275"></a><a name="zh-cn_topic_0225569012_p194361603275"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p1843618018277"><a name="zh-cn_topic_0225569012_p1843618018277"></a><a name="zh-cn_topic_0225569012_p1843618018277"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p1843614014271"><a name="zh-cn_topic_0225569012_p1843614014271"></a><a name="zh-cn_topic_0225569012_p1843614014271"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1543617032718"><a name="zh-cn_topic_0225569012_p1543617032718"></a><a name="zh-cn_topic_0225569012_p1543617032718"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row18436107273"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p6857230153111"><a name="zh-cn_topic_0225569012_p6857230153111"></a><a name="zh-cn_topic_0225569012_p6857230153111"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p8857630103113"><a name="zh-cn_topic_0225569012_p8857630103113"></a><a name="zh-cn_topic_0225569012_p8857630103113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p13857133083119"><a name="zh-cn_topic_0225569012_p13857133083119"></a><a name="zh-cn_topic_0225569012_p13857133083119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p285763043116"><a name="zh-cn_topic_0225569012_p285763043116"></a><a name="zh-cn_topic_0225569012_p285763043116"></a>参数名称，由字母、数字、下划线、连线、点组成，以字母开头，最长32字节</p>
<p id="zh-cn_topic_0225569012_p18857130123115"><a name="zh-cn_topic_0225569012_p18857130123115"></a><a name="zh-cn_topic_0225569012_p18857130123115"></a>header位置的参数名称不区分大小写</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row14437120202717"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p15857630203119"><a name="zh-cn_topic_0225569012_p15857630203119"></a><a name="zh-cn_topic_0225569012_p15857630203119"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1185718301311"><a name="zh-cn_topic_0225569012_p1185718301311"></a><a name="zh-cn_topic_0225569012_p1185718301311"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p168571130163120"><a name="zh-cn_topic_0225569012_p168571130163120"></a><a name="zh-cn_topic_0225569012_p168571130163120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p685753003117"><a name="zh-cn_topic_0225569012_p685753003117"></a><a name="zh-cn_topic_0225569012_p685753003117"></a>参数值，当参数来源为REQUEST时，值为请求参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row343720182718"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p16857730133117"><a name="zh-cn_topic_0225569012_p16857730133117"></a><a name="zh-cn_topic_0225569012_p16857730133117"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p885843014319"><a name="zh-cn_topic_0225569012_p885843014319"></a><a name="zh-cn_topic_0225569012_p885843014319"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p38581530133118"><a name="zh-cn_topic_0225569012_p38581530133118"></a><a name="zh-cn_topic_0225569012_p38581530133118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p8858153063116"><a name="zh-cn_topic_0225569012_p8858153063116"></a><a name="zh-cn_topic_0225569012_p8858153063116"></a>参数位置，支持header、query、path</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row843780132711"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p5858530133116"><a name="zh-cn_topic_0225569012_p5858530133116"></a><a name="zh-cn_topic_0225569012_p5858530133116"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p08582307318"><a name="zh-cn_topic_0225569012_p08582307318"></a><a name="zh-cn_topic_0225569012_p08582307318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p8858330153118"><a name="zh-cn_topic_0225569012_p8858330153118"></a><a name="zh-cn_topic_0225569012_p8858330153118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p5858193011316"><a name="zh-cn_topic_0225569012_p5858193011316"></a><a name="zh-cn_topic_0225569012_p5858193011316"></a>参数映射来源，支持REQUEST、CONSTANT</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row128758406283"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p685893010318"><a name="zh-cn_topic_0225569012_p685893010318"></a><a name="zh-cn_topic_0225569012_p685893010318"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p685863013313"><a name="zh-cn_topic_0225569012_p685863013313"></a><a name="zh-cn_topic_0225569012_p685863013313"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p15858173020313"><a name="zh-cn_topic_0225569012_p15858173020313"></a><a name="zh-cn_topic_0225569012_p15858173020313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p9858030173112"><a name="zh-cn_topic_0225569012_p9858030173112"></a><a name="zh-cn_topic_0225569012_p9858030173112"></a>参数含义描述</p>
</td>
</tr>
</tbody>
</table>

**表 19**  后端httpEndpoints参数说明

<a name="zh-cn_topic_0225569012_table1239533823112"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row139611389311"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p1439683815315"><a name="zh-cn_topic_0225569012_p1439683815315"></a><a name="zh-cn_topic_0225569012_p1439683815315"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p2396838203119"><a name="zh-cn_topic_0225569012_p2396838203119"></a><a name="zh-cn_topic_0225569012_p2396838203119"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p1139663833111"><a name="zh-cn_topic_0225569012_p1139663833111"></a><a name="zh-cn_topic_0225569012_p1139663833111"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1396638123113"><a name="zh-cn_topic_0225569012_p1396638123113"></a><a name="zh-cn_topic_0225569012_p1396638123113"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row1639663814318"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p4169847802"><a name="zh-cn_topic_0225569012_p4169847802"></a><a name="zh-cn_topic_0225569012_p4169847802"></a>address</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p81695471404"><a name="zh-cn_topic_0225569012_p81695471404"></a><a name="zh-cn_topic_0225569012_p81695471404"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p7169104715014"><a name="zh-cn_topic_0225569012_p7169104715014"></a><a name="zh-cn_topic_0225569012_p7169104715014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1516916471703"><a name="zh-cn_topic_0225569012_p1516916471703"></a><a name="zh-cn_topic_0225569012_p1516916471703"></a>后端服务地址，格式为：&lt;域名或IP&gt;:[port]</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row5397438163117"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p316918475016"><a name="zh-cn_topic_0225569012_p316918475016"></a><a name="zh-cn_topic_0225569012_p316918475016"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1016974710013"><a name="zh-cn_topic_0225569012_p1016974710013"></a><a name="zh-cn_topic_0225569012_p1016974710013"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p4169154710014"><a name="zh-cn_topic_0225569012_p4169154710014"></a><a name="zh-cn_topic_0225569012_p4169154710014"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p151690479015"><a name="zh-cn_topic_0225569012_p151690479015"></a><a name="zh-cn_topic_0225569012_p151690479015"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row439743814310"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p0169447308"><a name="zh-cn_topic_0225569012_p0169447308"></a><a name="zh-cn_topic_0225569012_p0169447308"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p13169547908"><a name="zh-cn_topic_0225569012_p13169547908"></a><a name="zh-cn_topic_0225569012_p13169547908"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p41696471205"><a name="zh-cn_topic_0225569012_p41696471205"></a><a name="zh-cn_topic_0225569012_p41696471205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p41692047305"><a name="zh-cn_topic_0225569012_p41692047305"></a><a name="zh-cn_topic_0225569012_p41692047305"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row4398138153116"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p316934719018"><a name="zh-cn_topic_0225569012_p316934719018"></a><a name="zh-cn_topic_0225569012_p316934719018"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p316914710016"><a name="zh-cn_topic_0225569012_p316914710016"></a><a name="zh-cn_topic_0225569012_p316914710016"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p18169347807"><a name="zh-cn_topic_0225569012_p18169347807"></a><a name="zh-cn_topic_0225569012_p18169347807"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p61693476012"><a name="zh-cn_topic_0225569012_p61693476012"></a><a name="zh-cn_topic_0225569012_p61693476012"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row339863810311"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p616974711016"><a name="zh-cn_topic_0225569012_p616974711016"></a><a name="zh-cn_topic_0225569012_p616974711016"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1616913471019"><a name="zh-cn_topic_0225569012_p1616913471019"></a><a name="zh-cn_topic_0225569012_p1616913471019"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p516915471000"><a name="zh-cn_topic_0225569012_p516915471000"></a><a name="zh-cn_topic_0225569012_p516915471000"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1516974712019"><a name="zh-cn_topic_0225569012_p1516974712019"></a><a name="zh-cn_topic_0225569012_p1516974712019"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row7635433104612"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p191691539173611"><a name="zh-cn_topic_0225569012_p191691539173611"></a><a name="zh-cn_topic_0225569012_p191691539173611"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p916993963610"><a name="zh-cn_topic_0225569012_p916993963610"></a><a name="zh-cn_topic_0225569012_p916993963610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p317073923616"><a name="zh-cn_topic_0225569012_p317073923616"></a><a name="zh-cn_topic_0225569012_p317073923616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p5170539163616"><a name="zh-cn_topic_0225569012_p5170539163616"></a><a name="zh-cn_topic_0225569012_p5170539163616"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 20**  后端httpVpcEndpoints参数说明

<a name="zh-cn_topic_0225569012_table883265113385"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row18321551193814"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p188335514388"><a name="zh-cn_topic_0225569012_p188335514388"></a><a name="zh-cn_topic_0225569012_p188335514388"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p383316519388"><a name="zh-cn_topic_0225569012_p383316519388"></a><a name="zh-cn_topic_0225569012_p383316519388"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p68331551153818"><a name="zh-cn_topic_0225569012_p68331551153818"></a><a name="zh-cn_topic_0225569012_p68331551153818"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p3833951133812"><a name="zh-cn_topic_0225569012_p3833951133812"></a><a name="zh-cn_topic_0225569012_p3833951133812"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row15833551143815"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1611417262018"><a name="zh-cn_topic_0225569012_p1611417262018"></a><a name="zh-cn_topic_0225569012_p1611417262018"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1611418262018"><a name="zh-cn_topic_0225569012_p1611418262018"></a><a name="zh-cn_topic_0225569012_p1611418262018"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1511412614110"><a name="zh-cn_topic_0225569012_p1511412614110"></a><a name="zh-cn_topic_0225569012_p1511412614110"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p11146262117"><a name="zh-cn_topic_0225569012_p11146262117"></a><a name="zh-cn_topic_0225569012_p11146262117"></a>VPC通道名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row16834105113816"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p2114152615111"><a name="zh-cn_topic_0225569012_p2114152615111"></a><a name="zh-cn_topic_0225569012_p2114152615111"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p61142261911"><a name="zh-cn_topic_0225569012_p61142261911"></a><a name="zh-cn_topic_0225569012_p61142261911"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p20114202614118"><a name="zh-cn_topic_0225569012_p20114202614118"></a><a name="zh-cn_topic_0225569012_p20114202614118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p171148263113"><a name="zh-cn_topic_0225569012_p171148263113"></a><a name="zh-cn_topic_0225569012_p171148263113"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row2083585173814"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1114172611112"><a name="zh-cn_topic_0225569012_p1114172611112"></a><a name="zh-cn_topic_0225569012_p1114172611112"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p31141526212"><a name="zh-cn_topic_0225569012_p31141526212"></a><a name="zh-cn_topic_0225569012_p31141526212"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1111417263110"><a name="zh-cn_topic_0225569012_p1111417263110"></a><a name="zh-cn_topic_0225569012_p1111417263110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p191141426417"><a name="zh-cn_topic_0225569012_p191141426417"></a><a name="zh-cn_topic_0225569012_p191141426417"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row12835105111387"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p19114826117"><a name="zh-cn_topic_0225569012_p19114826117"></a><a name="zh-cn_topic_0225569012_p19114826117"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1011415260118"><a name="zh-cn_topic_0225569012_p1011415260118"></a><a name="zh-cn_topic_0225569012_p1011415260118"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p191159261412"><a name="zh-cn_topic_0225569012_p191159261412"></a><a name="zh-cn_topic_0225569012_p191159261412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p11115926118"><a name="zh-cn_topic_0225569012_p11115926118"></a><a name="zh-cn_topic_0225569012_p11115926118"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row18836951193818"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p91158265114"><a name="zh-cn_topic_0225569012_p91158265114"></a><a name="zh-cn_topic_0225569012_p91158265114"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p8115152611118"><a name="zh-cn_topic_0225569012_p8115152611118"></a><a name="zh-cn_topic_0225569012_p8115152611118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p9115126915"><a name="zh-cn_topic_0225569012_p9115126915"></a><a name="zh-cn_topic_0225569012_p9115126915"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p7115626115"><a name="zh-cn_topic_0225569012_p7115626115"></a><a name="zh-cn_topic_0225569012_p7115626115"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row6664020154010"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p12665192012406"><a name="zh-cn_topic_0225569012_p12665192012406"></a><a name="zh-cn_topic_0225569012_p12665192012406"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p752351114424"><a name="zh-cn_topic_0225569012_p752351114424"></a><a name="zh-cn_topic_0225569012_p752351114424"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p10665620104018"><a name="zh-cn_topic_0225569012_p10665620104018"></a><a name="zh-cn_topic_0225569012_p10665620104018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p7665152018405"><a name="zh-cn_topic_0225569012_p7665152018405"></a><a name="zh-cn_topic_0225569012_p7665152018405"></a>VPC通道代理主机</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row126916399464"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1205124114618"><a name="zh-cn_topic_0225569012_p1205124114618"></a><a name="zh-cn_topic_0225569012_p1205124114618"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p11205204144619"><a name="zh-cn_topic_0225569012_p11205204144619"></a><a name="zh-cn_topic_0225569012_p11205204144619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p172056411467"><a name="zh-cn_topic_0225569012_p172056411467"></a><a name="zh-cn_topic_0225569012_p172056411467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1520564144612"><a name="zh-cn_topic_0225569012_p1520564144612"></a><a name="zh-cn_topic_0225569012_p1520564144612"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 21**  后端functionEndpoints参数说明

<a name="zh-cn_topic_0225569012_table6690165310383"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row196901653183813"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p106907533388"><a name="zh-cn_topic_0225569012_p106907533388"></a><a name="zh-cn_topic_0225569012_p106907533388"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p169025323814"><a name="zh-cn_topic_0225569012_p169025323814"></a><a name="zh-cn_topic_0225569012_p169025323814"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p10690115303816"><a name="zh-cn_topic_0225569012_p10690115303816"></a><a name="zh-cn_topic_0225569012_p10690115303816"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p869135314384"><a name="zh-cn_topic_0225569012_p869135314384"></a><a name="zh-cn_topic_0225569012_p869135314384"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row11691253133813"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p51151441120"><a name="zh-cn_topic_0225569012_p51151441120"></a><a name="zh-cn_topic_0225569012_p51151441120"></a>function-urn</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1811519446117"><a name="zh-cn_topic_0225569012_p1811519446117"></a><a name="zh-cn_topic_0225569012_p1811519446117"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p91151944212"><a name="zh-cn_topic_0225569012_p91151944212"></a><a name="zh-cn_topic_0225569012_p91151944212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p2115544311"><a name="zh-cn_topic_0225569012_p2115544311"></a><a name="zh-cn_topic_0225569012_p2115544311"></a>函数URN地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1269105333811"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1011514441815"><a name="zh-cn_topic_0225569012_p1011514441815"></a><a name="zh-cn_topic_0225569012_p1011514441815"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p811512441111"><a name="zh-cn_topic_0225569012_p811512441111"></a><a name="zh-cn_topic_0225569012_p811512441111"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p11154443116"><a name="zh-cn_topic_0225569012_p11154443116"></a><a name="zh-cn_topic_0225569012_p11154443116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p911584415112"><a name="zh-cn_topic_0225569012_p911584415112"></a><a name="zh-cn_topic_0225569012_p911584415112"></a>函数版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row146917539386"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p911517441019"><a name="zh-cn_topic_0225569012_p911517441019"></a><a name="zh-cn_topic_0225569012_p911517441019"></a>invocation-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p81151344618"><a name="zh-cn_topic_0225569012_p81151344618"></a><a name="zh-cn_topic_0225569012_p81151344618"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p511510448120"><a name="zh-cn_topic_0225569012_p511510448120"></a><a name="zh-cn_topic_0225569012_p511510448120"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p141151144110"><a name="zh-cn_topic_0225569012_p141151144110"></a><a name="zh-cn_topic_0225569012_p141151144110"></a>函数调用类型，支持async、sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row56923530383"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p101161441114"><a name="zh-cn_topic_0225569012_p101161441114"></a><a name="zh-cn_topic_0225569012_p101161441114"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1411654410117"><a name="zh-cn_topic_0225569012_p1411654410117"></a><a name="zh-cn_topic_0225569012_p1411654410117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p51161044111"><a name="zh-cn_topic_0225569012_p51161044111"></a><a name="zh-cn_topic_0225569012_p51161044111"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1116844319"><a name="zh-cn_topic_0225569012_p1116844319"></a><a name="zh-cn_topic_0225569012_p1116844319"></a>函数超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row4948164516468"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p417724714468"><a name="zh-cn_topic_0225569012_p417724714468"></a><a name="zh-cn_topic_0225569012_p417724714468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p20177147174614"><a name="zh-cn_topic_0225569012_p20177147174614"></a><a name="zh-cn_topic_0225569012_p20177147174614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p2178184712466"><a name="zh-cn_topic_0225569012_p2178184712466"></a><a name="zh-cn_topic_0225569012_p2178184712466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p131781547144613"><a name="zh-cn_topic_0225569012_p131781547144613"></a><a name="zh-cn_topic_0225569012_p131781547144613"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 22**  后端mockEndpoints参数说明

<a name="zh-cn_topic_0225569012_table2097855511388"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row10979185563813"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p1697917552383"><a name="zh-cn_topic_0225569012_p1697917552383"></a><a name="zh-cn_topic_0225569012_p1697917552383"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p10979155533819"><a name="zh-cn_topic_0225569012_p10979155533819"></a><a name="zh-cn_topic_0225569012_p10979155533819"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p15979175515388"><a name="zh-cn_topic_0225569012_p15979175515388"></a><a name="zh-cn_topic_0225569012_p15979175515388"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1397935563813"><a name="zh-cn_topic_0225569012_p1397935563813"></a><a name="zh-cn_topic_0225569012_p1397935563813"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row897912554389"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p126352191325"><a name="zh-cn_topic_0225569012_p126352191325"></a><a name="zh-cn_topic_0225569012_p126352191325"></a>result-content</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p16356191424"><a name="zh-cn_topic_0225569012_p16356191424"></a><a name="zh-cn_topic_0225569012_p16356191424"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p186359191228"><a name="zh-cn_topic_0225569012_p186359191228"></a><a name="zh-cn_topic_0225569012_p186359191228"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p176355192219"><a name="zh-cn_topic_0225569012_p176355192219"></a><a name="zh-cn_topic_0225569012_p176355192219"></a>MOCK返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row4433155454616"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1576125519468"><a name="zh-cn_topic_0225569012_p1576125519468"></a><a name="zh-cn_topic_0225569012_p1576125519468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1857675514611"><a name="zh-cn_topic_0225569012_p1857675514611"></a><a name="zh-cn_topic_0225569012_p1857675514611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p105761955174616"><a name="zh-cn_topic_0225569012_p105761955174616"></a><a name="zh-cn_topic_0225569012_p105761955174616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p05768551462"><a name="zh-cn_topic_0225569012_p05768551462"></a><a name="zh-cn_topic_0225569012_p05768551462"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 23**  conditions参数说明

<a name="zh-cn_topic_0225569012_table2664522111210"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row206652225121"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p266519224129"><a name="zh-cn_topic_0225569012_p266519224129"></a><a name="zh-cn_topic_0225569012_p266519224129"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p16665162291216"><a name="zh-cn_topic_0225569012_p16665162291216"></a><a name="zh-cn_topic_0225569012_p16665162291216"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p06651922111211"><a name="zh-cn_topic_0225569012_p06651922111211"></a><a name="zh-cn_topic_0225569012_p06651922111211"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1665152215127"><a name="zh-cn_topic_0225569012_p1665152215127"></a><a name="zh-cn_topic_0225569012_p1665152215127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row13666132281210"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p13523114971213"><a name="zh-cn_topic_0225569012_p13523114971213"></a><a name="zh-cn_topic_0225569012_p13523114971213"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p852354961215"><a name="zh-cn_topic_0225569012_p852354961215"></a><a name="zh-cn_topic_0225569012_p852354961215"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p105235496124"><a name="zh-cn_topic_0225569012_p105235496124"></a><a name="zh-cn_topic_0225569012_p105235496124"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p135231249111213"><a name="zh-cn_topic_0225569012_p135231249111213"></a><a name="zh-cn_topic_0225569012_p135231249111213"></a>策略条件类型，支持equal、enum、pattern</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row866662212129"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p552314919127"><a name="zh-cn_topic_0225569012_p552314919127"></a><a name="zh-cn_topic_0225569012_p552314919127"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1752314911123"><a name="zh-cn_topic_0225569012_p1752314911123"></a><a name="zh-cn_topic_0225569012_p1752314911123"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p6523124911213"><a name="zh-cn_topic_0225569012_p6523124911213"></a><a name="zh-cn_topic_0225569012_p6523124911213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1652384910126"><a name="zh-cn_topic_0225569012_p1652384910126"></a><a name="zh-cn_topic_0225569012_p1652384910126"></a>策略条件值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row766772291212"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p952314912123"><a name="zh-cn_topic_0225569012_p952314912123"></a><a name="zh-cn_topic_0225569012_p952314912123"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p15231649111220"><a name="zh-cn_topic_0225569012_p15231649111220"></a><a name="zh-cn_topic_0225569012_p15231649111220"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p185231149101211"><a name="zh-cn_topic_0225569012_p185231149101211"></a><a name="zh-cn_topic_0225569012_p185231149101211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p12523649141215"><a name="zh-cn_topic_0225569012_p12523649141215"></a><a name="zh-cn_topic_0225569012_p12523649141215"></a>策略条件输入来源，支持source、request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1866742211122"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p552354961218"><a name="zh-cn_topic_0225569012_p552354961218"></a><a name="zh-cn_topic_0225569012_p552354961218"></a>parameter</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p85231849201217"><a name="zh-cn_topic_0225569012_p85231849201217"></a><a name="zh-cn_topic_0225569012_p85231849201217"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p6524134921211"><a name="zh-cn_topic_0225569012_p6524134921211"></a><a name="zh-cn_topic_0225569012_p6524134921211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p14524349161211"><a name="zh-cn_topic_0225569012_p14524349161211"></a><a name="zh-cn_topic_0225569012_p14524349161211"></a>策略条件输入来源为request时，请求入参的名称</p>
</td>
</tr>
</tbody>
</table>

**表 24**  x-apigateway-access-controls参数说明

<a name="zh-cn_topic_0225569012_table1621715417575"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row1321811416572"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p62187455710"><a name="zh-cn_topic_0225569012_p62187455710"></a><a name="zh-cn_topic_0225569012_p62187455710"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p15218124155713"><a name="zh-cn_topic_0225569012_p15218124155713"></a><a name="zh-cn_topic_0225569012_p15218124155713"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p121844195713"><a name="zh-cn_topic_0225569012_p121844195713"></a><a name="zh-cn_topic_0225569012_p121844195713"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p62188417574"><a name="zh-cn_topic_0225569012_p62188417574"></a><a name="zh-cn_topic_0225569012_p62188417574"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row162189412576"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p321816445710"><a name="zh-cn_topic_0225569012_p321816445710"></a><a name="zh-cn_topic_0225569012_p321816445710"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1218845574"><a name="zh-cn_topic_0225569012_p1218845574"></a><a name="zh-cn_topic_0225569012_p1218845574"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p921894145719"><a name="zh-cn_topic_0225569012_p921894145719"></a><a name="zh-cn_topic_0225569012_p921894145719"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p12218114145711"><a name="zh-cn_topic_0225569012_p12218114145711"></a><a name="zh-cn_topic_0225569012_p12218114145711"></a>指定名称的访问控制策略，参考<a href="#zh-cn_topic_0225569012_table6136187195718">表 acl_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 25**  acl\_name参数说明

<a name="zh-cn_topic_0225569012_table6136187195718"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row1113713795718"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p71370735720"><a name="zh-cn_topic_0225569012_p71370735720"></a><a name="zh-cn_topic_0225569012_p71370735720"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p131382755714"><a name="zh-cn_topic_0225569012_p131382755714"></a><a name="zh-cn_topic_0225569012_p131382755714"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p013817717576"><a name="zh-cn_topic_0225569012_p013817717576"></a><a name="zh-cn_topic_0225569012_p013817717576"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1313814715572"><a name="zh-cn_topic_0225569012_p1313814715572"></a><a name="zh-cn_topic_0225569012_p1313814715572"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row13138117115713"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p615210151511"><a name="zh-cn_topic_0225569012_p615210151511"></a><a name="zh-cn_topic_0225569012_p615210151511"></a>acl-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p121521215816"><a name="zh-cn_topic_0225569012_p121521215816"></a><a name="zh-cn_topic_0225569012_p121521215816"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p14152181510116"><a name="zh-cn_topic_0225569012_p14152181510116"></a><a name="zh-cn_topic_0225569012_p14152181510116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p81521151511"><a name="zh-cn_topic_0225569012_p81521151511"></a><a name="zh-cn_topic_0225569012_p81521151511"></a>访问控制行为，支持PERMIT、DENY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row9518174805812"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p16152615718"><a name="zh-cn_topic_0225569012_p16152615718"></a><a name="zh-cn_topic_0225569012_p16152615718"></a>entity-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p151521715813"><a name="zh-cn_topic_0225569012_p151521715813"></a><a name="zh-cn_topic_0225569012_p151521715813"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p14152151511112"><a name="zh-cn_topic_0225569012_p14152151511112"></a><a name="zh-cn_topic_0225569012_p14152151511112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p151528158116"><a name="zh-cn_topic_0225569012_p151528158116"></a><a name="zh-cn_topic_0225569012_p151528158116"></a>访问控制对象，支持IP、DOMAIN</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row19475115016587"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p71526151714"><a name="zh-cn_topic_0225569012_p71526151714"></a><a name="zh-cn_topic_0225569012_p71526151714"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p131521151112"><a name="zh-cn_topic_0225569012_p131521151112"></a><a name="zh-cn_topic_0225569012_p131521151112"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p151520155116"><a name="zh-cn_topic_0225569012_p151520155116"></a><a name="zh-cn_topic_0225569012_p151520155116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p9152115418"><a name="zh-cn_topic_0225569012_p9152115418"></a><a name="zh-cn_topic_0225569012_p9152115418"></a>访问控制策略值，多个值以“,”间隔</p>
</td>
</tr>
</tbody>
</table>

**表 26**  x-apigateway-ratelimits参数说明

<a name="zh-cn_topic_0225569012_table18116161025717"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row011618104574"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p171174105578"><a name="zh-cn_topic_0225569012_p171174105578"></a><a name="zh-cn_topic_0225569012_p171174105578"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p511713106574"><a name="zh-cn_topic_0225569012_p511713106574"></a><a name="zh-cn_topic_0225569012_p511713106574"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p11117181055714"><a name="zh-cn_topic_0225569012_p11117181055714"></a><a name="zh-cn_topic_0225569012_p11117181055714"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p1011720104575"><a name="zh-cn_topic_0225569012_p1011720104575"></a><a name="zh-cn_topic_0225569012_p1011720104575"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row3117181035713"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1711713103574"><a name="zh-cn_topic_0225569012_p1711713103574"></a><a name="zh-cn_topic_0225569012_p1711713103574"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1919113207418"><a name="zh-cn_topic_0225569012_p1919113207418"></a><a name="zh-cn_topic_0225569012_p1919113207418"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p4191152017419"><a name="zh-cn_topic_0225569012_p4191152017419"></a><a name="zh-cn_topic_0225569012_p4191152017419"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1411731095717"><a name="zh-cn_topic_0225569012_p1411731095717"></a><a name="zh-cn_topic_0225569012_p1411731095717"></a>指定名称的流控策略，参考<a href="#zh-cn_topic_0225569012_table1480213012577">表 throttle_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 27**  throttle\_name参数说明

<a name="zh-cn_topic_0225569012_table1480213012577"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row208029016573"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p780270195711"><a name="zh-cn_topic_0225569012_p780270195711"></a><a name="zh-cn_topic_0225569012_p780270195711"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p38029017572"><a name="zh-cn_topic_0225569012_p38029017572"></a><a name="zh-cn_topic_0225569012_p38029017572"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p198021709572"><a name="zh-cn_topic_0225569012_p198021709572"></a><a name="zh-cn_topic_0225569012_p198021709572"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p12803100145719"><a name="zh-cn_topic_0225569012_p12803100145719"></a><a name="zh-cn_topic_0225569012_p12803100145719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row1780340155718"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p11316142219208"><a name="zh-cn_topic_0225569012_p11316142219208"></a><a name="zh-cn_topic_0225569012_p11316142219208"></a>api-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p53165229200"><a name="zh-cn_topic_0225569012_p53165229200"></a><a name="zh-cn_topic_0225569012_p53165229200"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p6316122213202"><a name="zh-cn_topic_0225569012_p6316122213202"></a><a name="zh-cn_topic_0225569012_p6316122213202"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p1831682219206"><a name="zh-cn_topic_0225569012_p1831682219206"></a><a name="zh-cn_topic_0225569012_p1831682219206"></a>API访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row17861852161911"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p131614221202"><a name="zh-cn_topic_0225569012_p131614221202"></a><a name="zh-cn_topic_0225569012_p131614221202"></a>user-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p73161722192011"><a name="zh-cn_topic_0225569012_p73161722192011"></a><a name="zh-cn_topic_0225569012_p73161722192011"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p12316112216206"><a name="zh-cn_topic_0225569012_p12316112216206"></a><a name="zh-cn_topic_0225569012_p12316112216206"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p3317622152014"><a name="zh-cn_topic_0225569012_p3317622152014"></a><a name="zh-cn_topic_0225569012_p3317622152014"></a>用户访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row178003032016"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p16317132202018"><a name="zh-cn_topic_0225569012_p16317132202018"></a><a name="zh-cn_topic_0225569012_p16317132202018"></a>app-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1931711224208"><a name="zh-cn_topic_0225569012_p1931711224208"></a><a name="zh-cn_topic_0225569012_p1931711224208"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p73171022172017"><a name="zh-cn_topic_0225569012_p73171022172017"></a><a name="zh-cn_topic_0225569012_p73171022172017"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p231772282010"><a name="zh-cn_topic_0225569012_p231772282010"></a><a name="zh-cn_topic_0225569012_p231772282010"></a>应用访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1652010920206"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p231716224204"><a name="zh-cn_topic_0225569012_p231716224204"></a><a name="zh-cn_topic_0225569012_p231716224204"></a>ip-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p10317922182016"><a name="zh-cn_topic_0225569012_p10317922182016"></a><a name="zh-cn_topic_0225569012_p10317922182016"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1731752272020"><a name="zh-cn_topic_0225569012_p1731752272020"></a><a name="zh-cn_topic_0225569012_p1731752272020"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p931717225208"><a name="zh-cn_topic_0225569012_p931717225208"></a><a name="zh-cn_topic_0225569012_p931717225208"></a>源IP访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row24088557198"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p031718221206"><a name="zh-cn_topic_0225569012_p031718221206"></a><a name="zh-cn_topic_0225569012_p031718221206"></a>interval</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p53171221202"><a name="zh-cn_topic_0225569012_p53171221202"></a><a name="zh-cn_topic_0225569012_p53171221202"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1631762211204"><a name="zh-cn_topic_0225569012_p1631762211204"></a><a name="zh-cn_topic_0225569012_p1631762211204"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p531717220201"><a name="zh-cn_topic_0225569012_p531717220201"></a><a name="zh-cn_topic_0225569012_p531717220201"></a>流控策略时间周期</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row7911629200"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p5317122272010"><a name="zh-cn_topic_0225569012_p5317122272010"></a><a name="zh-cn_topic_0225569012_p5317122272010"></a>unit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p93171822202011"><a name="zh-cn_topic_0225569012_p93171822202011"></a><a name="zh-cn_topic_0225569012_p93171822202011"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p131772262010"><a name="zh-cn_topic_0225569012_p131772262010"></a><a name="zh-cn_topic_0225569012_p131772262010"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p931817223200"><a name="zh-cn_topic_0225569012_p931817223200"></a><a name="zh-cn_topic_0225569012_p931817223200"></a>流控策略时间周期单位，支持SECOND、MINUTE、HOUR、DAY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1369195711911"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p6318122252010"><a name="zh-cn_topic_0225569012_p6318122252010"></a><a name="zh-cn_topic_0225569012_p6318122252010"></a>shared</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p731852292016"><a name="zh-cn_topic_0225569012_p731852292016"></a><a name="zh-cn_topic_0225569012_p731852292016"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1131822215208"><a name="zh-cn_topic_0225569012_p1131822215208"></a><a name="zh-cn_topic_0225569012_p1131822215208"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p143181222142017"><a name="zh-cn_topic_0225569012_p143181222142017"></a><a name="zh-cn_topic_0225569012_p143181222142017"></a>是否共享流控策略</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row88492155206"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p931802213200"><a name="zh-cn_topic_0225569012_p931802213200"></a><a name="zh-cn_topic_0225569012_p931802213200"></a>special</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p16318152219204"><a name="zh-cn_topic_0225569012_p16318152219204"></a><a name="zh-cn_topic_0225569012_p16318152219204"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p1831892232016"><a name="zh-cn_topic_0225569012_p1831892232016"></a><a name="zh-cn_topic_0225569012_p1831892232016"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p9318622152016"><a name="zh-cn_topic_0225569012_p9318622152016"></a><a name="zh-cn_topic_0225569012_p9318622152016"></a>特殊流控策略对象数组定义，参考<a href="#zh-cn_topic_0225569012_table133925592200">表 special参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 28**  special参数说明

<a name="zh-cn_topic_0225569012_table133925592200"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row123921559172011"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225569012_p9392115912016"><a name="zh-cn_topic_0225569012_p9392115912016"></a><a name="zh-cn_topic_0225569012_p9392115912016"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225569012_p20395145982014"><a name="zh-cn_topic_0225569012_p20395145982014"></a><a name="zh-cn_topic_0225569012_p20395145982014"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225569012_p2039575992016"><a name="zh-cn_topic_0225569012_p2039575992016"></a><a name="zh-cn_topic_0225569012_p2039575992016"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225569012_p7395159102016"><a name="zh-cn_topic_0225569012_p7395159102016"></a><a name="zh-cn_topic_0225569012_p7395159102016"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row5395145913200"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p66771031236"><a name="zh-cn_topic_0225569012_p66771031236"></a><a name="zh-cn_topic_0225569012_p66771031236"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p196771135239"><a name="zh-cn_topic_0225569012_p196771135239"></a><a name="zh-cn_topic_0225569012_p196771135239"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p36776362318"><a name="zh-cn_topic_0225569012_p36776362318"></a><a name="zh-cn_topic_0225569012_p36776362318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p156776382310"><a name="zh-cn_topic_0225569012_p156776382310"></a><a name="zh-cn_topic_0225569012_p156776382310"></a>特殊流控策略类型，支持APP、USER</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row039555992011"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p1067716313239"><a name="zh-cn_topic_0225569012_p1067716313239"></a><a name="zh-cn_topic_0225569012_p1067716313239"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p667714382310"><a name="zh-cn_topic_0225569012_p667714382310"></a><a name="zh-cn_topic_0225569012_p667714382310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p10677103182319"><a name="zh-cn_topic_0225569012_p10677103182319"></a><a name="zh-cn_topic_0225569012_p10677103182319"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p196774372313"><a name="zh-cn_topic_0225569012_p196774372313"></a><a name="zh-cn_topic_0225569012_p196774372313"></a>访问次数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row12396145952012"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225569012_p267715319237"><a name="zh-cn_topic_0225569012_p267715319237"></a><a name="zh-cn_topic_0225569012_p267715319237"></a>instance</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225569012_p1067793172317"><a name="zh-cn_topic_0225569012_p1067793172317"></a><a name="zh-cn_topic_0225569012_p1067793172317"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225569012_p46777362318"><a name="zh-cn_topic_0225569012_p46777362318"></a><a name="zh-cn_topic_0225569012_p46777362318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225569012_p76776332319"><a name="zh-cn_topic_0225569012_p76776332319"></a><a name="zh-cn_topic_0225569012_p76776332319"></a>特殊APP或USER的对象标识</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"swagger": "2.0",
	"info": {
		"description": "api group test",
		"title": "APIGroup_test",
		"version": "2019-09-12-17:38:10"
	},
	"host": "6b075335476a4943bf70c3db1343c912.apigw.example.com",
	"paths": {
		"/test/{path}": {
			"get": {
				"security": [
					{
						"apig-auth-app": []
					}
				],
				"description": "api test",
				"schemes": [
					"https"
				],
				"operationId": "API_test",
				"parameters": [
					{
						"type": "string",
						"description": "header parameter",
						"name": "header",
						"in": "header",
						"required": true
					},
					{
						"type": "string",
						"description": "path parameter",
						"name": "path",
						"in": "path",
						"required": true
					},
					{
						"type": "number",
						"default": "123",
						"description": "query parameter",
						"name": "query",
						"in": "query"
					}
				],
				"responses": {
					"default": {
						"$ref": "#/responses/default"
					},
					"x-apigateway-result-failure-sample": "",
					"x-apigateway-result-normal-sample": "success"
				},
				"x-apigateway-backend": {
					"httpEndpoints": {
						"address": "1.1.1.1:443",
						"description": "",
						"method": "GET",
						"path": "/test/{path}",
						"scheme": "https",
						"timeout": 5000
					},
					"parameters": [
						{
							"description": "",
							"in": "HEADER",
							"name": "header",
							"origin": "REQUEST",
							"value": "header"
						},
						{
							"description": "",
							"in": "PATH",
							"name": "path",
							"origin": "REQUEST",
							"value": "path"
						},
						{
							"description": "",
							"in": "QUERY",
							"name": "query",
							"origin": "REQUEST",
							"value": "query"
						}
					],
					"type": "HTTP"
				},
				"x-apigateway-backend-policies": [
					{
						"conditions": [
							{
								"origin": "param",
								"parameter": "path",
								"type": "exact",
								"value": "path"
							},
							{
								"origin": "source",
								"parameter": "",
								"type": "",
								"value": "1.0.0.0/8"
							}
						],
						"effectMode": "ANY",
						"httpVpcEndpoints": {
							"method": "POST",
							"name": "VPC_n9ct",
							"path": "/",
							"scheme": "HTTPS",
							"timeout": 5000
						},
						"name": "policy_test",
						"type": "HTTP-VPC"
					}
				],
				"x-apigateway-cors": false,
				"x-apigateway-match-mode": "NORMAL",
				"x-apigateway-request-type": "public"
			}
		}
	},
	"responses": {
		"default": {
			"description": "response example"
		}
	},
	"securityDefinitions": {
		"apig-auth-app": {
			"type": "apiKey",
			"name": "Authorization",
			"in": "header",
			"x-apigateway-auth-type": "AppSigv1"
		},
		"apig-auth-iam": {
			"type": "apiKey",
			"name": "unused",
			"in": "header",
			"x-apigateway-auth-type": "IAM"
		}
	}
}
```

## 响应码<a name="zh-cn_topic_0225569012_section66318442384"></a>

**表 29**  返回消息说明

<a name="zh-cn_topic_0225569012_table11438104424617"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225569012_row1643820448464"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225569012_p4272113476"><a name="zh-cn_topic_0225569012_p4272113476"></a><a name="zh-cn_topic_0225569012_p4272113476"></a>响应码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225569012_p202192154718"><a name="zh-cn_topic_0225569012_p202192154718"></a><a name="zh-cn_topic_0225569012_p202192154718"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225569012_row24383446462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569012_p62162184714"><a name="zh-cn_topic_0225569012_p62162184714"></a><a name="zh-cn_topic_0225569012_p62162184714"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569012_p112162113475"><a name="zh-cn_topic_0225569012_p112162113475"></a><a name="zh-cn_topic_0225569012_p112162113475"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row6438154417469"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569012_p1228216472"><a name="zh-cn_topic_0225569012_p1228216472"></a><a name="zh-cn_topic_0225569012_p1228216472"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569012_p132182116477"><a name="zh-cn_topic_0225569012_p132182116477"></a><a name="zh-cn_topic_0225569012_p132182116477"></a>bad request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1943874416467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569012_p12262144711"><a name="zh-cn_topic_0225569012_p12262144711"></a><a name="zh-cn_topic_0225569012_p12262144711"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569012_p20220215475"><a name="zh-cn_topic_0225569012_p20220215475"></a><a name="zh-cn_topic_0225569012_p20220215475"></a>unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row1043834417462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569012_p1292117477"><a name="zh-cn_topic_0225569012_p1292117477"></a><a name="zh-cn_topic_0225569012_p1292117477"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569012_p32921144714"><a name="zh-cn_topic_0225569012_p32921144714"></a><a name="zh-cn_topic_0225569012_p32921144714"></a>forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225569012_row6439344194617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225569012_p7282116471"><a name="zh-cn_topic_0225569012_p7282116471"></a><a name="zh-cn_topic_0225569012_p7282116471"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225569012_p62112110471"><a name="zh-cn_topic_0225569012_p62112110471"></a><a name="zh-cn_topic_0225569012_p62112110471"></a>server internal error</p>
</td>
</tr>
</tbody>
</table>

