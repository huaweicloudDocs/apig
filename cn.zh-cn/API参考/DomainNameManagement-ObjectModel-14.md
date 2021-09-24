# 对象模型<a name="ZH-CN_TOPIC_0000001081976145"></a>

本节介绍自定义域名及证书的对象模型。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  域名对象模型

<a name="zh-cn_topic_0118924565_table49332581"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924565_row15637543"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924565_p58681484"><a name="zh-cn_topic_0118924565_p58681484"></a><a name="zh-cn_topic_0118924565_p58681484"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924565_p55579749"><a name="zh-cn_topic_0118924565_p55579749"></a><a name="zh-cn_topic_0118924565_p55579749"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924565_p5665819"><a name="zh-cn_topic_0118924565_p5665819"></a><a name="zh-cn_topic_0118924565_p5665819"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924565_p56278165"><a name="zh-cn_topic_0118924565_p56278165"></a><a name="zh-cn_topic_0118924565_p56278165"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924565_p62237499"><a name="zh-cn_topic_0118924565_p62237499"></a><a name="zh-cn_topic_0118924565_p62237499"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924565_row8072695"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p49908526"><a name="zh-cn_topic_0118924565_p49908526"></a><a name="zh-cn_topic_0118924565_p49908526"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p16058826"><a name="zh-cn_topic_0118924565_p16058826"></a><a name="zh-cn_topic_0118924565_p16058826"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p25696563"><a name="zh-cn_topic_0118924565_p25696563"></a><a name="zh-cn_topic_0118924565_p25696563"></a>域名的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p1046864"><a name="zh-cn_topic_0118924565_p1046864"></a><a name="zh-cn_topic_0118924565_p1046864"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p17687178"><a name="zh-cn_topic_0118924565_p17687178"></a><a name="zh-cn_topic_0118924565_p17687178"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924565_row24966877"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p9051148"><a name="zh-cn_topic_0118924565_p9051148"></a><a name="zh-cn_topic_0118924565_p9051148"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p62054412"><a name="zh-cn_topic_0118924565_p62054412"></a><a name="zh-cn_topic_0118924565_p62054412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p60351493"><a name="zh-cn_topic_0118924565_p60351493"></a><a name="zh-cn_topic_0118924565_p60351493"></a>自定义域名</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p56632734"><a name="zh-cn_topic_0118924565_p56632734"></a><a name="zh-cn_topic_0118924565_p56632734"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p23848703"><a name="zh-cn_topic_0118924565_p23848703"></a><a name="zh-cn_topic_0118924565_p23848703"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924565_row13311738"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p4509019"><a name="zh-cn_topic_0118924565_p4509019"></a><a name="zh-cn_topic_0118924565_p4509019"></a>cname_status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p29686297"><a name="zh-cn_topic_0118924565_p29686297"></a><a name="zh-cn_topic_0118924565_p29686297"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p55779867"><a name="zh-cn_topic_0118924565_p55779867"></a><a name="zh-cn_topic_0118924565_p55779867"></a>cname解析状态</p>
<a name="zh-cn_topic_0118924565_ul53721145134416"></a><a name="zh-cn_topic_0118924565_ul53721145134416"></a><ul id="zh-cn_topic_0118924565_ul53721145134416"><li>1 未解析</li><li>2 解析中</li><li>3 解析成功</li><li>4 解析失败</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p21875402"><a name="zh-cn_topic_0118924565_p21875402"></a><a name="zh-cn_topic_0118924565_p21875402"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p27077133"><a name="zh-cn_topic_0118924565_p27077133"></a><a name="zh-cn_topic_0118924565_p27077133"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924565_row42367610"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p9224375"><a name="zh-cn_topic_0118924565_p9224375"></a><a name="zh-cn_topic_0118924565_p9224375"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p8976892"><a name="zh-cn_topic_0118924565_p8976892"></a><a name="zh-cn_topic_0118924565_p8976892"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p79993152715"><a name="zh-cn_topic_0118924565_p79993152715"></a><a name="zh-cn_topic_0118924565_p79993152715"></a>证书的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p15296911"><a name="zh-cn_topic_0118924565_p15296911"></a><a name="zh-cn_topic_0118924565_p15296911"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p31090241"><a name="zh-cn_topic_0118924565_p31090241"></a><a name="zh-cn_topic_0118924565_p31090241"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924565_row11376719"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p49099023"><a name="zh-cn_topic_0118924565_p49099023"></a><a name="zh-cn_topic_0118924565_p49099023"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p17597936"><a name="zh-cn_topic_0118924565_p17597936"></a><a name="zh-cn_topic_0118924565_p17597936"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p16681305"><a name="zh-cn_topic_0118924565_p16681305"></a><a name="zh-cn_topic_0118924565_p16681305"></a>API分组的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p13967064"><a name="zh-cn_topic_0118924565_p13967064"></a><a name="zh-cn_topic_0118924565_p13967064"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p57590436"><a name="zh-cn_topic_0118924565_p57590436"></a><a name="zh-cn_topic_0118924565_p57590436"></a>是</p>
</td>
</tr>
</tbody>
</table>

**表 2**  证书对象模型

<a name="zh-cn_topic_0118924565_table41340048"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924565_row37775636"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118924565_p39927684"><a name="zh-cn_topic_0118924565_p39927684"></a><a name="zh-cn_topic_0118924565_p39927684"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118924565_p12916952"><a name="zh-cn_topic_0118924565_p12916952"></a><a name="zh-cn_topic_0118924565_p12916952"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118924565_p39640185"><a name="zh-cn_topic_0118924565_p39640185"></a><a name="zh-cn_topic_0118924565_p39640185"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118924565_p56738382"><a name="zh-cn_topic_0118924565_p56738382"></a><a name="zh-cn_topic_0118924565_p56738382"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118924565_p32406207"><a name="zh-cn_topic_0118924565_p32406207"></a><a name="zh-cn_topic_0118924565_p32406207"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924565_row7657142"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p16248728"><a name="zh-cn_topic_0118924565_p16248728"></a><a name="zh-cn_topic_0118924565_p16248728"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p41078607"><a name="zh-cn_topic_0118924565_p41078607"></a><a name="zh-cn_topic_0118924565_p41078607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p39032899"><a name="zh-cn_topic_0118924565_p39032899"></a><a name="zh-cn_topic_0118924565_p39032899"></a>证书的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p7548251"><a name="zh-cn_topic_0118924565_p7548251"></a><a name="zh-cn_topic_0118924565_p7548251"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p7428608"><a name="zh-cn_topic_0118924565_p7428608"></a><a name="zh-cn_topic_0118924565_p7428608"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924565_row66857474"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p46746341"><a name="zh-cn_topic_0118924565_p46746341"></a><a name="zh-cn_topic_0118924565_p46746341"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p28357256"><a name="zh-cn_topic_0118924565_p28357256"></a><a name="zh-cn_topic_0118924565_p28357256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p11219768"><a name="zh-cn_topic_0118924565_p11219768"></a><a name="zh-cn_topic_0118924565_p11219768"></a>证书的名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p59038887"><a name="zh-cn_topic_0118924565_p59038887"></a><a name="zh-cn_topic_0118924565_p59038887"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p17420548"><a name="zh-cn_topic_0118924565_p17420548"></a><a name="zh-cn_topic_0118924565_p17420548"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924565_row22567210"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p16004721"><a name="zh-cn_topic_0118924565_p16004721"></a><a name="zh-cn_topic_0118924565_p16004721"></a>context</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p21314016"><a name="zh-cn_topic_0118924565_p21314016"></a><a name="zh-cn_topic_0118924565_p21314016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p48713760"><a name="zh-cn_topic_0118924565_p48713760"></a><a name="zh-cn_topic_0118924565_p48713760"></a>证书的内容</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p53500505"><a name="zh-cn_topic_0118924565_p53500505"></a><a name="zh-cn_topic_0118924565_p53500505"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p38573618"><a name="zh-cn_topic_0118924565_p38573618"></a><a name="zh-cn_topic_0118924565_p38573618"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924565_row11618242"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118924565_p1553518"><a name="zh-cn_topic_0118924565_p1553518"></a><a name="zh-cn_topic_0118924565_p1553518"></a>private_key</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118924565_p58726159"><a name="zh-cn_topic_0118924565_p58726159"></a><a name="zh-cn_topic_0118924565_p58726159"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118924565_p59198477"><a name="zh-cn_topic_0118924565_p59198477"></a><a name="zh-cn_topic_0118924565_p59198477"></a>证书的私钥</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118924565_p30347343"><a name="zh-cn_topic_0118924565_p30347343"></a><a name="zh-cn_topic_0118924565_p30347343"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118924565_p42215742"><a name="zh-cn_topic_0118924565_p42215742"></a><a name="zh-cn_topic_0118924565_p42215742"></a>是</p>
</td>
</tr>
</tbody>
</table>

