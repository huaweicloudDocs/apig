# 对象模型<a name="ZH-CN_TOPIC_0000001081837317"></a>

本节介绍VPC通道的对象模型。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  VPC通道对象模型

<a name="zh-cn_topic_0118924572_table49332581"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924572_row15637543"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924572_p58681484"><a name="zh-cn_topic_0118924572_p58681484"></a><a name="zh-cn_topic_0118924572_p58681484"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924572_p55579749"><a name="zh-cn_topic_0118924572_p55579749"></a><a name="zh-cn_topic_0118924572_p55579749"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924572_p5665819"><a name="zh-cn_topic_0118924572_p5665819"></a><a name="zh-cn_topic_0118924572_p5665819"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924572_p56278165"><a name="zh-cn_topic_0118924572_p56278165"></a><a name="zh-cn_topic_0118924572_p56278165"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924572_p62237499"><a name="zh-cn_topic_0118924572_p62237499"></a><a name="zh-cn_topic_0118924572_p62237499"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924572_row8072695"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p49908526"><a name="zh-cn_topic_0118924572_p49908526"></a><a name="zh-cn_topic_0118924572_p49908526"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p16058826"><a name="zh-cn_topic_0118924572_p16058826"></a><a name="zh-cn_topic_0118924572_p16058826"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p25696563"><a name="zh-cn_topic_0118924572_p25696563"></a><a name="zh-cn_topic_0118924572_p25696563"></a>VPC通道的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p1046864"><a name="zh-cn_topic_0118924572_p1046864"></a><a name="zh-cn_topic_0118924572_p1046864"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p17687178"><a name="zh-cn_topic_0118924572_p17687178"></a><a name="zh-cn_topic_0118924572_p17687178"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row24966877"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p9051148"><a name="zh-cn_topic_0118924572_p9051148"></a><a name="zh-cn_topic_0118924572_p9051148"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p62054412"><a name="zh-cn_topic_0118924572_p62054412"></a><a name="zh-cn_topic_0118924572_p62054412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p60351493"><a name="zh-cn_topic_0118924572_p60351493"></a><a name="zh-cn_topic_0118924572_p60351493"></a>VPC通道的名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p56632734"><a name="zh-cn_topic_0118924572_p56632734"></a><a name="zh-cn_topic_0118924572_p56632734"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p23848703"><a name="zh-cn_topic_0118924572_p23848703"></a><a name="zh-cn_topic_0118924572_p23848703"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row13311738"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p4509019"><a name="zh-cn_topic_0118924572_p4509019"></a><a name="zh-cn_topic_0118924572_p4509019"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p29686297"><a name="zh-cn_topic_0118924572_p29686297"></a><a name="zh-cn_topic_0118924572_p29686297"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p55779867"><a name="zh-cn_topic_0118924572_p55779867"></a><a name="zh-cn_topic_0118924572_p55779867"></a>VPC通道的类型</p>
<a name="zh-cn_topic_0118924572_ul53721145134416"></a><a name="zh-cn_topic_0118924572_ul53721145134416"></a><ul id="zh-cn_topic_0118924572_ul53721145134416"><li>2：Builtin通道类型</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p21875402"><a name="zh-cn_topic_0118924572_p21875402"></a><a name="zh-cn_topic_0118924572_p21875402"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p27077133"><a name="zh-cn_topic_0118924572_p27077133"></a><a name="zh-cn_topic_0118924572_p27077133"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row82661851161"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p926619591611"><a name="zh-cn_topic_0118924572_p926619591611"></a><a name="zh-cn_topic_0118924572_p926619591611"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p182661752166"><a name="zh-cn_topic_0118924572_p182661752166"></a><a name="zh-cn_topic_0118924572_p182661752166"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p12663581620"><a name="zh-cn_topic_0118924572_p12663581620"></a><a name="zh-cn_topic_0118924572_p12663581620"></a>VPC通道的状态</p>
<a name="zh-cn_topic_0118924572_ul15791839184416"></a><a name="zh-cn_topic_0118924572_ul15791839184416"></a><ul id="zh-cn_topic_0118924572_ul15791839184416"><li>1：正常</li><li>2：异常</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p7266350167"><a name="zh-cn_topic_0118924572_p7266350167"></a><a name="zh-cn_topic_0118924572_p7266350167"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p152667591616"><a name="zh-cn_topic_0118924572_p152667591616"></a><a name="zh-cn_topic_0118924572_p152667591616"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row42367610"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p9224375"><a name="zh-cn_topic_0118924572_p9224375"></a><a name="zh-cn_topic_0118924572_p9224375"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p8976892"><a name="zh-cn_topic_0118924572_p8976892"></a><a name="zh-cn_topic_0118924572_p8976892"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p79993152715"><a name="zh-cn_topic_0118924572_p79993152715"></a><a name="zh-cn_topic_0118924572_p79993152715"></a>租户的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p15296911"><a name="zh-cn_topic_0118924572_p15296911"></a><a name="zh-cn_topic_0118924572_p15296911"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p31090241"><a name="zh-cn_topic_0118924572_p31090241"></a><a name="zh-cn_topic_0118924572_p31090241"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row11376719"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p49099023"><a name="zh-cn_topic_0118924572_p49099023"></a><a name="zh-cn_topic_0118924572_p49099023"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p17597936"><a name="zh-cn_topic_0118924572_p17597936"></a><a name="zh-cn_topic_0118924572_p17597936"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p16681305"><a name="zh-cn_topic_0118924572_p16681305"></a><a name="zh-cn_topic_0118924572_p16681305"></a>端口</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p13967064"><a name="zh-cn_topic_0118924572_p13967064"></a><a name="zh-cn_topic_0118924572_p13967064"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p57590436"><a name="zh-cn_topic_0118924572_p57590436"></a><a name="zh-cn_topic_0118924572_p57590436"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row82989413144"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p192983401416"><a name="zh-cn_topic_0118924572_p192983401416"></a><a name="zh-cn_topic_0118924572_p192983401416"></a>balance_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p182985416144"><a name="zh-cn_topic_0118924572_p182985416144"></a><a name="zh-cn_topic_0118924572_p182985416144"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p22981401418"><a name="zh-cn_topic_0118924572_p22981401418"></a><a name="zh-cn_topic_0118924572_p22981401418"></a>分发算法</p>
<a name="zh-cn_topic_0118924572_ul31881612450"></a><a name="zh-cn_topic_0118924572_ul31881612450"></a><ul id="zh-cn_topic_0118924572_ul31881612450"><li>1：加权轮询（wrr）</li><li>2：加权最少连接（wleastconn）</li><li>3：源地址哈希（source）</li><li>4：URI哈希（uri）</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p8298154131413"><a name="zh-cn_topic_0118924572_p8298154131413"></a><a name="zh-cn_topic_0118924572_p8298154131413"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p1298148144"><a name="zh-cn_topic_0118924572_p1298148144"></a><a name="zh-cn_topic_0118924572_p1298148144"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row684511713148"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p8845107161418"><a name="zh-cn_topic_0118924572_p8845107161418"></a><a name="zh-cn_topic_0118924572_p8845107161418"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p188451179141"><a name="zh-cn_topic_0118924572_p188451179141"></a><a name="zh-cn_topic_0118924572_p188451179141"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p198451273146"><a name="zh-cn_topic_0118924572_p198451273146"></a><a name="zh-cn_topic_0118924572_p198451273146"></a>创建时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p784537191416"><a name="zh-cn_topic_0118924572_p784537191416"></a><a name="zh-cn_topic_0118924572_p784537191416"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p128457751410"><a name="zh-cn_topic_0118924572_p128457751410"></a><a name="zh-cn_topic_0118924572_p128457751410"></a>是</p>
</td>
</tr>
</tbody>
</table>

**表 2**  健康检查对象模型

<a name="zh-cn_topic_0118924572_table41340048"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924572_row37775636"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924572_p39927684"><a name="zh-cn_topic_0118924572_p39927684"></a><a name="zh-cn_topic_0118924572_p39927684"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924572_p12916952"><a name="zh-cn_topic_0118924572_p12916952"></a><a name="zh-cn_topic_0118924572_p12916952"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924572_p39640185"><a name="zh-cn_topic_0118924572_p39640185"></a><a name="zh-cn_topic_0118924572_p39640185"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924572_p56738382"><a name="zh-cn_topic_0118924572_p56738382"></a><a name="zh-cn_topic_0118924572_p56738382"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924572_p32406207"><a name="zh-cn_topic_0118924572_p32406207"></a><a name="zh-cn_topic_0118924572_p32406207"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924572_row5223161311563"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p143411395613"><a name="zh-cn_topic_0118924572_p143411395613"></a><a name="zh-cn_topic_0118924572_p143411395613"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p43451314563"><a name="zh-cn_topic_0118924572_p43451314563"></a><a name="zh-cn_topic_0118924572_p43451314563"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p8501113105613"><a name="zh-cn_topic_0118924572_p8501113105613"></a><a name="zh-cn_topic_0118924572_p8501113105613"></a>健康检查的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p1850121317564"><a name="zh-cn_topic_0118924572_p1850121317564"></a><a name="zh-cn_topic_0118924572_p1850121317564"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p2501713175617"><a name="zh-cn_topic_0118924572_p2501713175617"></a><a name="zh-cn_topic_0118924572_p2501713175617"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row92231713195610"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p105091312566"><a name="zh-cn_topic_0118924572_p105091312566"></a><a name="zh-cn_topic_0118924572_p105091312566"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p195018139566"><a name="zh-cn_topic_0118924572_p195018139566"></a><a name="zh-cn_topic_0118924572_p195018139566"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p135016132562"><a name="zh-cn_topic_0118924572_p135016132562"></a><a name="zh-cn_topic_0118924572_p135016132562"></a>VPC通道的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p35051312566"><a name="zh-cn_topic_0118924572_p35051312566"></a><a name="zh-cn_topic_0118924572_p35051312566"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p125001365613"><a name="zh-cn_topic_0118924572_p125001365613"></a><a name="zh-cn_topic_0118924572_p125001365613"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row132231913105617"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p05011138562"><a name="zh-cn_topic_0118924572_p05011138562"></a><a name="zh-cn_topic_0118924572_p05011138562"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p1666161335612"><a name="zh-cn_topic_0118924572_p1666161335612"></a><a name="zh-cn_topic_0118924572_p1666161335612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p1666121315567"><a name="zh-cn_topic_0118924572_p1666121315567"></a><a name="zh-cn_topic_0118924572_p1666121315567"></a>协议</p>
<a name="zh-cn_topic_0118924572_ul166101312568"></a><a name="zh-cn_topic_0118924572_ul166101312568"></a><ul id="zh-cn_topic_0118924572_ul166101312568"><li>tcp</li><li>http</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p766201365612"><a name="zh-cn_topic_0118924572_p766201365612"></a><a name="zh-cn_topic_0118924572_p766201365612"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p966101325618"><a name="zh-cn_topic_0118924572_p966101325618"></a><a name="zh-cn_topic_0118924572_p966101325618"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row7223191375620"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p266171335616"><a name="zh-cn_topic_0118924572_p266171335616"></a><a name="zh-cn_topic_0118924572_p266171335616"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p1266141345614"><a name="zh-cn_topic_0118924572_p1266141345614"></a><a name="zh-cn_topic_0118924572_p1266141345614"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p12661130563"><a name="zh-cn_topic_0118924572_p12661130563"></a><a name="zh-cn_topic_0118924572_p12661130563"></a>路径，仅当协议为http时生效</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p982101312567"><a name="zh-cn_topic_0118924572_p982101312567"></a><a name="zh-cn_topic_0118924572_p982101312567"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p2821513195610"><a name="zh-cn_topic_0118924572_p2821513195610"></a><a name="zh-cn_topic_0118924572_p2821513195610"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row5223413165612"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p582913105612"><a name="zh-cn_topic_0118924572_p582913105612"></a><a name="zh-cn_topic_0118924572_p582913105612"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p18261314567"><a name="zh-cn_topic_0118924572_p18261314567"></a><a name="zh-cn_topic_0118924572_p18261314567"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p78214132565"><a name="zh-cn_topic_0118924572_p78214132565"></a><a name="zh-cn_topic_0118924572_p78214132565"></a>端口，无值时，使用通道端口</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p882101320565"><a name="zh-cn_topic_0118924572_p882101320565"></a><a name="zh-cn_topic_0118924572_p882101320565"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p682161319562"><a name="zh-cn_topic_0118924572_p682161319562"></a><a name="zh-cn_topic_0118924572_p682161319562"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row1222381315566"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p1898513175610"><a name="zh-cn_topic_0118924572_p1898513175610"></a><a name="zh-cn_topic_0118924572_p1898513175610"></a>threshold_normal</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p39861317569"><a name="zh-cn_topic_0118924572_p39861317569"></a><a name="zh-cn_topic_0118924572_p39861317569"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p1798813185617"><a name="zh-cn_topic_0118924572_p1798813185617"></a><a name="zh-cn_topic_0118924572_p1798813185617"></a>正常阙值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p9982013135612"><a name="zh-cn_topic_0118924572_p9982013135612"></a><a name="zh-cn_topic_0118924572_p9982013135612"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p14981013145615"><a name="zh-cn_topic_0118924572_p14981013145615"></a><a name="zh-cn_topic_0118924572_p14981013145615"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row102231713165613"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p1598191305619"><a name="zh-cn_topic_0118924572_p1598191305619"></a><a name="zh-cn_topic_0118924572_p1598191305619"></a>threshold_abnormal</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p169821319568"><a name="zh-cn_topic_0118924572_p169821319568"></a><a name="zh-cn_topic_0118924572_p169821319568"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p1898161316565"><a name="zh-cn_topic_0118924572_p1898161316565"></a><a name="zh-cn_topic_0118924572_p1898161316565"></a>异常阙值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p1111331335618"><a name="zh-cn_topic_0118924572_p1111331335618"></a><a name="zh-cn_topic_0118924572_p1111331335618"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p13113113165614"><a name="zh-cn_topic_0118924572_p13113113165614"></a><a name="zh-cn_topic_0118924572_p13113113165614"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row19223121325615"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p91131813195616"><a name="zh-cn_topic_0118924572_p91131813195616"></a><a name="zh-cn_topic_0118924572_p91131813195616"></a>time_out</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p181131113155618"><a name="zh-cn_topic_0118924572_p181131113155618"></a><a name="zh-cn_topic_0118924572_p181131113155618"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p1511311311562"><a name="zh-cn_topic_0118924572_p1511311311562"></a><a name="zh-cn_topic_0118924572_p1511311311562"></a>超时时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p6113113175618"><a name="zh-cn_topic_0118924572_p6113113175618"></a><a name="zh-cn_topic_0118924572_p6113113175618"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p211318135568"><a name="zh-cn_topic_0118924572_p211318135568"></a><a name="zh-cn_topic_0118924572_p211318135568"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row175831246256"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p6583546354"><a name="zh-cn_topic_0118924572_p6583546354"></a><a name="zh-cn_topic_0118924572_p6583546354"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p165832460510"><a name="zh-cn_topic_0118924572_p165832460510"></a><a name="zh-cn_topic_0118924572_p165832460510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p958312467512"><a name="zh-cn_topic_0118924572_p958312467512"></a><a name="zh-cn_topic_0118924572_p958312467512"></a>间隔时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p258316465515"><a name="zh-cn_topic_0118924572_p258316465515"></a><a name="zh-cn_topic_0118924572_p258316465515"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p9583246452"><a name="zh-cn_topic_0118924572_p9583246452"></a><a name="zh-cn_topic_0118924572_p9583246452"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row4393833700"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p1439315331004"><a name="zh-cn_topic_0118924572_p1439315331004"></a><a name="zh-cn_topic_0118924572_p1439315331004"></a>http_code</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p83936331018"><a name="zh-cn_topic_0118924572_p83936331018"></a><a name="zh-cn_topic_0118924572_p83936331018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p123932033506"><a name="zh-cn_topic_0118924572_p123932033506"></a><a name="zh-cn_topic_0118924572_p123932033506"></a>成功状态码，仅当协议为http时生效</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p153934331014"><a name="zh-cn_topic_0118924572_p153934331014"></a><a name="zh-cn_topic_0118924572_p153934331014"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p1539303315019"><a name="zh-cn_topic_0118924572_p1539303315019"></a><a name="zh-cn_topic_0118924572_p1539303315019"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row53936368013"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p739310361703"><a name="zh-cn_topic_0118924572_p739310361703"></a><a name="zh-cn_topic_0118924572_p739310361703"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p539313361704"><a name="zh-cn_topic_0118924572_p539313361704"></a><a name="zh-cn_topic_0118924572_p539313361704"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p173933360010"><a name="zh-cn_topic_0118924572_p173933360010"></a><a name="zh-cn_topic_0118924572_p173933360010"></a>创建时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p93935369017"><a name="zh-cn_topic_0118924572_p93935369017"></a><a name="zh-cn_topic_0118924572_p93935369017"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p133931636002"><a name="zh-cn_topic_0118924572_p133931636002"></a><a name="zh-cn_topic_0118924572_p133931636002"></a>是</p>
</td>
</tr>
</tbody>
</table>

**表 3**  后端实例对象模型

<a name="zh-cn_topic_0118924572_table1432431421012"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924572_row14324114141017"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924572_p133241714171014"><a name="zh-cn_topic_0118924572_p133241714171014"></a><a name="zh-cn_topic_0118924572_p133241714171014"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924572_p1132420146104"><a name="zh-cn_topic_0118924572_p1132420146104"></a><a name="zh-cn_topic_0118924572_p1132420146104"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924572_p1324114101013"><a name="zh-cn_topic_0118924572_p1324114101013"></a><a name="zh-cn_topic_0118924572_p1324114101013"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924572_p183401214181015"><a name="zh-cn_topic_0118924572_p183401214181015"></a><a name="zh-cn_topic_0118924572_p183401214181015"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924572_p163401714101018"><a name="zh-cn_topic_0118924572_p163401714101018"></a><a name="zh-cn_topic_0118924572_p163401714101018"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924572_row6500215122212"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p192037153227"><a name="zh-cn_topic_0118924572_p192037153227"></a><a name="zh-cn_topic_0118924572_p192037153227"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p1320321582216"><a name="zh-cn_topic_0118924572_p1320321582216"></a><a name="zh-cn_topic_0118924572_p1320321582216"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p720321522212"><a name="zh-cn_topic_0118924572_p720321522212"></a><a name="zh-cn_topic_0118924572_p720321522212"></a>后端实例对象的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p182031415122213"><a name="zh-cn_topic_0118924572_p182031415122213"></a><a name="zh-cn_topic_0118924572_p182031415122213"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p18218101511226"><a name="zh-cn_topic_0118924572_p18218101511226"></a><a name="zh-cn_topic_0118924572_p18218101511226"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row850021515227"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p17218101510221"><a name="zh-cn_topic_0118924572_p17218101510221"></a><a name="zh-cn_topic_0118924572_p17218101510221"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p42186152226"><a name="zh-cn_topic_0118924572_p42186152226"></a><a name="zh-cn_topic_0118924572_p42186152226"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p1218151552213"><a name="zh-cn_topic_0118924572_p1218151552213"></a><a name="zh-cn_topic_0118924572_p1218151552213"></a>VPC通道的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p1521821512227"><a name="zh-cn_topic_0118924572_p1521821512227"></a><a name="zh-cn_topic_0118924572_p1521821512227"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p152183157227"><a name="zh-cn_topic_0118924572_p152183157227"></a><a name="zh-cn_topic_0118924572_p152183157227"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row195001615122214"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p18218161518224"><a name="zh-cn_topic_0118924572_p18218161518224"></a><a name="zh-cn_topic_0118924572_p18218161518224"></a>ext_vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p52342015172213"><a name="zh-cn_topic_0118924572_p52342015172213"></a><a name="zh-cn_topic_0118924572_p52342015172213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p135137169232"><a name="zh-cn_topic_0118924572_p135137169232"></a><a name="zh-cn_topic_0118924572_p135137169232"></a>后端实例对象的主机关联的VPC的编号</p>
<p id="zh-cn_topic_0118924572_p17270618242"><a name="zh-cn_topic_0118924572_p17270618242"></a><a name="zh-cn_topic_0118924572_p17270618242"></a><strong id="zh-cn_topic_0118924572_b15914018"><a name="zh-cn_topic_0118924572_b15914018"></a><a name="zh-cn_topic_0118924572_b15914018"></a>该字段已废弃</strong></p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p52341150224"><a name="zh-cn_topic_0118924572_p52341150224"></a><a name="zh-cn_topic_0118924572_p52341150224"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p3234101532216"><a name="zh-cn_topic_0118924572_p3234101532216"></a><a name="zh-cn_topic_0118924572_p3234101532216"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row35008152227"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p11234111519223"><a name="zh-cn_topic_0118924572_p11234111519223"></a><a name="zh-cn_topic_0118924572_p11234111519223"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p202505154226"><a name="zh-cn_topic_0118924572_p202505154226"></a><a name="zh-cn_topic_0118924572_p202505154226"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p4250161542220"><a name="zh-cn_topic_0118924572_p4250161542220"></a><a name="zh-cn_topic_0118924572_p4250161542220"></a>实例的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p1025021542220"><a name="zh-cn_topic_0118924572_p1025021542220"></a><a name="zh-cn_topic_0118924572_p1025021542220"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p625031582214"><a name="zh-cn_topic_0118924572_p625031582214"></a><a name="zh-cn_topic_0118924572_p625031582214"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row1550017155228"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p162500159226"><a name="zh-cn_topic_0118924572_p162500159226"></a><a name="zh-cn_topic_0118924572_p162500159226"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p1025051592220"><a name="zh-cn_topic_0118924572_p1025051592220"></a><a name="zh-cn_topic_0118924572_p1025051592220"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p52501815202219"><a name="zh-cn_topic_0118924572_p52501815202219"></a><a name="zh-cn_topic_0118924572_p52501815202219"></a>实例的名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p19266215142215"><a name="zh-cn_topic_0118924572_p19266215142215"></a><a name="zh-cn_topic_0118924572_p19266215142215"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p12661815182217"><a name="zh-cn_topic_0118924572_p12661815182217"></a><a name="zh-cn_topic_0118924572_p12661815182217"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row1500141516221"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p172661415102214"><a name="zh-cn_topic_0118924572_p172661415102214"></a><a name="zh-cn_topic_0118924572_p172661415102214"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p172661615172213"><a name="zh-cn_topic_0118924572_p172661615172213"></a><a name="zh-cn_topic_0118924572_p172661615172213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p92660153226"><a name="zh-cn_topic_0118924572_p92660153226"></a><a name="zh-cn_topic_0118924572_p92660153226"></a>后端实例对象的主机地址</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p82666158221"><a name="zh-cn_topic_0118924572_p82666158221"></a><a name="zh-cn_topic_0118924572_p82666158221"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p11281191514228"><a name="zh-cn_topic_0118924572_p11281191514228"></a><a name="zh-cn_topic_0118924572_p11281191514228"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row3500101572211"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p52817155227"><a name="zh-cn_topic_0118924572_p52817155227"></a><a name="zh-cn_topic_0118924572_p52817155227"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p52814156225"><a name="zh-cn_topic_0118924572_p52814156225"></a><a name="zh-cn_topic_0118924572_p52814156225"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p1428171517225"><a name="zh-cn_topic_0118924572_p1428171517225"></a><a name="zh-cn_topic_0118924572_p1428171517225"></a>后端实例对象状态</p>
<a name="zh-cn_topic_0118924572_ul19875172515297"></a><a name="zh-cn_topic_0118924572_ul19875172515297"></a><ul id="zh-cn_topic_0118924572_ul19875172515297"><li>1：正常</li><li>2：异常</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p142812152221"><a name="zh-cn_topic_0118924572_p142812152221"></a><a name="zh-cn_topic_0118924572_p142812152221"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p3281515102213"><a name="zh-cn_topic_0118924572_p3281515102213"></a><a name="zh-cn_topic_0118924572_p3281515102213"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row450061592220"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p12979153222"><a name="zh-cn_topic_0118924572_p12979153222"></a><a name="zh-cn_topic_0118924572_p12979153222"></a>weight</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p1229717155226"><a name="zh-cn_topic_0118924572_p1229717155226"></a><a name="zh-cn_topic_0118924572_p1229717155226"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p122971715152214"><a name="zh-cn_topic_0118924572_p122971715152214"></a><a name="zh-cn_topic_0118924572_p122971715152214"></a>权重值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p92977156226"><a name="zh-cn_topic_0118924572_p92977156226"></a><a name="zh-cn_topic_0118924572_p92977156226"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p62976156222"><a name="zh-cn_topic_0118924572_p62976156222"></a><a name="zh-cn_topic_0118924572_p62976156222"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924572_row950021515227"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924572_p163271815192212"><a name="zh-cn_topic_0118924572_p163271815192212"></a><a name="zh-cn_topic_0118924572_p163271815192212"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924572_p0327201516227"><a name="zh-cn_topic_0118924572_p0327201516227"></a><a name="zh-cn_topic_0118924572_p0327201516227"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924572_p16327191515222"><a name="zh-cn_topic_0118924572_p16327191515222"></a><a name="zh-cn_topic_0118924572_p16327191515222"></a>创建时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924572_p0327151532218"><a name="zh-cn_topic_0118924572_p0327151532218"></a><a name="zh-cn_topic_0118924572_p0327151532218"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924572_p332715151227"><a name="zh-cn_topic_0118924572_p332715151227"></a><a name="zh-cn_topic_0118924572_p332715151227"></a>是</p>
</td>
</tr>
</tbody>
</table>

