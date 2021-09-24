# 查看特殊设置列表<a name="ZH-CN_TOPIC_0000001081976197"></a>

## 功能介绍<a name="zh-cn_topic_0225568880_section53699803"></a>

查看给流控策略设置的特殊配置。

## URI<a name="zh-cn_topic_0225568880_section13536187"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568880_table40932678"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568880_row32630007"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568880_p25784877"><a name="zh-cn_topic_0225568880_p25784877"></a><a name="zh-cn_topic_0225568880_p25784877"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568880_p8200292"><a name="zh-cn_topic_0225568880_p8200292"></a><a name="zh-cn_topic_0225568880_p8200292"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568880_row60243907"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568880_p47918323"><a name="zh-cn_topic_0225568880_p47918323"></a><a name="zh-cn_topic_0225568880_p47918323"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568880_p56178972"><a name="zh-cn_topic_0225568880_p56178972"></a><a name="zh-cn_topic_0225568880_p56178972"></a>/v1/{project_id}/apigw/instances/{instance_id}/throttle-specials/{strategy_id}[?page_size, page_no, instance_type, app_name, user]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：strategy\_id、app\_name、user、 page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568880_table53867817"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568880_row12559801"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568880_p10710956"><a name="zh-cn_topic_0225568880_p10710956"></a><a name="zh-cn_topic_0225568880_p10710956"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.549999999999997%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568880_p62281116"><a name="zh-cn_topic_0225568880_p62281116"></a><a name="zh-cn_topic_0225568880_p62281116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="21.98%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568880_p11605616"><a name="zh-cn_topic_0225568880_p11605616"></a><a name="zh-cn_topic_0225568880_p11605616"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="32.47%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568880_p530833"><a name="zh-cn_topic_0225568880_p530833"></a><a name="zh-cn_topic_0225568880_p530833"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568880_row171520509178"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p55878963"><a name="zh-cn_topic_0225568880_p55878963"></a><a name="zh-cn_topic_0225568880_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p29902160"><a name="zh-cn_topic_0225568880_p29902160"></a><a name="zh-cn_topic_0225568880_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p6155914"><a name="zh-cn_topic_0225568880_p6155914"></a><a name="zh-cn_topic_0225568880_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p28867016"><a name="zh-cn_topic_0225568880_p28867016"></a><a name="zh-cn_topic_0225568880_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row36407497172"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p1780913159538"><a name="zh-cn_topic_0225568880_p1780913159538"></a><a name="zh-cn_topic_0225568880_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p9809215115310"><a name="zh-cn_topic_0225568880_p9809215115310"></a><a name="zh-cn_topic_0225568880_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p1280914152538"><a name="zh-cn_topic_0225568880_p1280914152538"></a><a name="zh-cn_topic_0225568880_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p1880914157537"><a name="zh-cn_topic_0225568880_p1880914157537"></a><a name="zh-cn_topic_0225568880_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row42997478"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p60243671"><a name="zh-cn_topic_0225568880_p60243671"></a><a name="zh-cn_topic_0225568880_p60243671"></a>strategy_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p47899214"><a name="zh-cn_topic_0225568880_p47899214"></a><a name="zh-cn_topic_0225568880_p47899214"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p54631088"><a name="zh-cn_topic_0225568880_p54631088"></a><a name="zh-cn_topic_0225568880_p54631088"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p63042023"><a name="zh-cn_topic_0225568880_p63042023"></a><a name="zh-cn_topic_0225568880_p63042023"></a>流控策略的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row30507302"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p55172407"><a name="zh-cn_topic_0225568880_p55172407"></a><a name="zh-cn_topic_0225568880_p55172407"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p39779984"><a name="zh-cn_topic_0225568880_p39779984"></a><a name="zh-cn_topic_0225568880_p39779984"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p953306"><a name="zh-cn_topic_0225568880_p953306"></a><a name="zh-cn_topic_0225568880_p953306"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p10108989"><a name="zh-cn_topic_0225568880_p10108989"></a><a name="zh-cn_topic_0225568880_p10108989"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row23872039"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p54586977"><a name="zh-cn_topic_0225568880_p54586977"></a><a name="zh-cn_topic_0225568880_p54586977"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p59468999"><a name="zh-cn_topic_0225568880_p59468999"></a><a name="zh-cn_topic_0225568880_p59468999"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p52259651"><a name="zh-cn_topic_0225568880_p52259651"></a><a name="zh-cn_topic_0225568880_p52259651"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p5173306"><a name="zh-cn_topic_0225568880_p5173306"></a><a name="zh-cn_topic_0225568880_p5173306"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row15125101515175"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p212531571712"><a name="zh-cn_topic_0225568880_p212531571712"></a><a name="zh-cn_topic_0225568880_p212531571712"></a>instance_type</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p6125131521715"><a name="zh-cn_topic_0225568880_p6125131521715"></a><a name="zh-cn_topic_0225568880_p6125131521715"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p16125915191714"><a name="zh-cn_topic_0225568880_p16125915191714"></a><a name="zh-cn_topic_0225568880_p16125915191714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p101250157175"><a name="zh-cn_topic_0225568880_p101250157175"></a><a name="zh-cn_topic_0225568880_p101250157175"></a>特殊流控类型:  APP, USER</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row410983481718"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p181091834121710"><a name="zh-cn_topic_0225568880_p181091834121710"></a><a name="zh-cn_topic_0225568880_p181091834121710"></a>app_name</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p12109133417175"><a name="zh-cn_topic_0225568880_p12109133417175"></a><a name="zh-cn_topic_0225568880_p12109133417175"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p6109163471713"><a name="zh-cn_topic_0225568880_p6109163471713"></a><a name="zh-cn_topic_0225568880_p6109163471713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p1210933412175"><a name="zh-cn_topic_0225568880_p1210933412175"></a><a name="zh-cn_topic_0225568880_p1210933412175"></a>筛选的特殊应用名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row1243343015612"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568880_p343313303568"><a name="zh-cn_topic_0225568880_p343313303568"></a><a name="zh-cn_topic_0225568880_p343313303568"></a>user</p>
</td>
<td class="cellrowborder" valign="top" width="20.549999999999997%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568880_p2433103011567"><a name="zh-cn_topic_0225568880_p2433103011567"></a><a name="zh-cn_topic_0225568880_p2433103011567"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.98%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568880_p1243319307563"><a name="zh-cn_topic_0225568880_p1243319307563"></a><a name="zh-cn_topic_0225568880_p1243319307563"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="32.47%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568880_p1743383018563"><a name="zh-cn_topic_0225568880_p1743383018563"></a><a name="zh-cn_topic_0225568880_p1743383018563"></a>筛选的特殊租户的帐号ID</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568880_section54716821"></a>

无

## 响应消息<a name="zh-cn_topic_0225568880_section2877544"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568880_table25878126"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568880_row28160051"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568880_p66371643"><a name="zh-cn_topic_0225568880_p66371643"></a><a name="zh-cn_topic_0225568880_p66371643"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568880_p7393979"><a name="zh-cn_topic_0225568880_p7393979"></a><a name="zh-cn_topic_0225568880_p7393979"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568880_p62041436"><a name="zh-cn_topic_0225568880_p62041436"></a><a name="zh-cn_topic_0225568880_p62041436"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568880_row59300421"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p38604831"><a name="zh-cn_topic_0225568880_p38604831"></a><a name="zh-cn_topic_0225568880_p38604831"></a>throttle_specials</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p39983634"><a name="zh-cn_topic_0225568880_p39983634"></a><a name="zh-cn_topic_0225568880_p39983634"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p17448901"><a name="zh-cn_topic_0225568880_p17448901"></a><a name="zh-cn_topic_0225568880_p17448901"></a>本次查询返回的特殊配置列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row22822382"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p36673636"><a name="zh-cn_topic_0225568880_p36673636"></a><a name="zh-cn_topic_0225568880_p36673636"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p17774576"><a name="zh-cn_topic_0225568880_p17774576"></a><a name="zh-cn_topic_0225568880_p17774576"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p30454519"><a name="zh-cn_topic_0225568880_p30454519"></a><a name="zh-cn_topic_0225568880_p30454519"></a>符合条件的特殊设置总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row5655221"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p55419779"><a name="zh-cn_topic_0225568880_p55419779"></a><a name="zh-cn_topic_0225568880_p55419779"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p59817089"><a name="zh-cn_topic_0225568880_p59817089"></a><a name="zh-cn_topic_0225568880_p59817089"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p13346007"><a name="zh-cn_topic_0225568880_p13346007"></a><a name="zh-cn_topic_0225568880_p13346007"></a>本次查询返回的列表长度</p>
</td>
</tr>
</tbody>
</table>

**表 4**  throttle\_specials参数说明

<a name="zh-cn_topic_0225568880_table53005203"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568880_row55893062"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568880_p31044143"><a name="zh-cn_topic_0225568880_p31044143"></a><a name="zh-cn_topic_0225568880_p31044143"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568880_p31547616"><a name="zh-cn_topic_0225568880_p31547616"></a><a name="zh-cn_topic_0225568880_p31547616"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568880_p5220098"><a name="zh-cn_topic_0225568880_p5220098"></a><a name="zh-cn_topic_0225568880_p5220098"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568880_row20174780"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p23544503"><a name="zh-cn_topic_0225568880_p23544503"></a><a name="zh-cn_topic_0225568880_p23544503"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p28056603"><a name="zh-cn_topic_0225568880_p28056603"></a><a name="zh-cn_topic_0225568880_p28056603"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p57992334"><a name="zh-cn_topic_0225568880_p57992334"></a><a name="zh-cn_topic_0225568880_p57992334"></a>特殊配置的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row52168966"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p64936726"><a name="zh-cn_topic_0225568880_p64936726"></a><a name="zh-cn_topic_0225568880_p64936726"></a>strategy_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p25383434"><a name="zh-cn_topic_0225568880_p25383434"></a><a name="zh-cn_topic_0225568880_p25383434"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p42792267"><a name="zh-cn_topic_0225568880_p42792267"></a><a name="zh-cn_topic_0225568880_p42792267"></a>流控策略编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row49586083"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p57049793"><a name="zh-cn_topic_0225568880_p57049793"></a><a name="zh-cn_topic_0225568880_p57049793"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p57630560"><a name="zh-cn_topic_0225568880_p57630560"></a><a name="zh-cn_topic_0225568880_p57630560"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p37563816"><a name="zh-cn_topic_0225568880_p37563816"></a><a name="zh-cn_topic_0225568880_p37563816"></a>特殊对象的身份标识</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row768118995716"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p28677105577"><a name="zh-cn_topic_0225568880_p28677105577"></a><a name="zh-cn_topic_0225568880_p28677105577"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p88691010165715"><a name="zh-cn_topic_0225568880_p88691010165715"></a><a name="zh-cn_topic_0225568880_p88691010165715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p16872191085717"><a name="zh-cn_topic_0225568880_p16872191085717"></a><a name="zh-cn_topic_0225568880_p16872191085717"></a>作用的APP或租户的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row2530026"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p3605569"><a name="zh-cn_topic_0225568880_p3605569"></a><a name="zh-cn_topic_0225568880_p3605569"></a>instance_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p23615701"><a name="zh-cn_topic_0225568880_p23615701"></a><a name="zh-cn_topic_0225568880_p23615701"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p33823629"><a name="zh-cn_topic_0225568880_p33823629"></a><a name="zh-cn_topic_0225568880_p33823629"></a>特殊对象的类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row35977210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p28472932"><a name="zh-cn_topic_0225568880_p28472932"></a><a name="zh-cn_topic_0225568880_p28472932"></a>call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p24606183"><a name="zh-cn_topic_0225568880_p24606183"></a><a name="zh-cn_topic_0225568880_p24606183"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p46943786"><a name="zh-cn_topic_0225568880_p46943786"></a><a name="zh-cn_topic_0225568880_p46943786"></a>特殊对象在流控时间内能够访问API的最大次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row19840891"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p63608321"><a name="zh-cn_topic_0225568880_p63608321"></a><a name="zh-cn_topic_0225568880_p63608321"></a>apply_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p52000413"><a name="zh-cn_topic_0225568880_p52000413"></a><a name="zh-cn_topic_0225568880_p52000413"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p51283892"><a name="zh-cn_topic_0225568880_p51283892"></a><a name="zh-cn_topic_0225568880_p51283892"></a>设置时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row17977161825718"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p166372135718"><a name="zh-cn_topic_0225568880_p166372135718"></a><a name="zh-cn_topic_0225568880_p166372135718"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p865122175719"><a name="zh-cn_topic_0225568880_p865122175719"></a><a name="zh-cn_topic_0225568880_p865122175719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p266192165714"><a name="zh-cn_topic_0225568880_p266192165714"></a><a name="zh-cn_topic_0225568880_p266192165714"></a>作用的APP编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row58901850"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568880_p6320568"><a name="zh-cn_topic_0225568880_p6320568"></a><a name="zh-cn_topic_0225568880_p6320568"></a>app_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568880_p42203974"><a name="zh-cn_topic_0225568880_p42203974"></a><a name="zh-cn_topic_0225568880_p42203974"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568880_p63078700"><a name="zh-cn_topic_0225568880_p63078700"></a><a name="zh-cn_topic_0225568880_p63078700"></a>作用的APP名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 1,
	"size": 1,
	"throttle_specials": [{
		"id": "778879b8-df10-495b-a087-874859fdea6d",
		"strategy_id": "a3106cfe-801f-4919-b0d7-d785dc5b47f9",
		"instance_id": "98efd77d-10b5-4eca-8170-ed30a4a286a4",
		"instance_name": "app_002",
		"instance_type": "APP",
		"call_limits": 180,
		"apply_time": "2017-12-29T03:11:18Z",
		"app_id": "98efd77d-10b5-4eca-8170-ed30a4a286a4",
		"app_name": "app_002"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568880_section22689348"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568880_table52089279"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568880_row19305289"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568880_p20224568"><a name="zh-cn_topic_0225568880_p20224568"></a><a name="zh-cn_topic_0225568880_p20224568"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568880_p27577336"><a name="zh-cn_topic_0225568880_p27577336"></a><a name="zh-cn_topic_0225568880_p27577336"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568880_row19171761"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568880_p9408778"><a name="zh-cn_topic_0225568880_p9408778"></a><a name="zh-cn_topic_0225568880_p9408778"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568880_p23913515"><a name="zh-cn_topic_0225568880_p23913515"></a><a name="zh-cn_topic_0225568880_p23913515"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row13895046"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568880_p51756967"><a name="zh-cn_topic_0225568880_p51756967"></a><a name="zh-cn_topic_0225568880_p51756967"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568880_p31564837"><a name="zh-cn_topic_0225568880_p31564837"></a><a name="zh-cn_topic_0225568880_p31564837"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row15648082"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568880_p59535142"><a name="zh-cn_topic_0225568880_p59535142"></a><a name="zh-cn_topic_0225568880_p59535142"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568880_p57617161"><a name="zh-cn_topic_0225568880_p57617161"></a><a name="zh-cn_topic_0225568880_p57617161"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row48792409"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568880_p59871065"><a name="zh-cn_topic_0225568880_p59871065"></a><a name="zh-cn_topic_0225568880_p59871065"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568880_p17718077"><a name="zh-cn_topic_0225568880_p17718077"></a><a name="zh-cn_topic_0225568880_p17718077"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568880_row440216351571"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568880_p9402163514714"><a name="zh-cn_topic_0225568880_p9402163514714"></a><a name="zh-cn_topic_0225568880_p9402163514714"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568880_p740212352716"><a name="zh-cn_topic_0225568880_p740212352716"></a><a name="zh-cn_topic_0225568880_p740212352716"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

