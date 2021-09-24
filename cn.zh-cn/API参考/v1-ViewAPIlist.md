# 查询API列表<a name="ZH-CN_TOPIC_0000001082221249"></a>

## 功能介绍<a name="zh-cn_topic_0225568823_section31536236"></a>

查看API列表，返回API详细信息、发布信息等，但不能查看到后端服务信息。

## URI<a name="zh-cn_topic_0225568823_section15390672"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568823_table4929521"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568823_row21328449"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568823_p49882799"><a name="zh-cn_topic_0225568823_p49882799"></a><a name="zh-cn_topic_0225568823_p49882799"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568823_p13974922"><a name="zh-cn_topic_0225568823_p13974922"></a><a name="zh-cn_topic_0225568823_p13974922"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568823_row58226873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568823_p18756261"><a name="zh-cn_topic_0225568823_p18756261"></a><a name="zh-cn_topic_0225568823_p18756261"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568823_p42862133"><a name="zh-cn_topic_0225568823_p42862133"></a><a name="zh-cn_topic_0225568823_p42862133"></a>/v1/{project_id}/apigw/instances/{instance_id}/apis[?page_size, page_no, id, name, group_id, req_protocol, req_method, req_uri, auth_type, env_id, type,status, tags]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、name、group\_id、req\_protocol、req\_method、req\_uri、auth\_type、env\_id、type、status、tags、page\_size、page\_no。

## 请求消息<a name="zh-cn_topic_0225568823_section4298322"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0225568823_table309072"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568823_row29526596"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568823_p42844056"><a name="zh-cn_topic_0225568823_p42844056"></a><a name="zh-cn_topic_0225568823_p42844056"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568823_p47816505"><a name="zh-cn_topic_0225568823_p47816505"></a><a name="zh-cn_topic_0225568823_p47816505"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.61%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568823_p47931662"><a name="zh-cn_topic_0225568823_p47931662"></a><a name="zh-cn_topic_0225568823_p47931662"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="37.04%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568823_p57259391"><a name="zh-cn_topic_0225568823_p57259391"></a><a name="zh-cn_topic_0225568823_p57259391"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568823_row1701205616189"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p1076285717184"><a name="zh-cn_topic_0225568823_p1076285717184"></a><a name="zh-cn_topic_0225568823_p1076285717184"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p17762457101817"><a name="zh-cn_topic_0225568823_p17762457101817"></a><a name="zh-cn_topic_0225568823_p17762457101817"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p147621357181819"><a name="zh-cn_topic_0225568823_p147621357181819"></a><a name="zh-cn_topic_0225568823_p147621357181819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p5762157171820"><a name="zh-cn_topic_0225568823_p5762157171820"></a><a name="zh-cn_topic_0225568823_p5762157171820"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row9525115619183"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p37621057191818"><a name="zh-cn_topic_0225568823_p37621057191818"></a><a name="zh-cn_topic_0225568823_p37621057191818"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p1576255771817"><a name="zh-cn_topic_0225568823_p1576255771817"></a><a name="zh-cn_topic_0225568823_p1576255771817"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p276265719181"><a name="zh-cn_topic_0225568823_p276265719181"></a><a name="zh-cn_topic_0225568823_p276265719181"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p147621657111817"><a name="zh-cn_topic_0225568823_p147621657111817"></a><a name="zh-cn_topic_0225568823_p147621657111817"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row7499126"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p3449432"><a name="zh-cn_topic_0225568823_p3449432"></a><a name="zh-cn_topic_0225568823_p3449432"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p10968591"><a name="zh-cn_topic_0225568823_p10968591"></a><a name="zh-cn_topic_0225568823_p10968591"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p16040707"><a name="zh-cn_topic_0225568823_p16040707"></a><a name="zh-cn_topic_0225568823_p16040707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p24228891"><a name="zh-cn_topic_0225568823_p24228891"></a><a name="zh-cn_topic_0225568823_p24228891"></a>API的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row16733432"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p13230786"><a name="zh-cn_topic_0225568823_p13230786"></a><a name="zh-cn_topic_0225568823_p13230786"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p65060773"><a name="zh-cn_topic_0225568823_p65060773"></a><a name="zh-cn_topic_0225568823_p65060773"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p35431240"><a name="zh-cn_topic_0225568823_p35431240"></a><a name="zh-cn_topic_0225568823_p35431240"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p51358163"><a name="zh-cn_topic_0225568823_p51358163"></a><a name="zh-cn_topic_0225568823_p51358163"></a>API的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row59570287"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p60463979"><a name="zh-cn_topic_0225568823_p60463979"></a><a name="zh-cn_topic_0225568823_p60463979"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p65744098"><a name="zh-cn_topic_0225568823_p65744098"></a><a name="zh-cn_topic_0225568823_p65744098"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p23671742"><a name="zh-cn_topic_0225568823_p23671742"></a><a name="zh-cn_topic_0225568823_p23671742"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p38362983"><a name="zh-cn_topic_0225568823_p38362983"></a><a name="zh-cn_topic_0225568823_p38362983"></a>API所属分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row9722532"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p49327594"><a name="zh-cn_topic_0225568823_p49327594"></a><a name="zh-cn_topic_0225568823_p49327594"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p36112177"><a name="zh-cn_topic_0225568823_p36112177"></a><a name="zh-cn_topic_0225568823_p36112177"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p39405216"><a name="zh-cn_topic_0225568823_p39405216"></a><a name="zh-cn_topic_0225568823_p39405216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p37705952"><a name="zh-cn_topic_0225568823_p37705952"></a><a name="zh-cn_topic_0225568823_p37705952"></a>请求协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row3809254"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p40114146"><a name="zh-cn_topic_0225568823_p40114146"></a><a name="zh-cn_topic_0225568823_p40114146"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p28020354"><a name="zh-cn_topic_0225568823_p28020354"></a><a name="zh-cn_topic_0225568823_p28020354"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p55056174"><a name="zh-cn_topic_0225568823_p55056174"></a><a name="zh-cn_topic_0225568823_p55056174"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p30365135"><a name="zh-cn_topic_0225568823_p30365135"></a><a name="zh-cn_topic_0225568823_p30365135"></a>请求方法</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row4850767"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p57367866"><a name="zh-cn_topic_0225568823_p57367866"></a><a name="zh-cn_topic_0225568823_p57367866"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p16285582"><a name="zh-cn_topic_0225568823_p16285582"></a><a name="zh-cn_topic_0225568823_p16285582"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p44063729"><a name="zh-cn_topic_0225568823_p44063729"></a><a name="zh-cn_topic_0225568823_p44063729"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p12392334"><a name="zh-cn_topic_0225568823_p12392334"></a><a name="zh-cn_topic_0225568823_p12392334"></a>请求路径</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row44422145"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p41423973"><a name="zh-cn_topic_0225568823_p41423973"></a><a name="zh-cn_topic_0225568823_p41423973"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p67007510"><a name="zh-cn_topic_0225568823_p67007510"></a><a name="zh-cn_topic_0225568823_p67007510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p58899195"><a name="zh-cn_topic_0225568823_p58899195"></a><a name="zh-cn_topic_0225568823_p58899195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p6105468"><a name="zh-cn_topic_0225568823_p6105468"></a><a name="zh-cn_topic_0225568823_p6105468"></a>授权类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row54949219"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p21701787"><a name="zh-cn_topic_0225568823_p21701787"></a><a name="zh-cn_topic_0225568823_p21701787"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p13014307"><a name="zh-cn_topic_0225568823_p13014307"></a><a name="zh-cn_topic_0225568823_p13014307"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p47525923"><a name="zh-cn_topic_0225568823_p47525923"></a><a name="zh-cn_topic_0225568823_p47525923"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p24394564"><a name="zh-cn_topic_0225568823_p24394564"></a><a name="zh-cn_topic_0225568823_p24394564"></a>发布的环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row18224488"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p66897437"><a name="zh-cn_topic_0225568823_p66897437"></a><a name="zh-cn_topic_0225568823_p66897437"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p49983302"><a name="zh-cn_topic_0225568823_p49983302"></a><a name="zh-cn_topic_0225568823_p49983302"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p22115660"><a name="zh-cn_topic_0225568823_p22115660"></a><a name="zh-cn_topic_0225568823_p22115660"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p46538006"><a name="zh-cn_topic_0225568823_p46538006"></a><a name="zh-cn_topic_0225568823_p46538006"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row15164448154320"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p8509135192518"><a name="zh-cn_topic_0225568823_p8509135192518"></a><a name="zh-cn_topic_0225568823_p8509135192518"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p165091851162513"><a name="zh-cn_topic_0225568823_p165091851162513"></a><a name="zh-cn_topic_0225568823_p165091851162513"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p550915152518"><a name="zh-cn_topic_0225568823_p550915152518"></a><a name="zh-cn_topic_0225568823_p550915152518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p650975122517"><a name="zh-cn_topic_0225568823_p650975122517"></a><a name="zh-cn_topic_0225568823_p650975122517"></a>标签</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row16188872"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p36230260"><a name="zh-cn_topic_0225568823_p36230260"></a><a name="zh-cn_topic_0225568823_p36230260"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p48969944"><a name="zh-cn_topic_0225568823_p48969944"></a><a name="zh-cn_topic_0225568823_p48969944"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p7142557"><a name="zh-cn_topic_0225568823_p7142557"></a><a name="zh-cn_topic_0225568823_p7142557"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p41676267"><a name="zh-cn_topic_0225568823_p41676267"></a><a name="zh-cn_topic_0225568823_p41676267"></a>每页显示的条数，默认值：20，最大值500。page_size值为0时，返回所有API。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row39542084"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p48792241"><a name="zh-cn_topic_0225568823_p48792241"></a><a name="zh-cn_topic_0225568823_p48792241"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p59857467"><a name="zh-cn_topic_0225568823_p59857467"></a><a name="zh-cn_topic_0225568823_p59857467"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p16616649"><a name="zh-cn_topic_0225568823_p16616649"></a><a name="zh-cn_topic_0225568823_p16616649"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p3771332"><a name="zh-cn_topic_0225568823_p3771332"></a><a name="zh-cn_topic_0225568823_p3771332"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row136191246154813"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568823_p26191463489"><a name="zh-cn_topic_0225568823_p26191463489"></a><a name="zh-cn_topic_0225568823_p26191463489"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568823_p1261984620484"><a name="zh-cn_topic_0225568823_p1261984620484"></a><a name="zh-cn_topic_0225568823_p1261984620484"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="20.61%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568823_p261916461487"><a name="zh-cn_topic_0225568823_p261916461487"></a><a name="zh-cn_topic_0225568823_p261916461487"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.04%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568823_p10619154674815"><a name="zh-cn_topic_0225568823_p10619154674815"></a><a name="zh-cn_topic_0225568823_p10619154674815"></a>指定需要精确匹配查找的参数名称，目前仅支持name、req_uri</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="zh-cn_topic_0225568823_section12619772"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568823_table62034025"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568823_row12774732"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568823_p28120399"><a name="zh-cn_topic_0225568823_p28120399"></a><a name="zh-cn_topic_0225568823_p28120399"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568823_p63159826"><a name="zh-cn_topic_0225568823_p63159826"></a><a name="zh-cn_topic_0225568823_p63159826"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568823_p15672253"><a name="zh-cn_topic_0225568823_p15672253"></a><a name="zh-cn_topic_0225568823_p15672253"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568823_row61492985"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p14875885"><a name="zh-cn_topic_0225568823_p14875885"></a><a name="zh-cn_topic_0225568823_p14875885"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p64096066"><a name="zh-cn_topic_0225568823_p64096066"></a><a name="zh-cn_topic_0225568823_p64096066"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p24398880"><a name="zh-cn_topic_0225568823_p24398880"></a><a name="zh-cn_topic_0225568823_p24398880"></a>符合条件的API总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row18263329"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p2934686"><a name="zh-cn_topic_0225568823_p2934686"></a><a name="zh-cn_topic_0225568823_p2934686"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p36383032"><a name="zh-cn_topic_0225568823_p36383032"></a><a name="zh-cn_topic_0225568823_p36383032"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p61344470"><a name="zh-cn_topic_0225568823_p61344470"></a><a name="zh-cn_topic_0225568823_p61344470"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row15229322"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p25615594"><a name="zh-cn_topic_0225568823_p25615594"></a><a name="zh-cn_topic_0225568823_p25615594"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p61597251"><a name="zh-cn_topic_0225568823_p61597251"></a><a name="zh-cn_topic_0225568823_p61597251"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p23321404"><a name="zh-cn_topic_0225568823_p23321404"></a><a name="zh-cn_topic_0225568823_p23321404"></a>本次查询到的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="zh-cn_topic_0225568823_table8566044"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568823_row21338628"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568823_p50707320"><a name="zh-cn_topic_0225568823_p50707320"></a><a name="zh-cn_topic_0225568823_p50707320"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568823_p13652219"><a name="zh-cn_topic_0225568823_p13652219"></a><a name="zh-cn_topic_0225568823_p13652219"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568823_p32087992"><a name="zh-cn_topic_0225568823_p32087992"></a><a name="zh-cn_topic_0225568823_p32087992"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568823_row48990549"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p8811514"><a name="zh-cn_topic_0225568823_p8811514"></a><a name="zh-cn_topic_0225568823_p8811514"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p42644048"><a name="zh-cn_topic_0225568823_p42644048"></a><a name="zh-cn_topic_0225568823_p42644048"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p31615870"><a name="zh-cn_topic_0225568823_p31615870"></a><a name="zh-cn_topic_0225568823_p31615870"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row16107382"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p29629597"><a name="zh-cn_topic_0225568823_p29629597"></a><a name="zh-cn_topic_0225568823_p29629597"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p51187119"><a name="zh-cn_topic_0225568823_p51187119"></a><a name="zh-cn_topic_0225568823_p51187119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p52515990"><a name="zh-cn_topic_0225568823_p52515990"></a><a name="zh-cn_topic_0225568823_p52515990"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row2881869"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p32104846"><a name="zh-cn_topic_0225568823_p32104846"></a><a name="zh-cn_topic_0225568823_p32104846"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p50355735"><a name="zh-cn_topic_0225568823_p50355735"></a><a name="zh-cn_topic_0225568823_p50355735"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p52282769"><a name="zh-cn_topic_0225568823_p52282769"></a><a name="zh-cn_topic_0225568823_p52282769"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row782880"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p63413318"><a name="zh-cn_topic_0225568823_p63413318"></a><a name="zh-cn_topic_0225568823_p63413318"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p36205104"><a name="zh-cn_topic_0225568823_p36205104"></a><a name="zh-cn_topic_0225568823_p36205104"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p46932294"><a name="zh-cn_topic_0225568823_p46932294"></a><a name="zh-cn_topic_0225568823_p46932294"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row19737470"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p55231234"><a name="zh-cn_topic_0225568823_p55231234"></a><a name="zh-cn_topic_0225568823_p55231234"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p44544999"><a name="zh-cn_topic_0225568823_p44544999"></a><a name="zh-cn_topic_0225568823_p44544999"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p51375189"><a name="zh-cn_topic_0225568823_p51375189"></a><a name="zh-cn_topic_0225568823_p51375189"></a>API的状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row59723518"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p5766795"><a name="zh-cn_topic_0225568823_p5766795"></a><a name="zh-cn_topic_0225568823_p5766795"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p64457269"><a name="zh-cn_topic_0225568823_p64457269"></a><a name="zh-cn_topic_0225568823_p64457269"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p53656291"><a name="zh-cn_topic_0225568823_p53656291"></a><a name="zh-cn_topic_0225568823_p53656291"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row13144575"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p58077679"><a name="zh-cn_topic_0225568823_p58077679"></a><a name="zh-cn_topic_0225568823_p58077679"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p6671576"><a name="zh-cn_topic_0225568823_p6671576"></a><a name="zh-cn_topic_0225568823_p6671576"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p3526753"><a name="zh-cn_topic_0225568823_p3526753"></a><a name="zh-cn_topic_0225568823_p3526753"></a>API版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row31740777"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p20866117"><a name="zh-cn_topic_0225568823_p20866117"></a><a name="zh-cn_topic_0225568823_p20866117"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p12433942"><a name="zh-cn_topic_0225568823_p12433942"></a><a name="zh-cn_topic_0225568823_p12433942"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p516420"><a name="zh-cn_topic_0225568823_p516420"></a><a name="zh-cn_topic_0225568823_p516420"></a>API访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row4647785"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p40926317"><a name="zh-cn_topic_0225568823_p40926317"></a><a name="zh-cn_topic_0225568823_p40926317"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p26697344"><a name="zh-cn_topic_0225568823_p26697344"></a><a name="zh-cn_topic_0225568823_p26697344"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p15001293"><a name="zh-cn_topic_0225568823_p15001293"></a><a name="zh-cn_topic_0225568823_p15001293"></a>API请求方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row793912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p64306892"><a name="zh-cn_topic_0225568823_p64306892"></a><a name="zh-cn_topic_0225568823_p64306892"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p41475757"><a name="zh-cn_topic_0225568823_p41475757"></a><a name="zh-cn_topic_0225568823_p41475757"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p4093122"><a name="zh-cn_topic_0225568823_p4093122"></a><a name="zh-cn_topic_0225568823_p4093122"></a>API访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row36838099"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p31096082"><a name="zh-cn_topic_0225568823_p31096082"></a><a name="zh-cn_topic_0225568823_p31096082"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p35754746"><a name="zh-cn_topic_0225568823_p35754746"></a><a name="zh-cn_topic_0225568823_p35754746"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p10453298"><a name="zh-cn_topic_0225568823_p10453298"></a><a name="zh-cn_topic_0225568823_p10453298"></a>API认证方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row39420599177"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p45549491969"><a name="zh-cn_topic_0225568823_p45549491969"></a><a name="zh-cn_topic_0225568823_p45549491969"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p19554194910611"><a name="zh-cn_topic_0225568823_p19554194910611"></a><a name="zh-cn_topic_0225568823_p19554194910611"></a>字段数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p155541490617"><a name="zh-cn_topic_0225568823_p155541490617"></a><a name="zh-cn_topic_0225568823_p155541490617"></a>API认证方式参数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row36853316346"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p4426105522114"><a name="zh-cn_topic_0225568823_p4426105522114"></a><a name="zh-cn_topic_0225568823_p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p43515104346"><a name="zh-cn_topic_0225568823_p43515104346"></a><a name="zh-cn_topic_0225568823_p43515104346"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p116491557133012"><a name="zh-cn_topic_0225568823_p116491557133012"></a><a name="zh-cn_topic_0225568823_p116491557133012"></a>前端自定义认证对象的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row26970819"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p37152759"><a name="zh-cn_topic_0225568823_p37152759"></a><a name="zh-cn_topic_0225568823_p37152759"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p56583503"><a name="zh-cn_topic_0225568823_p56583503"></a><a name="zh-cn_topic_0225568823_p56583503"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p19861044"><a name="zh-cn_topic_0225568823_p19861044"></a><a name="zh-cn_topic_0225568823_p19861044"></a>API匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row44531670"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p50295545"><a name="zh-cn_topic_0225568823_p50295545"></a><a name="zh-cn_topic_0225568823_p50295545"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p47407324"><a name="zh-cn_topic_0225568823_p47407324"></a><a name="zh-cn_topic_0225568823_p47407324"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p14788007"><a name="zh-cn_topic_0225568823_p14788007"></a><a name="zh-cn_topic_0225568823_p14788007"></a>API注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row65983203"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p43039263"><a name="zh-cn_topic_0225568823_p43039263"></a><a name="zh-cn_topic_0225568823_p43039263"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p63628246"><a name="zh-cn_topic_0225568823_p63628246"></a><a name="zh-cn_topic_0225568823_p63628246"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p53614322"><a name="zh-cn_topic_0225568823_p53614322"></a><a name="zh-cn_topic_0225568823_p53614322"></a>API修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row12766858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p27482552"><a name="zh-cn_topic_0225568823_p27482552"></a><a name="zh-cn_topic_0225568823_p27482552"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p11494206"><a name="zh-cn_topic_0225568823_p11494206"></a><a name="zh-cn_topic_0225568823_p11494206"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p58615493"><a name="zh-cn_topic_0225568823_p58615493"></a><a name="zh-cn_topic_0225568823_p58615493"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row57777392"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p49457179"><a name="zh-cn_topic_0225568823_p49457179"></a><a name="zh-cn_topic_0225568823_p49457179"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p46608538"><a name="zh-cn_topic_0225568823_p46608538"></a><a name="zh-cn_topic_0225568823_p46608538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p17195222"><a name="zh-cn_topic_0225568823_p17195222"></a><a name="zh-cn_topic_0225568823_p17195222"></a>后端类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row20539270"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p53068135"><a name="zh-cn_topic_0225568823_p53068135"></a><a name="zh-cn_topic_0225568823_p53068135"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p3551673"><a name="zh-cn_topic_0225568823_p3551673"></a><a name="zh-cn_topic_0225568823_p3551673"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p19250083"><a name="zh-cn_topic_0225568823_p19250083"></a><a name="zh-cn_topic_0225568823_p19250083"></a>发布的环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row39033025"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p7558467"><a name="zh-cn_topic_0225568823_p7558467"></a><a name="zh-cn_topic_0225568823_p7558467"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p8256114"><a name="zh-cn_topic_0225568823_p8256114"></a><a name="zh-cn_topic_0225568823_p8256114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p64765493"><a name="zh-cn_topic_0225568823_p64765493"></a><a name="zh-cn_topic_0225568823_p64765493"></a>发布的环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row46018530"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p36513439"><a name="zh-cn_topic_0225568823_p36513439"></a><a name="zh-cn_topic_0225568823_p36513439"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p4798564"><a name="zh-cn_topic_0225568823_p4798564"></a><a name="zh-cn_topic_0225568823_p4798564"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p53139418"><a name="zh-cn_topic_0225568823_p53139418"></a><a name="zh-cn_topic_0225568823_p53139418"></a>发布记录的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row29624732"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p50793096"><a name="zh-cn_topic_0225568823_p50793096"></a><a name="zh-cn_topic_0225568823_p50793096"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p20600108"><a name="zh-cn_topic_0225568823_p20600108"></a><a name="zh-cn_topic_0225568823_p20600108"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p57996081"><a name="zh-cn_topic_0225568823_p57996081"></a><a name="zh-cn_topic_0225568823_p57996081"></a>是否需要编排</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row02521055181212"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p16252655131214"><a name="zh-cn_topic_0225568823_p16252655131214"></a><a name="zh-cn_topic_0225568823_p16252655131214"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p17252195514120"><a name="zh-cn_topic_0225568823_p17252195514120"></a><a name="zh-cn_topic_0225568823_p17252195514120"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p0252955151218"><a name="zh-cn_topic_0225568823_p0252955151218"></a><a name="zh-cn_topic_0225568823_p0252955151218"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row1455379135"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p7679321181114"><a name="zh-cn_topic_0225568823_p7679321181114"></a><a name="zh-cn_topic_0225568823_p7679321181114"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p166791021161110"><a name="zh-cn_topic_0225568823_p166791021161110"></a><a name="zh-cn_topic_0225568823_p166791021161110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p1167913211111"><a name="zh-cn_topic_0225568823_p1167913211111"></a><a name="zh-cn_topic_0225568823_p1167913211111"></a>服务名称标签，待废弃字段</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row12685122214420"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p5689175210267"><a name="zh-cn_topic_0225568823_p5689175210267"></a><a name="zh-cn_topic_0225568823_p5689175210267"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p969065252610"><a name="zh-cn_topic_0225568823_p969065252610"></a><a name="zh-cn_topic_0225568823_p969065252610"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p10599103122713"><a name="zh-cn_topic_0225568823_p10599103122713"></a><a name="zh-cn_topic_0225568823_p10599103122713"></a>标签</p>
</td>
</tr>
</tbody>
</table>

**表 5**  auth\_opt参数说明

<a name="zh-cn_topic_0225568823_table3296221173715"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568823_row829715213377"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568823_p17297192173718"><a name="zh-cn_topic_0225568823_p17297192173718"></a><a name="zh-cn_topic_0225568823_p17297192173718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568823_p9297821143718"><a name="zh-cn_topic_0225568823_p9297821143718"></a><a name="zh-cn_topic_0225568823_p9297821143718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568823_p4297152163717"><a name="zh-cn_topic_0225568823_p4297152163717"></a><a name="zh-cn_topic_0225568823_p4297152163717"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568823_row4297421123717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568823_p1848964315375"><a name="zh-cn_topic_0225568823_p1848964315375"></a><a name="zh-cn_topic_0225568823_p1848964315375"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568823_p4489164310372"><a name="zh-cn_topic_0225568823_p4489164310372"></a><a name="zh-cn_topic_0225568823_p4489164310372"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568823_p1948934316376"><a name="zh-cn_topic_0225568823_p1948934316376"></a><a name="zh-cn_topic_0225568823_p1948934316376"></a>AppCode简易认证类型</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 3,
  "size": 3,
  "apis": [
    {
      "name": "test",
      "type": 1,
      "version": "V0.0.1",
      "req_protocol": "HTTPS",
      "req_method": "GET",
      "req_uri": "/test/{project_id}",
      "auth_type": "APP",
      "auth_opt": {
        "app_code_auth_type": "DISABLE"
      },
      "tags": ["APIG-SN-test", "test"],
      "cors": false,
      "match_mode": "NORMAL",
      "backend_type": "HTTP",
      "group_id": "f71f69876f90456ca6fd18ed012fdc11",
      "id": "81efcfd94b8747a0b21e8c04144a4e8c",
      "status": 1,
      "arrange_necessary": 2,
      "register_time": "2018-08-15T03:41:11Z",
      "update_time": "2018-08-15T03:41:11Z",
      "group_name": "group0002"
    },
    {
      "name": "bbbbb",
      "type": 1,
      "version": "0.0.1",
      "req_protocol": "HTTPS",
      "req_method": "GET",
      "req_uri": "/test002",
      "auth_type": "APP",
      "auth_opt": {
        "app_code_auth_type": "DISABLE"
      },
      "tags": ["APIG-SN-test", "test"],
      "cors": false,
      "match_mode": "NORMAL",
      "backend_type": "MOCK",
      "remark": "aaa",
      "group_id": "70f1b578da9b4dfe889b4c33d1b995c2",
      "id": "91c26288acea4448be205265d77dae22",
      "status": 1,
      "arrange_necessary": 2,
      "register_time": "2018-07-27T11:54:24Z",
      "update_time": "2018-07-27T11:54:24Z",
      "group_name": "test001",
      "run_env_name": "RELEASE",
      "run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "publish_id": "a6e06a00c382436eb524fa2dd343cb6d"
    },
    {
      "name": "aaa",
      "type": 1,
      "version": "0.0.1",
      "req_protocol": "HTTPS",
      "req_method": "GET",
      "req_uri": "/test001",
      "auth_type": "APP",
      "auth_opt": {
        "app_code_auth_type": "DISABLE"
      },
      "tags": ["APIG-SN-test", "test"],
      "cors": false,
      "match_mode": "NORMAL",
      "backend_type": "MOCK",
      "remark": "aaa",
      "group_id": "70f1b578da9b4dfe889b4c33d1b995c2",
      "id": "aebacac6095942b4b2dd2b209bb7b9bc",
      "status": 1,
      "arrange_necessary": 2,
      "register_time": "2018-07-27T11:23:34Z",
      "update_time": "2018-07-27T11:23:34Z",
      "group_name": "test001",
      "run_env_name": "RELEASE",
      "run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "publish_id": "1bc8b2b741a04bd4af3ef9d7cd003104"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0225568823_section38684899"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0225568823_table37042451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568823_row40505160"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568823_p59692522"><a name="zh-cn_topic_0225568823_p59692522"></a><a name="zh-cn_topic_0225568823_p59692522"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568823_p3256100"><a name="zh-cn_topic_0225568823_p3256100"></a><a name="zh-cn_topic_0225568823_p3256100"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568823_row62417567"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568823_p22658179"><a name="zh-cn_topic_0225568823_p22658179"></a><a name="zh-cn_topic_0225568823_p22658179"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568823_p50988816"><a name="zh-cn_topic_0225568823_p50988816"></a><a name="zh-cn_topic_0225568823_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row9031982"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568823_p60501950"><a name="zh-cn_topic_0225568823_p60501950"></a><a name="zh-cn_topic_0225568823_p60501950"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568823_p1710898"><a name="zh-cn_topic_0225568823_p1710898"></a><a name="zh-cn_topic_0225568823_p1710898"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row15398085"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568823_p39285387"><a name="zh-cn_topic_0225568823_p39285387"></a><a name="zh-cn_topic_0225568823_p39285387"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568823_p9203142078"><a name="zh-cn_topic_0225568823_p9203142078"></a><a name="zh-cn_topic_0225568823_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568823_row50671481"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568823_p10749328"><a name="zh-cn_topic_0225568823_p10749328"></a><a name="zh-cn_topic_0225568823_p10749328"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568823_p65389202"><a name="zh-cn_topic_0225568823_p65389202"></a><a name="zh-cn_topic_0225568823_p65389202"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

