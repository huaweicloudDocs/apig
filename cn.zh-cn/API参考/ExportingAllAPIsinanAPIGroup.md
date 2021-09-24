# 导出分组下所有API<a name="ZH-CN_TOPIC_0000001081976155"></a>

## 功能介绍<a name="zh-cn_topic_0128578015_section39777523194"></a>

提供用户导出API定义的接口。

导出指定分组指定环境中发布的API的基础/全量/扩展Swagger定义。

## URI<a name="zh-cn_topic_0128578015_section16371135218203"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0128578015_table11507134785618"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row1150904725614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0128578015_p75091547155615"><a name="zh-cn_topic_0128578015_p75091547155615"></a><a name="zh-cn_topic_0128578015_p75091547155615"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0128578015_p16509947105618"><a name="zh-cn_topic_0128578015_p16509947105618"></a><a name="zh-cn_topic_0128578015_p16509947105618"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row450934716564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0128578015_p14509154711566"><a name="zh-cn_topic_0128578015_p14509154711566"></a><a name="zh-cn_topic_0128578015_p14509154711566"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0128578015_p1213518364578"><a name="zh-cn_topic_0128578015_p1213518364578"></a><a name="zh-cn_topic_0128578015_p1213518364578"></a>/v1.0/apigw/openapi?env_id={0}&amp;group_id={1}&amp;define={2}&amp;version={3}&amp;type={4}</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0128578015_section178868115223"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0128578015_table871144945810"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row14734499589"><th class="cellrowborder" valign="top" width="16.831683168316832%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p1973174918589"><a name="zh-cn_topic_0128578015_p1973174918589"></a><a name="zh-cn_topic_0128578015_p1973174918589"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.341534153415342%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p4731749125817"><a name="zh-cn_topic_0128578015_p4731749125817"></a><a name="zh-cn_topic_0128578015_p4731749125817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.691369136913693%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p1730491589"><a name="zh-cn_topic_0128578015_p1730491589"></a><a name="zh-cn_topic_0128578015_p1730491589"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.13541354135414%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p1073649175817"><a name="zh-cn_topic_0128578015_p1073649175817"></a><a name="zh-cn_topic_0128578015_p1073649175817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row87315493588"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p173061841314"><a name="zh-cn_topic_0128578015_p173061841314"></a><a name="zh-cn_topic_0128578015_p173061841314"></a>env_id/env</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p969851813"><a name="zh-cn_topic_0128578015_p969851813"></a><a name="zh-cn_topic_0128578015_p969851813"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p26925114116"><a name="zh-cn_topic_0128578015_p26925114116"></a><a name="zh-cn_topic_0128578015_p26925114116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p19691651310"><a name="zh-cn_topic_0128578015_p19691651310"></a><a name="zh-cn_topic_0128578015_p19691651310"></a>API分组发布的环境ID，目前支持env_id和env，两个均存在时以env_id为准，建议使用env_id</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row197434912586"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p16306144114116"><a name="zh-cn_topic_0128578015_p16306144114116"></a><a name="zh-cn_topic_0128578015_p16306144114116"></a>group_id/group</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p126913519113"><a name="zh-cn_topic_0128578015_p126913519113"></a><a name="zh-cn_topic_0128578015_p126913519113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p369125113111"><a name="zh-cn_topic_0128578015_p369125113111"></a><a name="zh-cn_topic_0128578015_p369125113111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p86912517116"><a name="zh-cn_topic_0128578015_p86912517116"></a><a name="zh-cn_topic_0128578015_p86912517116"></a>API分组ID，目前支持group_id和group，两个均存在时以group_id为准，建议使用group_id</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row67415491585"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p83064412117"><a name="zh-cn_topic_0128578015_p83064412117"></a><a name="zh-cn_topic_0128578015_p83064412117"></a>define</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p3691511113"><a name="zh-cn_topic_0128578015_p3691511113"></a><a name="zh-cn_topic_0128578015_p3691511113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p6697511314"><a name="zh-cn_topic_0128578015_p6697511314"></a><a name="zh-cn_topic_0128578015_p6697511314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p294920378347"><a name="zh-cn_topic_0128578015_p294920378347"></a><a name="zh-cn_topic_0128578015_p294920378347"></a>导出API的定义范围：</p>
<a name="zh-cn_topic_0128578015_ul169331437173420"></a><a name="zh-cn_topic_0128578015_ul169331437173420"></a><ul id="zh-cn_topic_0128578015_ul169331437173420"><li>base：基础定义</li><li>full：全量定义</li><li>all：扩展定义</li></ul>
<p id="zh-cn_topic_0128578015_p184466500348"><a name="zh-cn_topic_0128578015_p184466500348"></a><a name="zh-cn_topic_0128578015_p184466500348"></a>默认为base</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row8723131211572"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p147231112105720"><a name="zh-cn_topic_0128578015_p147231112105720"></a><a name="zh-cn_topic_0128578015_p147231112105720"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p16723512135714"><a name="zh-cn_topic_0128578015_p16723512135714"></a><a name="zh-cn_topic_0128578015_p16723512135714"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p8723712115711"><a name="zh-cn_topic_0128578015_p8723712115711"></a><a name="zh-cn_topic_0128578015_p8723712115711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1972317129578"><a name="zh-cn_topic_0128578015_p1972317129578"></a><a name="zh-cn_topic_0128578015_p1972317129578"></a>导出的API定义版本，默认为当前时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row14825155574"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p178210154576"><a name="zh-cn_topic_0128578015_p178210154576"></a><a name="zh-cn_topic_0128578015_p178210154576"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p68241555711"><a name="zh-cn_topic_0128578015_p68241555711"></a><a name="zh-cn_topic_0128578015_p68241555711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p4821315105719"><a name="zh-cn_topic_0128578015_p4821315105719"></a><a name="zh-cn_topic_0128578015_p4821315105719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p68281565719"><a name="zh-cn_topic_0128578015_p68281565719"></a><a name="zh-cn_topic_0128578015_p68281565719"></a>导出的API定义的格式：json/yaml，默认为json</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0128578015_section526345615258"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0128578015_table26691411183213"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row18670201115326"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p186708117326"><a name="zh-cn_topic_0128578015_p186708117326"></a><a name="zh-cn_topic_0128578015_p186708117326"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p1867014116325"><a name="zh-cn_topic_0128578015_p1867014116325"></a><a name="zh-cn_topic_0128578015_p1867014116325"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p176701911203219"><a name="zh-cn_topic_0128578015_p176701911203219"></a><a name="zh-cn_topic_0128578015_p176701911203219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.44554455445545%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p0670141143214"><a name="zh-cn_topic_0128578015_p0670141143214"></a><a name="zh-cn_topic_0128578015_p0670141143214"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row1567014117329"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p067014119324"><a name="zh-cn_topic_0128578015_p067014119324"></a><a name="zh-cn_topic_0128578015_p067014119324"></a>swagger</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p867031143220"><a name="zh-cn_topic_0128578015_p867031143220"></a><a name="zh-cn_topic_0128578015_p867031143220"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p66706117322"><a name="zh-cn_topic_0128578015_p66706117322"></a><a name="zh-cn_topic_0128578015_p66706117322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p567051133218"><a name="zh-cn_topic_0128578015_p567051133218"></a><a name="zh-cn_topic_0128578015_p567051133218"></a>固定值2.0</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row12670141173215"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p10670161193210"><a name="zh-cn_topic_0128578015_p10670161193210"></a><a name="zh-cn_topic_0128578015_p10670161193210"></a>info</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1067051133211"><a name="zh-cn_topic_0128578015_p1067051133211"></a><a name="zh-cn_topic_0128578015_p1067051133211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p667171173218"><a name="zh-cn_topic_0128578015_p667171173218"></a><a name="zh-cn_topic_0128578015_p667171173218"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1167111115320"><a name="zh-cn_topic_0128578015_p1167111115320"></a><a name="zh-cn_topic_0128578015_p1167111115320"></a>参考<a href="#zh-cn_topic_0128578015_table13672201112325">表4</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row11671511173219"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p767110111324"><a name="zh-cn_topic_0128578015_p767110111324"></a><a name="zh-cn_topic_0128578015_p767110111324"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p4671111153217"><a name="zh-cn_topic_0128578015_p4671111153217"></a><a name="zh-cn_topic_0128578015_p4671111153217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p156711411143212"><a name="zh-cn_topic_0128578015_p156711411143212"></a><a name="zh-cn_topic_0128578015_p156711411143212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p176717117325"><a name="zh-cn_topic_0128578015_p176717117325"></a><a name="zh-cn_topic_0128578015_p176717117325"></a>API分组绑定的子域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row15671191163213"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1767151117329"><a name="zh-cn_topic_0128578015_p1767151117329"></a><a name="zh-cn_topic_0128578015_p1767151117329"></a>paths</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p16711411183212"><a name="zh-cn_topic_0128578015_p16711411183212"></a><a name="zh-cn_topic_0128578015_p16711411183212"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p196711811143218"><a name="zh-cn_topic_0128578015_p196711811143218"></a><a name="zh-cn_topic_0128578015_p196711811143218"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1067121116324"><a name="zh-cn_topic_0128578015_p1067121116324"></a><a name="zh-cn_topic_0128578015_p1067121116324"></a>参考<a href="#zh-cn_topic_0128578015_table76741113321">表 paths参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row14671191173212"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p19671911103219"><a name="zh-cn_topic_0128578015_p19671911103219"></a><a name="zh-cn_topic_0128578015_p19671911103219"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p9671191123213"><a name="zh-cn_topic_0128578015_p9671191123213"></a><a name="zh-cn_topic_0128578015_p9671191123213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p16710118329"><a name="zh-cn_topic_0128578015_p16710118329"></a><a name="zh-cn_topic_0128578015_p16710118329"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p96712110328"><a name="zh-cn_topic_0128578015_p96712110328"></a><a name="zh-cn_topic_0128578015_p96712110328"></a>公用响应定义，可以被引用在{method}的操作中，参考<a href="#zh-cn_topic_0128578015_table10688811153215">表9</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row10671101133216"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1567113114328"><a name="zh-cn_topic_0128578015_p1567113114328"></a><a name="zh-cn_topic_0128578015_p1567113114328"></a>securityDefinitions</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p106711311193220"><a name="zh-cn_topic_0128578015_p106711311193220"></a><a name="zh-cn_topic_0128578015_p106711311193220"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p156711211163220"><a name="zh-cn_topic_0128578015_p156711211163220"></a><a name="zh-cn_topic_0128578015_p156711211163220"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p76711111153216"><a name="zh-cn_topic_0128578015_p76711111153216"></a><a name="zh-cn_topic_0128578015_p76711111153216"></a>定义鉴权方式，参考<a href="#zh-cn_topic_0128578015_table20698111119323">表13</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row15840124816259"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1884194822510"><a name="zh-cn_topic_0128578015_p1884194822510"></a><a name="zh-cn_topic_0128578015_p1884194822510"></a>x-apigateway-access-controls</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p13841148172510"><a name="zh-cn_topic_0128578015_p13841148172510"></a><a name="zh-cn_topic_0128578015_p13841148172510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1784154813256"><a name="zh-cn_topic_0128578015_p1784154813256"></a><a name="zh-cn_topic_0128578015_p1784154813256"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p384164813253"><a name="zh-cn_topic_0128578015_p384164813253"></a><a name="zh-cn_topic_0128578015_p384164813253"></a>访问控制信息，参考<a href="#zh-cn_topic_0128578015_table2090754816252">表 x-apigateway-access-controls参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row684144814253"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p98411348102518"><a name="zh-cn_topic_0128578015_p98411348102518"></a><a name="zh-cn_topic_0128578015_p98411348102518"></a>x-apigateway-ratelimits</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p13841134852518"><a name="zh-cn_topic_0128578015_p13841134852518"></a><a name="zh-cn_topic_0128578015_p13841134852518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p178411048152517"><a name="zh-cn_topic_0128578015_p178411048152517"></a><a name="zh-cn_topic_0128578015_p178411048152517"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p28411648202513"><a name="zh-cn_topic_0128578015_p28411648202513"></a><a name="zh-cn_topic_0128578015_p28411648202513"></a>流量控制信息，参考<a href="#zh-cn_topic_0128578015_table18913124872513">表 x-apigateway-ratelimits参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 4**  info参数说明

<a name="zh-cn_topic_0128578015_table13672201112325"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row6673111113210"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p1167301173215"><a name="zh-cn_topic_0128578015_p1167301173215"></a><a name="zh-cn_topic_0128578015_p1167301173215"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p15673181103217"><a name="zh-cn_topic_0128578015_p15673181103217"></a><a name="zh-cn_topic_0128578015_p15673181103217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p86731811143212"><a name="zh-cn_topic_0128578015_p86731811143212"></a><a name="zh-cn_topic_0128578015_p86731811143212"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p16731611193211"><a name="zh-cn_topic_0128578015_p16731611193211"></a><a name="zh-cn_topic_0128578015_p16731611193211"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row0673161173211"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p4673151103216"><a name="zh-cn_topic_0128578015_p4673151103216"></a><a name="zh-cn_topic_0128578015_p4673151103216"></a>title</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p10673101114324"><a name="zh-cn_topic_0128578015_p10673101114324"></a><a name="zh-cn_topic_0128578015_p10673101114324"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1367361133218"><a name="zh-cn_topic_0128578015_p1367361133218"></a><a name="zh-cn_topic_0128578015_p1367361133218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p136731011193213"><a name="zh-cn_topic_0128578015_p136731011193213"></a><a name="zh-cn_topic_0128578015_p136731011193213"></a>API分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row15673411133218"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p16673101117323"><a name="zh-cn_topic_0128578015_p16673101117323"></a><a name="zh-cn_topic_0128578015_p16673101117323"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p136730119321"><a name="zh-cn_topic_0128578015_p136730119321"></a><a name="zh-cn_topic_0128578015_p136730119321"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p13673181153216"><a name="zh-cn_topic_0128578015_p13673181153216"></a><a name="zh-cn_topic_0128578015_p13673181153216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p19673141133214"><a name="zh-cn_topic_0128578015_p19673141133214"></a><a name="zh-cn_topic_0128578015_p19673141133214"></a>版本号，用户输入自定义版本号或者使用默认的当前时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row116733119323"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p76731611133217"><a name="zh-cn_topic_0128578015_p76731611133217"></a><a name="zh-cn_topic_0128578015_p76731611133217"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1667391117325"><a name="zh-cn_topic_0128578015_p1667391117325"></a><a name="zh-cn_topic_0128578015_p1667391117325"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p0673171183214"><a name="zh-cn_topic_0128578015_p0673171183214"></a><a name="zh-cn_topic_0128578015_p0673171183214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p196731811123210"><a name="zh-cn_topic_0128578015_p196731811123210"></a><a name="zh-cn_topic_0128578015_p196731811123210"></a>分组描述信息</p>
</td>
</tr>
</tbody>
</table>

**表 5**  paths参数说明

<a name="zh-cn_topic_0128578015_table76741113321"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row166745112325"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p767471123213"><a name="zh-cn_topic_0128578015_p767471123213"></a><a name="zh-cn_topic_0128578015_p767471123213"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p66741511133219"><a name="zh-cn_topic_0128578015_p66741511133219"></a><a name="zh-cn_topic_0128578015_p66741511133219"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p1067481133216"><a name="zh-cn_topic_0128578015_p1067481133216"></a><a name="zh-cn_topic_0128578015_p1067481133216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p116747117329"><a name="zh-cn_topic_0128578015_p116747117329"></a><a name="zh-cn_topic_0128578015_p116747117329"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row76751911103212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p12675101183210"><a name="zh-cn_topic_0128578015_p12675101183210"></a><a name="zh-cn_topic_0128578015_p12675101183210"></a>uri</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p10675161163217"><a name="zh-cn_topic_0128578015_p10675161163217"></a><a name="zh-cn_topic_0128578015_p10675161163217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p12675171123219"><a name="zh-cn_topic_0128578015_p12675171123219"></a><a name="zh-cn_topic_0128578015_p12675171123219"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p17675101110324"><a name="zh-cn_topic_0128578015_p17675101110324"></a><a name="zh-cn_topic_0128578015_p17675101110324"></a>API访问地址，参考<a href="#zh-cn_topic_0128578015_table126750112327">表6</a></p>
</td>
</tr>
</tbody>
</table>

**表 6**  uri参数说明

<a name="zh-cn_topic_0128578015_table126750112327"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row20675311123213"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p10675311153215"><a name="zh-cn_topic_0128578015_p10675311153215"></a><a name="zh-cn_topic_0128578015_p10675311153215"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p146751411123216"><a name="zh-cn_topic_0128578015_p146751411123216"></a><a name="zh-cn_topic_0128578015_p146751411123216"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p367510118325"><a name="zh-cn_topic_0128578015_p367510118325"></a><a name="zh-cn_topic_0128578015_p367510118325"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p667671173215"><a name="zh-cn_topic_0128578015_p667671173215"></a><a name="zh-cn_topic_0128578015_p667671173215"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row15676911173212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p0676131173214"><a name="zh-cn_topic_0128578015_p0676131173214"></a><a name="zh-cn_topic_0128578015_p0676131173214"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1676611193214"><a name="zh-cn_topic_0128578015_p1676611193214"></a><a name="zh-cn_topic_0128578015_p1676611193214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p16676151143220"><a name="zh-cn_topic_0128578015_p16676151143220"></a><a name="zh-cn_topic_0128578015_p16676151143220"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p867621163218"><a name="zh-cn_topic_0128578015_p867621163218"></a><a name="zh-cn_topic_0128578015_p867621163218"></a>API访问方法，参考<a href="#zh-cn_topic_0128578015_table4676711113211">表7</a></p>
</td>
</tr>
</tbody>
</table>

**表 7**  method参数说明

<a name="zh-cn_topic_0128578015_table4676711113211"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row12676111173219"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p13676201119326"><a name="zh-cn_topic_0128578015_p13676201119326"></a><a name="zh-cn_topic_0128578015_p13676201119326"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p126761411133212"><a name="zh-cn_topic_0128578015_p126761411133212"></a><a name="zh-cn_topic_0128578015_p126761411133212"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p15676111153210"><a name="zh-cn_topic_0128578015_p15676111153210"></a><a name="zh-cn_topic_0128578015_p15676111153210"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p106761111323"><a name="zh-cn_topic_0128578015_p106761111323"></a><a name="zh-cn_topic_0128578015_p106761111323"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row12849144802517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p08503484253"><a name="zh-cn_topic_0128578015_p08503484253"></a><a name="zh-cn_topic_0128578015_p08503484253"></a>operationId</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p0850204842510"><a name="zh-cn_topic_0128578015_p0850204842510"></a><a name="zh-cn_topic_0128578015_p0850204842510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p085094842516"><a name="zh-cn_topic_0128578015_p085094842516"></a><a name="zh-cn_topic_0128578015_p085094842516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p485094872511"><a name="zh-cn_topic_0128578015_p485094872511"></a><a name="zh-cn_topic_0128578015_p485094872511"></a>API的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row2677161110322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p18677111113217"><a name="zh-cn_topic_0128578015_p18677111113217"></a><a name="zh-cn_topic_0128578015_p18677111113217"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1367731117322"><a name="zh-cn_topic_0128578015_p1367731117322"></a><a name="zh-cn_topic_0128578015_p1367731117322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p186771311163220"><a name="zh-cn_topic_0128578015_p186771311163220"></a><a name="zh-cn_topic_0128578015_p186771311163220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p76771111193215"><a name="zh-cn_topic_0128578015_p76771111193215"></a><a name="zh-cn_topic_0128578015_p76771111193215"></a>API的描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row967712119324"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p06775117324"><a name="zh-cn_topic_0128578015_p06775117324"></a><a name="zh-cn_topic_0128578015_p06775117324"></a>schemes</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1267710115326"><a name="zh-cn_topic_0128578015_p1267710115326"></a><a name="zh-cn_topic_0128578015_p1267710115326"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p9678911163213"><a name="zh-cn_topic_0128578015_p9678911163213"></a><a name="zh-cn_topic_0128578015_p9678911163213"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1678151173216"><a name="zh-cn_topic_0128578015_p1678151173216"></a><a name="zh-cn_topic_0128578015_p1678151173216"></a>API的请求协议对象数组定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row8664174194720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1617514115018"><a name="zh-cn_topic_0128578015_p1617514115018"></a><a name="zh-cn_topic_0128578015_p1617514115018"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p18175144135015"><a name="zh-cn_topic_0128578015_p18175144135015"></a><a name="zh-cn_topic_0128578015_p18175144135015"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1717614445015"><a name="zh-cn_topic_0128578015_p1717614445015"></a><a name="zh-cn_topic_0128578015_p1717614445015"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p191765465013"><a name="zh-cn_topic_0128578015_p191765465013"></a><a name="zh-cn_topic_0128578015_p191765465013"></a>API标签对象数组定义</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row14678171111326"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p167817111329"><a name="zh-cn_topic_0128578015_p167817111329"></a><a name="zh-cn_topic_0128578015_p167817111329"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p367881110322"><a name="zh-cn_topic_0128578015_p367881110322"></a><a name="zh-cn_topic_0128578015_p367881110322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p86782118325"><a name="zh-cn_topic_0128578015_p86782118325"></a><a name="zh-cn_topic_0128578015_p86782118325"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p13678511133220"><a name="zh-cn_topic_0128578015_p13678511133220"></a><a name="zh-cn_topic_0128578015_p13678511133220"></a>请求参数对象数组定义，参考<a href="#zh-cn_topic_0128578015_table36830118324">表 前端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row12678411183218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p13678191119326"><a name="zh-cn_topic_0128578015_p13678191119326"></a><a name="zh-cn_topic_0128578015_p13678191119326"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p46782111321"><a name="zh-cn_topic_0128578015_p46782111321"></a><a name="zh-cn_topic_0128578015_p46782111321"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p66781811133211"><a name="zh-cn_topic_0128578015_p66781811133211"></a><a name="zh-cn_topic_0128578015_p66781811133211"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1467891115325"><a name="zh-cn_topic_0128578015_p1467891115325"></a><a name="zh-cn_topic_0128578015_p1467891115325"></a>响应定义，参考<a href="#zh-cn_topic_0128578015_table10688811153215">表9</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row6852144810252"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p15852648132516"><a name="zh-cn_topic_0128578015_p15852648132516"></a><a name="zh-cn_topic_0128578015_p15852648132516"></a>security</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p985254812519"><a name="zh-cn_topic_0128578015_p985254812519"></a><a name="zh-cn_topic_0128578015_p985254812519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p20852948192520"><a name="zh-cn_topic_0128578015_p20852948192520"></a><a name="zh-cn_topic_0128578015_p20852948192520"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1185244832513"><a name="zh-cn_topic_0128578015_p1185244832513"></a><a name="zh-cn_topic_0128578015_p1185244832513"></a>API的认证类型对象数组定义，参考<a href="#zh-cn_topic_0128578015_table986594862513">表 security参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row185314892514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p8853748182515"><a name="zh-cn_topic_0128578015_p8853748182515"></a><a name="zh-cn_topic_0128578015_p8853748182515"></a>x-apigateway-access-control</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p18853114818258"><a name="zh-cn_topic_0128578015_p18853114818258"></a><a name="zh-cn_topic_0128578015_p18853114818258"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p885316488254"><a name="zh-cn_topic_0128578015_p885316488254"></a><a name="zh-cn_topic_0128578015_p885316488254"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p885318487254"><a name="zh-cn_topic_0128578015_p885318487254"></a><a name="zh-cn_topic_0128578015_p885318487254"></a>API绑定的访问控制对象数组定义</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row11853104814258"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1385324810256"><a name="zh-cn_topic_0128578015_p1385324810256"></a><a name="zh-cn_topic_0128578015_p1385324810256"></a>x-apigateway-backend</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p7853248172514"><a name="zh-cn_topic_0128578015_p7853248172514"></a><a name="zh-cn_topic_0128578015_p7853248172514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p6853184852511"><a name="zh-cn_topic_0128578015_p6853184852511"></a><a name="zh-cn_topic_0128578015_p6853184852511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p4853174816257"><a name="zh-cn_topic_0128578015_p4853174816257"></a><a name="zh-cn_topic_0128578015_p4853174816257"></a>API的后端信息，参考<a href="#zh-cn_topic_0128578015_table387619483252">表 x-apigateway-backend参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1685384815256"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1485334813258"><a name="zh-cn_topic_0128578015_p1485334813258"></a><a name="zh-cn_topic_0128578015_p1485334813258"></a>x-apigateway-backend-policies</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p685464852511"><a name="zh-cn_topic_0128578015_p685464852511"></a><a name="zh-cn_topic_0128578015_p685464852511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p785419483251"><a name="zh-cn_topic_0128578015_p785419483251"></a><a name="zh-cn_topic_0128578015_p785419483251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p18541148122518"><a name="zh-cn_topic_0128578015_p18541148122518"></a><a name="zh-cn_topic_0128578015_p18541148122518"></a>API的策略后端信息，参考<a href="#zh-cn_topic_0128578015_table1988034862512">表 x-apigateway-backend-policies参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row6854164802518"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1285414488259"><a name="zh-cn_topic_0128578015_p1285414488259"></a><a name="zh-cn_topic_0128578015_p1285414488259"></a>x-apigateway-cors</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p13854104814259"><a name="zh-cn_topic_0128578015_p13854104814259"></a><a name="zh-cn_topic_0128578015_p13854104814259"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p198541648152518"><a name="zh-cn_topic_0128578015_p198541648152518"></a><a name="zh-cn_topic_0128578015_p198541648152518"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1985410480253"><a name="zh-cn_topic_0128578015_p1985410480253"></a><a name="zh-cn_topic_0128578015_p1985410480253"></a>是否支持跨域</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row16854154817253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p2085454816256"><a name="zh-cn_topic_0128578015_p2085454816256"></a><a name="zh-cn_topic_0128578015_p2085454816256"></a>x-apigateway-match-mode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p98551248162511"><a name="zh-cn_topic_0128578015_p98551248162511"></a><a name="zh-cn_topic_0128578015_p98551248162511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p14855948102517"><a name="zh-cn_topic_0128578015_p14855948102517"></a><a name="zh-cn_topic_0128578015_p14855948102517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p18551948122513"><a name="zh-cn_topic_0128578015_p18551948122513"></a><a name="zh-cn_topic_0128578015_p18551948122513"></a>API的匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row11855164832513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1885514480253"><a name="zh-cn_topic_0128578015_p1885514480253"></a><a name="zh-cn_topic_0128578015_p1885514480253"></a>x-apigateway-ratelimit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p5855648142511"><a name="zh-cn_topic_0128578015_p5855648142511"></a><a name="zh-cn_topic_0128578015_p5855648142511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p885504815254"><a name="zh-cn_topic_0128578015_p885504815254"></a><a name="zh-cn_topic_0128578015_p885504815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p15855124810253"><a name="zh-cn_topic_0128578015_p15855124810253"></a><a name="zh-cn_topic_0128578015_p15855124810253"></a>API绑定的流量控制名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row885554810255"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p5855144872514"><a name="zh-cn_topic_0128578015_p5855144872514"></a><a name="zh-cn_topic_0128578015_p5855144872514"></a>x-apigateway-request-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p4855144822512"><a name="zh-cn_topic_0128578015_p4855144822512"></a><a name="zh-cn_topic_0128578015_p4855144822512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p108550488256"><a name="zh-cn_topic_0128578015_p108550488256"></a><a name="zh-cn_topic_0128578015_p108550488256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p28561348162511"><a name="zh-cn_topic_0128578015_p28561348162511"></a><a name="zh-cn_topic_0128578015_p28561348162511"></a>API的类型</p>
</td>
</tr>
</tbody>
</table>

**表 8**  前端parameters参数说明

<a name="zh-cn_topic_0128578015_table36830118324"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row6684911173220"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p166841611163216"><a name="zh-cn_topic_0128578015_p166841611163216"></a><a name="zh-cn_topic_0128578015_p166841611163216"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p368431143218"><a name="zh-cn_topic_0128578015_p368431143218"></a><a name="zh-cn_topic_0128578015_p368431143218"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p18684311183214"><a name="zh-cn_topic_0128578015_p18684311183214"></a><a name="zh-cn_topic_0128578015_p18684311183214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p1468416118322"><a name="zh-cn_topic_0128578015_p1468416118322"></a><a name="zh-cn_topic_0128578015_p1468416118322"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row20684811123219"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p8684511173220"><a name="zh-cn_topic_0128578015_p8684511173220"></a><a name="zh-cn_topic_0128578015_p8684511173220"></a>maximum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p176841011123219"><a name="zh-cn_topic_0128578015_p176841011123219"></a><a name="zh-cn_topic_0128578015_p176841011123219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p868431114329"><a name="zh-cn_topic_0128578015_p868431114329"></a><a name="zh-cn_topic_0128578015_p868431114329"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p768491112320"><a name="zh-cn_topic_0128578015_p768491112320"></a><a name="zh-cn_topic_0128578015_p768491112320"></a>参数为数值类型时，最大参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1268571193217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p196851211173217"><a name="zh-cn_topic_0128578015_p196851211173217"></a><a name="zh-cn_topic_0128578015_p196851211173217"></a>minimum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p126851311133213"><a name="zh-cn_topic_0128578015_p126851311133213"></a><a name="zh-cn_topic_0128578015_p126851311133213"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p106851611163214"><a name="zh-cn_topic_0128578015_p106851611163214"></a><a name="zh-cn_topic_0128578015_p106851611163214"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p166858113328"><a name="zh-cn_topic_0128578015_p166858113328"></a><a name="zh-cn_topic_0128578015_p166858113328"></a>参数为数值类型时，最小参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row468521173219"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1368511118323"><a name="zh-cn_topic_0128578015_p1368511118323"></a><a name="zh-cn_topic_0128578015_p1368511118323"></a>maxLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p186851611173215"><a name="zh-cn_topic_0128578015_p186851611173215"></a><a name="zh-cn_topic_0128578015_p186851611173215"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p2685131193212"><a name="zh-cn_topic_0128578015_p2685131193212"></a><a name="zh-cn_topic_0128578015_p2685131193212"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p068571123216"><a name="zh-cn_topic_0128578015_p068571123216"></a><a name="zh-cn_topic_0128578015_p068571123216"></a>参数为字符串类型时，参数的最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1868521153217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p166852011123219"><a name="zh-cn_topic_0128578015_p166852011123219"></a><a name="zh-cn_topic_0128578015_p166852011123219"></a>minLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1368531123219"><a name="zh-cn_topic_0128578015_p1368531123219"></a><a name="zh-cn_topic_0128578015_p1368531123219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p3685101193212"><a name="zh-cn_topic_0128578015_p3685101193212"></a><a name="zh-cn_topic_0128578015_p3685101193212"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p11685141114328"><a name="zh-cn_topic_0128578015_p11685141114328"></a><a name="zh-cn_topic_0128578015_p11685141114328"></a>参数为字符串类型时，参数的最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1868551183213"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p3685101117325"><a name="zh-cn_topic_0128578015_p3685101117325"></a><a name="zh-cn_topic_0128578015_p3685101117325"></a>pattern</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1868651116326"><a name="zh-cn_topic_0128578015_p1868651116326"></a><a name="zh-cn_topic_0128578015_p1868651116326"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p166861611163212"><a name="zh-cn_topic_0128578015_p166861611163212"></a><a name="zh-cn_topic_0128578015_p166861611163212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1686181111329"><a name="zh-cn_topic_0128578015_p1686181111329"></a><a name="zh-cn_topic_0128578015_p1686181111329"></a>参数值为正则匹配表达式</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row106861511153212"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p12686191123215"><a name="zh-cn_topic_0128578015_p12686191123215"></a><a name="zh-cn_topic_0128578015_p12686191123215"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1868601183216"><a name="zh-cn_topic_0128578015_p1868601183216"></a><a name="zh-cn_topic_0128578015_p1868601183216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p46861111193213"><a name="zh-cn_topic_0128578015_p46861111193213"></a><a name="zh-cn_topic_0128578015_p46861111193213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1368671111327"><a name="zh-cn_topic_0128578015_p1368671111327"></a><a name="zh-cn_topic_0128578015_p1368671111327"></a>参数类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row5686011103219"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p36867115328"><a name="zh-cn_topic_0128578015_p36867115328"></a><a name="zh-cn_topic_0128578015_p36867115328"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p13686171118322"><a name="zh-cn_topic_0128578015_p13686171118322"></a><a name="zh-cn_topic_0128578015_p13686171118322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1168641143213"><a name="zh-cn_topic_0128578015_p1168641143213"></a><a name="zh-cn_topic_0128578015_p1168641143213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p368691118328"><a name="zh-cn_topic_0128578015_p368691118328"></a><a name="zh-cn_topic_0128578015_p368691118328"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row8686161110323"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p3686151118323"><a name="zh-cn_topic_0128578015_p3686151118323"></a><a name="zh-cn_topic_0128578015_p3686151118323"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p136879113323"><a name="zh-cn_topic_0128578015_p136879113323"></a><a name="zh-cn_topic_0128578015_p136879113323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1168713119325"><a name="zh-cn_topic_0128578015_p1168713119325"></a><a name="zh-cn_topic_0128578015_p1168713119325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p10687131123219"><a name="zh-cn_topic_0128578015_p10687131123219"></a><a name="zh-cn_topic_0128578015_p10687131123219"></a>参数描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row11687171116324"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p06871611113220"><a name="zh-cn_topic_0128578015_p06871611113220"></a><a name="zh-cn_topic_0128578015_p06871611113220"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p14687611183220"><a name="zh-cn_topic_0128578015_p14687611183220"></a><a name="zh-cn_topic_0128578015_p14687611183220"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p6687101116325"><a name="zh-cn_topic_0128578015_p6687101116325"></a><a name="zh-cn_topic_0128578015_p6687101116325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1468791110328"><a name="zh-cn_topic_0128578015_p1468791110328"></a><a name="zh-cn_topic_0128578015_p1468791110328"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1468718119325"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p268711173220"><a name="zh-cn_topic_0128578015_p268711173220"></a><a name="zh-cn_topic_0128578015_p268711173220"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p176871811163215"><a name="zh-cn_topic_0128578015_p176871811163215"></a><a name="zh-cn_topic_0128578015_p176871811163215"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p468761115326"><a name="zh-cn_topic_0128578015_p468761115326"></a><a name="zh-cn_topic_0128578015_p468761115326"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p18688171173216"><a name="zh-cn_topic_0128578015_p18688171173216"></a><a name="zh-cn_topic_0128578015_p18688171173216"></a>参数位置，支持path、header、query、formData、body</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row14688141120324"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p136885114325"><a name="zh-cn_topic_0128578015_p136885114325"></a><a name="zh-cn_topic_0128578015_p136885114325"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p168841143212"><a name="zh-cn_topic_0128578015_p168841143212"></a><a name="zh-cn_topic_0128578015_p168841143212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p568801111329"><a name="zh-cn_topic_0128578015_p568801111329"></a><a name="zh-cn_topic_0128578015_p568801111329"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p106881911103215"><a name="zh-cn_topic_0128578015_p106881911103215"></a><a name="zh-cn_topic_0128578015_p106881911103215"></a>参数是否必需，参数位置为path时必需</p>
</td>
</tr>
</tbody>
</table>

**表 9**  responses参数说明

<a name="zh-cn_topic_0128578015_table10688811153215"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row1688011113217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p36892112323"><a name="zh-cn_topic_0128578015_p36892112323"></a><a name="zh-cn_topic_0128578015_p36892112323"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p368919110326"><a name="zh-cn_topic_0128578015_p368919110326"></a><a name="zh-cn_topic_0128578015_p368919110326"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p8689161114326"><a name="zh-cn_topic_0128578015_p8689161114326"></a><a name="zh-cn_topic_0128578015_p8689161114326"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p1468981113214"><a name="zh-cn_topic_0128578015_p1468981113214"></a><a name="zh-cn_topic_0128578015_p1468981113214"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row1268901163218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p86896111320"><a name="zh-cn_topic_0128578015_p86896111320"></a><a name="zh-cn_topic_0128578015_p86896111320"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p368951114322"><a name="zh-cn_topic_0128578015_p368951114322"></a><a name="zh-cn_topic_0128578015_p368951114322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p106891118328"><a name="zh-cn_topic_0128578015_p106891118328"></a><a name="zh-cn_topic_0128578015_p106891118328"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p7689131120326"><a name="zh-cn_topic_0128578015_p7689131120326"></a><a name="zh-cn_topic_0128578015_p7689131120326"></a>缺省响应，描述未定义的响应码</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row206901911173220"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p66901211133216"><a name="zh-cn_topic_0128578015_p66901211133216"></a><a name="zh-cn_topic_0128578015_p66901211133216"></a>status_code</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p16690181119323"><a name="zh-cn_topic_0128578015_p16690181119323"></a><a name="zh-cn_topic_0128578015_p16690181119323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p8690611113216"><a name="zh-cn_topic_0128578015_p8690611113216"></a><a name="zh-cn_topic_0128578015_p8690611113216"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1169018115328"><a name="zh-cn_topic_0128578015_p1169018115328"></a><a name="zh-cn_topic_0128578015_p1169018115328"></a>响应状态码，值为响应对象，参考<a href="#zh-cn_topic_0128578015_table76941111143210">表11</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1774720508918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p774812501894"><a name="zh-cn_topic_0128578015_p774812501894"></a><a name="zh-cn_topic_0128578015_p774812501894"></a>x-apigateway-result-failure-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p474815020916"><a name="zh-cn_topic_0128578015_p474815020916"></a><a name="zh-cn_topic_0128578015_p474815020916"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p11749105017914"><a name="zh-cn_topic_0128578015_p11749105017914"></a><a name="zh-cn_topic_0128578015_p11749105017914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p14749750398"><a name="zh-cn_topic_0128578015_p14749750398"></a><a name="zh-cn_topic_0128578015_p14749750398"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row71795541897"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1117913541917"><a name="zh-cn_topic_0128578015_p1117913541917"></a><a name="zh-cn_topic_0128578015_p1117913541917"></a>x-apigateway-result-normal-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p517914541191"><a name="zh-cn_topic_0128578015_p517914541191"></a><a name="zh-cn_topic_0128578015_p517914541191"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p171791554493"><a name="zh-cn_topic_0128578015_p171791554493"></a><a name="zh-cn_topic_0128578015_p171791554493"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p111791154598"><a name="zh-cn_topic_0128578015_p111791154598"></a><a name="zh-cn_topic_0128578015_p111791154598"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
</tbody>
</table>

**表 10**  security参数说明

<a name="zh-cn_topic_0128578015_table986594862513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row086674852515"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p986654810257"><a name="zh-cn_topic_0128578015_p986654810257"></a><a name="zh-cn_topic_0128578015_p986654810257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p986624819250"><a name="zh-cn_topic_0128578015_p986624819250"></a><a name="zh-cn_topic_0128578015_p986624819250"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p188661348112516"><a name="zh-cn_topic_0128578015_p188661348112516"></a><a name="zh-cn_topic_0128578015_p188661348112516"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p14866248132510"><a name="zh-cn_topic_0128578015_p14866248132510"></a><a name="zh-cn_topic_0128578015_p14866248132510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row17866114810256"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p17771954155713"><a name="zh-cn_topic_0128578015_p17771954155713"></a><a name="zh-cn_topic_0128578015_p17771954155713"></a>apig-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1677354115716"><a name="zh-cn_topic_0128578015_p1677354115716"></a><a name="zh-cn_topic_0128578015_p1677354115716"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p87705410572"><a name="zh-cn_topic_0128578015_p87705410572"></a><a name="zh-cn_topic_0128578015_p87705410572"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p117713541579"><a name="zh-cn_topic_0128578015_p117713541579"></a><a name="zh-cn_topic_0128578015_p117713541579"></a>API的认证类型对象数组定义，为空数组</p>
<p id="zh-cn_topic_0128578015_p6722101419557"><a name="zh-cn_topic_0128578015_p6722101419557"></a><a name="zh-cn_topic_0128578015_p6722101419557"></a>apig-auth-type支持：</p>
<a name="zh-cn_topic_0128578015_ul3401225145518"></a><a name="zh-cn_topic_0128578015_ul3401225145518"></a><ul id="zh-cn_topic_0128578015_ul3401225145518"><li>APP认证： apig-auth-app</li><li>IAM认证：apig-auth-iam</li><li>NONE：不填写</li></ul>
</td>
</tr>
</tbody>
</table>

**表 11**  status code参数说明

<a name="zh-cn_topic_0128578015_table76941111143210"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row8694611133212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p1569401115329"><a name="zh-cn_topic_0128578015_p1569401115329"></a><a name="zh-cn_topic_0128578015_p1569401115329"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p15695101193210"><a name="zh-cn_topic_0128578015_p15695101193210"></a><a name="zh-cn_topic_0128578015_p15695101193210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p269521173215"><a name="zh-cn_topic_0128578015_p269521173215"></a><a name="zh-cn_topic_0128578015_p269521173215"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p17695161153216"><a name="zh-cn_topic_0128578015_p17695161153216"></a><a name="zh-cn_topic_0128578015_p17695161153216"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row1269591133216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1469518113321"><a name="zh-cn_topic_0128578015_p1469518113321"></a><a name="zh-cn_topic_0128578015_p1469518113321"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p56951311133214"><a name="zh-cn_topic_0128578015_p56951311133214"></a><a name="zh-cn_topic_0128578015_p56951311133214"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p166952117322"><a name="zh-cn_topic_0128578015_p166952117322"></a><a name="zh-cn_topic_0128578015_p166952117322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p156957111322"><a name="zh-cn_topic_0128578015_p156957111322"></a><a name="zh-cn_topic_0128578015_p156957111322"></a>响应描述信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row669517112325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p069571133216"><a name="zh-cn_topic_0128578015_p069571133216"></a><a name="zh-cn_topic_0128578015_p069571133216"></a>schema</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p176952116328"><a name="zh-cn_topic_0128578015_p176952116328"></a><a name="zh-cn_topic_0128578015_p176952116328"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p669671153211"><a name="zh-cn_topic_0128578015_p669671153211"></a><a name="zh-cn_topic_0128578015_p669671153211"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p569616114324"><a name="zh-cn_topic_0128578015_p569616114324"></a><a name="zh-cn_topic_0128578015_p569616114324"></a>响应正文定义，参考<a href="#zh-cn_topic_0128578015_table669611115329">表12</a></p>
</td>
</tr>
</tbody>
</table>

**表 12**  schema参数说明

<a name="zh-cn_topic_0128578015_table669611115329"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row1669620112329"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p8697111183220"><a name="zh-cn_topic_0128578015_p8697111183220"></a><a name="zh-cn_topic_0128578015_p8697111183220"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p1769712113328"><a name="zh-cn_topic_0128578015_p1769712113328"></a><a name="zh-cn_topic_0128578015_p1769712113328"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p8697311193217"><a name="zh-cn_topic_0128578015_p8697311193217"></a><a name="zh-cn_topic_0128578015_p8697311193217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p069781118329"><a name="zh-cn_topic_0128578015_p069781118329"></a><a name="zh-cn_topic_0128578015_p069781118329"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row176977117320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p669791114323"><a name="zh-cn_topic_0128578015_p669791114323"></a><a name="zh-cn_topic_0128578015_p669791114323"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1697141115325"><a name="zh-cn_topic_0128578015_p1697141115325"></a><a name="zh-cn_topic_0128578015_p1697141115325"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p16978113325"><a name="zh-cn_topic_0128578015_p16978113325"></a><a name="zh-cn_topic_0128578015_p16978113325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1369816118326"><a name="zh-cn_topic_0128578015_p1369816118326"></a><a name="zh-cn_topic_0128578015_p1369816118326"></a>BODY体描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row12698131143214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p169801116326"><a name="zh-cn_topic_0128578015_p169801116326"></a><a name="zh-cn_topic_0128578015_p169801116326"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p369811113323"><a name="zh-cn_topic_0128578015_p369811113323"></a><a name="zh-cn_topic_0128578015_p369811113323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p16698181163220"><a name="zh-cn_topic_0128578015_p16698181163220"></a><a name="zh-cn_topic_0128578015_p16698181163220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1698111183210"><a name="zh-cn_topic_0128578015_p1698111183210"></a><a name="zh-cn_topic_0128578015_p1698111183210"></a>BODY体类型：FORM/STREAM（表单/字节流）</p>
</td>
</tr>
</tbody>
</table>

**表 13**  securityDefinitions参数说明

<a name="zh-cn_topic_0128578015_table20698111119323"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row769913115322"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p5699171113327"><a name="zh-cn_topic_0128578015_p5699171113327"></a><a name="zh-cn_topic_0128578015_p5699171113327"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p66995116320"><a name="zh-cn_topic_0128578015_p66995116320"></a><a name="zh-cn_topic_0128578015_p66995116320"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p1699511113214"><a name="zh-cn_topic_0128578015_p1699511113214"></a><a name="zh-cn_topic_0128578015_p1699511113214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.46534653465347%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p16991111153212"><a name="zh-cn_topic_0128578015_p16991111153212"></a><a name="zh-cn_topic_0128578015_p16991111153212"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row8699911193217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p569913112328"><a name="zh-cn_topic_0128578015_p569913112328"></a><a name="zh-cn_topic_0128578015_p569913112328"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p569914119320"><a name="zh-cn_topic_0128578015_p569914119320"></a><a name="zh-cn_topic_0128578015_p569914119320"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p20699611123220"><a name="zh-cn_topic_0128578015_p20699611123220"></a><a name="zh-cn_topic_0128578015_p20699611123220"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="53.46534653465347%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1169951143212"><a name="zh-cn_topic_0128578015_p1169951143212"></a><a name="zh-cn_topic_0128578015_p1169951143212"></a>自定义鉴权方式名称，参考<a href="#zh-cn_topic_0128578015_table1969951114328">表14</a></p>
</td>
</tr>
</tbody>
</table>

**表 14**  name参数说明

<a name="zh-cn_topic_0128578015_table1969951114328"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row670031103213"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p170013113323"><a name="zh-cn_topic_0128578015_p170013113323"></a><a name="zh-cn_topic_0128578015_p170013113323"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p1670001114329"><a name="zh-cn_topic_0128578015_p1670001114329"></a><a name="zh-cn_topic_0128578015_p1670001114329"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p18700211113213"><a name="zh-cn_topic_0128578015_p18700211113213"></a><a name="zh-cn_topic_0128578015_p18700211113213"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p187006118322"><a name="zh-cn_topic_0128578015_p187006118322"></a><a name="zh-cn_topic_0128578015_p187006118322"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row117008118323"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1070061193217"><a name="zh-cn_topic_0128578015_p1070061193217"></a><a name="zh-cn_topic_0128578015_p1070061193217"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p070071153213"><a name="zh-cn_topic_0128578015_p070071153213"></a><a name="zh-cn_topic_0128578015_p070071153213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p20700121119320"><a name="zh-cn_topic_0128578015_p20700121119320"></a><a name="zh-cn_topic_0128578015_p20700121119320"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p6700201143210"><a name="zh-cn_topic_0128578015_p6700201143210"></a><a name="zh-cn_topic_0128578015_p6700201143210"></a>鉴权类型，支持apiKey</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1070071113210"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1701111103215"><a name="zh-cn_topic_0128578015_p1701111103215"></a><a name="zh-cn_topic_0128578015_p1701111103215"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p167015118329"><a name="zh-cn_topic_0128578015_p167015118329"></a><a name="zh-cn_topic_0128578015_p167015118329"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p970181120324"><a name="zh-cn_topic_0128578015_p970181120324"></a><a name="zh-cn_topic_0128578015_p970181120324"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p6701131117328"><a name="zh-cn_topic_0128578015_p6701131117328"></a><a name="zh-cn_topic_0128578015_p6701131117328"></a>apiKey参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row7701161117327"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p970111163211"><a name="zh-cn_topic_0128578015_p970111163211"></a><a name="zh-cn_topic_0128578015_p970111163211"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p270113118328"><a name="zh-cn_topic_0128578015_p270113118328"></a><a name="zh-cn_topic_0128578015_p270113118328"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p7701711113216"><a name="zh-cn_topic_0128578015_p7701711113216"></a><a name="zh-cn_topic_0128578015_p7701711113216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1701171118324"><a name="zh-cn_topic_0128578015_p1701171118324"></a><a name="zh-cn_topic_0128578015_p1701171118324"></a>apiKey参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row870191193211"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p14701111113219"><a name="zh-cn_topic_0128578015_p14701111113219"></a><a name="zh-cn_topic_0128578015_p14701111113219"></a>x-apigateway-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1870114116327"><a name="zh-cn_topic_0128578015_p1870114116327"></a><a name="zh-cn_topic_0128578015_p1870114116327"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1270220115323"><a name="zh-cn_topic_0128578015_p1270220115323"></a><a name="zh-cn_topic_0128578015_p1270220115323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p070231118324"><a name="zh-cn_topic_0128578015_p070231118324"></a><a name="zh-cn_topic_0128578015_p070231118324"></a>扩展鉴权类型，基于apiKey鉴权方式的扩展，网关自定义的鉴权方式，支持AppSigv1、IAM、IAM_NONE</p>
</td>
</tr>
</tbody>
</table>

**表 15**  x-apigateway-backend参数说明

<a name="zh-cn_topic_0128578015_table387619483252"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row1487734812520"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p487734814254"><a name="zh-cn_topic_0128578015_p487734814254"></a><a name="zh-cn_topic_0128578015_p487734814254"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p58771548122516"><a name="zh-cn_topic_0128578015_p58771548122516"></a><a name="zh-cn_topic_0128578015_p58771548122516"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p287774812511"><a name="zh-cn_topic_0128578015_p287774812511"></a><a name="zh-cn_topic_0128578015_p287774812511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p13877134815251"><a name="zh-cn_topic_0128578015_p13877134815251"></a><a name="zh-cn_topic_0128578015_p13877134815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row10877114822512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p2878144892516"><a name="zh-cn_topic_0128578015_p2878144892516"></a><a name="zh-cn_topic_0128578015_p2878144892516"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p15878648182515"><a name="zh-cn_topic_0128578015_p15878648182515"></a><a name="zh-cn_topic_0128578015_p15878648182515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p587811480258"><a name="zh-cn_topic_0128578015_p587811480258"></a><a name="zh-cn_topic_0128578015_p587811480258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p2878134802519"><a name="zh-cn_topic_0128578015_p2878134802519"></a><a name="zh-cn_topic_0128578015_p2878134802519"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row8878174811255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p187864862516"><a name="zh-cn_topic_0128578015_p187864862516"></a><a name="zh-cn_topic_0128578015_p187864862516"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p387834820252"><a name="zh-cn_topic_0128578015_p387834820252"></a><a name="zh-cn_topic_0128578015_p387834820252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p0878848142512"><a name="zh-cn_topic_0128578015_p0878848142512"></a><a name="zh-cn_topic_0128578015_p0878848142512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1887854802516"><a name="zh-cn_topic_0128578015_p1887854802516"></a><a name="zh-cn_topic_0128578015_p1887854802516"></a>后端参数对象数组定义，参考<a href="#zh-cn_topic_0128578015_table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1387834892518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1587934817256"><a name="zh-cn_topic_0128578015_p1587934817256"></a><a name="zh-cn_topic_0128578015_p1587934817256"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p587924822511"><a name="zh-cn_topic_0128578015_p587924822511"></a><a name="zh-cn_topic_0128578015_p587924822511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p20879124802513"><a name="zh-cn_topic_0128578015_p20879124802513"></a><a name="zh-cn_topic_0128578015_p20879124802513"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p19879134862517"><a name="zh-cn_topic_0128578015_p19879134862517"></a><a name="zh-cn_topic_0128578015_p19879134862517"></a>API后端定义</p>
<p id="zh-cn_topic_0128578015_p9879144815251"><a name="zh-cn_topic_0128578015_p9879144815251"></a><a name="zh-cn_topic_0128578015_p9879144815251"></a>backend_define支持：</p>
<a name="zh-cn_topic_0128578015_ul587916489258"></a><a name="zh-cn_topic_0128578015_ul587916489258"></a><ul id="zh-cn_topic_0128578015_ul587916489258"><li>httpEndpoints，参考<a href="#zh-cn_topic_0128578015_table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#zh-cn_topic_0128578015_table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#zh-cn_topic_0128578015_table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#zh-cn_topic_0128578015_table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
</tbody>
</table>

**表 16**  x-apigateway-backend-policies参数说明

<a name="zh-cn_topic_0128578015_table1988034862512"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row788004814256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p148801248112517"><a name="zh-cn_topic_0128578015_p148801248112517"></a><a name="zh-cn_topic_0128578015_p148801248112517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p28801048112514"><a name="zh-cn_topic_0128578015_p28801048112514"></a><a name="zh-cn_topic_0128578015_p28801048112514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p5880164872513"><a name="zh-cn_topic_0128578015_p5880164872513"></a><a name="zh-cn_topic_0128578015_p5880164872513"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p8881948132519"><a name="zh-cn_topic_0128578015_p8881948132519"></a><a name="zh-cn_topic_0128578015_p8881948132519"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row118811748112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p688117485256"><a name="zh-cn_topic_0128578015_p688117485256"></a><a name="zh-cn_topic_0128578015_p688117485256"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p688164822510"><a name="zh-cn_topic_0128578015_p688164822510"></a><a name="zh-cn_topic_0128578015_p688164822510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p178819481257"><a name="zh-cn_topic_0128578015_p178819481257"></a><a name="zh-cn_topic_0128578015_p178819481257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p13881448102510"><a name="zh-cn_topic_0128578015_p13881448102510"></a><a name="zh-cn_topic_0128578015_p13881448102510"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row9881134862515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p19881204822515"><a name="zh-cn_topic_0128578015_p19881204822515"></a><a name="zh-cn_topic_0128578015_p19881204822515"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1888114862515"><a name="zh-cn_topic_0128578015_p1888114862515"></a><a name="zh-cn_topic_0128578015_p1888114862515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p78817484250"><a name="zh-cn_topic_0128578015_p78817484250"></a><a name="zh-cn_topic_0128578015_p78817484250"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1588144814252"><a name="zh-cn_topic_0128578015_p1588144814252"></a><a name="zh-cn_topic_0128578015_p1588144814252"></a>后端策略名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row588184817258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p2882124882517"><a name="zh-cn_topic_0128578015_p2882124882517"></a><a name="zh-cn_topic_0128578015_p2882124882517"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p988244811251"><a name="zh-cn_topic_0128578015_p988244811251"></a><a name="zh-cn_topic_0128578015_p988244811251"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p5882248152519"><a name="zh-cn_topic_0128578015_p5882248152519"></a><a name="zh-cn_topic_0128578015_p5882248152519"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p188218488257"><a name="zh-cn_topic_0128578015_p188218488257"></a><a name="zh-cn_topic_0128578015_p188218488257"></a>后端参数对象数组定义，参考<a href="#zh-cn_topic_0128578015_table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1188204822510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p19882184892513"><a name="zh-cn_topic_0128578015_p19882184892513"></a><a name="zh-cn_topic_0128578015_p19882184892513"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p6882104862512"><a name="zh-cn_topic_0128578015_p6882104862512"></a><a name="zh-cn_topic_0128578015_p6882104862512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p138821548172512"><a name="zh-cn_topic_0128578015_p138821548172512"></a><a name="zh-cn_topic_0128578015_p138821548172512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p15882164816258"><a name="zh-cn_topic_0128578015_p15882164816258"></a><a name="zh-cn_topic_0128578015_p15882164816258"></a>API后端定义</p>
<p id="zh-cn_topic_0128578015_p188214481259"><a name="zh-cn_topic_0128578015_p188214481259"></a><a name="zh-cn_topic_0128578015_p188214481259"></a>backend_define支持：</p>
<a name="zh-cn_topic_0128578015_ul0883104814256"></a><a name="zh-cn_topic_0128578015_ul0883104814256"></a><ul id="zh-cn_topic_0128578015_ul0883104814256"><li>httpEndpoints，参考<a href="#zh-cn_topic_0128578015_table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#zh-cn_topic_0128578015_table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#zh-cn_topic_0128578015_table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#zh-cn_topic_0128578015_table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row48838483257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p18883948172520"><a name="zh-cn_topic_0128578015_p18883948172520"></a><a name="zh-cn_topic_0128578015_p18883948172520"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p6883184852518"><a name="zh-cn_topic_0128578015_p6883184852518"></a><a name="zh-cn_topic_0128578015_p6883184852518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p68846483259"><a name="zh-cn_topic_0128578015_p68846483259"></a><a name="zh-cn_topic_0128578015_p68846483259"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p988404813253"><a name="zh-cn_topic_0128578015_p988404813253"></a><a name="zh-cn_topic_0128578015_p988404813253"></a>策略条件对象数组定义，参考<a href="#zh-cn_topic_0128578015_table1790444832520">表 conditions参数说明</a></p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row8601019134513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1571041123212"><a name="zh-cn_topic_0128578015_p1571041123212"></a><a name="zh-cn_topic_0128578015_p1571041123212"></a>effectMode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p12710161117322"><a name="zh-cn_topic_0128578015_p12710161117322"></a><a name="zh-cn_topic_0128578015_p12710161117322"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1571131163218"><a name="zh-cn_topic_0128578015_p1571131163218"></a><a name="zh-cn_topic_0128578015_p1571131163218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p167111211143213"><a name="zh-cn_topic_0128578015_p167111211143213"></a><a name="zh-cn_topic_0128578015_p167111211143213"></a>关联的策略组合模式，支持ANY、ALL</p>
</td>
</tr>
</tbody>
</table>

**表 17**  后端parameters参数说明

<a name="zh-cn_topic_0128578015_table14884114882511"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row1088574822512"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p88856489251"><a name="zh-cn_topic_0128578015_p88856489251"></a><a name="zh-cn_topic_0128578015_p88856489251"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p18885048132510"><a name="zh-cn_topic_0128578015_p18885048132510"></a><a name="zh-cn_topic_0128578015_p18885048132510"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p19885124810250"><a name="zh-cn_topic_0128578015_p19885124810250"></a><a name="zh-cn_topic_0128578015_p19885124810250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p188851448172515"><a name="zh-cn_topic_0128578015_p188851448172515"></a><a name="zh-cn_topic_0128578015_p188851448172515"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row138861748112511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p788674832520"><a name="zh-cn_topic_0128578015_p788674832520"></a><a name="zh-cn_topic_0128578015_p788674832520"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p148868484256"><a name="zh-cn_topic_0128578015_p148868484256"></a><a name="zh-cn_topic_0128578015_p148868484256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1688664812515"><a name="zh-cn_topic_0128578015_p1688664812515"></a><a name="zh-cn_topic_0128578015_p1688664812515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p14886948102519"><a name="zh-cn_topic_0128578015_p14886948102519"></a><a name="zh-cn_topic_0128578015_p14886948102519"></a>参数名称，由字母、数字、下划线、连线、点组成，以字母开头，最长32字节</p>
<p id="zh-cn_topic_0128578015_p1988624813251"><a name="zh-cn_topic_0128578015_p1988624813251"></a><a name="zh-cn_topic_0128578015_p1988624813251"></a>header位置的参数名称不区分大小写</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row388674862513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1888620480254"><a name="zh-cn_topic_0128578015_p1888620480254"></a><a name="zh-cn_topic_0128578015_p1888620480254"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p98861548152515"><a name="zh-cn_topic_0128578015_p98861548152515"></a><a name="zh-cn_topic_0128578015_p98861548152515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p0886174810255"><a name="zh-cn_topic_0128578015_p0886174810255"></a><a name="zh-cn_topic_0128578015_p0886174810255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p19886748182513"><a name="zh-cn_topic_0128578015_p19886748182513"></a><a name="zh-cn_topic_0128578015_p19886748182513"></a>参数值，当参数来源为REQUEST时，值为请求参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row10886148132513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p13887134822517"><a name="zh-cn_topic_0128578015_p13887134822517"></a><a name="zh-cn_topic_0128578015_p13887134822517"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1788764862518"><a name="zh-cn_topic_0128578015_p1788764862518"></a><a name="zh-cn_topic_0128578015_p1788764862518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p18887164815251"><a name="zh-cn_topic_0128578015_p18887164815251"></a><a name="zh-cn_topic_0128578015_p18887164815251"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p8887174812258"><a name="zh-cn_topic_0128578015_p8887174812258"></a><a name="zh-cn_topic_0128578015_p8887174812258"></a>参数位置，支持header、query、path</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row788711486259"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p4887148182510"><a name="zh-cn_topic_0128578015_p4887148182510"></a><a name="zh-cn_topic_0128578015_p4887148182510"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1588714814252"><a name="zh-cn_topic_0128578015_p1588714814252"></a><a name="zh-cn_topic_0128578015_p1588714814252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p14887144815254"><a name="zh-cn_topic_0128578015_p14887144815254"></a><a name="zh-cn_topic_0128578015_p14887144815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p9887104882515"><a name="zh-cn_topic_0128578015_p9887104882515"></a><a name="zh-cn_topic_0128578015_p9887104882515"></a>参数映射来源，支持REQUEST、CONSTANT</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row10888204816254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1988894882514"><a name="zh-cn_topic_0128578015_p1988894882514"></a><a name="zh-cn_topic_0128578015_p1988894882514"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1788864811250"><a name="zh-cn_topic_0128578015_p1788864811250"></a><a name="zh-cn_topic_0128578015_p1788864811250"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1288854812255"><a name="zh-cn_topic_0128578015_p1288854812255"></a><a name="zh-cn_topic_0128578015_p1288854812255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p17888184822511"><a name="zh-cn_topic_0128578015_p17888184822511"></a><a name="zh-cn_topic_0128578015_p17888184822511"></a>参数含义描述</p>
</td>
</tr>
</tbody>
</table>

**表 18**  后端httpEndpoints参数说明

<a name="zh-cn_topic_0128578015_table1788894822518"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row988984817253"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p18892048172520"><a name="zh-cn_topic_0128578015_p18892048172520"></a><a name="zh-cn_topic_0128578015_p18892048172520"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p12889204812514"><a name="zh-cn_topic_0128578015_p12889204812514"></a><a name="zh-cn_topic_0128578015_p12889204812514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p168897485253"><a name="zh-cn_topic_0128578015_p168897485253"></a><a name="zh-cn_topic_0128578015_p168897485253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p4889144818251"><a name="zh-cn_topic_0128578015_p4889144818251"></a><a name="zh-cn_topic_0128578015_p4889144818251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row7889164818257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p158899481251"><a name="zh-cn_topic_0128578015_p158899481251"></a><a name="zh-cn_topic_0128578015_p158899481251"></a>address</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p19889134812514"><a name="zh-cn_topic_0128578015_p19889134812514"></a><a name="zh-cn_topic_0128578015_p19889134812514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p289054818257"><a name="zh-cn_topic_0128578015_p289054818257"></a><a name="zh-cn_topic_0128578015_p289054818257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p389044816256"><a name="zh-cn_topic_0128578015_p389044816256"></a><a name="zh-cn_topic_0128578015_p389044816256"></a>后端服务地址，格式为：&lt;域名或IP&gt;:[port]</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row13890348152517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p48902486252"><a name="zh-cn_topic_0128578015_p48902486252"></a><a name="zh-cn_topic_0128578015_p48902486252"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p198901048142519"><a name="zh-cn_topic_0128578015_p198901048142519"></a><a name="zh-cn_topic_0128578015_p198901048142519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p188901488253"><a name="zh-cn_topic_0128578015_p188901488253"></a><a name="zh-cn_topic_0128578015_p188901488253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p689013488253"><a name="zh-cn_topic_0128578015_p689013488253"></a><a name="zh-cn_topic_0128578015_p689013488253"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row88902048112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p13890134816252"><a name="zh-cn_topic_0128578015_p13890134816252"></a><a name="zh-cn_topic_0128578015_p13890134816252"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1089013489252"><a name="zh-cn_topic_0128578015_p1089013489252"></a><a name="zh-cn_topic_0128578015_p1089013489252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p118901148172513"><a name="zh-cn_topic_0128578015_p118901148172513"></a><a name="zh-cn_topic_0128578015_p118901148172513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1989074812515"><a name="zh-cn_topic_0128578015_p1989074812515"></a><a name="zh-cn_topic_0128578015_p1989074812515"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row7890104822514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p5890144882519"><a name="zh-cn_topic_0128578015_p5890144882519"></a><a name="zh-cn_topic_0128578015_p5890144882519"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p28911948182519"><a name="zh-cn_topic_0128578015_p28911948182519"></a><a name="zh-cn_topic_0128578015_p28911948182519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p68915482252"><a name="zh-cn_topic_0128578015_p68915482252"></a><a name="zh-cn_topic_0128578015_p68915482252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p188912048192510"><a name="zh-cn_topic_0128578015_p188912048192510"></a><a name="zh-cn_topic_0128578015_p188912048192510"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row13891204812255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p58911948132514"><a name="zh-cn_topic_0128578015_p58911948132514"></a><a name="zh-cn_topic_0128578015_p58911948132514"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1389194814256"><a name="zh-cn_topic_0128578015_p1389194814256"></a><a name="zh-cn_topic_0128578015_p1389194814256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p889124812510"><a name="zh-cn_topic_0128578015_p889124812510"></a><a name="zh-cn_topic_0128578015_p889124812510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p189264813251"><a name="zh-cn_topic_0128578015_p189264813251"></a><a name="zh-cn_topic_0128578015_p189264813251"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row7635433104612"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p171721112324"><a name="zh-cn_topic_0128578015_p171721112324"></a><a name="zh-cn_topic_0128578015_p171721112324"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p871801119323"><a name="zh-cn_topic_0128578015_p871801119323"></a><a name="zh-cn_topic_0128578015_p871801119323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p19718611193219"><a name="zh-cn_topic_0128578015_p19718611193219"></a><a name="zh-cn_topic_0128578015_p19718611193219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1571891123210"><a name="zh-cn_topic_0128578015_p1571891123210"></a><a name="zh-cn_topic_0128578015_p1571891123210"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 19**  后端httpVpcEndpoints参数说明

<a name="zh-cn_topic_0128578015_table1089314812254"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row489354813256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p16893104820253"><a name="zh-cn_topic_0128578015_p16893104820253"></a><a name="zh-cn_topic_0128578015_p16893104820253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p14893548102518"><a name="zh-cn_topic_0128578015_p14893548102518"></a><a name="zh-cn_topic_0128578015_p14893548102518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p7893184852520"><a name="zh-cn_topic_0128578015_p7893184852520"></a><a name="zh-cn_topic_0128578015_p7893184852520"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p1789304832517"><a name="zh-cn_topic_0128578015_p1789304832517"></a><a name="zh-cn_topic_0128578015_p1789304832517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row389304819258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p089494814258"><a name="zh-cn_topic_0128578015_p089494814258"></a><a name="zh-cn_topic_0128578015_p089494814258"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p188941948112519"><a name="zh-cn_topic_0128578015_p188941948112519"></a><a name="zh-cn_topic_0128578015_p188941948112519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p2089418484250"><a name="zh-cn_topic_0128578015_p2089418484250"></a><a name="zh-cn_topic_0128578015_p2089418484250"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p78948486252"><a name="zh-cn_topic_0128578015_p78948486252"></a><a name="zh-cn_topic_0128578015_p78948486252"></a>VPC通道名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row19894104862518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1089464852513"><a name="zh-cn_topic_0128578015_p1089464852513"></a><a name="zh-cn_topic_0128578015_p1089464852513"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p138945480256"><a name="zh-cn_topic_0128578015_p138945480256"></a><a name="zh-cn_topic_0128578015_p138945480256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p989454862516"><a name="zh-cn_topic_0128578015_p989454862516"></a><a name="zh-cn_topic_0128578015_p989454862516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p2894248162512"><a name="zh-cn_topic_0128578015_p2894248162512"></a><a name="zh-cn_topic_0128578015_p2894248162512"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1189484812512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1589413486258"><a name="zh-cn_topic_0128578015_p1589413486258"></a><a name="zh-cn_topic_0128578015_p1589413486258"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p148947482254"><a name="zh-cn_topic_0128578015_p148947482254"></a><a name="zh-cn_topic_0128578015_p148947482254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1689418486254"><a name="zh-cn_topic_0128578015_p1689418486254"></a><a name="zh-cn_topic_0128578015_p1689418486254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p2089444817252"><a name="zh-cn_topic_0128578015_p2089444817252"></a><a name="zh-cn_topic_0128578015_p2089444817252"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row14895164817252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p11895194818252"><a name="zh-cn_topic_0128578015_p11895194818252"></a><a name="zh-cn_topic_0128578015_p11895194818252"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p28958484255"><a name="zh-cn_topic_0128578015_p28958484255"></a><a name="zh-cn_topic_0128578015_p28958484255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p13895448142512"><a name="zh-cn_topic_0128578015_p13895448142512"></a><a name="zh-cn_topic_0128578015_p13895448142512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1189594813254"><a name="zh-cn_topic_0128578015_p1189594813254"></a><a name="zh-cn_topic_0128578015_p1189594813254"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1689594819251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p0895104832517"><a name="zh-cn_topic_0128578015_p0895104832517"></a><a name="zh-cn_topic_0128578015_p0895104832517"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p11895184862514"><a name="zh-cn_topic_0128578015_p11895184862514"></a><a name="zh-cn_topic_0128578015_p11895184862514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p108951948172512"><a name="zh-cn_topic_0128578015_p108951948172512"></a><a name="zh-cn_topic_0128578015_p108951948172512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1289515487258"><a name="zh-cn_topic_0128578015_p1289515487258"></a><a name="zh-cn_topic_0128578015_p1289515487258"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row18895184802511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p2895134820259"><a name="zh-cn_topic_0128578015_p2895134820259"></a><a name="zh-cn_topic_0128578015_p2895134820259"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p9895144815256"><a name="zh-cn_topic_0128578015_p9895144815256"></a><a name="zh-cn_topic_0128578015_p9895144815256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p168952482254"><a name="zh-cn_topic_0128578015_p168952482254"></a><a name="zh-cn_topic_0128578015_p168952482254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p9896194812253"><a name="zh-cn_topic_0128578015_p9896194812253"></a><a name="zh-cn_topic_0128578015_p9896194812253"></a>VPC通道代理主机</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row126916399464"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1205124114618"><a name="zh-cn_topic_0128578015_p1205124114618"></a><a name="zh-cn_topic_0128578015_p1205124114618"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p11205204144619"><a name="zh-cn_topic_0128578015_p11205204144619"></a><a name="zh-cn_topic_0128578015_p11205204144619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p172056411467"><a name="zh-cn_topic_0128578015_p172056411467"></a><a name="zh-cn_topic_0128578015_p172056411467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1520564144612"><a name="zh-cn_topic_0128578015_p1520564144612"></a><a name="zh-cn_topic_0128578015_p1520564144612"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 20**  后端functionEndpoints参数说明

<a name="zh-cn_topic_0128578015_table18971648202512"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row14897184815257"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p1389711486257"><a name="zh-cn_topic_0128578015_p1389711486257"></a><a name="zh-cn_topic_0128578015_p1389711486257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p1589724814251"><a name="zh-cn_topic_0128578015_p1589724814251"></a><a name="zh-cn_topic_0128578015_p1589724814251"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p589714815258"><a name="zh-cn_topic_0128578015_p589714815258"></a><a name="zh-cn_topic_0128578015_p589714815258"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p389818487257"><a name="zh-cn_topic_0128578015_p389818487257"></a><a name="zh-cn_topic_0128578015_p389818487257"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row58981348182516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1689814802516"><a name="zh-cn_topic_0128578015_p1689814802516"></a><a name="zh-cn_topic_0128578015_p1689814802516"></a>function-urn</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p7898114818255"><a name="zh-cn_topic_0128578015_p7898114818255"></a><a name="zh-cn_topic_0128578015_p7898114818255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p13898114852515"><a name="zh-cn_topic_0128578015_p13898114852515"></a><a name="zh-cn_topic_0128578015_p13898114852515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p589884811259"><a name="zh-cn_topic_0128578015_p589884811259"></a><a name="zh-cn_topic_0128578015_p589884811259"></a>函数URN地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row128984488256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p12899648152514"><a name="zh-cn_topic_0128578015_p12899648152514"></a><a name="zh-cn_topic_0128578015_p12899648152514"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1189984814258"><a name="zh-cn_topic_0128578015_p1189984814258"></a><a name="zh-cn_topic_0128578015_p1189984814258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p178991448162510"><a name="zh-cn_topic_0128578015_p178991448162510"></a><a name="zh-cn_topic_0128578015_p178991448162510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1899174832517"><a name="zh-cn_topic_0128578015_p1899174832517"></a><a name="zh-cn_topic_0128578015_p1899174832517"></a>函数版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row0899134815250"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p9899348162513"><a name="zh-cn_topic_0128578015_p9899348162513"></a><a name="zh-cn_topic_0128578015_p9899348162513"></a>invocation-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p289910485254"><a name="zh-cn_topic_0128578015_p289910485254"></a><a name="zh-cn_topic_0128578015_p289910485254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p18991348102516"><a name="zh-cn_topic_0128578015_p18991348102516"></a><a name="zh-cn_topic_0128578015_p18991348102516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p189984818250"><a name="zh-cn_topic_0128578015_p189984818250"></a><a name="zh-cn_topic_0128578015_p189984818250"></a>函数调用类型，支持async、sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row28995482255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1290018487253"><a name="zh-cn_topic_0128578015_p1290018487253"></a><a name="zh-cn_topic_0128578015_p1290018487253"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p490010489253"><a name="zh-cn_topic_0128578015_p490010489253"></a><a name="zh-cn_topic_0128578015_p490010489253"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p3900148112515"><a name="zh-cn_topic_0128578015_p3900148112515"></a><a name="zh-cn_topic_0128578015_p3900148112515"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p3900154822516"><a name="zh-cn_topic_0128578015_p3900154822516"></a><a name="zh-cn_topic_0128578015_p3900154822516"></a>函数超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row4948164516468"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p417724714468"><a name="zh-cn_topic_0128578015_p417724714468"></a><a name="zh-cn_topic_0128578015_p417724714468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p20177147174614"><a name="zh-cn_topic_0128578015_p20177147174614"></a><a name="zh-cn_topic_0128578015_p20177147174614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p2178184712466"><a name="zh-cn_topic_0128578015_p2178184712466"></a><a name="zh-cn_topic_0128578015_p2178184712466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p131781547144613"><a name="zh-cn_topic_0128578015_p131781547144613"></a><a name="zh-cn_topic_0128578015_p131781547144613"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 21**  后端mockEndpoints参数说明

<a name="zh-cn_topic_0128578015_table1790184862513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row1901104812518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p6902348122511"><a name="zh-cn_topic_0128578015_p6902348122511"></a><a name="zh-cn_topic_0128578015_p6902348122511"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p690215486256"><a name="zh-cn_topic_0128578015_p690215486256"></a><a name="zh-cn_topic_0128578015_p690215486256"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p7902548202519"><a name="zh-cn_topic_0128578015_p7902548202519"></a><a name="zh-cn_topic_0128578015_p7902548202519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p17902148202518"><a name="zh-cn_topic_0128578015_p17902148202518"></a><a name="zh-cn_topic_0128578015_p17902148202518"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row69021348202511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p14902448112512"><a name="zh-cn_topic_0128578015_p14902448112512"></a><a name="zh-cn_topic_0128578015_p14902448112512"></a>result-content</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p8902104816254"><a name="zh-cn_topic_0128578015_p8902104816254"></a><a name="zh-cn_topic_0128578015_p8902104816254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p19903648122510"><a name="zh-cn_topic_0128578015_p19903648122510"></a><a name="zh-cn_topic_0128578015_p19903648122510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p12903948172517"><a name="zh-cn_topic_0128578015_p12903948172517"></a><a name="zh-cn_topic_0128578015_p12903948172517"></a>MOCK返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row4433155454616"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1576125519468"><a name="zh-cn_topic_0128578015_p1576125519468"></a><a name="zh-cn_topic_0128578015_p1576125519468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1857675514611"><a name="zh-cn_topic_0128578015_p1857675514611"></a><a name="zh-cn_topic_0128578015_p1857675514611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p105761955174616"><a name="zh-cn_topic_0128578015_p105761955174616"></a><a name="zh-cn_topic_0128578015_p105761955174616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p05768551462"><a name="zh-cn_topic_0128578015_p05768551462"></a><a name="zh-cn_topic_0128578015_p05768551462"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 22**  conditions参数说明

<a name="zh-cn_topic_0128578015_table1790444832520"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row199040482254"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p169051248112512"><a name="zh-cn_topic_0128578015_p169051248112512"></a><a name="zh-cn_topic_0128578015_p169051248112512"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p590554862518"><a name="zh-cn_topic_0128578015_p590554862518"></a><a name="zh-cn_topic_0128578015_p590554862518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p190564892511"><a name="zh-cn_topic_0128578015_p190564892511"></a><a name="zh-cn_topic_0128578015_p190564892511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p4905194815251"><a name="zh-cn_topic_0128578015_p4905194815251"></a><a name="zh-cn_topic_0128578015_p4905194815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row390544872514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p69056485258"><a name="zh-cn_topic_0128578015_p69056485258"></a><a name="zh-cn_topic_0128578015_p69056485258"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1290514820256"><a name="zh-cn_topic_0128578015_p1290514820256"></a><a name="zh-cn_topic_0128578015_p1290514820256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p190574819257"><a name="zh-cn_topic_0128578015_p190574819257"></a><a name="zh-cn_topic_0128578015_p190574819257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1190554892513"><a name="zh-cn_topic_0128578015_p1190554892513"></a><a name="zh-cn_topic_0128578015_p1190554892513"></a>策略条件类型，支持equal、enum、pattern</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row590619487256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p59061248132511"><a name="zh-cn_topic_0128578015_p59061248132511"></a><a name="zh-cn_topic_0128578015_p59061248132511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p159064483250"><a name="zh-cn_topic_0128578015_p159064483250"></a><a name="zh-cn_topic_0128578015_p159064483250"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1990644812258"><a name="zh-cn_topic_0128578015_p1990644812258"></a><a name="zh-cn_topic_0128578015_p1990644812258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1390694812519"><a name="zh-cn_topic_0128578015_p1390694812519"></a><a name="zh-cn_topic_0128578015_p1390694812519"></a>策略条件值</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row19906114813251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p209067480258"><a name="zh-cn_topic_0128578015_p209067480258"></a><a name="zh-cn_topic_0128578015_p209067480258"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p14906184813256"><a name="zh-cn_topic_0128578015_p14906184813256"></a><a name="zh-cn_topic_0128578015_p14906184813256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1690694811252"><a name="zh-cn_topic_0128578015_p1690694811252"></a><a name="zh-cn_topic_0128578015_p1690694811252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p159071748102517"><a name="zh-cn_topic_0128578015_p159071748102517"></a><a name="zh-cn_topic_0128578015_p159071748102517"></a>策略条件输入来源，支持source、request</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row16907248202516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p6907648162519"><a name="zh-cn_topic_0128578015_p6907648162519"></a><a name="zh-cn_topic_0128578015_p6907648162519"></a>parameter</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1290714882519"><a name="zh-cn_topic_0128578015_p1290714882519"></a><a name="zh-cn_topic_0128578015_p1290714882519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1690719487254"><a name="zh-cn_topic_0128578015_p1690719487254"></a><a name="zh-cn_topic_0128578015_p1690719487254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p149071484250"><a name="zh-cn_topic_0128578015_p149071484250"></a><a name="zh-cn_topic_0128578015_p149071484250"></a>策略条件输入来源为request时，请求入参的名称</p>
</td>
</tr>
</tbody>
</table>

**表 23**  x-apigateway-access-controls参数说明

<a name="zh-cn_topic_0128578015_table2090754816252"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row179081748172515"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p209087484253"><a name="zh-cn_topic_0128578015_p209087484253"></a><a name="zh-cn_topic_0128578015_p209087484253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p1490854819254"><a name="zh-cn_topic_0128578015_p1490854819254"></a><a name="zh-cn_topic_0128578015_p1490854819254"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p09082048122514"><a name="zh-cn_topic_0128578015_p09082048122514"></a><a name="zh-cn_topic_0128578015_p09082048122514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p390944819252"><a name="zh-cn_topic_0128578015_p390944819252"></a><a name="zh-cn_topic_0128578015_p390944819252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row5909114852510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p18909174811252"><a name="zh-cn_topic_0128578015_p18909174811252"></a><a name="zh-cn_topic_0128578015_p18909174811252"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p109091448202516"><a name="zh-cn_topic_0128578015_p109091448202516"></a><a name="zh-cn_topic_0128578015_p109091448202516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p79098488251"><a name="zh-cn_topic_0128578015_p79098488251"></a><a name="zh-cn_topic_0128578015_p79098488251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p11909114819251"><a name="zh-cn_topic_0128578015_p11909114819251"></a><a name="zh-cn_topic_0128578015_p11909114819251"></a>指定名称的访问控制策略，参考<a href="#zh-cn_topic_0128578015_table39092048142510">表 acl_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 24**  acl\_name参数说明

<a name="zh-cn_topic_0128578015_table39092048142510"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row191014812256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p991017483255"><a name="zh-cn_topic_0128578015_p991017483255"></a><a name="zh-cn_topic_0128578015_p991017483255"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p69108489253"><a name="zh-cn_topic_0128578015_p69108489253"></a><a name="zh-cn_topic_0128578015_p69108489253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p1591016486250"><a name="zh-cn_topic_0128578015_p1591016486250"></a><a name="zh-cn_topic_0128578015_p1591016486250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p891110481252"><a name="zh-cn_topic_0128578015_p891110481252"></a><a name="zh-cn_topic_0128578015_p891110481252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row49111048102517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p129110482258"><a name="zh-cn_topic_0128578015_p129110482258"></a><a name="zh-cn_topic_0128578015_p129110482258"></a>acl-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p20911104892511"><a name="zh-cn_topic_0128578015_p20911104892511"></a><a name="zh-cn_topic_0128578015_p20911104892511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p13911174815258"><a name="zh-cn_topic_0128578015_p13911174815258"></a><a name="zh-cn_topic_0128578015_p13911174815258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p17911174882519"><a name="zh-cn_topic_0128578015_p17911174882519"></a><a name="zh-cn_topic_0128578015_p17911174882519"></a>访问控制行为，支持PERMIT、DENY</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row191154882520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1191254820251"><a name="zh-cn_topic_0128578015_p1191254820251"></a><a name="zh-cn_topic_0128578015_p1191254820251"></a>entity-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p169121248142514"><a name="zh-cn_topic_0128578015_p169121248142514"></a><a name="zh-cn_topic_0128578015_p169121248142514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p691294818254"><a name="zh-cn_topic_0128578015_p691294818254"></a><a name="zh-cn_topic_0128578015_p691294818254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p8912948182515"><a name="zh-cn_topic_0128578015_p8912948182515"></a><a name="zh-cn_topic_0128578015_p8912948182515"></a>访问控制对象，支持IP、DOMAIN</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1391211489258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p11912194872511"><a name="zh-cn_topic_0128578015_p11912194872511"></a><a name="zh-cn_topic_0128578015_p11912194872511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p3912248192514"><a name="zh-cn_topic_0128578015_p3912248192514"></a><a name="zh-cn_topic_0128578015_p3912248192514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p6912848192513"><a name="zh-cn_topic_0128578015_p6912848192513"></a><a name="zh-cn_topic_0128578015_p6912848192513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p9913194862512"><a name="zh-cn_topic_0128578015_p9913194862512"></a><a name="zh-cn_topic_0128578015_p9913194862512"></a>访问控制策略值，多个值以“,”间隔</p>
</td>
</tr>
</tbody>
</table>

**表 25**  x-apigateway-ratelimits参数说明

<a name="zh-cn_topic_0128578015_table18913124872513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row17913648192518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p19913848152517"><a name="zh-cn_topic_0128578015_p19913848152517"></a><a name="zh-cn_topic_0128578015_p19913848152517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p891324822519"><a name="zh-cn_topic_0128578015_p891324822519"></a><a name="zh-cn_topic_0128578015_p891324822519"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p591411483253"><a name="zh-cn_topic_0128578015_p591411483253"></a><a name="zh-cn_topic_0128578015_p591411483253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p15914144811250"><a name="zh-cn_topic_0128578015_p15914144811250"></a><a name="zh-cn_topic_0128578015_p15914144811250"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row1391424802514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p99141748112512"><a name="zh-cn_topic_0128578015_p99141748112512"></a><a name="zh-cn_topic_0128578015_p99141748112512"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p149141489252"><a name="zh-cn_topic_0128578015_p149141489252"></a><a name="zh-cn_topic_0128578015_p149141489252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p99145487257"><a name="zh-cn_topic_0128578015_p99145487257"></a><a name="zh-cn_topic_0128578015_p99145487257"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p39151248192510"><a name="zh-cn_topic_0128578015_p39151248192510"></a><a name="zh-cn_topic_0128578015_p39151248192510"></a>指定名称的流控策略，参考<a href="#zh-cn_topic_0128578015_table179155483256">表 throttle_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 26**  throttle\_name参数说明

<a name="zh-cn_topic_0128578015_table179155483256"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row3915114811258"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p1191616488258"><a name="zh-cn_topic_0128578015_p1191616488258"></a><a name="zh-cn_topic_0128578015_p1191616488258"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p199164484253"><a name="zh-cn_topic_0128578015_p199164484253"></a><a name="zh-cn_topic_0128578015_p199164484253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p29161648202514"><a name="zh-cn_topic_0128578015_p29161648202514"></a><a name="zh-cn_topic_0128578015_p29161648202514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p89168486252"><a name="zh-cn_topic_0128578015_p89168486252"></a><a name="zh-cn_topic_0128578015_p89168486252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row39169488253"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p119161548182514"><a name="zh-cn_topic_0128578015_p119161548182514"></a><a name="zh-cn_topic_0128578015_p119161548182514"></a>api-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1391664819255"><a name="zh-cn_topic_0128578015_p1391664819255"></a><a name="zh-cn_topic_0128578015_p1391664819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p19174485250"><a name="zh-cn_topic_0128578015_p19174485250"></a><a name="zh-cn_topic_0128578015_p19174485250"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p59171489257"><a name="zh-cn_topic_0128578015_p59171489257"></a><a name="zh-cn_topic_0128578015_p59171489257"></a>API访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row14917194852515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p189171648112514"><a name="zh-cn_topic_0128578015_p189171648112514"></a><a name="zh-cn_topic_0128578015_p189171648112514"></a>user-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p18917174813252"><a name="zh-cn_topic_0128578015_p18917174813252"></a><a name="zh-cn_topic_0128578015_p18917174813252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p199171348162512"><a name="zh-cn_topic_0128578015_p199171348162512"></a><a name="zh-cn_topic_0128578015_p199171348162512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p4917448162510"><a name="zh-cn_topic_0128578015_p4917448162510"></a><a name="zh-cn_topic_0128578015_p4917448162510"></a>用户访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row129177484252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p6918104872519"><a name="zh-cn_topic_0128578015_p6918104872519"></a><a name="zh-cn_topic_0128578015_p6918104872519"></a>app-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1091894814255"><a name="zh-cn_topic_0128578015_p1091894814255"></a><a name="zh-cn_topic_0128578015_p1091894814255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p891804811257"><a name="zh-cn_topic_0128578015_p891804811257"></a><a name="zh-cn_topic_0128578015_p891804811257"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p1918748152512"><a name="zh-cn_topic_0128578015_p1918748152512"></a><a name="zh-cn_topic_0128578015_p1918748152512"></a>应用访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row5918648192514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p179181648112513"><a name="zh-cn_topic_0128578015_p179181648112513"></a><a name="zh-cn_topic_0128578015_p179181648112513"></a>ip-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p15918548132512"><a name="zh-cn_topic_0128578015_p15918548132512"></a><a name="zh-cn_topic_0128578015_p15918548132512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p69181248132518"><a name="zh-cn_topic_0128578015_p69181248132518"></a><a name="zh-cn_topic_0128578015_p69181248132518"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p169192488255"><a name="zh-cn_topic_0128578015_p169192488255"></a><a name="zh-cn_topic_0128578015_p169192488255"></a>源IP访问次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row79191948142513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p491994816255"><a name="zh-cn_topic_0128578015_p491994816255"></a><a name="zh-cn_topic_0128578015_p491994816255"></a>interval</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p11919114819255"><a name="zh-cn_topic_0128578015_p11919114819255"></a><a name="zh-cn_topic_0128578015_p11919114819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p79191648132510"><a name="zh-cn_topic_0128578015_p79191648132510"></a><a name="zh-cn_topic_0128578015_p79191648132510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p119195483257"><a name="zh-cn_topic_0128578015_p119195483257"></a><a name="zh-cn_topic_0128578015_p119195483257"></a>流控策略时间周期</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row199198489254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p1919154812517"><a name="zh-cn_topic_0128578015_p1919154812517"></a><a name="zh-cn_topic_0128578015_p1919154812517"></a>unit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1391916487253"><a name="zh-cn_topic_0128578015_p1391916487253"></a><a name="zh-cn_topic_0128578015_p1391916487253"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p292015486259"><a name="zh-cn_topic_0128578015_p292015486259"></a><a name="zh-cn_topic_0128578015_p292015486259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p3920748112517"><a name="zh-cn_topic_0128578015_p3920748112517"></a><a name="zh-cn_topic_0128578015_p3920748112517"></a>流控策略时间周期单位，支持SECOND、MINUTE、HOUR、DAY</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row14920174811258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p7920948132515"><a name="zh-cn_topic_0128578015_p7920948132515"></a><a name="zh-cn_topic_0128578015_p7920948132515"></a>shared</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p192019487254"><a name="zh-cn_topic_0128578015_p192019487254"></a><a name="zh-cn_topic_0128578015_p192019487254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1920124892513"><a name="zh-cn_topic_0128578015_p1920124892513"></a><a name="zh-cn_topic_0128578015_p1920124892513"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p17920174842518"><a name="zh-cn_topic_0128578015_p17920174842518"></a><a name="zh-cn_topic_0128578015_p17920174842518"></a>是否共享流控策略</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1392010481255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p6921194816259"><a name="zh-cn_topic_0128578015_p6921194816259"></a><a name="zh-cn_topic_0128578015_p6921194816259"></a>special</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p29212489254"><a name="zh-cn_topic_0128578015_p29212489254"></a><a name="zh-cn_topic_0128578015_p29212489254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p792119480253"><a name="zh-cn_topic_0128578015_p792119480253"></a><a name="zh-cn_topic_0128578015_p792119480253"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p15921144832520"><a name="zh-cn_topic_0128578015_p15921144832520"></a><a name="zh-cn_topic_0128578015_p15921144832520"></a>特殊流控策略对象数组定义，参考<a href="#zh-cn_topic_0128578015_table6921174842513">表 special参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 27**  special参数说明

<a name="zh-cn_topic_0128578015_table6921174842513"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row5922248112514"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0128578015_p1492234818256"><a name="zh-cn_topic_0128578015_p1492234818256"></a><a name="zh-cn_topic_0128578015_p1492234818256"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0128578015_p1292214818252"><a name="zh-cn_topic_0128578015_p1292214818252"></a><a name="zh-cn_topic_0128578015_p1292214818252"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0128578015_p1192217488256"><a name="zh-cn_topic_0128578015_p1192217488256"></a><a name="zh-cn_topic_0128578015_p1192217488256"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0128578015_p19922144810251"><a name="zh-cn_topic_0128578015_p19922144810251"></a><a name="zh-cn_topic_0128578015_p19922144810251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row109221348122519"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p4923448142518"><a name="zh-cn_topic_0128578015_p4923448142518"></a><a name="zh-cn_topic_0128578015_p4923448142518"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p792311483258"><a name="zh-cn_topic_0128578015_p792311483258"></a><a name="zh-cn_topic_0128578015_p792311483258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p392311487256"><a name="zh-cn_topic_0128578015_p392311487256"></a><a name="zh-cn_topic_0128578015_p392311487256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p292315488259"><a name="zh-cn_topic_0128578015_p292315488259"></a><a name="zh-cn_topic_0128578015_p292315488259"></a>特殊流控策略类型，支持APP、USER</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1692304842514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p192311482252"><a name="zh-cn_topic_0128578015_p192311482252"></a><a name="zh-cn_topic_0128578015_p192311482252"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p1292364814256"><a name="zh-cn_topic_0128578015_p1292364814256"></a><a name="zh-cn_topic_0128578015_p1292364814256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p1092344819252"><a name="zh-cn_topic_0128578015_p1092344819252"></a><a name="zh-cn_topic_0128578015_p1092344819252"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p13923134817259"><a name="zh-cn_topic_0128578015_p13923134817259"></a><a name="zh-cn_topic_0128578015_p13923134817259"></a>访问次数</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row13923948122511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0128578015_p15923248172511"><a name="zh-cn_topic_0128578015_p15923248172511"></a><a name="zh-cn_topic_0128578015_p15923248172511"></a>instance</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0128578015_p4924448162510"><a name="zh-cn_topic_0128578015_p4924448162510"></a><a name="zh-cn_topic_0128578015_p4924448162510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0128578015_p119249482253"><a name="zh-cn_topic_0128578015_p119249482253"></a><a name="zh-cn_topic_0128578015_p119249482253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0128578015_p5924154822518"><a name="zh-cn_topic_0128578015_p5924154822518"></a><a name="zh-cn_topic_0128578015_p5924154822518"></a>特殊APP或USER的对象标识</p>
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

## 响应码<a name="zh-cn_topic_0128578015_section66318442384"></a>

**表 28**  返回消息说明

<a name="zh-cn_topic_0128578015_table11438104424617"></a>
<table><thead align="left"><tr id="zh-cn_topic_0128578015_row1643820448464"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0128578015_p4272113476"><a name="zh-cn_topic_0128578015_p4272113476"></a><a name="zh-cn_topic_0128578015_p4272113476"></a>响应码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0128578015_p202192154718"><a name="zh-cn_topic_0128578015_p202192154718"></a><a name="zh-cn_topic_0128578015_p202192154718"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0128578015_row24383446462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0128578015_p62162184714"><a name="zh-cn_topic_0128578015_p62162184714"></a><a name="zh-cn_topic_0128578015_p62162184714"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0128578015_p112162113475"><a name="zh-cn_topic_0128578015_p112162113475"></a><a name="zh-cn_topic_0128578015_p112162113475"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row6438154417469"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0128578015_p1228216472"><a name="zh-cn_topic_0128578015_p1228216472"></a><a name="zh-cn_topic_0128578015_p1228216472"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0128578015_p132182116477"><a name="zh-cn_topic_0128578015_p132182116477"></a><a name="zh-cn_topic_0128578015_p132182116477"></a>bad request</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1943874416467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0128578015_p12262144711"><a name="zh-cn_topic_0128578015_p12262144711"></a><a name="zh-cn_topic_0128578015_p12262144711"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0128578015_p20220215475"><a name="zh-cn_topic_0128578015_p20220215475"></a><a name="zh-cn_topic_0128578015_p20220215475"></a>unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row1043834417462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0128578015_p1292117477"><a name="zh-cn_topic_0128578015_p1292117477"></a><a name="zh-cn_topic_0128578015_p1292117477"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0128578015_p32921144714"><a name="zh-cn_topic_0128578015_p32921144714"></a><a name="zh-cn_topic_0128578015_p32921144714"></a>forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0128578015_row6439344194617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0128578015_p7282116471"><a name="zh-cn_topic_0128578015_p7282116471"></a><a name="zh-cn_topic_0128578015_p7282116471"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0128578015_p62112110471"><a name="zh-cn_topic_0128578015_p62112110471"></a><a name="zh-cn_topic_0128578015_p62112110471"></a>server internal error</p>
</td>
</tr>
</tbody>
</table>

