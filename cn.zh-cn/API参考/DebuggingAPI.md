# 调试API<a name="ZH-CN_TOPIC_0000001082135093"></a>

## 功能介绍<a name="zh-cn_topic_0127644985_section56312882"></a>

调试一个API在指定运行环境下的定义，接口调用者需要具有操作该API的权限。

## URI<a name="zh-cn_topic_0127644985_section37053890"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0127644985_table61687544"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127644985_row6551303"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127644985_p60893511"><a name="zh-cn_topic_0127644985_p60893511"></a><a name="zh-cn_topic_0127644985_p60893511"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127644985_p33427368"><a name="zh-cn_topic_0127644985_p33427368"></a><a name="zh-cn_topic_0127644985_p33427368"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127644985_row23262289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127644985_p103940534920"><a name="zh-cn_topic_0127644985_p103940534920"></a><a name="zh-cn_topic_0127644985_p103940534920"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127644985_p18327454"><a name="zh-cn_topic_0127644985_p18327454"></a><a name="zh-cn_topic_0127644985_p18327454"></a>/v1.0/apigw/apis/debug/{api_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0127644985_table8128785"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127644985_row50936577"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0127644985_p32222095"><a name="zh-cn_topic_0127644985_p32222095"></a><a name="zh-cn_topic_0127644985_p32222095"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0127644985_p59852877"><a name="zh-cn_topic_0127644985_p59852877"></a><a name="zh-cn_topic_0127644985_p59852877"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0127644985_p16244835"><a name="zh-cn_topic_0127644985_p16244835"></a><a name="zh-cn_topic_0127644985_p16244835"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0127644985_p40763258"><a name="zh-cn_topic_0127644985_p40763258"></a><a name="zh-cn_topic_0127644985_p40763258"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127644985_row13489593"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p120121165010"><a name="zh-cn_topic_0127644985_p120121165010"></a><a name="zh-cn_topic_0127644985_p120121165010"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p55742162"><a name="zh-cn_topic_0127644985_p55742162"></a><a name="zh-cn_topic_0127644985_p55742162"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p18821243"><a name="zh-cn_topic_0127644985_p18821243"></a><a name="zh-cn_topic_0127644985_p18821243"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p48125676"><a name="zh-cn_topic_0127644985_p48125676"></a><a name="zh-cn_topic_0127644985_p48125676"></a>API的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0127644985_section65049557"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0127644985_table309072"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127644985_row29526596"><th class="cellrowborder" valign="top" width="19%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0127644985_p42844056"><a name="zh-cn_topic_0127644985_p42844056"></a><a name="zh-cn_topic_0127644985_p42844056"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0127644985_p47816505"><a name="zh-cn_topic_0127644985_p47816505"></a><a name="zh-cn_topic_0127644985_p47816505"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0127644985_p47931662"><a name="zh-cn_topic_0127644985_p47931662"></a><a name="zh-cn_topic_0127644985_p47931662"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="48%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0127644985_p57259391"><a name="zh-cn_topic_0127644985_p57259391"></a><a name="zh-cn_topic_0127644985_p57259391"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127644985_row7499126"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p16816103665116"><a name="zh-cn_topic_0127644985_p16816103665116"></a><a name="zh-cn_topic_0127644985_p16816103665116"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p10968591"><a name="zh-cn_topic_0127644985_p10968591"></a><a name="zh-cn_topic_0127644985_p10968591"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p16040707"><a name="zh-cn_topic_0127644985_p16040707"></a><a name="zh-cn_topic_0127644985_p16040707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p67075592516"><a name="zh-cn_topic_0127644985_p67075592516"></a><a name="zh-cn_topic_0127644985_p67075592516"></a>API的请求协议</p>
<a name="zh-cn_topic_0127644985_ul20473632195218"></a><a name="zh-cn_topic_0127644985_ul20473632195218"></a><ul id="zh-cn_topic_0127644985_ul20473632195218"><li>HTTP</li><li>HTTPS</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row1152012375215"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p95203365216"><a name="zh-cn_topic_0127644985_p95203365216"></a><a name="zh-cn_topic_0127644985_p95203365216"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p752043175212"><a name="zh-cn_topic_0127644985_p752043175212"></a><a name="zh-cn_topic_0127644985_p752043175212"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p1652014315529"><a name="zh-cn_topic_0127644985_p1652014315529"></a><a name="zh-cn_topic_0127644985_p1652014315529"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p35201313527"><a name="zh-cn_topic_0127644985_p35201313527"></a><a name="zh-cn_topic_0127644985_p35201313527"></a>API的请求方法</p>
<a name="zh-cn_topic_0127644985_ul46261614"></a><a name="zh-cn_topic_0127644985_ul46261614"></a><ul id="zh-cn_topic_0127644985_ul46261614"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row15871156205219"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p1458775615522"><a name="zh-cn_topic_0127644985_p1458775615522"></a><a name="zh-cn_topic_0127644985_p1458775615522"></a>domain</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p13587205611527"><a name="zh-cn_topic_0127644985_p13587205611527"></a><a name="zh-cn_topic_0127644985_p13587205611527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p45876561525"><a name="zh-cn_topic_0127644985_p45876561525"></a><a name="zh-cn_topic_0127644985_p45876561525"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p1258755615522"><a name="zh-cn_topic_0127644985_p1258755615522"></a><a name="zh-cn_topic_0127644985_p1258755615522"></a>API的访问域名，未提供时根据mode的取值使用如下默认值：</p>
<a name="zh-cn_topic_0127644985_ul1486116516544"></a><a name="zh-cn_topic_0127644985_ul1486116516544"></a><ul id="zh-cn_topic_0127644985_ul1486116516544"><li>DEVELOPER  API分组的子域名</li><li>MARKET  云市场为API分组分配的域名</li><li>CONSUMER  API分组的子域名</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row1094714271532"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p10947102765310"><a name="zh-cn_topic_0127644985_p10947102765310"></a><a name="zh-cn_topic_0127644985_p10947102765310"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p16947122710538"><a name="zh-cn_topic_0127644985_p16947122710538"></a><a name="zh-cn_topic_0127644985_p16947122710538"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p11947122715536"><a name="zh-cn_topic_0127644985_p11947122715536"></a><a name="zh-cn_topic_0127644985_p11947122715536"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p1494752775317"><a name="zh-cn_topic_0127644985_p1494752775317"></a><a name="zh-cn_topic_0127644985_p1494752775317"></a>API的请求路径，需以"/"开头，最大长度1024</p>
<div class="note" id="zh-cn_topic_0127644985_note690163615371"><a name="zh-cn_topic_0127644985_note690163615371"></a><a name="zh-cn_topic_0127644985_note690163615371"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0127644985_p09053643719"><a name="zh-cn_topic_0127644985_p09053643719"></a><a name="zh-cn_topic_0127644985_p09053643719"></a>须符合路径规范，百分号编码格式可被正确解码</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row827441515565"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p17274715125612"><a name="zh-cn_topic_0127644985_p17274715125612"></a><a name="zh-cn_topic_0127644985_p17274715125612"></a>query</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p2027481516566"><a name="zh-cn_topic_0127644985_p2027481516566"></a><a name="zh-cn_topic_0127644985_p2027481516566"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p192741315105620"><a name="zh-cn_topic_0127644985_p192741315105620"></a><a name="zh-cn_topic_0127644985_p192741315105620"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p2858226330"><a name="zh-cn_topic_0127644985_p2858226330"></a><a name="zh-cn_topic_0127644985_p2858226330"></a>查询参数，每个参数值为字符串数组，每个参数名称有如下约束：</p>
<a name="zh-cn_topic_0127644985_ul08844490338"></a><a name="zh-cn_topic_0127644985_ul08844490338"></a><ul id="zh-cn_topic_0127644985_ul08844490338"><li>英文字母、数字、点、下划线、中连线组成</li><li>必须以英文字母开头，最长32字节</li><li>不支持以"X-Apig-"或"X-Sdk-"开头，不区分大小写</li><li>不支持取值为"X-Stage"，不区分大小写</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row1262645612597"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p132831832010"><a name="zh-cn_topic_0127644985_p132831832010"></a><a name="zh-cn_topic_0127644985_p132831832010"></a>header</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p1662685605920"><a name="zh-cn_topic_0127644985_p1662685605920"></a><a name="zh-cn_topic_0127644985_p1662685605920"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p6626195655913"><a name="zh-cn_topic_0127644985_p6626195655913"></a><a name="zh-cn_topic_0127644985_p6626195655913"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p17166141513342"><a name="zh-cn_topic_0127644985_p17166141513342"></a><a name="zh-cn_topic_0127644985_p17166141513342"></a>头域参数，每个参数值为字符串数组，每个参数名称有如下约束：</p>
<a name="zh-cn_topic_0127644985_ul14449184533417"></a><a name="zh-cn_topic_0127644985_ul14449184533417"></a><ul id="zh-cn_topic_0127644985_ul14449184533417"><li>英文字母、数字、点、中连线组成</li><li>必须以英文字母开头，最长32字节</li><li>不支持以"X-Apig-"或"X-Sdk-"开头，不区分大小写</li><li>不支持取值为"X-Stage"，不区分大小写</li><li>mode为MARKET或CONSUMER时，不支持取值为"X-Auth-Token"和"Authorization"，不区分大小写</li></ul>
<div class="note" id="zh-cn_topic_0127644985_note08274215316"><a name="zh-cn_topic_0127644985_note08274215316"></a><a name="zh-cn_topic_0127644985_note08274215316"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0127644985_p3982421537"><a name="zh-cn_topic_0127644985_p3982421537"></a><a name="zh-cn_topic_0127644985_p3982421537"></a>头域名称在使用前会被规范化，如："x-MY-hEaDer"会被规范化为"X-My-Header"</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row98331529264"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p1483319291666"><a name="zh-cn_topic_0127644985_p1483319291666"></a><a name="zh-cn_topic_0127644985_p1483319291666"></a>body</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p88332029760"><a name="zh-cn_topic_0127644985_p88332029760"></a><a name="zh-cn_topic_0127644985_p88332029760"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p5833142920613"><a name="zh-cn_topic_0127644985_p5833142920613"></a><a name="zh-cn_topic_0127644985_p5833142920613"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p14833329261"><a name="zh-cn_topic_0127644985_p14833329261"></a><a name="zh-cn_topic_0127644985_p14833329261"></a>请求消息体，最长2097152字节</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row85951774712"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p2595147373"><a name="zh-cn_topic_0127644985_p2595147373"></a><a name="zh-cn_topic_0127644985_p2595147373"></a>mode</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p1159512710713"><a name="zh-cn_topic_0127644985_p1159512710713"></a><a name="zh-cn_topic_0127644985_p1159512710713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p8595167470"><a name="zh-cn_topic_0127644985_p8595167470"></a><a name="zh-cn_topic_0127644985_p8595167470"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p15595571716"><a name="zh-cn_topic_0127644985_p15595571716"></a><a name="zh-cn_topic_0127644985_p15595571716"></a>调试模式</p>
<a name="zh-cn_topic_0127644985_ul583020438716"></a><a name="zh-cn_topic_0127644985_ul583020438716"></a><ul id="zh-cn_topic_0127644985_ul583020438716"><li>DEVELOPER 调试尚未发布的API定义</li><li>MARKET 调试云市场已购买的API</li><li>CONSUMER  调试指定运行环境下的API定义<div class="note" id="zh-cn_topic_0127644985_note1595864010817"><a name="zh-cn_topic_0127644985_note1595864010817"></a><a name="zh-cn_topic_0127644985_note1595864010817"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0127644985_p289123819351"><a name="zh-cn_topic_0127644985_p289123819351"></a><a name="zh-cn_topic_0127644985_p289123819351"></a>DEVELOPER模式，接口调用者必须是API拥有者。</p>
<p id="zh-cn_topic_0127644985_p1951214213517"><a name="zh-cn_topic_0127644985_p1951214213517"></a><a name="zh-cn_topic_0127644985_p1951214213517"></a>MARKET模式，接口调用者必须是API购买者或拥有者。</p>
<p id="zh-cn_topic_0127644985_p695810405813"><a name="zh-cn_topic_0127644985_p695810405813"></a><a name="zh-cn_topic_0127644985_p695810405813"></a>CONSUMER模式，接口调用者必须有API在指定环境上的授权信息或是API拥有者。</p>
</div></div>
</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row23911659899"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p15391145912918"><a name="zh-cn_topic_0127644985_p15391145912918"></a><a name="zh-cn_topic_0127644985_p15391145912918"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p1939195913918"><a name="zh-cn_topic_0127644985_p1939195913918"></a><a name="zh-cn_topic_0127644985_p1939195913918"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p83917599912"><a name="zh-cn_topic_0127644985_p83917599912"></a><a name="zh-cn_topic_0127644985_p83917599912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p14391145914910"><a name="zh-cn_topic_0127644985_p14391145914910"></a><a name="zh-cn_topic_0127644985_p14391145914910"></a>调试请求使用的APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row2563133541010"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p4563203501020"><a name="zh-cn_topic_0127644985_p4563203501020"></a><a name="zh-cn_topic_0127644985_p4563203501020"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p1256313359107"><a name="zh-cn_topic_0127644985_p1256313359107"></a><a name="zh-cn_topic_0127644985_p1256313359107"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p3563163518106"><a name="zh-cn_topic_0127644985_p3563163518106"></a><a name="zh-cn_topic_0127644985_p3563163518106"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p856393571013"><a name="zh-cn_topic_0127644985_p856393571013"></a><a name="zh-cn_topic_0127644985_p856393571013"></a>调试请求使用的APP的密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row14715186141111"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127644985_p671516618112"><a name="zh-cn_topic_0127644985_p671516618112"></a><a name="zh-cn_topic_0127644985_p671516618112"></a>stage</p>
</td>
<td class="cellrowborder" valign="top" width="18%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127644985_p20715668114"><a name="zh-cn_topic_0127644985_p20715668114"></a><a name="zh-cn_topic_0127644985_p20715668114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127644985_p18715663111"><a name="zh-cn_topic_0127644985_p18715663111"></a><a name="zh-cn_topic_0127644985_p18715663111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="48%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127644985_p15715136151112"><a name="zh-cn_topic_0127644985_p15715136151112"></a><a name="zh-cn_topic_0127644985_p15715136151112"></a>调试请求指定的运行环境，仅在mode为CONSUMER时有效，未提供时有如下默认值:</p>
<a name="zh-cn_topic_0127644985_ul18649106151217"></a><a name="zh-cn_topic_0127644985_ul18649106151217"></a><ul id="zh-cn_topic_0127644985_ul18649106151217"><li>CONSUMER   RELEASE</li></ul>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "mode": "DEVELOPER",
  "scheme": "HTTPS",
  "method": "GET",
  "path": "/test",
  "query": {
    "city": [
      "shenzhen",
      "beijing"
    ]
  },
  "header": {
    "X-My-City": [
      "shenzhen",
      "beijing"
    ]
  }
}
```

## 响应消息<a name="zh-cn_topic_0127644985_section34522802"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0127644985_table11945837"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127644985_row18624964"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0127644985_p32227090"><a name="zh-cn_topic_0127644985_p32227090"></a><a name="zh-cn_topic_0127644985_p32227090"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0127644985_p60257464"><a name="zh-cn_topic_0127644985_p60257464"></a><a name="zh-cn_topic_0127644985_p60257464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0127644985_p49016415"><a name="zh-cn_topic_0127644985_p49016415"></a><a name="zh-cn_topic_0127644985_p49016415"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127644985_row10906670"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127644985_p11025102"><a name="zh-cn_topic_0127644985_p11025102"></a><a name="zh-cn_topic_0127644985_p11025102"></a>request</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127644985_p20618087"><a name="zh-cn_topic_0127644985_p20618087"></a><a name="zh-cn_topic_0127644985_p20618087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127644985_p59452320"><a name="zh-cn_topic_0127644985_p59452320"></a><a name="zh-cn_topic_0127644985_p59452320"></a>调试请求报文内容</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row65308832"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127644985_p1538153014199"><a name="zh-cn_topic_0127644985_p1538153014199"></a><a name="zh-cn_topic_0127644985_p1538153014199"></a>response</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127644985_p1151149"><a name="zh-cn_topic_0127644985_p1151149"></a><a name="zh-cn_topic_0127644985_p1151149"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127644985_p10288103619190"><a name="zh-cn_topic_0127644985_p10288103619190"></a><a name="zh-cn_topic_0127644985_p10288103619190"></a>调试响应报文内容，响应消息体最大支持2097152字节，超过部分会被截断</p>
<div class="note" id="zh-cn_topic_0127644985_note1812205217375"><a name="zh-cn_topic_0127644985_note1812205217375"></a><a name="zh-cn_topic_0127644985_note1812205217375"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0127644985_p1682825273717"><a name="zh-cn_topic_0127644985_p1682825273717"></a><a name="zh-cn_topic_0127644985_p1682825273717"></a>响应消息体超过限制长度时，超过部分会被截断，并追加"[TRUNCATED]"信息。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row33881960"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127644985_p358425731919"><a name="zh-cn_topic_0127644985_p358425731919"></a><a name="zh-cn_topic_0127644985_p358425731919"></a>latency</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127644985_p34986207"><a name="zh-cn_topic_0127644985_p34986207"></a><a name="zh-cn_topic_0127644985_p34986207"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127644985_p84751816203"><a name="zh-cn_topic_0127644985_p84751816203"></a><a name="zh-cn_topic_0127644985_p84751816203"></a>调试耗时，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row3577279"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0127644985_p164021426202010"><a name="zh-cn_topic_0127644985_p164021426202010"></a><a name="zh-cn_topic_0127644985_p164021426202010"></a>log</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0127644985_p49535636"><a name="zh-cn_topic_0127644985_p49535636"></a><a name="zh-cn_topic_0127644985_p49535636"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0127644985_p20824543152020"><a name="zh-cn_topic_0127644985_p20824543152020"></a><a name="zh-cn_topic_0127644985_p20824543152020"></a>调试过程日志</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "request": "GET /test?city=shenzhen&city=beijing HTTP/1.1\r\nHost: edf94892b11d440795562cb81c5be059.apigw.example.com\r\nUser-Agent: APIGatewayDebugClient/1.0\r\nX-Apig-Mode: debug\r\nX-My-City: shenzhen\r\nX-My-City: beijing\r\n\r\n",
  "response": "HTTP/1.1 200 OK\r\nContent-Length: 33\r\nConnection: keep-alive\r\nContent-Type: application/json; charset=utf-8\r\nDate: Fri, 24 Aug 2018 10:36:47 GMT\r\nServer: api-gateway\r\nX-Apig-Latency: 13\r\nX-Apig-Ratelimit-Api: remain:92,limit:100,time:1 minute\r\nX-Apig-Ratelimit-Api-Allenv: remain:9,limit:10,time:1 second\r\nX-Apig-Upstream-Latency: 1\r\nX-Request-Id: 12f69943cc2fa4f8a3674ee947655339\r\n\r\n{\"version\":\"4.0.12.201808190004\"}",
  "latency": "12",
  "log": ""
}
```

## 状态码<a name="zh-cn_topic_0127644985_section48575109"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0127644985_table5357896"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127644985_row27259487"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127644985_p60534834"><a name="zh-cn_topic_0127644985_p60534834"></a><a name="zh-cn_topic_0127644985_p60534834"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127644985_p4374530"><a name="zh-cn_topic_0127644985_p4374530"></a><a name="zh-cn_topic_0127644985_p4374530"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127644985_row18792630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127644985_p45808055"><a name="zh-cn_topic_0127644985_p45808055"></a><a name="zh-cn_topic_0127644985_p45808055"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127644985_p50988816"><a name="zh-cn_topic_0127644985_p50988816"></a><a name="zh-cn_topic_0127644985_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row40966733"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127644985_p29971116"><a name="zh-cn_topic_0127644985_p29971116"></a><a name="zh-cn_topic_0127644985_p29971116"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127644985_p29757115610"><a name="zh-cn_topic_0127644985_p29757115610"></a><a name="zh-cn_topic_0127644985_p29757115610"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row38563414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127644985_p36628845"><a name="zh-cn_topic_0127644985_p36628845"></a><a name="zh-cn_topic_0127644985_p36628845"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127644985_p9203142078"><a name="zh-cn_topic_0127644985_p9203142078"></a><a name="zh-cn_topic_0127644985_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row60209613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127644985_p45140486"><a name="zh-cn_topic_0127644985_p45140486"></a><a name="zh-cn_topic_0127644985_p45140486"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127644985_p13949586"><a name="zh-cn_topic_0127644985_p13949586"></a><a name="zh-cn_topic_0127644985_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row24071607"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127644985_p3643149"><a name="zh-cn_topic_0127644985_p3643149"></a><a name="zh-cn_topic_0127644985_p3643149"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127644985_p26659623"><a name="zh-cn_topic_0127644985_p26659623"></a><a name="zh-cn_topic_0127644985_p26659623"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0127644985_row0236225132310"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127644985_p1723616257232"><a name="zh-cn_topic_0127644985_p1723616257232"></a><a name="zh-cn_topic_0127644985_p1723616257232"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127644985_p6236152502314"><a name="zh-cn_topic_0127644985_p6236152502314"></a><a name="zh-cn_topic_0127644985_p6236152502314"></a>Internal Server Error</p>
</td>
</tr>
</tbody>
</table>

