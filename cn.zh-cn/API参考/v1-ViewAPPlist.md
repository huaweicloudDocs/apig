# 查询APP列表<a name="ZH-CN_TOPIC_0000001081837343"></a>

## 功能介绍<a name="zh-cn_topic_0225568839_section48433431"></a>

查询APP列表。

## URI<a name="zh-cn_topic_0225568839_section33247697"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568839_table33538507"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568839_row26439774"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568839_p61246963"><a name="zh-cn_topic_0225568839_p61246963"></a><a name="zh-cn_topic_0225568839_p61246963"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568839_p62056956"><a name="zh-cn_topic_0225568839_p62056956"></a><a name="zh-cn_topic_0225568839_p62056956"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568839_row60557538"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568839_p6213516"><a name="zh-cn_topic_0225568839_p6213516"></a><a name="zh-cn_topic_0225568839_p6213516"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568839_p33532770"><a name="zh-cn_topic_0225568839_p33532770"></a><a name="zh-cn_topic_0225568839_p33532770"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps[?page_size, page_no, id, name, app_key, creator]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：id、name、app\_key、creator、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568839_table29558883"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568839_row37253980"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568839_p64782395"><a name="zh-cn_topic_0225568839_p64782395"></a><a name="zh-cn_topic_0225568839_p64782395"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.32%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568839_p12882667"><a name="zh-cn_topic_0225568839_p12882667"></a><a name="zh-cn_topic_0225568839_p12882667"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="18.86%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568839_p36863124"><a name="zh-cn_topic_0225568839_p36863124"></a><a name="zh-cn_topic_0225568839_p36863124"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="36.82%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568839_p33123037"><a name="zh-cn_topic_0225568839_p33123037"></a><a name="zh-cn_topic_0225568839_p33123037"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568839_row2037411811464"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p55878963"><a name="zh-cn_topic_0225568839_p55878963"></a><a name="zh-cn_topic_0225568839_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p29902160"><a name="zh-cn_topic_0225568839_p29902160"></a><a name="zh-cn_topic_0225568839_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p6155914"><a name="zh-cn_topic_0225568839_p6155914"></a><a name="zh-cn_topic_0225568839_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p28867016"><a name="zh-cn_topic_0225568839_p28867016"></a><a name="zh-cn_topic_0225568839_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row1215121874618"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p1780913159538"><a name="zh-cn_topic_0225568839_p1780913159538"></a><a name="zh-cn_topic_0225568839_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p9809215115310"><a name="zh-cn_topic_0225568839_p9809215115310"></a><a name="zh-cn_topic_0225568839_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p1280914152538"><a name="zh-cn_topic_0225568839_p1280914152538"></a><a name="zh-cn_topic_0225568839_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p1880914157537"><a name="zh-cn_topic_0225568839_p1880914157537"></a><a name="zh-cn_topic_0225568839_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row65720302"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p21744240"><a name="zh-cn_topic_0225568839_p21744240"></a><a name="zh-cn_topic_0225568839_p21744240"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p16453002"><a name="zh-cn_topic_0225568839_p16453002"></a><a name="zh-cn_topic_0225568839_p16453002"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p57624805"><a name="zh-cn_topic_0225568839_p57624805"></a><a name="zh-cn_topic_0225568839_p57624805"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p37097641"><a name="zh-cn_topic_0225568839_p37097641"></a><a name="zh-cn_topic_0225568839_p37097641"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row65443313"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p66416996"><a name="zh-cn_topic_0225568839_p66416996"></a><a name="zh-cn_topic_0225568839_p66416996"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p11067604"><a name="zh-cn_topic_0225568839_p11067604"></a><a name="zh-cn_topic_0225568839_p11067604"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p24060712"><a name="zh-cn_topic_0225568839_p24060712"></a><a name="zh-cn_topic_0225568839_p24060712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p2760649"><a name="zh-cn_topic_0225568839_p2760649"></a><a name="zh-cn_topic_0225568839_p2760649"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row1007519"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p14500243"><a name="zh-cn_topic_0225568839_p14500243"></a><a name="zh-cn_topic_0225568839_p14500243"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p33669035"><a name="zh-cn_topic_0225568839_p33669035"></a><a name="zh-cn_topic_0225568839_p33669035"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p42837328"><a name="zh-cn_topic_0225568839_p42837328"></a><a name="zh-cn_topic_0225568839_p42837328"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p47271529"><a name="zh-cn_topic_0225568839_p47271529"></a><a name="zh-cn_topic_0225568839_p47271529"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row22790581"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p34097752"><a name="zh-cn_topic_0225568839_p34097752"></a><a name="zh-cn_topic_0225568839_p34097752"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p10454499"><a name="zh-cn_topic_0225568839_p10454499"></a><a name="zh-cn_topic_0225568839_p10454499"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p41508095"><a name="zh-cn_topic_0225568839_p41508095"></a><a name="zh-cn_topic_0225568839_p41508095"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p6712531"><a name="zh-cn_topic_0225568839_p6712531"></a><a name="zh-cn_topic_0225568839_p6712531"></a>APP的KEY</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row2838323152510"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p148381123152516"><a name="zh-cn_topic_0225568839_p148381123152516"></a><a name="zh-cn_topic_0225568839_p148381123152516"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p10838223112516"><a name="zh-cn_topic_0225568839_p10838223112516"></a><a name="zh-cn_topic_0225568839_p10838223112516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p128381023202515"><a name="zh-cn_topic_0225568839_p128381023202515"></a><a name="zh-cn_topic_0225568839_p128381023202515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p78385238252"><a name="zh-cn_topic_0225568839_p78385238252"></a><a name="zh-cn_topic_0225568839_p78385238252"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0225568839_ul1126756132511"></a><a name="zh-cn_topic_0225568839_ul1126756132511"></a><ul id="zh-cn_topic_0225568839_ul1126756132511"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row60412786"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p61597518"><a name="zh-cn_topic_0225568839_p61597518"></a><a name="zh-cn_topic_0225568839_p61597518"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p23343095"><a name="zh-cn_topic_0225568839_p23343095"></a><a name="zh-cn_topic_0225568839_p23343095"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p11742548"><a name="zh-cn_topic_0225568839_p11742548"></a><a name="zh-cn_topic_0225568839_p11742548"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p11622350"><a name="zh-cn_topic_0225568839_p11622350"></a><a name="zh-cn_topic_0225568839_p11622350"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row37492289"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p16976560"><a name="zh-cn_topic_0225568839_p16976560"></a><a name="zh-cn_topic_0225568839_p16976560"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p32924144"><a name="zh-cn_topic_0225568839_p32924144"></a><a name="zh-cn_topic_0225568839_p32924144"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p49610025"><a name="zh-cn_topic_0225568839_p49610025"></a><a name="zh-cn_topic_0225568839_p49610025"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p58989058"><a name="zh-cn_topic_0225568839_p58989058"></a><a name="zh-cn_topic_0225568839_p58989058"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row1797011282498"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568839_p297092819498"><a name="zh-cn_topic_0225568839_p297092819498"></a><a name="zh-cn_topic_0225568839_p297092819498"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568839_p397092812491"><a name="zh-cn_topic_0225568839_p397092812491"></a><a name="zh-cn_topic_0225568839_p397092812491"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568839_p49701728194913"><a name="zh-cn_topic_0225568839_p49701728194913"></a><a name="zh-cn_topic_0225568839_p49701728194913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="36.82%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568839_p19970928194911"><a name="zh-cn_topic_0225568839_p19970928194911"></a><a name="zh-cn_topic_0225568839_p19970928194911"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568839_section30793819"></a>

无

## 响应消息<a name="zh-cn_topic_0225568839_section11271404"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568839_table23954455"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568839_row66752668"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568839_p38257064"><a name="zh-cn_topic_0225568839_p38257064"></a><a name="zh-cn_topic_0225568839_p38257064"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568839_p11814447"><a name="zh-cn_topic_0225568839_p11814447"></a><a name="zh-cn_topic_0225568839_p11814447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568839_p17446171"><a name="zh-cn_topic_0225568839_p17446171"></a><a name="zh-cn_topic_0225568839_p17446171"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568839_row3853780"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p43720769"><a name="zh-cn_topic_0225568839_p43720769"></a><a name="zh-cn_topic_0225568839_p43720769"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p51721419"><a name="zh-cn_topic_0225568839_p51721419"></a><a name="zh-cn_topic_0225568839_p51721419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p28685401"><a name="zh-cn_topic_0225568839_p28685401"></a><a name="zh-cn_topic_0225568839_p28685401"></a>符合条件的APP总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row56842021"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p40801013"><a name="zh-cn_topic_0225568839_p40801013"></a><a name="zh-cn_topic_0225568839_p40801013"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p16547774"><a name="zh-cn_topic_0225568839_p16547774"></a><a name="zh-cn_topic_0225568839_p16547774"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p65301287"><a name="zh-cn_topic_0225568839_p65301287"></a><a name="zh-cn_topic_0225568839_p65301287"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row50840671"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p24453659"><a name="zh-cn_topic_0225568839_p24453659"></a><a name="zh-cn_topic_0225568839_p24453659"></a>apps</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p34589388"><a name="zh-cn_topic_0225568839_p34589388"></a><a name="zh-cn_topic_0225568839_p34589388"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p50277082"><a name="zh-cn_topic_0225568839_p50277082"></a><a name="zh-cn_topic_0225568839_p50277082"></a>APP列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apps参数说明

<a name="zh-cn_topic_0225568839_table49840559"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568839_row181838"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568839_p14728898"><a name="zh-cn_topic_0225568839_p14728898"></a><a name="zh-cn_topic_0225568839_p14728898"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568839_p52190083"><a name="zh-cn_topic_0225568839_p52190083"></a><a name="zh-cn_topic_0225568839_p52190083"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568839_p66647160"><a name="zh-cn_topic_0225568839_p66647160"></a><a name="zh-cn_topic_0225568839_p66647160"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568839_row29710857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p57769248"><a name="zh-cn_topic_0225568839_p57769248"></a><a name="zh-cn_topic_0225568839_p57769248"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p48797474"><a name="zh-cn_topic_0225568839_p48797474"></a><a name="zh-cn_topic_0225568839_p48797474"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p60281337"><a name="zh-cn_topic_0225568839_p60281337"></a><a name="zh-cn_topic_0225568839_p60281337"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row5661128"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p55898233"><a name="zh-cn_topic_0225568839_p55898233"></a><a name="zh-cn_topic_0225568839_p55898233"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p31463026"><a name="zh-cn_topic_0225568839_p31463026"></a><a name="zh-cn_topic_0225568839_p31463026"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p65477212"><a name="zh-cn_topic_0225568839_p65477212"></a><a name="zh-cn_topic_0225568839_p65477212"></a>名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row52424003"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p18485849"><a name="zh-cn_topic_0225568839_p18485849"></a><a name="zh-cn_topic_0225568839_p18485849"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p20958771"><a name="zh-cn_topic_0225568839_p20958771"></a><a name="zh-cn_topic_0225568839_p20958771"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p19938873"><a name="zh-cn_topic_0225568839_p19938873"></a><a name="zh-cn_topic_0225568839_p19938873"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row45232137"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p39924477"><a name="zh-cn_topic_0225568839_p39924477"></a><a name="zh-cn_topic_0225568839_p39924477"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p12657234"><a name="zh-cn_topic_0225568839_p12657234"></a><a name="zh-cn_topic_0225568839_p12657234"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p18603056"><a name="zh-cn_topic_0225568839_p18603056"></a><a name="zh-cn_topic_0225568839_p18603056"></a>APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row33209777"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p5637422"><a name="zh-cn_topic_0225568839_p5637422"></a><a name="zh-cn_topic_0225568839_p5637422"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p53978056"><a name="zh-cn_topic_0225568839_p53978056"></a><a name="zh-cn_topic_0225568839_p53978056"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p10146406"><a name="zh-cn_topic_0225568839_p10146406"></a><a name="zh-cn_topic_0225568839_p10146406"></a>密钥</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row24208794"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p14755322"><a name="zh-cn_topic_0225568839_p14755322"></a><a name="zh-cn_topic_0225568839_p14755322"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p54330451"><a name="zh-cn_topic_0225568839_p54330451"></a><a name="zh-cn_topic_0225568839_p54330451"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p38690380"><a name="zh-cn_topic_0225568839_p38690380"></a><a name="zh-cn_topic_0225568839_p38690380"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row12669100"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p19564152"><a name="zh-cn_topic_0225568839_p19564152"></a><a name="zh-cn_topic_0225568839_p19564152"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p41192505"><a name="zh-cn_topic_0225568839_p41192505"></a><a name="zh-cn_topic_0225568839_p41192505"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p48258647"><a name="zh-cn_topic_0225568839_p48258647"></a><a name="zh-cn_topic_0225568839_p48258647"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row31674644"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p15509384"><a name="zh-cn_topic_0225568839_p15509384"></a><a name="zh-cn_topic_0225568839_p15509384"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p48300555"><a name="zh-cn_topic_0225568839_p48300555"></a><a name="zh-cn_topic_0225568839_p48300555"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p20030920"><a name="zh-cn_topic_0225568839_p20030920"></a><a name="zh-cn_topic_0225568839_p20030920"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row81831714928"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p111407484101"><a name="zh-cn_topic_0225568839_p111407484101"></a><a name="zh-cn_topic_0225568839_p111407484101"></a>creator</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p214013484105"><a name="zh-cn_topic_0225568839_p214013484105"></a><a name="zh-cn_topic_0225568839_p214013484105"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p214004841017"><a name="zh-cn_topic_0225568839_p214004841017"></a><a name="zh-cn_topic_0225568839_p214004841017"></a>APP的创建者，取值如下：</p>
<a name="zh-cn_topic_0225568839_ul101401948201015"></a><a name="zh-cn_topic_0225568839_ul101401948201015"></a><ul id="zh-cn_topic_0225568839_ul101401948201015"><li>USER：用户自行创建</li><li>MARKET：云市场分配</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row1326101675216"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p14855159163015"><a name="zh-cn_topic_0225568839_p14855159163015"></a><a name="zh-cn_topic_0225568839_p14855159163015"></a>app_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p12855195993012"><a name="zh-cn_topic_0225568839_p12855195993012"></a><a name="zh-cn_topic_0225568839_p12855195993012"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p1085575910302"><a name="zh-cn_topic_0225568839_p1085575910302"></a><a name="zh-cn_topic_0225568839_p1085575910302"></a>APP类型，默认为apig</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row16235953312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568839_p52361752033"><a name="zh-cn_topic_0225568839_p52361752033"></a><a name="zh-cn_topic_0225568839_p52361752033"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568839_p12236185032"><a name="zh-cn_topic_0225568839_p12236185032"></a><a name="zh-cn_topic_0225568839_p12236185032"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568839_p17236557312"><a name="zh-cn_topic_0225568839_p17236557312"></a><a name="zh-cn_topic_0225568839_p17236557312"></a>绑定的API数量</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"apps": [{
		"id": "98efd77d-10b5-4eca-8170-ed30a4a286a4",
		"name": "app_002",
		"status": 1,
		"app_key": "f627fbaa-2c8b-4f58-a690-f478f54d3fe2",
		"app_secret": "******",
		"remark": "第二个APP",
		"register_time": "2017-12-28T12:32:50Z",
		"update_time": "2017-12-28T12:32:50Z",
		"creator": "MARKET",
                "app_type": "apig",
                "bind_num": 2
	},
	{
		"id": "14b399ac-967f-4115-bb62-c0346b4537e9",
		"name": "app_001",
		"status": 1,
		"app_key": "d49b1cbf-cc81-4a5f-b2a0-61b568e376eb",
		"app_secret": "******",
		"remark": "第一个APP",
		"register_time": "2017-12-28T12:26:54Z",
		"update_time": "2017-12-28T12:29:35.571Z",
		"creator": "USER",
                "app_type": "apig",
                "bind_num": 2
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568839_section8708918"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568839_table10390965"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568839_row66877087"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568839_p48334990"><a name="zh-cn_topic_0225568839_p48334990"></a><a name="zh-cn_topic_0225568839_p48334990"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568839_p22820113"><a name="zh-cn_topic_0225568839_p22820113"></a><a name="zh-cn_topic_0225568839_p22820113"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568839_row36489873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568839_p2889717"><a name="zh-cn_topic_0225568839_p2889717"></a><a name="zh-cn_topic_0225568839_p2889717"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568839_p32740518"><a name="zh-cn_topic_0225568839_p32740518"></a><a name="zh-cn_topic_0225568839_p32740518"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row26229206"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568839_p44190948"><a name="zh-cn_topic_0225568839_p44190948"></a><a name="zh-cn_topic_0225568839_p44190948"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568839_p22697075"><a name="zh-cn_topic_0225568839_p22697075"></a><a name="zh-cn_topic_0225568839_p22697075"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row2947091"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568839_p37387781"><a name="zh-cn_topic_0225568839_p37387781"></a><a name="zh-cn_topic_0225568839_p37387781"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568839_p8511436"><a name="zh-cn_topic_0225568839_p8511436"></a><a name="zh-cn_topic_0225568839_p8511436"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568839_row9494067"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568839_p30821972"><a name="zh-cn_topic_0225568839_p30821972"></a><a name="zh-cn_topic_0225568839_p30821972"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568839_p13551805"><a name="zh-cn_topic_0225568839_p13551805"></a><a name="zh-cn_topic_0225568839_p13551805"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

