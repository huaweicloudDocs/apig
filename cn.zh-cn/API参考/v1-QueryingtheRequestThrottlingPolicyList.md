# 查询流控策略列表<a name="ZH-CN_TOPIC_0000001081837357"></a>

## 功能介绍<a name="zh-cn_topic_0225568866_section64935835"></a>

查询所有流控策略的信息。

## URI<a name="zh-cn_topic_0225568866_section47551608"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568866_table49932580"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568866_row33279153"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568866_p11256835"><a name="zh-cn_topic_0225568866_p11256835"></a><a name="zh-cn_topic_0225568866_p11256835"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568866_p39388458"><a name="zh-cn_topic_0225568866_p39388458"></a><a name="zh-cn_topic_0225568866_p39388458"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568866_row36348558"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568866_p58552086"><a name="zh-cn_topic_0225568866_p58552086"></a><a name="zh-cn_topic_0225568866_p58552086"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568866_p45098539"><a name="zh-cn_topic_0225568866_p45098539"></a><a name="zh-cn_topic_0225568866_p45098539"></a>/v1/{project_id}/apigw/instances/{instance_id}/throttles[?page_size, page_no, id, name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、name、page\_size、page\_no。

## 请求消息<a name="zh-cn_topic_0225568866_section25311293"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0225568866_table20251716"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568866_row341561"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568866_p27666514"><a name="zh-cn_topic_0225568866_p27666514"></a><a name="zh-cn_topic_0225568866_p27666514"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.39%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568866_p26395167"><a name="zh-cn_topic_0225568866_p26395167"></a><a name="zh-cn_topic_0225568866_p26395167"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.09%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568866_p57633801"><a name="zh-cn_topic_0225568866_p57633801"></a><a name="zh-cn_topic_0225568866_p57633801"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="37.519999999999996%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568866_p37826295"><a name="zh-cn_topic_0225568866_p37826295"></a><a name="zh-cn_topic_0225568866_p37826295"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568866_row84591223165020"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568866_p55878963"><a name="zh-cn_topic_0225568866_p55878963"></a><a name="zh-cn_topic_0225568866_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568866_p29902160"><a name="zh-cn_topic_0225568866_p29902160"></a><a name="zh-cn_topic_0225568866_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568866_p6155914"><a name="zh-cn_topic_0225568866_p6155914"></a><a name="zh-cn_topic_0225568866_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.519999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568866_p28867016"><a name="zh-cn_topic_0225568866_p28867016"></a><a name="zh-cn_topic_0225568866_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row19293192311503"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568866_p1780913159538"><a name="zh-cn_topic_0225568866_p1780913159538"></a><a name="zh-cn_topic_0225568866_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568866_p9809215115310"><a name="zh-cn_topic_0225568866_p9809215115310"></a><a name="zh-cn_topic_0225568866_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568866_p1280914152538"><a name="zh-cn_topic_0225568866_p1280914152538"></a><a name="zh-cn_topic_0225568866_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.519999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568866_p1880914157537"><a name="zh-cn_topic_0225568866_p1880914157537"></a><a name="zh-cn_topic_0225568866_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row44031058"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568866_p9745921"><a name="zh-cn_topic_0225568866_p9745921"></a><a name="zh-cn_topic_0225568866_p9745921"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568866_p51222125"><a name="zh-cn_topic_0225568866_p51222125"></a><a name="zh-cn_topic_0225568866_p51222125"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568866_p55351421"><a name="zh-cn_topic_0225568866_p55351421"></a><a name="zh-cn_topic_0225568866_p55351421"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.519999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568866_p54280089"><a name="zh-cn_topic_0225568866_p54280089"></a><a name="zh-cn_topic_0225568866_p54280089"></a>流控策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row18758760"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568866_p43064578"><a name="zh-cn_topic_0225568866_p43064578"></a><a name="zh-cn_topic_0225568866_p43064578"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568866_p65678813"><a name="zh-cn_topic_0225568866_p65678813"></a><a name="zh-cn_topic_0225568866_p65678813"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568866_p18383649"><a name="zh-cn_topic_0225568866_p18383649"></a><a name="zh-cn_topic_0225568866_p18383649"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.519999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568866_p12680564"><a name="zh-cn_topic_0225568866_p12680564"></a><a name="zh-cn_topic_0225568866_p12680564"></a>流控策略名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row6381319"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568866_p47124870"><a name="zh-cn_topic_0225568866_p47124870"></a><a name="zh-cn_topic_0225568866_p47124870"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568866_p59018158"><a name="zh-cn_topic_0225568866_p59018158"></a><a name="zh-cn_topic_0225568866_p59018158"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568866_p15741478"><a name="zh-cn_topic_0225568866_p15741478"></a><a name="zh-cn_topic_0225568866_p15741478"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="37.519999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568866_p67100182"><a name="zh-cn_topic_0225568866_p67100182"></a><a name="zh-cn_topic_0225568866_p67100182"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row67030731"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568866_p60780131"><a name="zh-cn_topic_0225568866_p60780131"></a><a name="zh-cn_topic_0225568866_p60780131"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568866_p24243592"><a name="zh-cn_topic_0225568866_p24243592"></a><a name="zh-cn_topic_0225568866_p24243592"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568866_p17573921"><a name="zh-cn_topic_0225568866_p17573921"></a><a name="zh-cn_topic_0225568866_p17573921"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="37.519999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568866_p14201495"><a name="zh-cn_topic_0225568866_p14201495"></a><a name="zh-cn_topic_0225568866_p14201495"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row1042422165017"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568866_p8422229507"><a name="zh-cn_topic_0225568866_p8422229507"></a><a name="zh-cn_topic_0225568866_p8422229507"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="18.39%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568866_p142132210505"><a name="zh-cn_topic_0225568866_p142132210505"></a><a name="zh-cn_topic_0225568866_p142132210505"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.09%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568866_p7421622175015"><a name="zh-cn_topic_0225568866_p7421622175015"></a><a name="zh-cn_topic_0225568866_p7421622175015"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.519999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568866_p174272275013"><a name="zh-cn_topic_0225568866_p174272275013"></a><a name="zh-cn_topic_0225568866_p174272275013"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0225568866_section36948876"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568866_table44970839"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568866_row22919699"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568866_p44556312"><a name="zh-cn_topic_0225568866_p44556312"></a><a name="zh-cn_topic_0225568866_p44556312"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568866_p52291534"><a name="zh-cn_topic_0225568866_p52291534"></a><a name="zh-cn_topic_0225568866_p52291534"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568866_p7755868"><a name="zh-cn_topic_0225568866_p7755868"></a><a name="zh-cn_topic_0225568866_p7755868"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568866_row24245611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p17737507"><a name="zh-cn_topic_0225568866_p17737507"></a><a name="zh-cn_topic_0225568866_p17737507"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p27451947"><a name="zh-cn_topic_0225568866_p27451947"></a><a name="zh-cn_topic_0225568866_p27451947"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p9015211"><a name="zh-cn_topic_0225568866_p9015211"></a><a name="zh-cn_topic_0225568866_p9015211"></a>符合条件的流控策略的数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row14028040"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p62529456"><a name="zh-cn_topic_0225568866_p62529456"></a><a name="zh-cn_topic_0225568866_p62529456"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p31721189"><a name="zh-cn_topic_0225568866_p31721189"></a><a name="zh-cn_topic_0225568866_p31721189"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p19279502"><a name="zh-cn_topic_0225568866_p19279502"></a><a name="zh-cn_topic_0225568866_p19279502"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row39297794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p29004725"><a name="zh-cn_topic_0225568866_p29004725"></a><a name="zh-cn_topic_0225568866_p29004725"></a>throttles</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p572496"><a name="zh-cn_topic_0225568866_p572496"></a><a name="zh-cn_topic_0225568866_p572496"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p46372220"><a name="zh-cn_topic_0225568866_p46372220"></a><a name="zh-cn_topic_0225568866_p46372220"></a>本次查询到的流控策略列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  throttles参数说明

<a name="zh-cn_topic_0225568866_table14696800"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568866_row18809457"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568866_p47171015"><a name="zh-cn_topic_0225568866_p47171015"></a><a name="zh-cn_topic_0225568866_p47171015"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568866_p62755870"><a name="zh-cn_topic_0225568866_p62755870"></a><a name="zh-cn_topic_0225568866_p62755870"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568866_p50060701"><a name="zh-cn_topic_0225568866_p50060701"></a><a name="zh-cn_topic_0225568866_p50060701"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568866_row28385005"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p17484086"><a name="zh-cn_topic_0225568866_p17484086"></a><a name="zh-cn_topic_0225568866_p17484086"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p6924831"><a name="zh-cn_topic_0225568866_p6924831"></a><a name="zh-cn_topic_0225568866_p6924831"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p24040400"><a name="zh-cn_topic_0225568866_p24040400"></a><a name="zh-cn_topic_0225568866_p24040400"></a>流控策略的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row15037011"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p10038404"><a name="zh-cn_topic_0225568866_p10038404"></a><a name="zh-cn_topic_0225568866_p10038404"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p7804434"><a name="zh-cn_topic_0225568866_p7804434"></a><a name="zh-cn_topic_0225568866_p7804434"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p28179428"><a name="zh-cn_topic_0225568866_p28179428"></a><a name="zh-cn_topic_0225568866_p28179428"></a>流控策略的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row52288267"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p7491198"><a name="zh-cn_topic_0225568866_p7491198"></a><a name="zh-cn_topic_0225568866_p7491198"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p2807339"><a name="zh-cn_topic_0225568866_p2807339"></a><a name="zh-cn_topic_0225568866_p2807339"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p26067896"><a name="zh-cn_topic_0225568866_p26067896"></a><a name="zh-cn_topic_0225568866_p26067896"></a>单个API流控时间内能够被访问的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row33284474"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p11687867"><a name="zh-cn_topic_0225568866_p11687867"></a><a name="zh-cn_topic_0225568866_p11687867"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p7193136"><a name="zh-cn_topic_0225568866_p7193136"></a><a name="zh-cn_topic_0225568866_p7193136"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p45773121"><a name="zh-cn_topic_0225568866_p45773121"></a><a name="zh-cn_topic_0225568866_p45773121"></a>单个用户流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row9304912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p15500440"><a name="zh-cn_topic_0225568866_p15500440"></a><a name="zh-cn_topic_0225568866_p15500440"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p47576112"><a name="zh-cn_topic_0225568866_p47576112"></a><a name="zh-cn_topic_0225568866_p47576112"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p28459840"><a name="zh-cn_topic_0225568866_p28459840"></a><a name="zh-cn_topic_0225568866_p28459840"></a>单个APP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row1989411328423"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p71235716345"><a name="zh-cn_topic_0225568866_p71235716345"></a><a name="zh-cn_topic_0225568866_p71235716345"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p612135773413"><a name="zh-cn_topic_0225568866_p612135773413"></a><a name="zh-cn_topic_0225568866_p612135773413"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p12122573347"><a name="zh-cn_topic_0225568866_p12122573347"></a><a name="zh-cn_topic_0225568866_p12122573347"></a>单个IP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row54811973"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p10584829"><a name="zh-cn_topic_0225568866_p10584829"></a><a name="zh-cn_topic_0225568866_p10584829"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p52064834"><a name="zh-cn_topic_0225568866_p52064834"></a><a name="zh-cn_topic_0225568866_p52064834"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p56502011"><a name="zh-cn_topic_0225568866_p56502011"></a><a name="zh-cn_topic_0225568866_p56502011"></a>流控的时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row38756055"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p52232730"><a name="zh-cn_topic_0225568866_p52232730"></a><a name="zh-cn_topic_0225568866_p52232730"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p2992709"><a name="zh-cn_topic_0225568866_p2992709"></a><a name="zh-cn_topic_0225568866_p2992709"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p41082881"><a name="zh-cn_topic_0225568866_p41082881"></a><a name="zh-cn_topic_0225568866_p41082881"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row34201613"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p18867236"><a name="zh-cn_topic_0225568866_p18867236"></a><a name="zh-cn_topic_0225568866_p18867236"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p51851168"><a name="zh-cn_topic_0225568866_p51851168"></a><a name="zh-cn_topic_0225568866_p51851168"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p39195113"><a name="zh-cn_topic_0225568866_p39195113"></a><a name="zh-cn_topic_0225568866_p39195113"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row17211702"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p51970588"><a name="zh-cn_topic_0225568866_p51970588"></a><a name="zh-cn_topic_0225568866_p51970588"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p48868099"><a name="zh-cn_topic_0225568866_p48868099"></a><a name="zh-cn_topic_0225568866_p48868099"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p66001938"><a name="zh-cn_topic_0225568866_p66001938"></a><a name="zh-cn_topic_0225568866_p66001938"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row57146537"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p65466760"><a name="zh-cn_topic_0225568866_p65466760"></a><a name="zh-cn_topic_0225568866_p65466760"></a>is_include_special_throttle</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p1207332"><a name="zh-cn_topic_0225568866_p1207332"></a><a name="zh-cn_topic_0225568866_p1207332"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p30685028"><a name="zh-cn_topic_0225568866_p30685028"></a><a name="zh-cn_topic_0225568866_p30685028"></a>是否包含特殊流控配置：</p>
<a name="zh-cn_topic_0225568866_ul107800420518"></a><a name="zh-cn_topic_0225568866_ul107800420518"></a><ul id="zh-cn_topic_0225568866_ul107800420518"><li>1：包含</li><li>2：不包含</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row231014181787"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p10310618881"><a name="zh-cn_topic_0225568866_p10310618881"></a><a name="zh-cn_topic_0225568866_p10310618881"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p33101918089"><a name="zh-cn_topic_0225568866_p33101918089"></a><a name="zh-cn_topic_0225568866_p33101918089"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p15805453105915"><a name="zh-cn_topic_0225568866_p15805453105915"></a><a name="zh-cn_topic_0225568866_p15805453105915"></a>流控策略的类型，取值如下：</p>
<a name="zh-cn_topic_0225568866_ul1043012241502"></a><a name="zh-cn_topic_0225568866_ul1043012241502"></a><ul id="zh-cn_topic_0225568866_ul1043012241502"><li>1   独享</li><li>2   共享</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row632313286512"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p14797139472"><a name="zh-cn_topic_0225568866_p14797139472"></a><a name="zh-cn_topic_0225568866_p14797139472"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p147913137471"><a name="zh-cn_topic_0225568866_p147913137471"></a><a name="zh-cn_topic_0225568866_p147913137471"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p11798139474"><a name="zh-cn_topic_0225568866_p11798139474"></a><a name="zh-cn_topic_0225568866_p11798139474"></a>流控绑定的API数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row172041856599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568866_p19770121614477"><a name="zh-cn_topic_0225568866_p19770121614477"></a><a name="zh-cn_topic_0225568866_p19770121614477"></a>enable_adaptive_control</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568866_p27566352475"><a name="zh-cn_topic_0225568866_p27566352475"></a><a name="zh-cn_topic_0225568866_p27566352475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568866_p39161837145716"><a name="zh-cn_topic_0225568866_p39161837145716"></a><a name="zh-cn_topic_0225568866_p39161837145716"></a>是否开启动态流控：</p>
<a name="zh-cn_topic_0225568866_ul17916103725711"></a><a name="zh-cn_topic_0225568866_ul17916103725711"></a><ul id="zh-cn_topic_0225568866_ul17916103725711"><li>TRUE</li><li>FALSE</li></ul>
<p id="zh-cn_topic_0225568866_p159161937155713"><a name="zh-cn_topic_0225568866_p159161937155713"></a><a name="zh-cn_topic_0225568866_p159161937155713"></a>暂不支持</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"throttles": [{
		"id": "a3106cfe-801f-4919-b0d7-d785dc5b47f9",
		"name": "每秒500次",
		"api_call_limits": 500,
		"user_call_limits": 200,
		"app_call_limits": 100,
                "app_call_limits": 100,
		"time_interval": 1,
		"time_unit": "SECOND",
		"create_time": "2017-12-29T02:04:08Z",
		"remark": "API每秒500次，用户200次，APP100次，IP100次",
		"is_inclu_special_throttle": 2,
                "type":1,
                "bind_num":1,
                "enable_adaptive_control": "FALSE"
	},
	{
		"id": "0325b671-2d50-4614-9868-22102262695d",
		"name": "每秒1000次",
		"api_call_limits": 1000,
		"user_call_limits": 500,
		"app_call_limits": 300,
                "ip_call_limits": 600,
		"time_interval": 1,
		"time_unit": "SECOND",
		"create_time": "2017-12-29T01:55:59Z",
		"remark": "API每秒1000次，用户500次，APP300次，IP600次",
		"is_inclu_special_throttle": 2,
                "type":1,
                "bind_num":1,
                "enable_adaptive_control": "FALSE"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568866_section26475052"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568866_table9470417"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568866_row506443"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568866_p41021952"><a name="zh-cn_topic_0225568866_p41021952"></a><a name="zh-cn_topic_0225568866_p41021952"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568866_p34443838"><a name="zh-cn_topic_0225568866_p34443838"></a><a name="zh-cn_topic_0225568866_p34443838"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568866_row38487468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568866_p30477170"><a name="zh-cn_topic_0225568866_p30477170"></a><a name="zh-cn_topic_0225568866_p30477170"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568866_p52731705"><a name="zh-cn_topic_0225568866_p52731705"></a><a name="zh-cn_topic_0225568866_p52731705"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row4823300"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568866_p55143023"><a name="zh-cn_topic_0225568866_p55143023"></a><a name="zh-cn_topic_0225568866_p55143023"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568866_p37399854"><a name="zh-cn_topic_0225568866_p37399854"></a><a name="zh-cn_topic_0225568866_p37399854"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row1054369"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568866_p18295034"><a name="zh-cn_topic_0225568866_p18295034"></a><a name="zh-cn_topic_0225568866_p18295034"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568866_p5502747"><a name="zh-cn_topic_0225568866_p5502747"></a><a name="zh-cn_topic_0225568866_p5502747"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568866_row49524726"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568866_p52079895"><a name="zh-cn_topic_0225568866_p52079895"></a><a name="zh-cn_topic_0225568866_p52079895"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568866_p43041044115313"><a name="zh-cn_topic_0225568866_p43041044115313"></a><a name="zh-cn_topic_0225568866_p43041044115313"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

