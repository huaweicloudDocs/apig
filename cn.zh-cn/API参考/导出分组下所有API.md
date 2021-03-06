# 导出分组下所有API<a name="apig-zh-api-180911238"></a>

## 功能介绍<a name="section39777523194"></a>

提供用户导出API定义的接口。

导出指定分组指定环境中发布的API的基础/全量/扩展Swagger定义。

## URI<a name="section16371135218203"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table11507134785618"></a>
<table><thead align="left"><tr id="row1150904725614"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p75091547155615"><a name="p75091547155615"></a><a name="p75091547155615"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p16509947105618"><a name="p16509947105618"></a><a name="p16509947105618"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row450934716564"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p14509154711566"><a name="p14509154711566"></a><a name="p14509154711566"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1213518364578"><a name="p1213518364578"></a><a name="p1213518364578"></a>/v1.0/apigw/openapi?env_id={0}&amp;group_id={1}&amp;define={2}&amp;version={3}&amp;type={4}</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section178868115223"></a>

**表 2**  参数说明

<a name="table871144945810"></a>
<table><thead align="left"><tr id="row14734499589"><th class="cellrowborder" valign="top" width="16.831683168316832%" id="mcps1.2.5.1.1"><p id="p1973174918589"><a name="p1973174918589"></a><a name="p1973174918589"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.341534153415342%" id="mcps1.2.5.1.2"><p id="p4731749125817"><a name="p4731749125817"></a><a name="p4731749125817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.691369136913693%" id="mcps1.2.5.1.3"><p id="p1730491589"><a name="p1730491589"></a><a name="p1730491589"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.13541354135414%" id="mcps1.2.5.1.4"><p id="p1073649175817"><a name="p1073649175817"></a><a name="p1073649175817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row87315493588"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="p173061841314"><a name="p173061841314"></a><a name="p173061841314"></a>env_id/env</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="p969851813"><a name="p969851813"></a><a name="p969851813"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="p26925114116"><a name="p26925114116"></a><a name="p26925114116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="p19691651310"><a name="p19691651310"></a><a name="p19691651310"></a>API分组发布的环境ID，目前支持env_id和env，两个均存在时以env_id为准，建议使用env_id</p>
</td>
</tr>
<tr id="row197434912586"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="p16306144114116"><a name="p16306144114116"></a><a name="p16306144114116"></a>group_id/group</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="p126913519113"><a name="p126913519113"></a><a name="p126913519113"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="p369125113111"><a name="p369125113111"></a><a name="p369125113111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="p86912517116"><a name="p86912517116"></a><a name="p86912517116"></a>API分组ID，目前支持group_id和group，两个均存在时以group_id为准，建议使用group_id</p>
</td>
</tr>
<tr id="row67415491585"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="p83064412117"><a name="p83064412117"></a><a name="p83064412117"></a>define</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="p3691511113"><a name="p3691511113"></a><a name="p3691511113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="p6697511314"><a name="p6697511314"></a><a name="p6697511314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="p294920378347"><a name="p294920378347"></a><a name="p294920378347"></a>导出API的定义范围：</p>
<a name="ul169331437173420"></a><a name="ul169331437173420"></a><ul id="ul169331437173420"><li>base：基础定义</li><li>full：全量定义</li><li>all：扩展定义</li></ul>
<p id="p184466500348"><a name="p184466500348"></a><a name="p184466500348"></a>默认为base</p>
</td>
</tr>
<tr id="row8723131211572"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="p147231112105720"><a name="p147231112105720"></a><a name="p147231112105720"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="p16723512135714"><a name="p16723512135714"></a><a name="p16723512135714"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="p8723712115711"><a name="p8723712115711"></a><a name="p8723712115711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="p1972317129578"><a name="p1972317129578"></a><a name="p1972317129578"></a>导出的API定义版本，默认为当前时间</p>
</td>
</tr>
<tr id="row14825155574"><td class="cellrowborder" valign="top" width="16.831683168316832%" headers="mcps1.2.5.1.1 "><p id="p178210154576"><a name="p178210154576"></a><a name="p178210154576"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="15.341534153415342%" headers="mcps1.2.5.1.2 "><p id="p68241555711"><a name="p68241555711"></a><a name="p68241555711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.691369136913693%" headers="mcps1.2.5.1.3 "><p id="p4821315105719"><a name="p4821315105719"></a><a name="p4821315105719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.13541354135414%" headers="mcps1.2.5.1.4 "><p id="p68281565719"><a name="p68281565719"></a><a name="p68281565719"></a>导出的API定义的格式：json/yaml，默认为json</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section526345615258"></a>

**表 3**  参数说明

<a name="table26691411183213"></a>
<table><thead align="left"><tr id="row18670201115326"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="p186708117326"><a name="p186708117326"></a><a name="p186708117326"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.2"><p id="p1867014116325"><a name="p1867014116325"></a><a name="p1867014116325"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="p176701911203219"><a name="p176701911203219"></a><a name="p176701911203219"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.44554455445545%" id="mcps1.2.5.1.4"><p id="p0670141143214"><a name="p0670141143214"></a><a name="p0670141143214"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1567014117329"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p067014119324"><a name="p067014119324"></a><a name="p067014119324"></a>swagger</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p867031143220"><a name="p867031143220"></a><a name="p867031143220"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p66706117322"><a name="p66706117322"></a><a name="p66706117322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p567051133218"><a name="p567051133218"></a><a name="p567051133218"></a>固定值2.0</p>
</td>
</tr>
<tr id="row12670141173215"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p10670161193210"><a name="p10670161193210"></a><a name="p10670161193210"></a>info</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p1067051133211"><a name="p1067051133211"></a><a name="p1067051133211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p667171173218"><a name="p667171173218"></a><a name="p667171173218"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p1167111115320"><a name="p1167111115320"></a><a name="p1167111115320"></a>参考<a href="#table13672201112325">表4</a></p>
</td>
</tr>
<tr id="row11671511173219"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p767110111324"><a name="p767110111324"></a><a name="p767110111324"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p4671111153217"><a name="p4671111153217"></a><a name="p4671111153217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p156711411143212"><a name="p156711411143212"></a><a name="p156711411143212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p176717117325"><a name="p176717117325"></a><a name="p176717117325"></a>API分组绑定的子域名</p>
</td>
</tr>
<tr id="row15671191163213"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p1767151117329"><a name="p1767151117329"></a><a name="p1767151117329"></a>paths</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p16711411183212"><a name="p16711411183212"></a><a name="p16711411183212"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p196711811143218"><a name="p196711811143218"></a><a name="p196711811143218"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p1067121116324"><a name="p1067121116324"></a><a name="p1067121116324"></a>参考<a href="#table76741113321">表 paths参数说明</a></p>
</td>
</tr>
<tr id="row14671191173212"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p19671911103219"><a name="p19671911103219"></a><a name="p19671911103219"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p9671191123213"><a name="p9671191123213"></a><a name="p9671191123213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p16710118329"><a name="p16710118329"></a><a name="p16710118329"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p96712110328"><a name="p96712110328"></a><a name="p96712110328"></a>公用响应定义，可以被引用在{method}的操作中，参考<a href="#table10688811153215">表9</a></p>
</td>
</tr>
<tr id="row10671101133216"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p1567113114328"><a name="p1567113114328"></a><a name="p1567113114328"></a>securityDefinitions</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p106711311193220"><a name="p106711311193220"></a><a name="p106711311193220"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p156711211163220"><a name="p156711211163220"></a><a name="p156711211163220"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p76711111153216"><a name="p76711111153216"></a><a name="p76711111153216"></a>定义鉴权方式，参考<a href="#table20698111119323">表13</a></p>
</td>
</tr>
<tr id="row15840124816259"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p1884194822510"><a name="p1884194822510"></a><a name="p1884194822510"></a>x-apigateway-access-controls</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p13841148172510"><a name="p13841148172510"></a><a name="p13841148172510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p1784154813256"><a name="p1784154813256"></a><a name="p1784154813256"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p384164813253"><a name="p384164813253"></a><a name="p384164813253"></a>访问控制信息，参考<a href="#table2090754816252">表 x-apigateway-access-controls参数说明</a></p>
</td>
</tr>
<tr id="row684144814253"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p98411348102518"><a name="p98411348102518"></a><a name="p98411348102518"></a>x-apigateway-ratelimits</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p13841134852518"><a name="p13841134852518"></a><a name="p13841134852518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p178411048152517"><a name="p178411048152517"></a><a name="p178411048152517"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p28411648202513"><a name="p28411648202513"></a><a name="p28411648202513"></a>流量控制信息，参考<a href="#table18913124872513">表 x-apigateway-ratelimits参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 4**  info参数说明

<a name="table13672201112325"></a>
<table><thead align="left"><tr id="row6673111113210"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="p1167301173215"><a name="p1167301173215"></a><a name="p1167301173215"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="p15673181103217"><a name="p15673181103217"></a><a name="p15673181103217"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="p86731811143212"><a name="p86731811143212"></a><a name="p86731811143212"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="p16731611193211"><a name="p16731611193211"></a><a name="p16731611193211"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row0673161173211"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p4673151103216"><a name="p4673151103216"></a><a name="p4673151103216"></a>title</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p10673101114324"><a name="p10673101114324"></a><a name="p10673101114324"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p1367361133218"><a name="p1367361133218"></a><a name="p1367361133218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p136731011193213"><a name="p136731011193213"></a><a name="p136731011193213"></a>API分组名称</p>
</td>
</tr>
<tr id="row15673411133218"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p16673101117323"><a name="p16673101117323"></a><a name="p16673101117323"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p136730119321"><a name="p136730119321"></a><a name="p136730119321"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p13673181153216"><a name="p13673181153216"></a><a name="p13673181153216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p19673141133214"><a name="p19673141133214"></a><a name="p19673141133214"></a>版本号，用户输入自定义版本号或者使用默认的当前时间</p>
</td>
</tr>
<tr id="row116733119323"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p76731611133217"><a name="p76731611133217"></a><a name="p76731611133217"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1667391117325"><a name="p1667391117325"></a><a name="p1667391117325"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p0673171183214"><a name="p0673171183214"></a><a name="p0673171183214"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p196731811123210"><a name="p196731811123210"></a><a name="p196731811123210"></a>分组描述信息</p>
</td>
</tr>
</tbody>
</table>

**表 5**  paths参数说明

<a name="table76741113321"></a>
<table><thead align="left"><tr id="row166745112325"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p767471123213"><a name="p767471123213"></a><a name="p767471123213"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.2"><p id="p66741511133219"><a name="p66741511133219"></a><a name="p66741511133219"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.3"><p id="p1067481133216"><a name="p1067481133216"></a><a name="p1067481133216"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="p116747117329"><a name="p116747117329"></a><a name="p116747117329"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row76751911103212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p12675101183210"><a name="p12675101183210"></a><a name="p12675101183210"></a>uri</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.2 "><p id="p10675161163217"><a name="p10675161163217"></a><a name="p10675161163217"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.3 "><p id="p12675171123219"><a name="p12675171123219"></a><a name="p12675171123219"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p17675101110324"><a name="p17675101110324"></a><a name="p17675101110324"></a>API访问地址，参考<a href="#table126750112327">表6</a></p>
</td>
</tr>
</tbody>
</table>

**表 6**  uri参数说明

<a name="table126750112327"></a>
<table><thead align="left"><tr id="row20675311123213"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p10675311153215"><a name="p10675311153215"></a><a name="p10675311153215"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p146751411123216"><a name="p146751411123216"></a><a name="p146751411123216"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p367510118325"><a name="p367510118325"></a><a name="p367510118325"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="p667671173215"><a name="p667671173215"></a><a name="p667671173215"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row15676911173212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p0676131173214"><a name="p0676131173214"></a><a name="p0676131173214"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1676611193214"><a name="p1676611193214"></a><a name="p1676611193214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p16676151143220"><a name="p16676151143220"></a><a name="p16676151143220"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p867621163218"><a name="p867621163218"></a><a name="p867621163218"></a>API访问方法，参考<a href="#table4676711113211">表7</a></p>
</td>
</tr>
</tbody>
</table>

**表 7**  method参数说明

<a name="table4676711113211"></a>
<table><thead align="left"><tr id="row12676111173219"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p13676201119326"><a name="p13676201119326"></a><a name="p13676201119326"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p126761411133212"><a name="p126761411133212"></a><a name="p126761411133212"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p15676111153210"><a name="p15676111153210"></a><a name="p15676111153210"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="p106761111323"><a name="p106761111323"></a><a name="p106761111323"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12849144802517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p08503484253"><a name="p08503484253"></a><a name="p08503484253"></a>operationId</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p0850204842510"><a name="p0850204842510"></a><a name="p0850204842510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p085094842516"><a name="p085094842516"></a><a name="p085094842516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p485094872511"><a name="p485094872511"></a><a name="p485094872511"></a>API的名称</p>
</td>
</tr>
<tr id="row2677161110322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p18677111113217"><a name="p18677111113217"></a><a name="p18677111113217"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1367731117322"><a name="p1367731117322"></a><a name="p1367731117322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p186771311163220"><a name="p186771311163220"></a><a name="p186771311163220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p76771111193215"><a name="p76771111193215"></a><a name="p76771111193215"></a>API的描述信息</p>
</td>
</tr>
<tr id="row967712119324"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p06775117324"><a name="p06775117324"></a><a name="p06775117324"></a>schemes</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1267710115326"><a name="p1267710115326"></a><a name="p1267710115326"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p9678911163213"><a name="p9678911163213"></a><a name="p9678911163213"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1678151173216"><a name="p1678151173216"></a><a name="p1678151173216"></a>API的请求协议对象数组定义，支持http、https</p>
</td>
</tr>
<tr id="row8664174194720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1617514115018"><a name="p1617514115018"></a><a name="p1617514115018"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p18175144135015"><a name="p18175144135015"></a><a name="p18175144135015"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1717614445015"><a name="p1717614445015"></a><a name="p1717614445015"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p191765465013"><a name="p191765465013"></a><a name="p191765465013"></a>API标签对象数组定义</p>
</td>
</tr>
<tr id="row14678171111326"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p167817111329"><a name="p167817111329"></a><a name="p167817111329"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p367881110322"><a name="p367881110322"></a><a name="p367881110322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p86782118325"><a name="p86782118325"></a><a name="p86782118325"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p13678511133220"><a name="p13678511133220"></a><a name="p13678511133220"></a>请求参数对象数组定义，参考<a href="#table36830118324">表 前端parameters参数说明</a></p>
</td>
</tr>
<tr id="row12678411183218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p13678191119326"><a name="p13678191119326"></a><a name="p13678191119326"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p46782111321"><a name="p46782111321"></a><a name="p46782111321"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p66781811133211"><a name="p66781811133211"></a><a name="p66781811133211"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1467891115325"><a name="p1467891115325"></a><a name="p1467891115325"></a>响应定义，参考<a href="#table10688811153215">表9</a></p>
</td>
</tr>
<tr id="row6852144810252"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15852648132516"><a name="p15852648132516"></a><a name="p15852648132516"></a>security</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p985254812519"><a name="p985254812519"></a><a name="p985254812519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p20852948192520"><a name="p20852948192520"></a><a name="p20852948192520"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1185244832513"><a name="p1185244832513"></a><a name="p1185244832513"></a>API的认证类型对象数组定义，参考<a href="#table986594862513">表 security参数说明</a></p>
</td>
</tr>
<tr id="row185314892514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8853748182515"><a name="p8853748182515"></a><a name="p8853748182515"></a>x-apigateway-access-control</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p18853114818258"><a name="p18853114818258"></a><a name="p18853114818258"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p885316488254"><a name="p885316488254"></a><a name="p885316488254"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p885318487254"><a name="p885318487254"></a><a name="p885318487254"></a>API绑定的访问控制对象数组定义</p>
</td>
</tr>
<tr id="row11853104814258"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1385324810256"><a name="p1385324810256"></a><a name="p1385324810256"></a>x-apigateway-backend</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p7853248172514"><a name="p7853248172514"></a><a name="p7853248172514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p6853184852511"><a name="p6853184852511"></a><a name="p6853184852511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p4853174816257"><a name="p4853174816257"></a><a name="p4853174816257"></a>API的后端信息，参考<a href="#table387619483252">表 x-apigateway-backend参数说明</a></p>
</td>
</tr>
<tr id="row1685384815256"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1485334813258"><a name="p1485334813258"></a><a name="p1485334813258"></a>x-apigateway-backend-policies</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p685464852511"><a name="p685464852511"></a><a name="p685464852511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p785419483251"><a name="p785419483251"></a><a name="p785419483251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p18541148122518"><a name="p18541148122518"></a><a name="p18541148122518"></a>API的策略后端信息，参考<a href="#table1988034862512">表 x-apigateway-backend-policies参数说明</a></p>
</td>
</tr>
<tr id="row6854164802518"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1285414488259"><a name="p1285414488259"></a><a name="p1285414488259"></a>x-apigateway-cors</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p13854104814259"><a name="p13854104814259"></a><a name="p13854104814259"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p198541648152518"><a name="p198541648152518"></a><a name="p198541648152518"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1985410480253"><a name="p1985410480253"></a><a name="p1985410480253"></a>是否支持跨域</p>
</td>
</tr>
<tr id="row16854154817253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2085454816256"><a name="p2085454816256"></a><a name="p2085454816256"></a>x-apigateway-match-mode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p98551248162511"><a name="p98551248162511"></a><a name="p98551248162511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p14855948102517"><a name="p14855948102517"></a><a name="p14855948102517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p18551948122513"><a name="p18551948122513"></a><a name="p18551948122513"></a>API的匹配方式</p>
</td>
</tr>
<tr id="row11855164832513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1885514480253"><a name="p1885514480253"></a><a name="p1885514480253"></a>x-apigateway-ratelimit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p5855648142511"><a name="p5855648142511"></a><a name="p5855648142511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p885504815254"><a name="p885504815254"></a><a name="p885504815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p15855124810253"><a name="p15855124810253"></a><a name="p15855124810253"></a>API绑定的流量控制名称</p>
</td>
</tr>
<tr id="row885554810255"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5855144872514"><a name="p5855144872514"></a><a name="p5855144872514"></a>x-apigateway-request-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p4855144822512"><a name="p4855144822512"></a><a name="p4855144822512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p108550488256"><a name="p108550488256"></a><a name="p108550488256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p28561348162511"><a name="p28561348162511"></a><a name="p28561348162511"></a>API的类型</p>
</td>
</tr>
</tbody>
</table>

**表 8**  前端parameters参数说明

<a name="table36830118324"></a>
<table><thead align="left"><tr id="row6684911173220"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="p166841611163216"><a name="p166841611163216"></a><a name="p166841611163216"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="p368431143218"><a name="p368431143218"></a><a name="p368431143218"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="p18684311183214"><a name="p18684311183214"></a><a name="p18684311183214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="p1468416118322"><a name="p1468416118322"></a><a name="p1468416118322"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20684811123219"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p8684511173220"><a name="p8684511173220"></a><a name="p8684511173220"></a>maximum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p176841011123219"><a name="p176841011123219"></a><a name="p176841011123219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p868431114329"><a name="p868431114329"></a><a name="p868431114329"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p768491112320"><a name="p768491112320"></a><a name="p768491112320"></a>参数为数值类型时，最大参数值</p>
</td>
</tr>
<tr id="row1268571193217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p196851211173217"><a name="p196851211173217"></a><a name="p196851211173217"></a>minimum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p126851311133213"><a name="p126851311133213"></a><a name="p126851311133213"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p106851611163214"><a name="p106851611163214"></a><a name="p106851611163214"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p166858113328"><a name="p166858113328"></a><a name="p166858113328"></a>参数为数值类型时，最小参数值</p>
</td>
</tr>
<tr id="row468521173219"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p1368511118323"><a name="p1368511118323"></a><a name="p1368511118323"></a>maxLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p186851611173215"><a name="p186851611173215"></a><a name="p186851611173215"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p2685131193212"><a name="p2685131193212"></a><a name="p2685131193212"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p068571123216"><a name="p068571123216"></a><a name="p068571123216"></a>参数为字符串类型时，参数的最大长度</p>
</td>
</tr>
<tr id="row1868521153217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p166852011123219"><a name="p166852011123219"></a><a name="p166852011123219"></a>minLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1368531123219"><a name="p1368531123219"></a><a name="p1368531123219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p3685101193212"><a name="p3685101193212"></a><a name="p3685101193212"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p11685141114328"><a name="p11685141114328"></a><a name="p11685141114328"></a>参数为字符串类型时，参数的最小长度</p>
</td>
</tr>
<tr id="row1868551183213"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p3685101117325"><a name="p3685101117325"></a><a name="p3685101117325"></a>pattern</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1868651116326"><a name="p1868651116326"></a><a name="p1868651116326"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p166861611163212"><a name="p166861611163212"></a><a name="p166861611163212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p1686181111329"><a name="p1686181111329"></a><a name="p1686181111329"></a>参数值为正则匹配表达式</p>
</td>
</tr>
<tr id="row106861511153212"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p12686191123215"><a name="p12686191123215"></a><a name="p12686191123215"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1868601183216"><a name="p1868601183216"></a><a name="p1868601183216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p46861111193213"><a name="p46861111193213"></a><a name="p46861111193213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p1368671111327"><a name="p1368671111327"></a><a name="p1368671111327"></a>参数类型</p>
</td>
</tr>
<tr id="row5686011103219"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p36867115328"><a name="p36867115328"></a><a name="p36867115328"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p13686171118322"><a name="p13686171118322"></a><a name="p13686171118322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1168641143213"><a name="p1168641143213"></a><a name="p1168641143213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p368691118328"><a name="p368691118328"></a><a name="p368691118328"></a>参数默认值</p>
</td>
</tr>
<tr id="row8686161110323"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p3686151118323"><a name="p3686151118323"></a><a name="p3686151118323"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p136879113323"><a name="p136879113323"></a><a name="p136879113323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1168713119325"><a name="p1168713119325"></a><a name="p1168713119325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p10687131123219"><a name="p10687131123219"></a><a name="p10687131123219"></a>参数描述信息</p>
</td>
</tr>
<tr id="row11687171116324"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p06871611113220"><a name="p06871611113220"></a><a name="p06871611113220"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p14687611183220"><a name="p14687611183220"></a><a name="p14687611183220"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p6687101116325"><a name="p6687101116325"></a><a name="p6687101116325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p1468791110328"><a name="p1468791110328"></a><a name="p1468791110328"></a>参数名称</p>
</td>
</tr>
<tr id="row1468718119325"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p268711173220"><a name="p268711173220"></a><a name="p268711173220"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p176871811163215"><a name="p176871811163215"></a><a name="p176871811163215"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p468761115326"><a name="p468761115326"></a><a name="p468761115326"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p18688171173216"><a name="p18688171173216"></a><a name="p18688171173216"></a>参数位置，支持path、header、query、formData、body</p>
</td>
</tr>
<tr id="row14688141120324"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p136885114325"><a name="p136885114325"></a><a name="p136885114325"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p168841143212"><a name="p168841143212"></a><a name="p168841143212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p568801111329"><a name="p568801111329"></a><a name="p568801111329"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p106881911103215"><a name="p106881911103215"></a><a name="p106881911103215"></a>参数是否必需，参数位置为path时必需</p>
</td>
</tr>
</tbody>
</table>

**表 9**  responses参数说明

<a name="table10688811153215"></a>
<table><thead align="left"><tr id="row1688011113217"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p36892112323"><a name="p36892112323"></a><a name="p36892112323"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p368919110326"><a name="p368919110326"></a><a name="p368919110326"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p8689161114326"><a name="p8689161114326"></a><a name="p8689161114326"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p1468981113214"><a name="p1468981113214"></a><a name="p1468981113214"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1268901163218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p86896111320"><a name="p86896111320"></a><a name="p86896111320"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p368951114322"><a name="p368951114322"></a><a name="p368951114322"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p106891118328"><a name="p106891118328"></a><a name="p106891118328"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p7689131120326"><a name="p7689131120326"></a><a name="p7689131120326"></a>缺省响应，描述未定义的响应码</p>
</td>
</tr>
<tr id="row206901911173220"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p66901211133216"><a name="p66901211133216"></a><a name="p66901211133216"></a>status_code</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p16690181119323"><a name="p16690181119323"></a><a name="p16690181119323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p8690611113216"><a name="p8690611113216"></a><a name="p8690611113216"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1169018115328"><a name="p1169018115328"></a><a name="p1169018115328"></a>响应状态码，值为响应对象，参考<a href="#table76941111143210">表11</a></p>
</td>
</tr>
<tr id="row1774720508918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p774812501894"><a name="p774812501894"></a><a name="p774812501894"></a>x-apigateway-result-failure-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p474815020916"><a name="p474815020916"></a><a name="p474815020916"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p11749105017914"><a name="p11749105017914"></a><a name="p11749105017914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p14749750398"><a name="p14749750398"></a><a name="p14749750398"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="row71795541897"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1117913541917"><a name="p1117913541917"></a><a name="p1117913541917"></a>x-apigateway-result-normal-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p517914541191"><a name="p517914541191"></a><a name="p517914541191"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p171791554493"><a name="p171791554493"></a><a name="p171791554493"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p111791154598"><a name="p111791154598"></a><a name="p111791154598"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
</tbody>
</table>

**表 10**  security参数说明

<a name="table986594862513"></a>
<table><thead align="left"><tr id="row086674852515"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="p986654810257"><a name="p986654810257"></a><a name="p986654810257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="p986624819250"><a name="p986624819250"></a><a name="p986624819250"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="p188661348112516"><a name="p188661348112516"></a><a name="p188661348112516"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="p14866248132510"><a name="p14866248132510"></a><a name="p14866248132510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17866114810256"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p17771954155713"><a name="p17771954155713"></a><a name="p17771954155713"></a>apig-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1677354115716"><a name="p1677354115716"></a><a name="p1677354115716"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p87705410572"><a name="p87705410572"></a><a name="p87705410572"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p117713541579"><a name="p117713541579"></a><a name="p117713541579"></a>API的认证类型对象数组定义，为空数组</p>
<p id="p6722101419557"><a name="p6722101419557"></a><a name="p6722101419557"></a>apig-auth-type支持：</p>
<a name="ul3401225145518"></a><a name="ul3401225145518"></a><ul id="ul3401225145518"><li>APP认证： apig-auth-app</li><li>IAM认证：apig-auth-iam</li><li>NONE：不填写</li></ul>
</td>
</tr>
</tbody>
</table>

**表 11**  status code参数说明

<a name="table76941111143210"></a>
<table><thead align="left"><tr id="row8694611133212"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1569401115329"><a name="p1569401115329"></a><a name="p1569401115329"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p15695101193210"><a name="p15695101193210"></a><a name="p15695101193210"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p269521173215"><a name="p269521173215"></a><a name="p269521173215"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p17695161153216"><a name="p17695161153216"></a><a name="p17695161153216"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1269591133216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1469518113321"><a name="p1469518113321"></a><a name="p1469518113321"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p56951311133214"><a name="p56951311133214"></a><a name="p56951311133214"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p166952117322"><a name="p166952117322"></a><a name="p166952117322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p156957111322"><a name="p156957111322"></a><a name="p156957111322"></a>响应描述信息</p>
</td>
</tr>
<tr id="row669517112325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p069571133216"><a name="p069571133216"></a><a name="p069571133216"></a>schema</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p176952116328"><a name="p176952116328"></a><a name="p176952116328"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p669671153211"><a name="p669671153211"></a><a name="p669671153211"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p569616114324"><a name="p569616114324"></a><a name="p569616114324"></a>响应正文定义，参考<a href="#table669611115329">表12</a></p>
</td>
</tr>
</tbody>
</table>

**表 12**  schema参数说明

<a name="table669611115329"></a>
<table><thead align="left"><tr id="row1669620112329"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p8697111183220"><a name="p8697111183220"></a><a name="p8697111183220"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p1769712113328"><a name="p1769712113328"></a><a name="p1769712113328"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p8697311193217"><a name="p8697311193217"></a><a name="p8697311193217"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p069781118329"><a name="p069781118329"></a><a name="p069781118329"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row176977117320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p669791114323"><a name="p669791114323"></a><a name="p669791114323"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p1697141115325"><a name="p1697141115325"></a><a name="p1697141115325"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p16978113325"><a name="p16978113325"></a><a name="p16978113325"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1369816118326"><a name="p1369816118326"></a><a name="p1369816118326"></a>BODY体描述</p>
</td>
</tr>
<tr id="row12698131143214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p169801116326"><a name="p169801116326"></a><a name="p169801116326"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p369811113323"><a name="p369811113323"></a><a name="p369811113323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p16698181163220"><a name="p16698181163220"></a><a name="p16698181163220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1698111183210"><a name="p1698111183210"></a><a name="p1698111183210"></a>BODY体类型：FORM/STREAM（表单/字节流）</p>
</td>
</tr>
</tbody>
</table>

**表 13**  securityDefinitions参数说明

<a name="table20698111119323"></a>
<table><thead align="left"><tr id="row769913115322"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="p5699171113327"><a name="p5699171113327"></a><a name="p5699171113327"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.2"><p id="p66995116320"><a name="p66995116320"></a><a name="p66995116320"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="p1699511113214"><a name="p1699511113214"></a><a name="p1699511113214"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.46534653465347%" id="mcps1.2.5.1.4"><p id="p16991111153212"><a name="p16991111153212"></a><a name="p16991111153212"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row8699911193217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p569913112328"><a name="p569913112328"></a><a name="p569913112328"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.2 "><p id="p569914119320"><a name="p569914119320"></a><a name="p569914119320"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p20699611123220"><a name="p20699611123220"></a><a name="p20699611123220"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="53.46534653465347%" headers="mcps1.2.5.1.4 "><p id="p1169951143212"><a name="p1169951143212"></a><a name="p1169951143212"></a>自定义鉴权方式名称，参考<a href="#table1969951114328">表14</a></p>
</td>
</tr>
</tbody>
</table>

**表 14**  name参数说明

<a name="table1969951114328"></a>
<table><thead align="left"><tr id="row670031103213"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p170013113323"><a name="p170013113323"></a><a name="p170013113323"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1670001114329"><a name="p1670001114329"></a><a name="p1670001114329"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p18700211113213"><a name="p18700211113213"></a><a name="p18700211113213"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p187006118322"><a name="p187006118322"></a><a name="p187006118322"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row117008118323"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1070061193217"><a name="p1070061193217"></a><a name="p1070061193217"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p070071153213"><a name="p070071153213"></a><a name="p070071153213"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p20700121119320"><a name="p20700121119320"></a><a name="p20700121119320"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p6700201143210"><a name="p6700201143210"></a><a name="p6700201143210"></a>鉴权类型，支持apiKey</p>
</td>
</tr>
<tr id="row1070071113210"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1701111103215"><a name="p1701111103215"></a><a name="p1701111103215"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p167015118329"><a name="p167015118329"></a><a name="p167015118329"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p970181120324"><a name="p970181120324"></a><a name="p970181120324"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p6701131117328"><a name="p6701131117328"></a><a name="p6701131117328"></a>apiKey参数名称</p>
</td>
</tr>
<tr id="row7701161117327"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p970111163211"><a name="p970111163211"></a><a name="p970111163211"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p270113118328"><a name="p270113118328"></a><a name="p270113118328"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p7701711113216"><a name="p7701711113216"></a><a name="p7701711113216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1701171118324"><a name="p1701171118324"></a><a name="p1701171118324"></a>apiKey参数位置</p>
</td>
</tr>
<tr id="row870191193211"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p14701111113219"><a name="p14701111113219"></a><a name="p14701111113219"></a>x-apigateway-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1870114116327"><a name="p1870114116327"></a><a name="p1870114116327"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1270220115323"><a name="p1270220115323"></a><a name="p1270220115323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p070231118324"><a name="p070231118324"></a><a name="p070231118324"></a>扩展鉴权类型，基于apiKey鉴权方式的扩展，网关自定义的鉴权方式，支持AppSigv1、IAM、IAM_NONE</p>
</td>
</tr>
</tbody>
</table>

**表 15**  x-apigateway-backend参数说明

<a name="table387619483252"></a>
<table><thead align="left"><tr id="row1487734812520"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p487734814254"><a name="p487734814254"></a><a name="p487734814254"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p58771548122516"><a name="p58771548122516"></a><a name="p58771548122516"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p287774812511"><a name="p287774812511"></a><a name="p287774812511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p13877134815251"><a name="p13877134815251"></a><a name="p13877134815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10877114822512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p2878144892516"><a name="p2878144892516"></a><a name="p2878144892516"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p15878648182515"><a name="p15878648182515"></a><a name="p15878648182515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p587811480258"><a name="p587811480258"></a><a name="p587811480258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p2878134802519"><a name="p2878134802519"></a><a name="p2878134802519"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="row8878174811255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p187864862516"><a name="p187864862516"></a><a name="p187864862516"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p387834820252"><a name="p387834820252"></a><a name="p387834820252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p0878848142512"><a name="p0878848142512"></a><a name="p0878848142512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1887854802516"><a name="p1887854802516"></a><a name="p1887854802516"></a>后端参数对象数组定义，参考<a href="#table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="row1387834892518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1587934817256"><a name="p1587934817256"></a><a name="p1587934817256"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p587924822511"><a name="p587924822511"></a><a name="p587924822511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p20879124802513"><a name="p20879124802513"></a><a name="p20879124802513"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p19879134862517"><a name="p19879134862517"></a><a name="p19879134862517"></a>API后端定义</p>
<p id="p9879144815251"><a name="p9879144815251"></a><a name="p9879144815251"></a>backend_define支持：</p>
<a name="ul587916489258"></a><a name="ul587916489258"></a><ul id="ul587916489258"><li>httpEndpoints，参考<a href="#table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
</tbody>
</table>

**表 16**  x-apigateway-backend-policies参数说明

<a name="table1988034862512"></a>
<table><thead align="left"><tr id="row788004814256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p148801248112517"><a name="p148801248112517"></a><a name="p148801248112517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p28801048112514"><a name="p28801048112514"></a><a name="p28801048112514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p5880164872513"><a name="p5880164872513"></a><a name="p5880164872513"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p8881948132519"><a name="p8881948132519"></a><a name="p8881948132519"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row118811748112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p688117485256"><a name="p688117485256"></a><a name="p688117485256"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p688164822510"><a name="p688164822510"></a><a name="p688164822510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p178819481257"><a name="p178819481257"></a><a name="p178819481257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p13881448102510"><a name="p13881448102510"></a><a name="p13881448102510"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="row9881134862515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p19881204822515"><a name="p19881204822515"></a><a name="p19881204822515"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1888114862515"><a name="p1888114862515"></a><a name="p1888114862515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p78817484250"><a name="p78817484250"></a><a name="p78817484250"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1588144814252"><a name="p1588144814252"></a><a name="p1588144814252"></a>后端策略名称</p>
</td>
</tr>
<tr id="row588184817258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p2882124882517"><a name="p2882124882517"></a><a name="p2882124882517"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p988244811251"><a name="p988244811251"></a><a name="p988244811251"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p5882248152519"><a name="p5882248152519"></a><a name="p5882248152519"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p188218488257"><a name="p188218488257"></a><a name="p188218488257"></a>后端参数对象数组定义，参考<a href="#table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="row1188204822510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p19882184892513"><a name="p19882184892513"></a><a name="p19882184892513"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p6882104862512"><a name="p6882104862512"></a><a name="p6882104862512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p138821548172512"><a name="p138821548172512"></a><a name="p138821548172512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p15882164816258"><a name="p15882164816258"></a><a name="p15882164816258"></a>API后端定义</p>
<p id="p188214481259"><a name="p188214481259"></a><a name="p188214481259"></a>backend_define支持：</p>
<a name="ul0883104814256"></a><a name="ul0883104814256"></a><ul id="ul0883104814256"><li>httpEndpoints，参考<a href="#table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
<tr id="row48838483257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p18883948172520"><a name="p18883948172520"></a><a name="p18883948172520"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p6883184852518"><a name="p6883184852518"></a><a name="p6883184852518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p68846483259"><a name="p68846483259"></a><a name="p68846483259"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p988404813253"><a name="p988404813253"></a><a name="p988404813253"></a>策略条件对象数组定义，参考<a href="#table1790444832520">表 conditions参数说明</a></p>
</td>
</tr>
<tr id="row8601019134513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1571041123212"><a name="p1571041123212"></a><a name="p1571041123212"></a>effectMode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p12710161117322"><a name="p12710161117322"></a><a name="p12710161117322"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1571131163218"><a name="p1571131163218"></a><a name="p1571131163218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p167111211143213"><a name="p167111211143213"></a><a name="p167111211143213"></a>关联的策略组合模式，支持ANY、ALL</p>
</td>
</tr>
</tbody>
</table>

**表 17**  后端parameters参数说明

<a name="table14884114882511"></a>
<table><thead align="left"><tr id="row1088574822512"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p88856489251"><a name="p88856489251"></a><a name="p88856489251"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p18885048132510"><a name="p18885048132510"></a><a name="p18885048132510"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p19885124810250"><a name="p19885124810250"></a><a name="p19885124810250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p188851448172515"><a name="p188851448172515"></a><a name="p188851448172515"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row138861748112511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p788674832520"><a name="p788674832520"></a><a name="p788674832520"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p148868484256"><a name="p148868484256"></a><a name="p148868484256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1688664812515"><a name="p1688664812515"></a><a name="p1688664812515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p14886948102519"><a name="p14886948102519"></a><a name="p14886948102519"></a>参数名称，由字母、数字、下划线、连线、点组成，以字母开头，最长32字节</p>
<p id="p1988624813251"><a name="p1988624813251"></a><a name="p1988624813251"></a>header位置的参数名称不区分大小写</p>
</td>
</tr>
<tr id="row388674862513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1888620480254"><a name="p1888620480254"></a><a name="p1888620480254"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p98861548152515"><a name="p98861548152515"></a><a name="p98861548152515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p0886174810255"><a name="p0886174810255"></a><a name="p0886174810255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p19886748182513"><a name="p19886748182513"></a><a name="p19886748182513"></a>参数值，当参数来源为REQUEST时，值为请求参数名称</p>
</td>
</tr>
<tr id="row10886148132513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p13887134822517"><a name="p13887134822517"></a><a name="p13887134822517"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1788764862518"><a name="p1788764862518"></a><a name="p1788764862518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p18887164815251"><a name="p18887164815251"></a><a name="p18887164815251"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p8887174812258"><a name="p8887174812258"></a><a name="p8887174812258"></a>参数位置，支持header、query、path</p>
</td>
</tr>
<tr id="row788711486259"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p4887148182510"><a name="p4887148182510"></a><a name="p4887148182510"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1588714814252"><a name="p1588714814252"></a><a name="p1588714814252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p14887144815254"><a name="p14887144815254"></a><a name="p14887144815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p9887104882515"><a name="p9887104882515"></a><a name="p9887104882515"></a>参数映射来源，支持REQUEST、CONSTANT</p>
</td>
</tr>
<tr id="row10888204816254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1988894882514"><a name="p1988894882514"></a><a name="p1988894882514"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1788864811250"><a name="p1788864811250"></a><a name="p1788864811250"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1288854812255"><a name="p1288854812255"></a><a name="p1288854812255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p17888184822511"><a name="p17888184822511"></a><a name="p17888184822511"></a>参数含义描述</p>
</td>
</tr>
</tbody>
</table>

**表 18**  后端httpEndpoints参数说明

<a name="table1788894822518"></a>
<table><thead align="left"><tr id="row988984817253"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p18892048172520"><a name="p18892048172520"></a><a name="p18892048172520"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p12889204812514"><a name="p12889204812514"></a><a name="p12889204812514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p168897485253"><a name="p168897485253"></a><a name="p168897485253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p4889144818251"><a name="p4889144818251"></a><a name="p4889144818251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7889164818257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p158899481251"><a name="p158899481251"></a><a name="p158899481251"></a>address</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p19889134812514"><a name="p19889134812514"></a><a name="p19889134812514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p289054818257"><a name="p289054818257"></a><a name="p289054818257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p389044816256"><a name="p389044816256"></a><a name="p389044816256"></a>后端服务地址，格式为：&lt;域名或IP&gt;:[port]</p>
</td>
</tr>
<tr id="row13890348152517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p48902486252"><a name="p48902486252"></a><a name="p48902486252"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p198901048142519"><a name="p198901048142519"></a><a name="p198901048142519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p188901488253"><a name="p188901488253"></a><a name="p188901488253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p689013488253"><a name="p689013488253"></a><a name="p689013488253"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="row88902048112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p13890134816252"><a name="p13890134816252"></a><a name="p13890134816252"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1089013489252"><a name="p1089013489252"></a><a name="p1089013489252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p118901148172513"><a name="p118901148172513"></a><a name="p118901148172513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1989074812515"><a name="p1989074812515"></a><a name="p1989074812515"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="row7890104822514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p5890144882519"><a name="p5890144882519"></a><a name="p5890144882519"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p28911948182519"><a name="p28911948182519"></a><a name="p28911948182519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p68915482252"><a name="p68915482252"></a><a name="p68915482252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p188912048192510"><a name="p188912048192510"></a><a name="p188912048192510"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="row13891204812255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p58911948132514"><a name="p58911948132514"></a><a name="p58911948132514"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1389194814256"><a name="p1389194814256"></a><a name="p1389194814256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p889124812510"><a name="p889124812510"></a><a name="p889124812510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p189264813251"><a name="p189264813251"></a><a name="p189264813251"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="row7635433104612"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p171721112324"><a name="p171721112324"></a><a name="p171721112324"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p871801119323"><a name="p871801119323"></a><a name="p871801119323"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p19718611193219"><a name="p19718611193219"></a><a name="p19718611193219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1571891123210"><a name="p1571891123210"></a><a name="p1571891123210"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 19**  后端httpVpcEndpoints参数说明

<a name="table1089314812254"></a>
<table><thead align="left"><tr id="row489354813256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p16893104820253"><a name="p16893104820253"></a><a name="p16893104820253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p14893548102518"><a name="p14893548102518"></a><a name="p14893548102518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p7893184852520"><a name="p7893184852520"></a><a name="p7893184852520"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p1789304832517"><a name="p1789304832517"></a><a name="p1789304832517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row389304819258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p089494814258"><a name="p089494814258"></a><a name="p089494814258"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p188941948112519"><a name="p188941948112519"></a><a name="p188941948112519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p2089418484250"><a name="p2089418484250"></a><a name="p2089418484250"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p78948486252"><a name="p78948486252"></a><a name="p78948486252"></a>VPC通道名称</p>
</td>
</tr>
<tr id="row19894104862518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1089464852513"><a name="p1089464852513"></a><a name="p1089464852513"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p138945480256"><a name="p138945480256"></a><a name="p138945480256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p989454862516"><a name="p989454862516"></a><a name="p989454862516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p2894248162512"><a name="p2894248162512"></a><a name="p2894248162512"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="row1189484812512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1589413486258"><a name="p1589413486258"></a><a name="p1589413486258"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p148947482254"><a name="p148947482254"></a><a name="p148947482254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1689418486254"><a name="p1689418486254"></a><a name="p1689418486254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p2089444817252"><a name="p2089444817252"></a><a name="p2089444817252"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="row14895164817252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p11895194818252"><a name="p11895194818252"></a><a name="p11895194818252"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p28958484255"><a name="p28958484255"></a><a name="p28958484255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p13895448142512"><a name="p13895448142512"></a><a name="p13895448142512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1189594813254"><a name="p1189594813254"></a><a name="p1189594813254"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="row1689594819251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p0895104832517"><a name="p0895104832517"></a><a name="p0895104832517"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p11895184862514"><a name="p11895184862514"></a><a name="p11895184862514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p108951948172512"><a name="p108951948172512"></a><a name="p108951948172512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1289515487258"><a name="p1289515487258"></a><a name="p1289515487258"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="row18895184802511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p2895134820259"><a name="p2895134820259"></a><a name="p2895134820259"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p9895144815256"><a name="p9895144815256"></a><a name="p9895144815256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p168952482254"><a name="p168952482254"></a><a name="p168952482254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p9896194812253"><a name="p9896194812253"></a><a name="p9896194812253"></a>VPC通道代理主机</p>
</td>
</tr>
<tr id="row126916399464"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1205124114618"><a name="p1205124114618"></a><a name="p1205124114618"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p11205204144619"><a name="p11205204144619"></a><a name="p11205204144619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p172056411467"><a name="p172056411467"></a><a name="p172056411467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1520564144612"><a name="p1520564144612"></a><a name="p1520564144612"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 20**  后端functionEndpoints参数说明

<a name="table18971648202512"></a>
<table><thead align="left"><tr id="row14897184815257"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1389711486257"><a name="p1389711486257"></a><a name="p1389711486257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1589724814251"><a name="p1589724814251"></a><a name="p1589724814251"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p589714815258"><a name="p589714815258"></a><a name="p589714815258"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p389818487257"><a name="p389818487257"></a><a name="p389818487257"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row58981348182516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1689814802516"><a name="p1689814802516"></a><a name="p1689814802516"></a>function-urn</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p7898114818255"><a name="p7898114818255"></a><a name="p7898114818255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p13898114852515"><a name="p13898114852515"></a><a name="p13898114852515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p589884811259"><a name="p589884811259"></a><a name="p589884811259"></a>函数URN地址</p>
</td>
</tr>
<tr id="row128984488256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p12899648152514"><a name="p12899648152514"></a><a name="p12899648152514"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1189984814258"><a name="p1189984814258"></a><a name="p1189984814258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p178991448162510"><a name="p178991448162510"></a><a name="p178991448162510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1899174832517"><a name="p1899174832517"></a><a name="p1899174832517"></a>函数版本</p>
</td>
</tr>
<tr id="row0899134815250"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p9899348162513"><a name="p9899348162513"></a><a name="p9899348162513"></a>invocation-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p289910485254"><a name="p289910485254"></a><a name="p289910485254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p18991348102516"><a name="p18991348102516"></a><a name="p18991348102516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p189984818250"><a name="p189984818250"></a><a name="p189984818250"></a>函数调用类型，支持async、sync</p>
</td>
</tr>
<tr id="row28995482255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1290018487253"><a name="p1290018487253"></a><a name="p1290018487253"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p490010489253"><a name="p490010489253"></a><a name="p490010489253"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p3900148112515"><a name="p3900148112515"></a><a name="p3900148112515"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p3900154822516"><a name="p3900154822516"></a><a name="p3900154822516"></a>函数超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="row4948164516468"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p417724714468"><a name="p417724714468"></a><a name="p417724714468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p20177147174614"><a name="p20177147174614"></a><a name="p20177147174614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p2178184712466"><a name="p2178184712466"></a><a name="p2178184712466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p131781547144613"><a name="p131781547144613"></a><a name="p131781547144613"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 21**  后端mockEndpoints参数说明

<a name="table1790184862513"></a>
<table><thead align="left"><tr id="row1901104812518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p6902348122511"><a name="p6902348122511"></a><a name="p6902348122511"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p690215486256"><a name="p690215486256"></a><a name="p690215486256"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p7902548202519"><a name="p7902548202519"></a><a name="p7902548202519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p17902148202518"><a name="p17902148202518"></a><a name="p17902148202518"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row69021348202511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p14902448112512"><a name="p14902448112512"></a><a name="p14902448112512"></a>result-content</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p8902104816254"><a name="p8902104816254"></a><a name="p8902104816254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p19903648122510"><a name="p19903648122510"></a><a name="p19903648122510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p12903948172517"><a name="p12903948172517"></a><a name="p12903948172517"></a>MOCK返回结果</p>
</td>
</tr>
<tr id="row4433155454616"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1576125519468"><a name="p1576125519468"></a><a name="p1576125519468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1857675514611"><a name="p1857675514611"></a><a name="p1857675514611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p105761955174616"><a name="p105761955174616"></a><a name="p105761955174616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p05768551462"><a name="p05768551462"></a><a name="p05768551462"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 22**  conditions参数说明

<a name="table1790444832520"></a>
<table><thead align="left"><tr id="row199040482254"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p169051248112512"><a name="p169051248112512"></a><a name="p169051248112512"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p590554862518"><a name="p590554862518"></a><a name="p590554862518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p190564892511"><a name="p190564892511"></a><a name="p190564892511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p4905194815251"><a name="p4905194815251"></a><a name="p4905194815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row390544872514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p69056485258"><a name="p69056485258"></a><a name="p69056485258"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1290514820256"><a name="p1290514820256"></a><a name="p1290514820256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p190574819257"><a name="p190574819257"></a><a name="p190574819257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1190554892513"><a name="p1190554892513"></a><a name="p1190554892513"></a>策略条件类型，支持equal、enum、pattern</p>
</td>
</tr>
<tr id="row590619487256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p59061248132511"><a name="p59061248132511"></a><a name="p59061248132511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p159064483250"><a name="p159064483250"></a><a name="p159064483250"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1990644812258"><a name="p1990644812258"></a><a name="p1990644812258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1390694812519"><a name="p1390694812519"></a><a name="p1390694812519"></a>策略条件值</p>
</td>
</tr>
<tr id="row19906114813251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p209067480258"><a name="p209067480258"></a><a name="p209067480258"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p14906184813256"><a name="p14906184813256"></a><a name="p14906184813256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1690694811252"><a name="p1690694811252"></a><a name="p1690694811252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p159071748102517"><a name="p159071748102517"></a><a name="p159071748102517"></a>策略条件输入来源，支持source、request</p>
</td>
</tr>
<tr id="row16907248202516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p6907648162519"><a name="p6907648162519"></a><a name="p6907648162519"></a>parameter</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1290714882519"><a name="p1290714882519"></a><a name="p1290714882519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1690719487254"><a name="p1690719487254"></a><a name="p1690719487254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p149071484250"><a name="p149071484250"></a><a name="p149071484250"></a>策略条件输入来源为request时，请求入参的名称</p>
</td>
</tr>
</tbody>
</table>

**表 23**  x-apigateway-access-controls参数说明

<a name="table2090754816252"></a>
<table><thead align="left"><tr id="row179081748172515"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p209087484253"><a name="p209087484253"></a><a name="p209087484253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1490854819254"><a name="p1490854819254"></a><a name="p1490854819254"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p09082048122514"><a name="p09082048122514"></a><a name="p09082048122514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p390944819252"><a name="p390944819252"></a><a name="p390944819252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5909114852510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p18909174811252"><a name="p18909174811252"></a><a name="p18909174811252"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p109091448202516"><a name="p109091448202516"></a><a name="p109091448202516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p79098488251"><a name="p79098488251"></a><a name="p79098488251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p11909114819251"><a name="p11909114819251"></a><a name="p11909114819251"></a>指定名称的访问控制策略，参考<a href="#table39092048142510">表 acl_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 24**  acl\_name参数说明

<a name="table39092048142510"></a>
<table><thead align="left"><tr id="row191014812256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p991017483255"><a name="p991017483255"></a><a name="p991017483255"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p69108489253"><a name="p69108489253"></a><a name="p69108489253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p1591016486250"><a name="p1591016486250"></a><a name="p1591016486250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p891110481252"><a name="p891110481252"></a><a name="p891110481252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49111048102517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p129110482258"><a name="p129110482258"></a><a name="p129110482258"></a>acl-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p20911104892511"><a name="p20911104892511"></a><a name="p20911104892511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p13911174815258"><a name="p13911174815258"></a><a name="p13911174815258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p17911174882519"><a name="p17911174882519"></a><a name="p17911174882519"></a>访问控制行为，支持PERMIT、DENY</p>
</td>
</tr>
<tr id="row191154882520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1191254820251"><a name="p1191254820251"></a><a name="p1191254820251"></a>entity-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p169121248142514"><a name="p169121248142514"></a><a name="p169121248142514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p691294818254"><a name="p691294818254"></a><a name="p691294818254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p8912948182515"><a name="p8912948182515"></a><a name="p8912948182515"></a>访问控制对象，支持IP、DOMAIN</p>
</td>
</tr>
<tr id="row1391211489258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p11912194872511"><a name="p11912194872511"></a><a name="p11912194872511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p3912248192514"><a name="p3912248192514"></a><a name="p3912248192514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p6912848192513"><a name="p6912848192513"></a><a name="p6912848192513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p9913194862512"><a name="p9913194862512"></a><a name="p9913194862512"></a>访问控制策略值，多个值以“,”间隔</p>
</td>
</tr>
</tbody>
</table>

**表 25**  x-apigateway-ratelimits参数说明

<a name="table18913124872513"></a>
<table><thead align="left"><tr id="row17913648192518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p19913848152517"><a name="p19913848152517"></a><a name="p19913848152517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p891324822519"><a name="p891324822519"></a><a name="p891324822519"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p591411483253"><a name="p591411483253"></a><a name="p591411483253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p15914144811250"><a name="p15914144811250"></a><a name="p15914144811250"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1391424802514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p99141748112512"><a name="p99141748112512"></a><a name="p99141748112512"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p149141489252"><a name="p149141489252"></a><a name="p149141489252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p99145487257"><a name="p99145487257"></a><a name="p99145487257"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p39151248192510"><a name="p39151248192510"></a><a name="p39151248192510"></a>指定名称的流控策略，参考<a href="#table179155483256">表 throttle_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 26**  throttle\_name参数说明

<a name="table179155483256"></a>
<table><thead align="left"><tr id="row3915114811258"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1191616488258"><a name="p1191616488258"></a><a name="p1191616488258"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p199164484253"><a name="p199164484253"></a><a name="p199164484253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p29161648202514"><a name="p29161648202514"></a><a name="p29161648202514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p89168486252"><a name="p89168486252"></a><a name="p89168486252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39169488253"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p119161548182514"><a name="p119161548182514"></a><a name="p119161548182514"></a>api-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1391664819255"><a name="p1391664819255"></a><a name="p1391664819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p19174485250"><a name="p19174485250"></a><a name="p19174485250"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p59171489257"><a name="p59171489257"></a><a name="p59171489257"></a>API访问次数限制</p>
</td>
</tr>
<tr id="row14917194852515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p189171648112514"><a name="p189171648112514"></a><a name="p189171648112514"></a>user-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p18917174813252"><a name="p18917174813252"></a><a name="p18917174813252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p199171348162512"><a name="p199171348162512"></a><a name="p199171348162512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p4917448162510"><a name="p4917448162510"></a><a name="p4917448162510"></a>用户访问次数限制</p>
</td>
</tr>
<tr id="row129177484252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p6918104872519"><a name="p6918104872519"></a><a name="p6918104872519"></a>app-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1091894814255"><a name="p1091894814255"></a><a name="p1091894814255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p891804811257"><a name="p891804811257"></a><a name="p891804811257"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1918748152512"><a name="p1918748152512"></a><a name="p1918748152512"></a>应用访问次数限制</p>
</td>
</tr>
<tr id="row5918648192514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p179181648112513"><a name="p179181648112513"></a><a name="p179181648112513"></a>ip-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p15918548132512"><a name="p15918548132512"></a><a name="p15918548132512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p69181248132518"><a name="p69181248132518"></a><a name="p69181248132518"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p169192488255"><a name="p169192488255"></a><a name="p169192488255"></a>源IP访问次数限制</p>
</td>
</tr>
<tr id="row79191948142513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p491994816255"><a name="p491994816255"></a><a name="p491994816255"></a>interval</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p11919114819255"><a name="p11919114819255"></a><a name="p11919114819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p79191648132510"><a name="p79191648132510"></a><a name="p79191648132510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p119195483257"><a name="p119195483257"></a><a name="p119195483257"></a>流控策略时间周期</p>
</td>
</tr>
<tr id="row199198489254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1919154812517"><a name="p1919154812517"></a><a name="p1919154812517"></a>unit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1391916487253"><a name="p1391916487253"></a><a name="p1391916487253"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p292015486259"><a name="p292015486259"></a><a name="p292015486259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p3920748112517"><a name="p3920748112517"></a><a name="p3920748112517"></a>流控策略时间周期单位，支持SECOND、MINUTE、HOUR、DAY</p>
</td>
</tr>
<tr id="row14920174811258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p7920948132515"><a name="p7920948132515"></a><a name="p7920948132515"></a>shared</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p192019487254"><a name="p192019487254"></a><a name="p192019487254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1920124892513"><a name="p1920124892513"></a><a name="p1920124892513"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p17920174842518"><a name="p17920174842518"></a><a name="p17920174842518"></a>是否共享流控策略</p>
</td>
</tr>
<tr id="row1392010481255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p6921194816259"><a name="p6921194816259"></a><a name="p6921194816259"></a>special</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p29212489254"><a name="p29212489254"></a><a name="p29212489254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p792119480253"><a name="p792119480253"></a><a name="p792119480253"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p15921144832520"><a name="p15921144832520"></a><a name="p15921144832520"></a>特殊流控策略对象数组定义，参考<a href="#table6921174842513">表 special参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 27**  special参数说明

<a name="table6921174842513"></a>
<table><thead align="left"><tr id="row5922248112514"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1492234818256"><a name="p1492234818256"></a><a name="p1492234818256"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1292214818252"><a name="p1292214818252"></a><a name="p1292214818252"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p1192217488256"><a name="p1192217488256"></a><a name="p1192217488256"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p19922144810251"><a name="p19922144810251"></a><a name="p19922144810251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row109221348122519"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p4923448142518"><a name="p4923448142518"></a><a name="p4923448142518"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p792311483258"><a name="p792311483258"></a><a name="p792311483258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p392311487256"><a name="p392311487256"></a><a name="p392311487256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p292315488259"><a name="p292315488259"></a><a name="p292315488259"></a>特殊流控策略类型，支持APP、USER</p>
</td>
</tr>
<tr id="row1692304842514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p192311482252"><a name="p192311482252"></a><a name="p192311482252"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1292364814256"><a name="p1292364814256"></a><a name="p1292364814256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1092344819252"><a name="p1092344819252"></a><a name="p1092344819252"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p13923134817259"><a name="p13923134817259"></a><a name="p13923134817259"></a>访问次数</p>
</td>
</tr>
<tr id="row13923948122511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p15923248172511"><a name="p15923248172511"></a><a name="p15923248172511"></a>instance</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p4924448162510"><a name="p4924448162510"></a><a name="p4924448162510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p119249482253"><a name="p119249482253"></a><a name="p119249482253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p5924154822518"><a name="p5924154822518"></a><a name="p5924154822518"></a>特殊APP或USER的对象标识</p>
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

## 响应码<a name="section66318442384"></a>

**表 28**  返回消息说明

<a name="table11438104424617"></a>
<table><thead align="left"><tr id="row1643820448464"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p4272113476"><a name="p4272113476"></a><a name="p4272113476"></a>响应码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p202192154718"><a name="p202192154718"></a><a name="p202192154718"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row24383446462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p62162184714"><a name="p62162184714"></a><a name="p62162184714"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p112162113475"><a name="p112162113475"></a><a name="p112162113475"></a>OK</p>
</td>
</tr>
<tr id="row6438154417469"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1228216472"><a name="p1228216472"></a><a name="p1228216472"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p132182116477"><a name="p132182116477"></a><a name="p132182116477"></a>bad request</p>
</td>
</tr>
<tr id="row1943874416467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p12262144711"><a name="p12262144711"></a><a name="p12262144711"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p20220215475"><a name="p20220215475"></a><a name="p20220215475"></a>unauthorized</p>
</td>
</tr>
<tr id="row1043834417462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1292117477"><a name="p1292117477"></a><a name="p1292117477"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p32921144714"><a name="p32921144714"></a><a name="p32921144714"></a>forbidden</p>
</td>
</tr>
<tr id="row6439344194617"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p7282116471"><a name="p7282116471"></a><a name="p7282116471"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p62112110471"><a name="p62112110471"></a><a name="p62112110471"></a>server internal error</p>
</td>
</tr>
</tbody>
</table>

