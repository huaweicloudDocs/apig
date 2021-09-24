# 对象模型<a name="ZH-CN_TOPIC_0000001082221171"></a>

本节介绍API及后端服务的对象模型。

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  API对象模型

<a name="zh-cn_topic_0118921492_table49332581"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row15637543"><th class="cellrowborder" valign="top" width="20.262026202620262%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p58681484"><a name="zh-cn_topic_0118921492_p58681484"></a><a name="zh-cn_topic_0118921492_p58681484"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.12181218121812%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p55579749"><a name="zh-cn_topic_0118921492_p55579749"></a><a name="zh-cn_topic_0118921492_p55579749"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.29332933293329%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p5665819"><a name="zh-cn_topic_0118921492_p5665819"></a><a name="zh-cn_topic_0118921492_p5665819"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.211721172117212%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p56278165"><a name="zh-cn_topic_0118921492_p56278165"></a><a name="zh-cn_topic_0118921492_p56278165"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p62237499"><a name="zh-cn_topic_0118921492_p62237499"></a><a name="zh-cn_topic_0118921492_p62237499"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row8072695"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p49908526"><a name="zh-cn_topic_0118921492_p49908526"></a><a name="zh-cn_topic_0118921492_p49908526"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p16058826"><a name="zh-cn_topic_0118921492_p16058826"></a><a name="zh-cn_topic_0118921492_p16058826"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p25696563"><a name="zh-cn_topic_0118921492_p25696563"></a><a name="zh-cn_topic_0118921492_p25696563"></a>API的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1046864"><a name="zh-cn_topic_0118921492_p1046864"></a><a name="zh-cn_topic_0118921492_p1046864"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p17687178"><a name="zh-cn_topic_0118921492_p17687178"></a><a name="zh-cn_topic_0118921492_p17687178"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row24966877"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p9051148"><a name="zh-cn_topic_0118921492_p9051148"></a><a name="zh-cn_topic_0118921492_p9051148"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p62054412"><a name="zh-cn_topic_0118921492_p62054412"></a><a name="zh-cn_topic_0118921492_p62054412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p60351493"><a name="zh-cn_topic_0118921492_p60351493"></a><a name="zh-cn_topic_0118921492_p60351493"></a>API的名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p56632734"><a name="zh-cn_topic_0118921492_p56632734"></a><a name="zh-cn_topic_0118921492_p56632734"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p23848703"><a name="zh-cn_topic_0118921492_p23848703"></a><a name="zh-cn_topic_0118921492_p23848703"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row13311738"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p4509019"><a name="zh-cn_topic_0118921492_p4509019"></a><a name="zh-cn_topic_0118921492_p4509019"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p29686297"><a name="zh-cn_topic_0118921492_p29686297"></a><a name="zh-cn_topic_0118921492_p29686297"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p55779867"><a name="zh-cn_topic_0118921492_p55779867"></a><a name="zh-cn_topic_0118921492_p55779867"></a>API所属分组的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p21875402"><a name="zh-cn_topic_0118921492_p21875402"></a><a name="zh-cn_topic_0118921492_p21875402"></a>CR</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p27077133"><a name="zh-cn_topic_0118921492_p27077133"></a><a name="zh-cn_topic_0118921492_p27077133"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row42367610"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p9224375"><a name="zh-cn_topic_0118921492_p9224375"></a><a name="zh-cn_topic_0118921492_p9224375"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p8976892"><a name="zh-cn_topic_0118921492_p8976892"></a><a name="zh-cn_topic_0118921492_p8976892"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p56039666"><a name="zh-cn_topic_0118921492_p56039666"></a><a name="zh-cn_topic_0118921492_p56039666"></a>API的类型：</p>
<a name="zh-cn_topic_0118921492_ul34594951"></a><a name="zh-cn_topic_0118921492_ul34594951"></a><ul id="zh-cn_topic_0118921492_ul34594951"><li>1：公有API</li><li>2：私有API</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p15296911"><a name="zh-cn_topic_0118921492_p15296911"></a><a name="zh-cn_topic_0118921492_p15296911"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p31090241"><a name="zh-cn_topic_0118921492_p31090241"></a><a name="zh-cn_topic_0118921492_p31090241"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row11376719"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p49099023"><a name="zh-cn_topic_0118921492_p49099023"></a><a name="zh-cn_topic_0118921492_p49099023"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p17597936"><a name="zh-cn_topic_0118921492_p17597936"></a><a name="zh-cn_topic_0118921492_p17597936"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p16146713"><a name="zh-cn_topic_0118921492_p16146713"></a><a name="zh-cn_topic_0118921492_p16146713"></a>API的状态：</p>
<a name="zh-cn_topic_0118921492_ul11102697"></a><a name="zh-cn_topic_0118921492_ul11102697"></a><ul id="zh-cn_topic_0118921492_ul11102697"><li>1：启用</li><li>2：禁用</li><li>3：已删除</li></ul>
<p id="zh-cn_topic_0118921492_p31679640"><a name="zh-cn_topic_0118921492_p31679640"></a><a name="zh-cn_topic_0118921492_p31679640"></a>默认1</p>
<p id="zh-cn_topic_0118921492_p16681305"><a name="zh-cn_topic_0118921492_p16681305"></a><a name="zh-cn_topic_0118921492_p16681305"></a><strong id="zh-cn_topic_0118921492_b15914018"><a name="zh-cn_topic_0118921492_b15914018"></a><a name="zh-cn_topic_0118921492_b15914018"></a>该字段已废弃</strong></p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p13967064"><a name="zh-cn_topic_0118921492_p13967064"></a><a name="zh-cn_topic_0118921492_p13967064"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p57590436"><a name="zh-cn_topic_0118921492_p57590436"></a><a name="zh-cn_topic_0118921492_p57590436"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row48551876"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p40387913"><a name="zh-cn_topic_0118921492_p40387913"></a><a name="zh-cn_topic_0118921492_p40387913"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p50195543"><a name="zh-cn_topic_0118921492_p50195543"></a><a name="zh-cn_topic_0118921492_p50195543"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p39307157"><a name="zh-cn_topic_0118921492_p39307157"></a><a name="zh-cn_topic_0118921492_p39307157"></a>API的版本</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p29763115"><a name="zh-cn_topic_0118921492_p29763115"></a><a name="zh-cn_topic_0118921492_p29763115"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p62002114"><a name="zh-cn_topic_0118921492_p62002114"></a><a name="zh-cn_topic_0118921492_p62002114"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row21148117"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p35275920"><a name="zh-cn_topic_0118921492_p35275920"></a><a name="zh-cn_topic_0118921492_p35275920"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p38777247"><a name="zh-cn_topic_0118921492_p38777247"></a><a name="zh-cn_topic_0118921492_p38777247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p53949291"><a name="zh-cn_topic_0118921492_p53949291"></a><a name="zh-cn_topic_0118921492_p53949291"></a>API的访问协议</p>
<a name="zh-cn_topic_0118921492_ul15781571"></a><a name="zh-cn_topic_0118921492_ul15781571"></a><ul id="zh-cn_topic_0118921492_ul15781571"><li>HTTP</li><li>HTTPS</li><li>BOTH：同时支持HTTP和HTTPS</li></ul>
<p id="zh-cn_topic_0118921492_p12301512"><a name="zh-cn_topic_0118921492_p12301512"></a><a name="zh-cn_topic_0118921492_p12301512"></a>默认：HTTPS</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p56898454"><a name="zh-cn_topic_0118921492_p56898454"></a><a name="zh-cn_topic_0118921492_p56898454"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p45372072"><a name="zh-cn_topic_0118921492_p45372072"></a><a name="zh-cn_topic_0118921492_p45372072"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row5695471"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p58679970"><a name="zh-cn_topic_0118921492_p58679970"></a><a name="zh-cn_topic_0118921492_p58679970"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p55457167"><a name="zh-cn_topic_0118921492_p55457167"></a><a name="zh-cn_topic_0118921492_p55457167"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p62845532"><a name="zh-cn_topic_0118921492_p62845532"></a><a name="zh-cn_topic_0118921492_p62845532"></a>API的访问方式</p>
<a name="zh-cn_topic_0118921492_ul28738878"></a><a name="zh-cn_topic_0118921492_ul28738878"></a><ul id="zh-cn_topic_0118921492_ul28738878"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p43849566"><a name="zh-cn_topic_0118921492_p43849566"></a><a name="zh-cn_topic_0118921492_p43849566"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p62153973"><a name="zh-cn_topic_0118921492_p62153973"></a><a name="zh-cn_topic_0118921492_p62153973"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row22514852"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p11763733"><a name="zh-cn_topic_0118921492_p11763733"></a><a name="zh-cn_topic_0118921492_p11763733"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p13338318"><a name="zh-cn_topic_0118921492_p13338318"></a><a name="zh-cn_topic_0118921492_p13338318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p6662008"><a name="zh-cn_topic_0118921492_p6662008"></a><a name="zh-cn_topic_0118921492_p6662008"></a>API的访问地址，不含域名、端口号、请求协议等，是URI</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p2751803"><a name="zh-cn_topic_0118921492_p2751803"></a><a name="zh-cn_topic_0118921492_p2751803"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p21569470"><a name="zh-cn_topic_0118921492_p21569470"></a><a name="zh-cn_topic_0118921492_p21569470"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row59907503"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p20669557"><a name="zh-cn_topic_0118921492_p20669557"></a><a name="zh-cn_topic_0118921492_p20669557"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p63621457"><a name="zh-cn_topic_0118921492_p63621457"></a><a name="zh-cn_topic_0118921492_p63621457"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p53064360"><a name="zh-cn_topic_0118921492_p53064360"></a><a name="zh-cn_topic_0118921492_p53064360"></a>API的认证方式</p>
<a name="zh-cn_topic_0118921492_ul7817198"></a><a name="zh-cn_topic_0118921492_ul7817198"></a><ul id="zh-cn_topic_0118921492_ul7817198"><li>NONE：无认证</li><li>APP：APP认证</li><li>IAM：IAM认证</li><li>AUTHORIZER：自定义认证</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p23003434"><a name="zh-cn_topic_0118921492_p23003434"></a><a name="zh-cn_topic_0118921492_p23003434"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p51338884"><a name="zh-cn_topic_0118921492_p51338884"></a><a name="zh-cn_topic_0118921492_p51338884"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row196391729111915"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p18639182918193"><a name="zh-cn_topic_0118921492_p18639182918193"></a><a name="zh-cn_topic_0118921492_p18639182918193"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p86488246201"><a name="zh-cn_topic_0118921492_p86488246201"></a><a name="zh-cn_topic_0118921492_p86488246201"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p17639829131912"><a name="zh-cn_topic_0118921492_p17639829131912"></a><a name="zh-cn_topic_0118921492_p17639829131912"></a>前端自定义认证对象的ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1538414416208"><a name="zh-cn_topic_0118921492_p1538414416208"></a><a name="zh-cn_topic_0118921492_p1538414416208"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1618134152219"><a name="zh-cn_topic_0118921492_p1618134152219"></a><a name="zh-cn_topic_0118921492_p1618134152219"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row59396775"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p46409462"><a name="zh-cn_topic_0118921492_p46409462"></a><a name="zh-cn_topic_0118921492_p46409462"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1070102"><a name="zh-cn_topic_0118921492_p1070102"></a><a name="zh-cn_topic_0118921492_p1070102"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p19569455"><a name="zh-cn_topic_0118921492_p19569455"></a><a name="zh-cn_topic_0118921492_p19569455"></a>API的路由匹配方式：</p>
<a name="zh-cn_topic_0118921492_ul41907368"></a><a name="zh-cn_topic_0118921492_ul41907368"></a><ul id="zh-cn_topic_0118921492_ul41907368"><li>SWA：前缀匹配</li><li>NORMAL：正常匹配</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p9225652"><a name="zh-cn_topic_0118921492_p9225652"></a><a name="zh-cn_topic_0118921492_p9225652"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p9080373"><a name="zh-cn_topic_0118921492_p9080373"></a><a name="zh-cn_topic_0118921492_p9080373"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row14614501"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p42923952"><a name="zh-cn_topic_0118921492_p42923952"></a><a name="zh-cn_topic_0118921492_p42923952"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p54288100"><a name="zh-cn_topic_0118921492_p54288100"></a><a name="zh-cn_topic_0118921492_p54288100"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p35259943"><a name="zh-cn_topic_0118921492_p35259943"></a><a name="zh-cn_topic_0118921492_p35259943"></a>是否需要编排</p>
<a name="zh-cn_topic_0118921492_ul48904039"></a><a name="zh-cn_topic_0118921492_ul48904039"></a><ul id="zh-cn_topic_0118921492_ul48904039"><li>1：是</li><li>2：否</li></ul>
<p id="zh-cn_topic_0118921492_p9572132612592"><a name="zh-cn_topic_0118921492_p9572132612592"></a><a name="zh-cn_topic_0118921492_p9572132612592"></a>目前默认为：2</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p40216166"><a name="zh-cn_topic_0118921492_p40216166"></a><a name="zh-cn_topic_0118921492_p40216166"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p36284028"><a name="zh-cn_topic_0118921492_p36284028"></a><a name="zh-cn_topic_0118921492_p36284028"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row58120801"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p10164418"><a name="zh-cn_topic_0118921492_p10164418"></a><a name="zh-cn_topic_0118921492_p10164418"></a>backend_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p18011561"><a name="zh-cn_topic_0118921492_p18011561"></a><a name="zh-cn_topic_0118921492_p18011561"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p49650299"><a name="zh-cn_topic_0118921492_p49650299"></a><a name="zh-cn_topic_0118921492_p49650299"></a>后端服务类型：</p>
<a name="zh-cn_topic_0118921492_ul44199513"></a><a name="zh-cn_topic_0118921492_ul44199513"></a><ul id="zh-cn_topic_0118921492_ul44199513"><li>HTTP：web后端</li><li>FUNCTION：函数服务</li><li>MOCK： MOCK</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p6225422"><a name="zh-cn_topic_0118921492_p6225422"></a><a name="zh-cn_topic_0118921492_p6225422"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p34497187"><a name="zh-cn_topic_0118921492_p34497187"></a><a name="zh-cn_topic_0118921492_p34497187"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row42039229"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p49734416"><a name="zh-cn_topic_0118921492_p49734416"></a><a name="zh-cn_topic_0118921492_p49734416"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1955875"><a name="zh-cn_topic_0118921492_p1955875"></a><a name="zh-cn_topic_0118921492_p1955875"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p24208158"><a name="zh-cn_topic_0118921492_p24208158"></a><a name="zh-cn_topic_0118921492_p24208158"></a>API注册时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p14703786"><a name="zh-cn_topic_0118921492_p14703786"></a><a name="zh-cn_topic_0118921492_p14703786"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p50156014"><a name="zh-cn_topic_0118921492_p50156014"></a><a name="zh-cn_topic_0118921492_p50156014"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row48750949"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p56512817"><a name="zh-cn_topic_0118921492_p56512817"></a><a name="zh-cn_topic_0118921492_p56512817"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p14135498"><a name="zh-cn_topic_0118921492_p14135498"></a><a name="zh-cn_topic_0118921492_p14135498"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p4124695"><a name="zh-cn_topic_0118921492_p4124695"></a><a name="zh-cn_topic_0118921492_p4124695"></a>API修改时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p65664897"><a name="zh-cn_topic_0118921492_p65664897"></a><a name="zh-cn_topic_0118921492_p65664897"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p17256431"><a name="zh-cn_topic_0118921492_p17256431"></a><a name="zh-cn_topic_0118921492_p17256431"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row21090155"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p30581019"><a name="zh-cn_topic_0118921492_p30581019"></a><a name="zh-cn_topic_0118921492_p30581019"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p61143492"><a name="zh-cn_topic_0118921492_p61143492"></a><a name="zh-cn_topic_0118921492_p61143492"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p53675789"><a name="zh-cn_topic_0118921492_p53675789"></a><a name="zh-cn_topic_0118921492_p53675789"></a>API描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p52771614"><a name="zh-cn_topic_0118921492_p52771614"></a><a name="zh-cn_topic_0118921492_p52771614"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p46642336"><a name="zh-cn_topic_0118921492_p46642336"></a><a name="zh-cn_topic_0118921492_p46642336"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row14125194914"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p94155104919"><a name="zh-cn_topic_0118921492_p94155104919"></a><a name="zh-cn_topic_0118921492_p94155104919"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1741105194920"><a name="zh-cn_topic_0118921492_p1741105194920"></a><a name="zh-cn_topic_0118921492_p1741105194920"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p34145194914"><a name="zh-cn_topic_0118921492_p34145194914"></a><a name="zh-cn_topic_0118921492_p34145194914"></a>API标签</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p24110514492"><a name="zh-cn_topic_0118921492_p24110514492"></a><a name="zh-cn_topic_0118921492_p24110514492"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p16411651184912"><a name="zh-cn_topic_0118921492_p16411651184912"></a><a name="zh-cn_topic_0118921492_p16411651184912"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row32138102505"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1221331035013"><a name="zh-cn_topic_0118921492_p1221331035013"></a><a name="zh-cn_topic_0118921492_p1221331035013"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p18213101075013"><a name="zh-cn_topic_0118921492_p18213101075013"></a><a name="zh-cn_topic_0118921492_p18213101075013"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p7213201015015"><a name="zh-cn_topic_0118921492_p7213201015015"></a><a name="zh-cn_topic_0118921492_p7213201015015"></a>是否支持跨域</p>
<a name="zh-cn_topic_0118921492_ul38673529507"></a><a name="zh-cn_topic_0118921492_ul38673529507"></a><ul id="zh-cn_topic_0118921492_ul38673529507"><li>TRUE  支持</li><li>FALSE   不支持</li></ul>
<p id="zh-cn_topic_0118921492_p17882165245011"><a name="zh-cn_topic_0118921492_p17882165245011"></a><a name="zh-cn_topic_0118921492_p17882165245011"></a>默认：FALSE</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p6213151015013"><a name="zh-cn_topic_0118921492_p6213151015013"></a><a name="zh-cn_topic_0118921492_p6213151015013"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p16213010145019"><a name="zh-cn_topic_0118921492_p16213010145019"></a><a name="zh-cn_topic_0118921492_p16213010145019"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row6296113117146"><td class="cellrowborder" valign="top" width="20.262026202620262%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1388814535919"><a name="zh-cn_topic_0118921492_p1388814535919"></a><a name="zh-cn_topic_0118921492_p1388814535919"></a>response_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.12181218121812%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p5888345115911"><a name="zh-cn_topic_0118921492_p5888345115911"></a><a name="zh-cn_topic_0118921492_p5888345115911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.29332933293329%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p14331422017"><a name="zh-cn_topic_0118921492_p14331422017"></a><a name="zh-cn_topic_0118921492_p14331422017"></a>分组自定义响应ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.211721172117212%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p6296183121418"><a name="zh-cn_topic_0118921492_p6296183121418"></a><a name="zh-cn_topic_0118921492_p6296183121418"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1229616314145"><a name="zh-cn_topic_0118921492_p1229616314145"></a><a name="zh-cn_topic_0118921492_p1229616314145"></a>否</p>
</td>
</tr>
</tbody>
</table>

**表 2**  web后端对象模型

<a name="zh-cn_topic_0118921492_table41340048"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row37775636"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p39927684"><a name="zh-cn_topic_0118921492_p39927684"></a><a name="zh-cn_topic_0118921492_p39927684"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p12916952"><a name="zh-cn_topic_0118921492_p12916952"></a><a name="zh-cn_topic_0118921492_p12916952"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p39640185"><a name="zh-cn_topic_0118921492_p39640185"></a><a name="zh-cn_topic_0118921492_p39640185"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p56738382"><a name="zh-cn_topic_0118921492_p56738382"></a><a name="zh-cn_topic_0118921492_p56738382"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p32406207"><a name="zh-cn_topic_0118921492_p32406207"></a><a name="zh-cn_topic_0118921492_p32406207"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row7657142"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p16248728"><a name="zh-cn_topic_0118921492_p16248728"></a><a name="zh-cn_topic_0118921492_p16248728"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p41078607"><a name="zh-cn_topic_0118921492_p41078607"></a><a name="zh-cn_topic_0118921492_p41078607"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p39032899"><a name="zh-cn_topic_0118921492_p39032899"></a><a name="zh-cn_topic_0118921492_p39032899"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p7548251"><a name="zh-cn_topic_0118921492_p7548251"></a><a name="zh-cn_topic_0118921492_p7548251"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p7428608"><a name="zh-cn_topic_0118921492_p7428608"></a><a name="zh-cn_topic_0118921492_p7428608"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row66857474"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p46746341"><a name="zh-cn_topic_0118921492_p46746341"></a><a name="zh-cn_topic_0118921492_p46746341"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p28357256"><a name="zh-cn_topic_0118921492_p28357256"></a><a name="zh-cn_topic_0118921492_p28357256"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p15236371"><a name="zh-cn_topic_0118921492_p15236371"></a><a name="zh-cn_topic_0118921492_p15236371"></a>状态：</p>
<a name="zh-cn_topic_0118921492_ul2909615"></a><a name="zh-cn_topic_0118921492_ul2909615"></a><ul id="zh-cn_topic_0118921492_ul2909615"><li>1：启用</li><li>2：禁用</li><li>3：已删除</li></ul>
<p id="zh-cn_topic_0118921492_p31072802"><a name="zh-cn_topic_0118921492_p31072802"></a><a name="zh-cn_topic_0118921492_p31072802"></a>默认1</p>
<p id="zh-cn_topic_0118921492_p11219768"><a name="zh-cn_topic_0118921492_p11219768"></a><a name="zh-cn_topic_0118921492_p11219768"></a><strong id="zh-cn_topic_0118921492_b33869054"><a name="zh-cn_topic_0118921492_b33869054"></a><a name="zh-cn_topic_0118921492_b33869054"></a>该字段已废弃</strong></p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p59038887"><a name="zh-cn_topic_0118921492_p59038887"></a><a name="zh-cn_topic_0118921492_p59038887"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p17420548"><a name="zh-cn_topic_0118921492_p17420548"></a><a name="zh-cn_topic_0118921492_p17420548"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row22567210"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p16004721"><a name="zh-cn_topic_0118921492_p16004721"></a><a name="zh-cn_topic_0118921492_p16004721"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p21314016"><a name="zh-cn_topic_0118921492_p21314016"></a><a name="zh-cn_topic_0118921492_p21314016"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p48713760"><a name="zh-cn_topic_0118921492_p48713760"></a><a name="zh-cn_topic_0118921492_p48713760"></a>版本</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p53500505"><a name="zh-cn_topic_0118921492_p53500505"></a><a name="zh-cn_topic_0118921492_p53500505"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p38573618"><a name="zh-cn_topic_0118921492_p38573618"></a><a name="zh-cn_topic_0118921492_p38573618"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row11618242"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1553518"><a name="zh-cn_topic_0118921492_p1553518"></a><a name="zh-cn_topic_0118921492_p1553518"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p58726159"><a name="zh-cn_topic_0118921492_p58726159"></a><a name="zh-cn_topic_0118921492_p58726159"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1779183781019"><a name="zh-cn_topic_0118921492_p1779183781019"></a><a name="zh-cn_topic_0118921492_p1779183781019"></a>后端endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p30347343"><a name="zh-cn_topic_0118921492_p30347343"></a><a name="zh-cn_topic_0118921492_p30347343"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p42215742"><a name="zh-cn_topic_0118921492_p42215742"></a><a name="zh-cn_topic_0118921492_p42215742"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row44397361"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p39416526"><a name="zh-cn_topic_0118921492_p39416526"></a><a name="zh-cn_topic_0118921492_p39416526"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p38622027"><a name="zh-cn_topic_0118921492_p38622027"></a><a name="zh-cn_topic_0118921492_p38622027"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p41376464"><a name="zh-cn_topic_0118921492_p41376464"></a><a name="zh-cn_topic_0118921492_p41376464"></a>访问协议</p>
<a name="zh-cn_topic_0118921492_ul36843862"></a><a name="zh-cn_topic_0118921492_ul36843862"></a><ul id="zh-cn_topic_0118921492_ul36843862"><li>HTTP</li><li>HTTPS</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p6450876"><a name="zh-cn_topic_0118921492_p6450876"></a><a name="zh-cn_topic_0118921492_p6450876"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p52758979"><a name="zh-cn_topic_0118921492_p52758979"></a><a name="zh-cn_topic_0118921492_p52758979"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row5068763"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p7916643"><a name="zh-cn_topic_0118921492_p7916643"></a><a name="zh-cn_topic_0118921492_p7916643"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p37268323"><a name="zh-cn_topic_0118921492_p37268323"></a><a name="zh-cn_topic_0118921492_p37268323"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p65944196"><a name="zh-cn_topic_0118921492_p65944196"></a><a name="zh-cn_topic_0118921492_p65944196"></a>请求方式</p>
<a name="zh-cn_topic_0118921492_ul56626856"></a><a name="zh-cn_topic_0118921492_ul56626856"></a><ul id="zh-cn_topic_0118921492_ul56626856"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p48177484"><a name="zh-cn_topic_0118921492_p48177484"></a><a name="zh-cn_topic_0118921492_p48177484"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p10062168"><a name="zh-cn_topic_0118921492_p10062168"></a><a name="zh-cn_topic_0118921492_p10062168"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row23450648"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p20454365"><a name="zh-cn_topic_0118921492_p20454365"></a><a name="zh-cn_topic_0118921492_p20454365"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p46190891"><a name="zh-cn_topic_0118921492_p46190891"></a><a name="zh-cn_topic_0118921492_p46190891"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p50474665"><a name="zh-cn_topic_0118921492_p50474665"></a><a name="zh-cn_topic_0118921492_p50474665"></a>访问地址，是URI</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p61916031"><a name="zh-cn_topic_0118921492_p61916031"></a><a name="zh-cn_topic_0118921492_p61916031"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p49142614"><a name="zh-cn_topic_0118921492_p49142614"></a><a name="zh-cn_topic_0118921492_p49142614"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row39630345"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p55941380"><a name="zh-cn_topic_0118921492_p55941380"></a><a name="zh-cn_topic_0118921492_p55941380"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p34957907"><a name="zh-cn_topic_0118921492_p34957907"></a><a name="zh-cn_topic_0118921492_p34957907"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p13018207"><a name="zh-cn_topic_0118921492_p13018207"></a><a name="zh-cn_topic_0118921492_p13018207"></a>超时时间，单位：毫秒（1-60000）</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p47841807"><a name="zh-cn_topic_0118921492_p47841807"></a><a name="zh-cn_topic_0118921492_p47841807"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p49981131"><a name="zh-cn_topic_0118921492_p49981131"></a><a name="zh-cn_topic_0118921492_p49981131"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row47177002"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p63240804"><a name="zh-cn_topic_0118921492_p63240804"></a><a name="zh-cn_topic_0118921492_p63240804"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p22231519"><a name="zh-cn_topic_0118921492_p22231519"></a><a name="zh-cn_topic_0118921492_p22231519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p55922627"><a name="zh-cn_topic_0118921492_p55922627"></a><a name="zh-cn_topic_0118921492_p55922627"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p33438902"><a name="zh-cn_topic_0118921492_p33438902"></a><a name="zh-cn_topic_0118921492_p33438902"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p24196579"><a name="zh-cn_topic_0118921492_p24196579"></a><a name="zh-cn_topic_0118921492_p24196579"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row16442622"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p56783986"><a name="zh-cn_topic_0118921492_p56783986"></a><a name="zh-cn_topic_0118921492_p56783986"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p36100147"><a name="zh-cn_topic_0118921492_p36100147"></a><a name="zh-cn_topic_0118921492_p36100147"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p38430760"><a name="zh-cn_topic_0118921492_p38430760"></a><a name="zh-cn_topic_0118921492_p38430760"></a>注册时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p25883833"><a name="zh-cn_topic_0118921492_p25883833"></a><a name="zh-cn_topic_0118921492_p25883833"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p16215760"><a name="zh-cn_topic_0118921492_p16215760"></a><a name="zh-cn_topic_0118921492_p16215760"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row11724112"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p10129000"><a name="zh-cn_topic_0118921492_p10129000"></a><a name="zh-cn_topic_0118921492_p10129000"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p15142648"><a name="zh-cn_topic_0118921492_p15142648"></a><a name="zh-cn_topic_0118921492_p15142648"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p18594985"><a name="zh-cn_topic_0118921492_p18594985"></a><a name="zh-cn_topic_0118921492_p18594985"></a>修改时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p29798818"><a name="zh-cn_topic_0118921492_p29798818"></a><a name="zh-cn_topic_0118921492_p29798818"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p64894092"><a name="zh-cn_topic_0118921492_p64894092"></a><a name="zh-cn_topic_0118921492_p64894092"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row47175923"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p63153417"><a name="zh-cn_topic_0118921492_p63153417"></a><a name="zh-cn_topic_0118921492_p63153417"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p15153123"><a name="zh-cn_topic_0118921492_p15153123"></a><a name="zh-cn_topic_0118921492_p15153123"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p19443433"><a name="zh-cn_topic_0118921492_p19443433"></a><a name="zh-cn_topic_0118921492_p19443433"></a>描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p31414277"><a name="zh-cn_topic_0118921492_p31414277"></a><a name="zh-cn_topic_0118921492_p31414277"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p61528476"><a name="zh-cn_topic_0118921492_p61528476"></a><a name="zh-cn_topic_0118921492_p61528476"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row16885378"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p25538400"><a name="zh-cn_topic_0118921492_p25538400"></a><a name="zh-cn_topic_0118921492_p25538400"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p55344494"><a name="zh-cn_topic_0118921492_p55344494"></a><a name="zh-cn_topic_0118921492_p55344494"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p53718996"><a name="zh-cn_topic_0118921492_p53718996"></a><a name="zh-cn_topic_0118921492_p53718996"></a>是否使用VPC通道</p>
<a name="zh-cn_topic_0118921492_ul13708920"></a><a name="zh-cn_topic_0118921492_ul13708920"></a><ul id="zh-cn_topic_0118921492_ul13708920"><li>1：使用</li><li>2：不使用</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p18348833"><a name="zh-cn_topic_0118921492_p18348833"></a><a name="zh-cn_topic_0118921492_p18348833"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p9860480"><a name="zh-cn_topic_0118921492_p9860480"></a><a name="zh-cn_topic_0118921492_p9860480"></a>否，默认不使用</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row21635459"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p7641724"><a name="zh-cn_topic_0118921492_p7641724"></a><a name="zh-cn_topic_0118921492_p7641724"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p14999869"><a name="zh-cn_topic_0118921492_p14999869"></a><a name="zh-cn_topic_0118921492_p14999869"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p7029871"><a name="zh-cn_topic_0118921492_p7029871"></a><a name="zh-cn_topic_0118921492_p7029871"></a>VPC通道信息</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p32548665"><a name="zh-cn_topic_0118921492_p32548665"></a><a name="zh-cn_topic_0118921492_p32548665"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p19196228"><a name="zh-cn_topic_0118921492_p19196228"></a><a name="zh-cn_topic_0118921492_p19196228"></a>否</p>
<p id="zh-cn_topic_0118921492_p38548329"><a name="zh-cn_topic_0118921492_p38548329"></a><a name="zh-cn_topic_0118921492_p38548329"></a>如果vpc_status=1，即：使用VPC通道，则该字段必填</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row104251555162115"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p4426105522114"><a name="zh-cn_topic_0118921492_p4426105522114"></a><a name="zh-cn_topic_0118921492_p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p142559710221"><a name="zh-cn_topic_0118921492_p142559710221"></a><a name="zh-cn_topic_0118921492_p142559710221"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p144265550215"><a name="zh-cn_topic_0118921492_p144265550215"></a><a name="zh-cn_topic_0118921492_p144265550215"></a>后端自定义认证对象的ID</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1156982062215"><a name="zh-cn_topic_0118921492_p1156982062215"></a><a name="zh-cn_topic_0118921492_p1156982062215"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p15412727152210"><a name="zh-cn_topic_0118921492_p15412727152210"></a><a name="zh-cn_topic_0118921492_p15412727152210"></a>否</p>
</td>
</tr>
</tbody>
</table>

**表 3**  MOCK后端对象模型

<a name="zh-cn_topic_0118921492_table36516114"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row6166330"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p29710736"><a name="zh-cn_topic_0118921492_p29710736"></a><a name="zh-cn_topic_0118921492_p29710736"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p57759422"><a name="zh-cn_topic_0118921492_p57759422"></a><a name="zh-cn_topic_0118921492_p57759422"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p48001645"><a name="zh-cn_topic_0118921492_p48001645"></a><a name="zh-cn_topic_0118921492_p48001645"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p62928069"><a name="zh-cn_topic_0118921492_p62928069"></a><a name="zh-cn_topic_0118921492_p62928069"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p64008813"><a name="zh-cn_topic_0118921492_p64008813"></a><a name="zh-cn_topic_0118921492_p64008813"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row17331341"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p61661390"><a name="zh-cn_topic_0118921492_p61661390"></a><a name="zh-cn_topic_0118921492_p61661390"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p28516695"><a name="zh-cn_topic_0118921492_p28516695"></a><a name="zh-cn_topic_0118921492_p28516695"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p28150993"><a name="zh-cn_topic_0118921492_p28150993"></a><a name="zh-cn_topic_0118921492_p28150993"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p65637988"><a name="zh-cn_topic_0118921492_p65637988"></a><a name="zh-cn_topic_0118921492_p65637988"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p15076791"><a name="zh-cn_topic_0118921492_p15076791"></a><a name="zh-cn_topic_0118921492_p15076791"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1473392"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p52235910"><a name="zh-cn_topic_0118921492_p52235910"></a><a name="zh-cn_topic_0118921492_p52235910"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p3250354"><a name="zh-cn_topic_0118921492_p3250354"></a><a name="zh-cn_topic_0118921492_p3250354"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p61952089"><a name="zh-cn_topic_0118921492_p61952089"></a><a name="zh-cn_topic_0118921492_p61952089"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p52063333"><a name="zh-cn_topic_0118921492_p52063333"></a><a name="zh-cn_topic_0118921492_p52063333"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p56380478"><a name="zh-cn_topic_0118921492_p56380478"></a><a name="zh-cn_topic_0118921492_p56380478"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row37662259"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p30744105"><a name="zh-cn_topic_0118921492_p30744105"></a><a name="zh-cn_topic_0118921492_p30744105"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p7244576"><a name="zh-cn_topic_0118921492_p7244576"></a><a name="zh-cn_topic_0118921492_p7244576"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p49939775"><a name="zh-cn_topic_0118921492_p49939775"></a><a name="zh-cn_topic_0118921492_p49939775"></a>状态：</p>
<a name="zh-cn_topic_0118921492_ul46804798"></a><a name="zh-cn_topic_0118921492_ul46804798"></a><ul id="zh-cn_topic_0118921492_ul46804798"><li>1：启用</li><li>2：禁用</li><li>3：已删除</li></ul>
<p id="zh-cn_topic_0118921492_p63228121"><a name="zh-cn_topic_0118921492_p63228121"></a><a name="zh-cn_topic_0118921492_p63228121"></a>默认1</p>
<p id="zh-cn_topic_0118921492_p32182177"><a name="zh-cn_topic_0118921492_p32182177"></a><a name="zh-cn_topic_0118921492_p32182177"></a><strong id="zh-cn_topic_0118921492_b21204137"><a name="zh-cn_topic_0118921492_b21204137"></a><a name="zh-cn_topic_0118921492_b21204137"></a>该字段已废弃</strong></p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p39813509"><a name="zh-cn_topic_0118921492_p39813509"></a><a name="zh-cn_topic_0118921492_p39813509"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p3668822"><a name="zh-cn_topic_0118921492_p3668822"></a><a name="zh-cn_topic_0118921492_p3668822"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row33019406"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p57326249"><a name="zh-cn_topic_0118921492_p57326249"></a><a name="zh-cn_topic_0118921492_p57326249"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p12914605"><a name="zh-cn_topic_0118921492_p12914605"></a><a name="zh-cn_topic_0118921492_p12914605"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p39450048"><a name="zh-cn_topic_0118921492_p39450048"></a><a name="zh-cn_topic_0118921492_p39450048"></a>版本</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p41337357"><a name="zh-cn_topic_0118921492_p41337357"></a><a name="zh-cn_topic_0118921492_p41337357"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p59991610"><a name="zh-cn_topic_0118921492_p59991610"></a><a name="zh-cn_topic_0118921492_p59991610"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row3053580"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p46013421"><a name="zh-cn_topic_0118921492_p46013421"></a><a name="zh-cn_topic_0118921492_p46013421"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p36099586"><a name="zh-cn_topic_0118921492_p36099586"></a><a name="zh-cn_topic_0118921492_p36099586"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p38385331"><a name="zh-cn_topic_0118921492_p38385331"></a><a name="zh-cn_topic_0118921492_p38385331"></a>返回结果</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p22204138"><a name="zh-cn_topic_0118921492_p22204138"></a><a name="zh-cn_topic_0118921492_p22204138"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p53704716"><a name="zh-cn_topic_0118921492_p53704716"></a><a name="zh-cn_topic_0118921492_p53704716"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row13580402"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p26270754"><a name="zh-cn_topic_0118921492_p26270754"></a><a name="zh-cn_topic_0118921492_p26270754"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p47556339"><a name="zh-cn_topic_0118921492_p47556339"></a><a name="zh-cn_topic_0118921492_p47556339"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p26858252"><a name="zh-cn_topic_0118921492_p26858252"></a><a name="zh-cn_topic_0118921492_p26858252"></a>注册时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p28034838"><a name="zh-cn_topic_0118921492_p28034838"></a><a name="zh-cn_topic_0118921492_p28034838"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p56229433"><a name="zh-cn_topic_0118921492_p56229433"></a><a name="zh-cn_topic_0118921492_p56229433"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row36302851"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p54849789"><a name="zh-cn_topic_0118921492_p54849789"></a><a name="zh-cn_topic_0118921492_p54849789"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p13647907"><a name="zh-cn_topic_0118921492_p13647907"></a><a name="zh-cn_topic_0118921492_p13647907"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p31738719"><a name="zh-cn_topic_0118921492_p31738719"></a><a name="zh-cn_topic_0118921492_p31738719"></a>修改时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p20699414"><a name="zh-cn_topic_0118921492_p20699414"></a><a name="zh-cn_topic_0118921492_p20699414"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p66039858"><a name="zh-cn_topic_0118921492_p66039858"></a><a name="zh-cn_topic_0118921492_p66039858"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row57487818"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p26001656"><a name="zh-cn_topic_0118921492_p26001656"></a><a name="zh-cn_topic_0118921492_p26001656"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p25759358"><a name="zh-cn_topic_0118921492_p25759358"></a><a name="zh-cn_topic_0118921492_p25759358"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p6133253"><a name="zh-cn_topic_0118921492_p6133253"></a><a name="zh-cn_topic_0118921492_p6133253"></a>描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p27031476"><a name="zh-cn_topic_0118921492_p27031476"></a><a name="zh-cn_topic_0118921492_p27031476"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p42065972"><a name="zh-cn_topic_0118921492_p42065972"></a><a name="zh-cn_topic_0118921492_p42065972"></a>否</p>
</td>
</tr>
</tbody>
</table>

**表 4**  函数工作流对象模型

<a name="zh-cn_topic_0118921492_table60209572"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row66748611"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p37928449"><a name="zh-cn_topic_0118921492_p37928449"></a><a name="zh-cn_topic_0118921492_p37928449"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p52305539"><a name="zh-cn_topic_0118921492_p52305539"></a><a name="zh-cn_topic_0118921492_p52305539"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p8890290"><a name="zh-cn_topic_0118921492_p8890290"></a><a name="zh-cn_topic_0118921492_p8890290"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p49024885"><a name="zh-cn_topic_0118921492_p49024885"></a><a name="zh-cn_topic_0118921492_p49024885"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p11592757"><a name="zh-cn_topic_0118921492_p11592757"></a><a name="zh-cn_topic_0118921492_p11592757"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row66598105"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p25737418"><a name="zh-cn_topic_0118921492_p25737418"></a><a name="zh-cn_topic_0118921492_p25737418"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p4356079"><a name="zh-cn_topic_0118921492_p4356079"></a><a name="zh-cn_topic_0118921492_p4356079"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p17298096"><a name="zh-cn_topic_0118921492_p17298096"></a><a name="zh-cn_topic_0118921492_p17298096"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p58968567"><a name="zh-cn_topic_0118921492_p58968567"></a><a name="zh-cn_topic_0118921492_p58968567"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p11724585"><a name="zh-cn_topic_0118921492_p11724585"></a><a name="zh-cn_topic_0118921492_p11724585"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row38412407"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p24397239"><a name="zh-cn_topic_0118921492_p24397239"></a><a name="zh-cn_topic_0118921492_p24397239"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p30019352"><a name="zh-cn_topic_0118921492_p30019352"></a><a name="zh-cn_topic_0118921492_p30019352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p15648449"><a name="zh-cn_topic_0118921492_p15648449"></a><a name="zh-cn_topic_0118921492_p15648449"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p59564891"><a name="zh-cn_topic_0118921492_p59564891"></a><a name="zh-cn_topic_0118921492_p59564891"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p60026894"><a name="zh-cn_topic_0118921492_p60026894"></a><a name="zh-cn_topic_0118921492_p60026894"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row3371136"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p4626570"><a name="zh-cn_topic_0118921492_p4626570"></a><a name="zh-cn_topic_0118921492_p4626570"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p39207872"><a name="zh-cn_topic_0118921492_p39207872"></a><a name="zh-cn_topic_0118921492_p39207872"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p21721100"><a name="zh-cn_topic_0118921492_p21721100"></a><a name="zh-cn_topic_0118921492_p21721100"></a>状态：</p>
<a name="zh-cn_topic_0118921492_ul61272172"></a><a name="zh-cn_topic_0118921492_ul61272172"></a><ul id="zh-cn_topic_0118921492_ul61272172"><li>1：启用</li><li>2：禁用</li><li>3：已删除</li></ul>
<p id="zh-cn_topic_0118921492_p24630783"><a name="zh-cn_topic_0118921492_p24630783"></a><a name="zh-cn_topic_0118921492_p24630783"></a>默认1</p>
<p id="zh-cn_topic_0118921492_p20350456"><a name="zh-cn_topic_0118921492_p20350456"></a><a name="zh-cn_topic_0118921492_p20350456"></a><strong id="zh-cn_topic_0118921492_b48936381"><a name="zh-cn_topic_0118921492_b48936381"></a><a name="zh-cn_topic_0118921492_b48936381"></a>该字段已废弃</strong></p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p4423891"><a name="zh-cn_topic_0118921492_p4423891"></a><a name="zh-cn_topic_0118921492_p4423891"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p22790890"><a name="zh-cn_topic_0118921492_p22790890"></a><a name="zh-cn_topic_0118921492_p22790890"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row3791421"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p38669688"><a name="zh-cn_topic_0118921492_p38669688"></a><a name="zh-cn_topic_0118921492_p38669688"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p45236999"><a name="zh-cn_topic_0118921492_p45236999"></a><a name="zh-cn_topic_0118921492_p45236999"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p40318291"><a name="zh-cn_topic_0118921492_p40318291"></a><a name="zh-cn_topic_0118921492_p40318291"></a>函数版本号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p44556099"><a name="zh-cn_topic_0118921492_p44556099"></a><a name="zh-cn_topic_0118921492_p44556099"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p52274239"><a name="zh-cn_topic_0118921492_p52274239"></a><a name="zh-cn_topic_0118921492_p52274239"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row706110"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p57194936"><a name="zh-cn_topic_0118921492_p57194936"></a><a name="zh-cn_topic_0118921492_p57194936"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p2278259"><a name="zh-cn_topic_0118921492_p2278259"></a><a name="zh-cn_topic_0118921492_p2278259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p50321303"><a name="zh-cn_topic_0118921492_p50321303"></a><a name="zh-cn_topic_0118921492_p50321303"></a>函数的URN</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p49493706"><a name="zh-cn_topic_0118921492_p49493706"></a><a name="zh-cn_topic_0118921492_p49493706"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p49567287"><a name="zh-cn_topic_0118921492_p49567287"></a><a name="zh-cn_topic_0118921492_p49567287"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row43452402"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p29983654"><a name="zh-cn_topic_0118921492_p29983654"></a><a name="zh-cn_topic_0118921492_p29983654"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p12756903"><a name="zh-cn_topic_0118921492_p12756903"></a><a name="zh-cn_topic_0118921492_p12756903"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p26676188"><a name="zh-cn_topic_0118921492_p26676188"></a><a name="zh-cn_topic_0118921492_p26676188"></a>函数类型：async|sync(异步|同步)</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p13287597"><a name="zh-cn_topic_0118921492_p13287597"></a><a name="zh-cn_topic_0118921492_p13287597"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p2553604"><a name="zh-cn_topic_0118921492_p2553604"></a><a name="zh-cn_topic_0118921492_p2553604"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row22982436"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p49638012"><a name="zh-cn_topic_0118921492_p49638012"></a><a name="zh-cn_topic_0118921492_p49638012"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p61256012"><a name="zh-cn_topic_0118921492_p61256012"></a><a name="zh-cn_topic_0118921492_p61256012"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p62789949"><a name="zh-cn_topic_0118921492_p62789949"></a><a name="zh-cn_topic_0118921492_p62789949"></a>超时时间（1-60000），单位：毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p52821110"><a name="zh-cn_topic_0118921492_p52821110"></a><a name="zh-cn_topic_0118921492_p52821110"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p50651552"><a name="zh-cn_topic_0118921492_p50651552"></a><a name="zh-cn_topic_0118921492_p50651552"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row53210791"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p15106813"><a name="zh-cn_topic_0118921492_p15106813"></a><a name="zh-cn_topic_0118921492_p15106813"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p15692311"><a name="zh-cn_topic_0118921492_p15692311"></a><a name="zh-cn_topic_0118921492_p15692311"></a>Date</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p63117661"><a name="zh-cn_topic_0118921492_p63117661"></a><a name="zh-cn_topic_0118921492_p63117661"></a>注册时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p12256953"><a name="zh-cn_topic_0118921492_p12256953"></a><a name="zh-cn_topic_0118921492_p12256953"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p53289104"><a name="zh-cn_topic_0118921492_p53289104"></a><a name="zh-cn_topic_0118921492_p53289104"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row9839894"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p58833972"><a name="zh-cn_topic_0118921492_p58833972"></a><a name="zh-cn_topic_0118921492_p58833972"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p822402"><a name="zh-cn_topic_0118921492_p822402"></a><a name="zh-cn_topic_0118921492_p822402"></a>Date</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p66614568"><a name="zh-cn_topic_0118921492_p66614568"></a><a name="zh-cn_topic_0118921492_p66614568"></a>修改时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p27070927"><a name="zh-cn_topic_0118921492_p27070927"></a><a name="zh-cn_topic_0118921492_p27070927"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p45261470"><a name="zh-cn_topic_0118921492_p45261470"></a><a name="zh-cn_topic_0118921492_p45261470"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row4700053"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p45159988"><a name="zh-cn_topic_0118921492_p45159988"></a><a name="zh-cn_topic_0118921492_p45159988"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p34080400"><a name="zh-cn_topic_0118921492_p34080400"></a><a name="zh-cn_topic_0118921492_p34080400"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p9048976"><a name="zh-cn_topic_0118921492_p9048976"></a><a name="zh-cn_topic_0118921492_p9048976"></a>描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p61878428"><a name="zh-cn_topic_0118921492_p61878428"></a><a name="zh-cn_topic_0118921492_p61878428"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p46096797"><a name="zh-cn_topic_0118921492_p46096797"></a><a name="zh-cn_topic_0118921492_p46096797"></a>否</p>
</td>
</tr>
</tbody>
</table>

**表 5**  请求参数对象模型

<a name="zh-cn_topic_0118921492_table13898234316"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row791715316318"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p1292213393116"><a name="zh-cn_topic_0118921492_p1292213393116"></a><a name="zh-cn_topic_0118921492_p1292213393116"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p139251437317"><a name="zh-cn_topic_0118921492_p139251437317"></a><a name="zh-cn_topic_0118921492_p139251437317"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p192810318313"><a name="zh-cn_topic_0118921492_p192810318313"></a><a name="zh-cn_topic_0118921492_p192810318313"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p1393143163113"><a name="zh-cn_topic_0118921492_p1393143163113"></a><a name="zh-cn_topic_0118921492_p1393143163113"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p149371433312"><a name="zh-cn_topic_0118921492_p149371433312"></a><a name="zh-cn_topic_0118921492_p149371433312"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row11941123193118"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p79467333117"><a name="zh-cn_topic_0118921492_p79467333117"></a><a name="zh-cn_topic_0118921492_p79467333117"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p095015312317"><a name="zh-cn_topic_0118921492_p095015312317"></a><a name="zh-cn_topic_0118921492_p095015312317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1495719316312"><a name="zh-cn_topic_0118921492_p1495719316312"></a><a name="zh-cn_topic_0118921492_p1495719316312"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p49609373114"><a name="zh-cn_topic_0118921492_p49609373114"></a><a name="zh-cn_topic_0118921492_p49609373114"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p16964203103111"><a name="zh-cn_topic_0118921492_p16964203103111"></a><a name="zh-cn_topic_0118921492_p16964203103111"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1096715343118"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p09705317314"><a name="zh-cn_topic_0118921492_p09705317314"></a><a name="zh-cn_topic_0118921492_p09705317314"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p149751531312"><a name="zh-cn_topic_0118921492_p149751531312"></a><a name="zh-cn_topic_0118921492_p149751531312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p12977113193118"><a name="zh-cn_topic_0118921492_p12977113193118"></a><a name="zh-cn_topic_0118921492_p12977113193118"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1098263173110"><a name="zh-cn_topic_0118921492_p1098263173110"></a><a name="zh-cn_topic_0118921492_p1098263173110"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p698617316315"><a name="zh-cn_topic_0118921492_p698617316315"></a><a name="zh-cn_topic_0118921492_p698617316315"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row119878320319"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p799419317316"><a name="zh-cn_topic_0118921492_p799419317316"></a><a name="zh-cn_topic_0118921492_p799419317316"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p79999393113"><a name="zh-cn_topic_0118921492_p79999393113"></a><a name="zh-cn_topic_0118921492_p79999393113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p42296485336"><a name="zh-cn_topic_0118921492_p42296485336"></a><a name="zh-cn_topic_0118921492_p42296485336"></a>参数名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1631104123113"><a name="zh-cn_topic_0118921492_p1631104123113"></a><a name="zh-cn_topic_0118921492_p1631104123113"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p93854183114"><a name="zh-cn_topic_0118921492_p93854183114"></a><a name="zh-cn_topic_0118921492_p93854183114"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row54124103115"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p164411416314"><a name="zh-cn_topic_0118921492_p164411416314"></a><a name="zh-cn_topic_0118921492_p164411416314"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p14496416313"><a name="zh-cn_topic_0118921492_p14496416313"></a><a name="zh-cn_topic_0118921492_p14496416313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p6244152615341"><a name="zh-cn_topic_0118921492_p6244152615341"></a><a name="zh-cn_topic_0118921492_p6244152615341"></a>参数类型：</p>
<a name="zh-cn_topic_0118921492_ul9247102613342"></a><a name="zh-cn_topic_0118921492_ul9247102613342"></a><ul id="zh-cn_topic_0118921492_ul9247102613342"><li>string</li><li>number</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p125611413112"><a name="zh-cn_topic_0118921492_p125611413112"></a><a name="zh-cn_topic_0118921492_p125611413112"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p66110417312"><a name="zh-cn_topic_0118921492_p66110417312"></a><a name="zh-cn_topic_0118921492_p66110417312"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1362549313"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p7661949315"><a name="zh-cn_topic_0118921492_p7661949315"></a><a name="zh-cn_topic_0118921492_p7661949315"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p137111473113"><a name="zh-cn_topic_0118921492_p137111473113"></a><a name="zh-cn_topic_0118921492_p137111473113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p321213285352"><a name="zh-cn_topic_0118921492_p321213285352"></a><a name="zh-cn_topic_0118921492_p321213285352"></a>参数位置：</p>
<a name="zh-cn_topic_0118921492_ul172162282351"></a><a name="zh-cn_topic_0118921492_ul172162282351"></a><ul id="zh-cn_topic_0118921492_ul172162282351"><li>PATH</li><li>QUERY</li><li>HEADER</li><li>FORMDATA</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p879184183119"><a name="zh-cn_topic_0118921492_p879184183119"></a><a name="zh-cn_topic_0118921492_p879184183119"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p178417418313"><a name="zh-cn_topic_0118921492_p178417418313"></a><a name="zh-cn_topic_0118921492_p178417418313"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row4851433116"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1490343314"><a name="zh-cn_topic_0118921492_p1490343314"></a><a name="zh-cn_topic_0118921492_p1490343314"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1920416311"><a name="zh-cn_topic_0118921492_p1920416311"></a><a name="zh-cn_topic_0118921492_p1920416311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p4964411314"><a name="zh-cn_topic_0118921492_p4964411314"></a><a name="zh-cn_topic_0118921492_p4964411314"></a>参数默认值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p810014410316"><a name="zh-cn_topic_0118921492_p810014410316"></a><a name="zh-cn_topic_0118921492_p810014410316"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p18105643319"><a name="zh-cn_topic_0118921492_p18105643319"></a><a name="zh-cn_topic_0118921492_p18105643319"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row5108114193114"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1411414413112"><a name="zh-cn_topic_0118921492_p1411414413112"></a><a name="zh-cn_topic_0118921492_p1411414413112"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p131199420314"><a name="zh-cn_topic_0118921492_p131199420314"></a><a name="zh-cn_topic_0118921492_p131199420314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p312215412312"><a name="zh-cn_topic_0118921492_p312215412312"></a><a name="zh-cn_topic_0118921492_p312215412312"></a>参数示例值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p812712414313"><a name="zh-cn_topic_0118921492_p812712414313"></a><a name="zh-cn_topic_0118921492_p812712414313"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p131331410313"><a name="zh-cn_topic_0118921492_p131331410313"></a><a name="zh-cn_topic_0118921492_p131331410313"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row313514133117"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1013934183112"><a name="zh-cn_topic_0118921492_p1013934183112"></a><a name="zh-cn_topic_0118921492_p1013934183112"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p114314483118"><a name="zh-cn_topic_0118921492_p114314483118"></a><a name="zh-cn_topic_0118921492_p114314483118"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p0887658194111"><a name="zh-cn_topic_0118921492_p0887658194111"></a><a name="zh-cn_topic_0118921492_p0887658194111"></a>参数是否必须：</p>
<a name="zh-cn_topic_0118921492_ul08951458174116"></a><a name="zh-cn_topic_0118921492_ul08951458174116"></a><ul id="zh-cn_topic_0118921492_ul08951458174116"><li>1：是</li><li>2：否</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1315015416314"><a name="zh-cn_topic_0118921492_p1315015416314"></a><a name="zh-cn_topic_0118921492_p1315015416314"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1615417423113"><a name="zh-cn_topic_0118921492_p1615417423113"></a><a name="zh-cn_topic_0118921492_p1615417423113"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row41581347318"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p131650473114"><a name="zh-cn_topic_0118921492_p131650473114"></a><a name="zh-cn_topic_0118921492_p131650473114"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p181695418316"><a name="zh-cn_topic_0118921492_p181695418316"></a><a name="zh-cn_topic_0118921492_p181695418316"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p199991656144115"><a name="zh-cn_topic_0118921492_p199991656144115"></a><a name="zh-cn_topic_0118921492_p199991656144115"></a>是否开启参数校验：</p>
<a name="zh-cn_topic_0118921492_ul172105784112"></a><a name="zh-cn_topic_0118921492_ul172105784112"></a><ul id="zh-cn_topic_0118921492_ul172105784112"><li>1：是</li><li>2：否</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p317613493117"><a name="zh-cn_topic_0118921492_p317613493117"></a><a name="zh-cn_topic_0118921492_p317613493117"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p9180174183111"><a name="zh-cn_topic_0118921492_p9180174183111"></a><a name="zh-cn_topic_0118921492_p9180174183111"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1318294163114"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p5186194113118"><a name="zh-cn_topic_0118921492_p5186194113118"></a><a name="zh-cn_topic_0118921492_p5186194113118"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p918924173114"><a name="zh-cn_topic_0118921492_p918924173114"></a><a name="zh-cn_topic_0118921492_p918924173114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1919419418312"><a name="zh-cn_topic_0118921492_p1919419418312"></a><a name="zh-cn_topic_0118921492_p1919419418312"></a>参数描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p172001413116"><a name="zh-cn_topic_0118921492_p172001413116"></a><a name="zh-cn_topic_0118921492_p172001413116"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p02026417314"><a name="zh-cn_topic_0118921492_p02026417314"></a><a name="zh-cn_topic_0118921492_p02026417314"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row128109163716"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p16814933710"><a name="zh-cn_topic_0118921492_p16814933710"></a><a name="zh-cn_topic_0118921492_p16814933710"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p48795378"><a name="zh-cn_topic_0118921492_p48795378"></a><a name="zh-cn_topic_0118921492_p48795378"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p108189133719"><a name="zh-cn_topic_0118921492_p108189133719"></a><a name="zh-cn_topic_0118921492_p108189133719"></a>参数枚举值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p781096375"><a name="zh-cn_topic_0118921492_p781096375"></a><a name="zh-cn_topic_0118921492_p781096375"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p381099371"><a name="zh-cn_topic_0118921492_p381099371"></a><a name="zh-cn_topic_0118921492_p381099371"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row392981623715"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p189291516143720"><a name="zh-cn_topic_0118921492_p189291516143720"></a><a name="zh-cn_topic_0118921492_p189291516143720"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p092921653718"><a name="zh-cn_topic_0118921492_p092921653718"></a><a name="zh-cn_topic_0118921492_p092921653718"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p39296165373"><a name="zh-cn_topic_0118921492_p39296165373"></a><a name="zh-cn_topic_0118921492_p39296165373"></a>参数最小值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p392961683713"><a name="zh-cn_topic_0118921492_p392961683713"></a><a name="zh-cn_topic_0118921492_p392961683713"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p392991613376"><a name="zh-cn_topic_0118921492_p392991613376"></a><a name="zh-cn_topic_0118921492_p392991613376"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row124461414193711"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p844611418376"><a name="zh-cn_topic_0118921492_p844611418376"></a><a name="zh-cn_topic_0118921492_p844611418376"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p8446151433713"><a name="zh-cn_topic_0118921492_p8446151433713"></a><a name="zh-cn_topic_0118921492_p8446151433713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1444611453710"><a name="zh-cn_topic_0118921492_p1444611453710"></a><a name="zh-cn_topic_0118921492_p1444611453710"></a>参数最大值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p7446214173711"><a name="zh-cn_topic_0118921492_p7446214173711"></a><a name="zh-cn_topic_0118921492_p7446214173711"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p13447151413717"><a name="zh-cn_topic_0118921492_p13447151413717"></a><a name="zh-cn_topic_0118921492_p13447151413717"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row19844131613380"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1184510164388"><a name="zh-cn_topic_0118921492_p1184510164388"></a><a name="zh-cn_topic_0118921492_p1184510164388"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p88451416143810"><a name="zh-cn_topic_0118921492_p88451416143810"></a><a name="zh-cn_topic_0118921492_p88451416143810"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p208455166389"><a name="zh-cn_topic_0118921492_p208455166389"></a><a name="zh-cn_topic_0118921492_p208455166389"></a>参数最小长度</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p484561693820"><a name="zh-cn_topic_0118921492_p484561693820"></a><a name="zh-cn_topic_0118921492_p484561693820"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p8845171612385"><a name="zh-cn_topic_0118921492_p8845171612385"></a><a name="zh-cn_topic_0118921492_p8845171612385"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row9410151316386"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p114107132384"><a name="zh-cn_topic_0118921492_p114107132384"></a><a name="zh-cn_topic_0118921492_p114107132384"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1341031343814"><a name="zh-cn_topic_0118921492_p1341031343814"></a><a name="zh-cn_topic_0118921492_p1341031343814"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p241051323817"><a name="zh-cn_topic_0118921492_p241051323817"></a><a name="zh-cn_topic_0118921492_p241051323817"></a>参数最大长度</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p8411151319389"><a name="zh-cn_topic_0118921492_p8411151319389"></a><a name="zh-cn_topic_0118921492_p8411151319389"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p541131311382"><a name="zh-cn_topic_0118921492_p541131311382"></a><a name="zh-cn_topic_0118921492_p541131311382"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1356915405380"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p95691401383"><a name="zh-cn_topic_0118921492_p95691401383"></a><a name="zh-cn_topic_0118921492_p95691401383"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1356994014389"><a name="zh-cn_topic_0118921492_p1356994014389"></a><a name="zh-cn_topic_0118921492_p1356994014389"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1356934013811"><a name="zh-cn_topic_0118921492_p1356934013811"></a><a name="zh-cn_topic_0118921492_p1356934013811"></a>正则校验规则（暂不支持）</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p2569340153815"><a name="zh-cn_topic_0118921492_p2569340153815"></a><a name="zh-cn_topic_0118921492_p2569340153815"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p20569940163815"><a name="zh-cn_topic_0118921492_p20569940163815"></a><a name="zh-cn_topic_0118921492_p20569940163815"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row6295647133815"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p329517477385"><a name="zh-cn_topic_0118921492_p329517477385"></a><a name="zh-cn_topic_0118921492_p329517477385"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p22951347193817"><a name="zh-cn_topic_0118921492_p22951347193817"></a><a name="zh-cn_topic_0118921492_p22951347193817"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1029544718380"><a name="zh-cn_topic_0118921492_p1029544718380"></a><a name="zh-cn_topic_0118921492_p1029544718380"></a>JSON校验规则（暂不支持）</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p13295847143819"><a name="zh-cn_topic_0118921492_p13295847143819"></a><a name="zh-cn_topic_0118921492_p13295847143819"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p5295204743816"><a name="zh-cn_topic_0118921492_p5295204743816"></a><a name="zh-cn_topic_0118921492_p5295204743816"></a>否</p>
</td>
</tr>
</tbody>
</table>

**表 6**  后端参数对象模型

<a name="zh-cn_topic_0118921492_table1399706153120"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row1022147113111"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p172717743114"><a name="zh-cn_topic_0118921492_p172717743114"></a><a name="zh-cn_topic_0118921492_p172717743114"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p33117143116"><a name="zh-cn_topic_0118921492_p33117143116"></a><a name="zh-cn_topic_0118921492_p33117143116"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p16352763112"><a name="zh-cn_topic_0118921492_p16352763112"></a><a name="zh-cn_topic_0118921492_p16352763112"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p6391174311"><a name="zh-cn_topic_0118921492_p6391174311"></a><a name="zh-cn_topic_0118921492_p6391174311"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p10444715311"><a name="zh-cn_topic_0118921492_p10444715311"></a><a name="zh-cn_topic_0118921492_p10444715311"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row55117763118"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p454127113113"><a name="zh-cn_topic_0118921492_p454127113113"></a><a name="zh-cn_topic_0118921492_p454127113113"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p4612716311"><a name="zh-cn_topic_0118921492_p4612716311"></a><a name="zh-cn_topic_0118921492_p4612716311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p2689733119"><a name="zh-cn_topic_0118921492_p2689733119"></a><a name="zh-cn_topic_0118921492_p2689733119"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p187577153113"><a name="zh-cn_topic_0118921492_p187577153113"></a><a name="zh-cn_topic_0118921492_p187577153113"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p12811579318"><a name="zh-cn_topic_0118921492_p12811579318"></a><a name="zh-cn_topic_0118921492_p12811579318"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row78320723117"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p189019713313"><a name="zh-cn_topic_0118921492_p189019713313"></a><a name="zh-cn_topic_0118921492_p189019713313"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p7946793117"><a name="zh-cn_topic_0118921492_p7946793117"></a><a name="zh-cn_topic_0118921492_p7946793117"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p81008716313"><a name="zh-cn_topic_0118921492_p81008716313"></a><a name="zh-cn_topic_0118921492_p81008716313"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1105173311"><a name="zh-cn_topic_0118921492_p1105173311"></a><a name="zh-cn_topic_0118921492_p1105173311"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1611027113113"><a name="zh-cn_topic_0118921492_p1611027113113"></a><a name="zh-cn_topic_0118921492_p1611027113113"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row611387193116"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p17117167133113"><a name="zh-cn_topic_0118921492_p17117167133113"></a><a name="zh-cn_topic_0118921492_p17117167133113"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p12122774316"><a name="zh-cn_topic_0118921492_p12122774316"></a><a name="zh-cn_topic_0118921492_p12122774316"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1315419783113"><a name="zh-cn_topic_0118921492_p1315419783113"></a><a name="zh-cn_topic_0118921492_p1315419783113"></a>对应的请求参数的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p15161147103118"><a name="zh-cn_topic_0118921492_p15161147103118"></a><a name="zh-cn_topic_0118921492_p15161147103118"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p01637710315"><a name="zh-cn_topic_0118921492_p01637710315"></a><a name="zh-cn_topic_0118921492_p01637710315"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1416517723119"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p01728719319"><a name="zh-cn_topic_0118921492_p01728719319"></a><a name="zh-cn_topic_0118921492_p01728719319"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1517614723112"><a name="zh-cn_topic_0118921492_p1517614723112"></a><a name="zh-cn_topic_0118921492_p1517614723112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p21792763118"><a name="zh-cn_topic_0118921492_p21792763118"></a><a name="zh-cn_topic_0118921492_p21792763118"></a>参数名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1918697183118"><a name="zh-cn_topic_0118921492_p1918697183118"></a><a name="zh-cn_topic_0118921492_p1918697183118"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p51921793111"><a name="zh-cn_topic_0118921492_p51921793111"></a><a name="zh-cn_topic_0118921492_p51921793111"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row61959710318"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1220013714316"><a name="zh-cn_topic_0118921492_p1220013714316"></a><a name="zh-cn_topic_0118921492_p1220013714316"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p17207107123110"><a name="zh-cn_topic_0118921492_p17207107123110"></a><a name="zh-cn_topic_0118921492_p17207107123110"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p207516219517"><a name="zh-cn_topic_0118921492_p207516219517"></a><a name="zh-cn_topic_0118921492_p207516219517"></a>参数位置：</p>
<a name="zh-cn_topic_0118921492_ul5825219516"></a><a name="zh-cn_topic_0118921492_ul5825219516"></a><ul id="zh-cn_topic_0118921492_ul5825219516"><li>PATH</li><li>QUERY</li><li>HEADER</li><li>FORMDATA</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p321727193116"><a name="zh-cn_topic_0118921492_p321727193116"></a><a name="zh-cn_topic_0118921492_p321727193116"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1522213733113"><a name="zh-cn_topic_0118921492_p1522213733113"></a><a name="zh-cn_topic_0118921492_p1522213733113"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row182253743112"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p3230207103119"><a name="zh-cn_topic_0118921492_p3230207103119"></a><a name="zh-cn_topic_0118921492_p3230207103119"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p192341874319"><a name="zh-cn_topic_0118921492_p192341874319"></a><a name="zh-cn_topic_0118921492_p192341874319"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p76691321175012"><a name="zh-cn_topic_0118921492_p76691321175012"></a><a name="zh-cn_topic_0118921492_p76691321175012"></a>参数类型：</p>
<a name="zh-cn_topic_0118921492_ul1967222110504"></a><a name="zh-cn_topic_0118921492_ul1967222110504"></a><ul id="zh-cn_topic_0118921492_ul1967222110504"><li>REQUEST</li><li>CONSTANT</li><li>SYSTEM</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p224297123117"><a name="zh-cn_topic_0118921492_p224297123117"></a><a name="zh-cn_topic_0118921492_p224297123117"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p17249575312"><a name="zh-cn_topic_0118921492_p17249575312"></a><a name="zh-cn_topic_0118921492_p17249575312"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row92529783114"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p02561076311"><a name="zh-cn_topic_0118921492_p02561076311"></a><a name="zh-cn_topic_0118921492_p02561076311"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p13260177173112"><a name="zh-cn_topic_0118921492_p13260177173112"></a><a name="zh-cn_topic_0118921492_p13260177173112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p193831019185018"><a name="zh-cn_topic_0118921492_p193831019185018"></a><a name="zh-cn_topic_0118921492_p193831019185018"></a>参数值：</p>
<a name="zh-cn_topic_0118921492_ul137031843112118"></a><a name="zh-cn_topic_0118921492_ul137031843112118"></a><ul id="zh-cn_topic_0118921492_ul137031843112118"><li>类型为REQUEST时，值为请求参数的参数名称。</li><li>类型为SYSTEM时，值为网关参数名称。</li><li>类别为CONSTANT时，值为参数真正的值。</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p4270137183114"><a name="zh-cn_topic_0118921492_p4270137183114"></a><a name="zh-cn_topic_0118921492_p4270137183114"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p52753711312"><a name="zh-cn_topic_0118921492_p52753711312"></a><a name="zh-cn_topic_0118921492_p52753711312"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row12775718316"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1128413733111"><a name="zh-cn_topic_0118921492_p1128413733111"></a><a name="zh-cn_topic_0118921492_p1128413733111"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p19289167143114"><a name="zh-cn_topic_0118921492_p19289167143114"></a><a name="zh-cn_topic_0118921492_p19289167143114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p829367203115"><a name="zh-cn_topic_0118921492_p829367203115"></a><a name="zh-cn_topic_0118921492_p829367203115"></a>描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p4300672315"><a name="zh-cn_topic_0118921492_p4300672315"></a><a name="zh-cn_topic_0118921492_p4300672315"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p9303471315"><a name="zh-cn_topic_0118921492_p9303471315"></a><a name="zh-cn_topic_0118921492_p9303471315"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row163061770317"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1231447163116"><a name="zh-cn_topic_0118921492_p1231447163116"></a><a name="zh-cn_topic_0118921492_p1231447163116"></a>policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1431915743111"><a name="zh-cn_topic_0118921492_p1431915743111"></a><a name="zh-cn_topic_0118921492_p1431915743111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1732412714315"><a name="zh-cn_topic_0118921492_p1732412714315"></a><a name="zh-cn_topic_0118921492_p1732412714315"></a>关联的策略条件编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1332816703119"><a name="zh-cn_topic_0118921492_p1332816703119"></a><a name="zh-cn_topic_0118921492_p1332816703119"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1433457113113"><a name="zh-cn_topic_0118921492_p1433457113113"></a><a name="zh-cn_topic_0118921492_p1433457113113"></a>否</p>
</td>
</tr>
</tbody>
</table>

**表 7**  WEB策略后端对象模型

<a name="zh-cn_topic_0118921492_table2731722541"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row11140162215413"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p31550221743"><a name="zh-cn_topic_0118921492_p31550221743"></a><a name="zh-cn_topic_0118921492_p31550221743"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p1517820221647"><a name="zh-cn_topic_0118921492_p1517820221647"></a><a name="zh-cn_topic_0118921492_p1517820221647"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p220082215419"><a name="zh-cn_topic_0118921492_p220082215419"></a><a name="zh-cn_topic_0118921492_p220082215419"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p132194221843"><a name="zh-cn_topic_0118921492_p132194221843"></a><a name="zh-cn_topic_0118921492_p132194221843"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p15228172216411"><a name="zh-cn_topic_0118921492_p15228172216411"></a><a name="zh-cn_topic_0118921492_p15228172216411"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row624211222419"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1425019221543"><a name="zh-cn_topic_0118921492_p1425019221543"></a><a name="zh-cn_topic_0118921492_p1425019221543"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p122626224410"><a name="zh-cn_topic_0118921492_p122626224410"></a><a name="zh-cn_topic_0118921492_p122626224410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p115165221949"><a name="zh-cn_topic_0118921492_p115165221949"></a><a name="zh-cn_topic_0118921492_p115165221949"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p552552211417"><a name="zh-cn_topic_0118921492_p552552211417"></a><a name="zh-cn_topic_0118921492_p552552211417"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1953416221342"><a name="zh-cn_topic_0118921492_p1953416221342"></a><a name="zh-cn_topic_0118921492_p1953416221342"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row5499124015919"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p54312429914"><a name="zh-cn_topic_0118921492_p54312429914"></a><a name="zh-cn_topic_0118921492_p54312429914"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p196015427911"><a name="zh-cn_topic_0118921492_p196015427911"></a><a name="zh-cn_topic_0118921492_p196015427911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p107484210918"><a name="zh-cn_topic_0118921492_p107484210918"></a><a name="zh-cn_topic_0118921492_p107484210918"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p595124211914"><a name="zh-cn_topic_0118921492_p595124211914"></a><a name="zh-cn_topic_0118921492_p595124211914"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1011204217915"><a name="zh-cn_topic_0118921492_p1011204217915"></a><a name="zh-cn_topic_0118921492_p1011204217915"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row7539142215410"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p6548142213410"><a name="zh-cn_topic_0118921492_p6548142213410"></a><a name="zh-cn_topic_0118921492_p6548142213410"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p115594229418"><a name="zh-cn_topic_0118921492_p115594229418"></a><a name="zh-cn_topic_0118921492_p115594229418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1457710221849"><a name="zh-cn_topic_0118921492_p1457710221849"></a><a name="zh-cn_topic_0118921492_p1457710221849"></a>策略后端名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1958718228418"><a name="zh-cn_topic_0118921492_p1958718228418"></a><a name="zh-cn_topic_0118921492_p1958718228418"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p75954222416"><a name="zh-cn_topic_0118921492_p75954222416"></a><a name="zh-cn_topic_0118921492_p75954222416"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row19598522144"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p968313529492"><a name="zh-cn_topic_0118921492_p968313529492"></a><a name="zh-cn_topic_0118921492_p968313529492"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p3683352184919"><a name="zh-cn_topic_0118921492_p3683352184919"></a><a name="zh-cn_topic_0118921492_p3683352184919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p136831852144910"><a name="zh-cn_topic_0118921492_p136831852144910"></a><a name="zh-cn_topic_0118921492_p136831852144910"></a>后端endpoint</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p36838526490"><a name="zh-cn_topic_0118921492_p36838526490"></a><a name="zh-cn_topic_0118921492_p36838526490"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1068395219498"><a name="zh-cn_topic_0118921492_p1068395219498"></a><a name="zh-cn_topic_0118921492_p1068395219498"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row264802215415"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p7683752154915"><a name="zh-cn_topic_0118921492_p7683752154915"></a><a name="zh-cn_topic_0118921492_p7683752154915"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p5684152104913"><a name="zh-cn_topic_0118921492_p5684152104913"></a><a name="zh-cn_topic_0118921492_p5684152104913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p768418525491"><a name="zh-cn_topic_0118921492_p768418525491"></a><a name="zh-cn_topic_0118921492_p768418525491"></a>访问协议</p>
<a name="zh-cn_topic_0118921492_ul668414526495"></a><a name="zh-cn_topic_0118921492_ul668414526495"></a><ul id="zh-cn_topic_0118921492_ul668414526495"><li>HTTP</li><li>HTTPS</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1768435244918"><a name="zh-cn_topic_0118921492_p1768435244918"></a><a name="zh-cn_topic_0118921492_p1768435244918"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1468465218499"><a name="zh-cn_topic_0118921492_p1468465218499"></a><a name="zh-cn_topic_0118921492_p1468465218499"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row670619221143"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p13684145294919"><a name="zh-cn_topic_0118921492_p13684145294919"></a><a name="zh-cn_topic_0118921492_p13684145294919"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p3684205244914"><a name="zh-cn_topic_0118921492_p3684205244914"></a><a name="zh-cn_topic_0118921492_p3684205244914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1368410526494"><a name="zh-cn_topic_0118921492_p1368410526494"></a><a name="zh-cn_topic_0118921492_p1368410526494"></a>请求方式</p>
<a name="zh-cn_topic_0118921492_ul868415220497"></a><a name="zh-cn_topic_0118921492_ul868415220497"></a><ul id="zh-cn_topic_0118921492_ul868415220497"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1568575294913"><a name="zh-cn_topic_0118921492_p1568575294913"></a><a name="zh-cn_topic_0118921492_p1568575294913"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p368565274916"><a name="zh-cn_topic_0118921492_p368565274916"></a><a name="zh-cn_topic_0118921492_p368565274916"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row680814221841"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p166867524496"><a name="zh-cn_topic_0118921492_p166867524496"></a><a name="zh-cn_topic_0118921492_p166867524496"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p18686152184911"><a name="zh-cn_topic_0118921492_p18686152184911"></a><a name="zh-cn_topic_0118921492_p18686152184911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p176861252134915"><a name="zh-cn_topic_0118921492_p176861252134915"></a><a name="zh-cn_topic_0118921492_p176861252134915"></a>访问地址，是URI</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p17686252154911"><a name="zh-cn_topic_0118921492_p17686252154911"></a><a name="zh-cn_topic_0118921492_p17686252154911"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p9686452104911"><a name="zh-cn_topic_0118921492_p9686452104911"></a><a name="zh-cn_topic_0118921492_p9686452104911"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row2089319226414"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1868614529495"><a name="zh-cn_topic_0118921492_p1868614529495"></a><a name="zh-cn_topic_0118921492_p1868614529495"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p15686752164912"><a name="zh-cn_topic_0118921492_p15686752164912"></a><a name="zh-cn_topic_0118921492_p15686752164912"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p11686252194916"><a name="zh-cn_topic_0118921492_p11686252194916"></a><a name="zh-cn_topic_0118921492_p11686252194916"></a>超时时间，单位：毫秒（1-60000）</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p5686195212491"><a name="zh-cn_topic_0118921492_p5686195212491"></a><a name="zh-cn_topic_0118921492_p5686195212491"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p4687125215495"><a name="zh-cn_topic_0118921492_p4687125215495"></a><a name="zh-cn_topic_0118921492_p4687125215495"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row19509221744"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p3687105214496"><a name="zh-cn_topic_0118921492_p3687105214496"></a><a name="zh-cn_topic_0118921492_p3687105214496"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p15687125211498"><a name="zh-cn_topic_0118921492_p15687125211498"></a><a name="zh-cn_topic_0118921492_p15687125211498"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p5687752194915"><a name="zh-cn_topic_0118921492_p5687752194915"></a><a name="zh-cn_topic_0118921492_p5687752194915"></a>是否使用VPC通道</p>
<a name="zh-cn_topic_0118921492_ul12687452134918"></a><a name="zh-cn_topic_0118921492_ul12687452134918"></a><ul id="zh-cn_topic_0118921492_ul12687452134918"><li>1：使用</li><li>2：不使用</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p106871952104911"><a name="zh-cn_topic_0118921492_p106871952104911"></a><a name="zh-cn_topic_0118921492_p106871952104911"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p136871652164912"><a name="zh-cn_topic_0118921492_p136871652164912"></a><a name="zh-cn_topic_0118921492_p136871652164912"></a>否，默认不使用</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1715234415"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p12688252154919"><a name="zh-cn_topic_0118921492_p12688252154919"></a><a name="zh-cn_topic_0118921492_p12688252154919"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p668895214913"><a name="zh-cn_topic_0118921492_p668895214913"></a><a name="zh-cn_topic_0118921492_p668895214913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p166882528495"><a name="zh-cn_topic_0118921492_p166882528495"></a><a name="zh-cn_topic_0118921492_p166882528495"></a>VPC通道信息</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1468855264914"><a name="zh-cn_topic_0118921492_p1468855264914"></a><a name="zh-cn_topic_0118921492_p1468855264914"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p11688952164912"><a name="zh-cn_topic_0118921492_p11688952164912"></a><a name="zh-cn_topic_0118921492_p11688952164912"></a>否</p>
<p id="zh-cn_topic_0118921492_p86889526497"><a name="zh-cn_topic_0118921492_p86889526497"></a><a name="zh-cn_topic_0118921492_p86889526497"></a>如果vpc_status=1，即：使用VPC通道，则该字段必填</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row252419501198"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p95241250393"><a name="zh-cn_topic_0118921492_p95241250393"></a><a name="zh-cn_topic_0118921492_p95241250393"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1552445015911"><a name="zh-cn_topic_0118921492_p1552445015911"></a><a name="zh-cn_topic_0118921492_p1552445015911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p183251758111017"><a name="zh-cn_topic_0118921492_p183251758111017"></a><a name="zh-cn_topic_0118921492_p183251758111017"></a>关联的策略组合模式</p>
<a name="zh-cn_topic_0118921492_ul433155821016"></a><a name="zh-cn_topic_0118921492_ul433155821016"></a><ul id="zh-cn_topic_0118921492_ul433155821016"><li>ALL</li><li>ANY</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p95241050496"><a name="zh-cn_topic_0118921492_p95241050496"></a><a name="zh-cn_topic_0118921492_p95241050496"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p19524850396"><a name="zh-cn_topic_0118921492_p19524850396"></a><a name="zh-cn_topic_0118921492_p19524850396"></a>是</p>
</td>
</tr>
</tbody>
</table>

**表 8**  MOCK策略后端对象模型

<a name="zh-cn_topic_0118921492_table334114273417"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row138114271943"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p1138918272410"><a name="zh-cn_topic_0118921492_p1138918272410"></a><a name="zh-cn_topic_0118921492_p1138918272410"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p740018271342"><a name="zh-cn_topic_0118921492_p740018271342"></a><a name="zh-cn_topic_0118921492_p740018271342"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p194071827141"><a name="zh-cn_topic_0118921492_p194071827141"></a><a name="zh-cn_topic_0118921492_p194071827141"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p1641322711414"><a name="zh-cn_topic_0118921492_p1641322711414"></a><a name="zh-cn_topic_0118921492_p1641322711414"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p1741917276420"><a name="zh-cn_topic_0118921492_p1741917276420"></a><a name="zh-cn_topic_0118921492_p1741917276420"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row24282279414"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p488113910115"><a name="zh-cn_topic_0118921492_p488113910115"></a><a name="zh-cn_topic_0118921492_p488113910115"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1299039111112"><a name="zh-cn_topic_0118921492_p1299039111112"></a><a name="zh-cn_topic_0118921492_p1299039111112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p41091439141116"><a name="zh-cn_topic_0118921492_p41091439141116"></a><a name="zh-cn_topic_0118921492_p41091439141116"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1512593913112"><a name="zh-cn_topic_0118921492_p1512593913112"></a><a name="zh-cn_topic_0118921492_p1512593913112"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p2138153916111"><a name="zh-cn_topic_0118921492_p2138153916111"></a><a name="zh-cn_topic_0118921492_p2138153916111"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row0477427645"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p2016173971119"><a name="zh-cn_topic_0118921492_p2016173971119"></a><a name="zh-cn_topic_0118921492_p2016173971119"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p3176639111112"><a name="zh-cn_topic_0118921492_p3176639111112"></a><a name="zh-cn_topic_0118921492_p3176639111112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1518723941113"><a name="zh-cn_topic_0118921492_p1518723941113"></a><a name="zh-cn_topic_0118921492_p1518723941113"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p15202183914110"><a name="zh-cn_topic_0118921492_p15202183914110"></a><a name="zh-cn_topic_0118921492_p15202183914110"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p9217173941120"><a name="zh-cn_topic_0118921492_p9217173941120"></a><a name="zh-cn_topic_0118921492_p9217173941120"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row952414271419"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p324143918112"><a name="zh-cn_topic_0118921492_p324143918112"></a><a name="zh-cn_topic_0118921492_p324143918112"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p025316398118"><a name="zh-cn_topic_0118921492_p025316398118"></a><a name="zh-cn_topic_0118921492_p025316398118"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p2264133961119"><a name="zh-cn_topic_0118921492_p2264133961119"></a><a name="zh-cn_topic_0118921492_p2264133961119"></a>策略后端名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p102759396110"><a name="zh-cn_topic_0118921492_p102759396110"></a><a name="zh-cn_topic_0118921492_p102759396110"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p172901139101117"><a name="zh-cn_topic_0118921492_p172901139101117"></a><a name="zh-cn_topic_0118921492_p172901139101117"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row95701227141"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p206921952114910"><a name="zh-cn_topic_0118921492_p206921952114910"></a><a name="zh-cn_topic_0118921492_p206921952114910"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p106921552154912"><a name="zh-cn_topic_0118921492_p106921552154912"></a><a name="zh-cn_topic_0118921492_p106921552154912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p469295216497"><a name="zh-cn_topic_0118921492_p469295216497"></a><a name="zh-cn_topic_0118921492_p469295216497"></a>返回结果</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1769211526491"><a name="zh-cn_topic_0118921492_p1769211526491"></a><a name="zh-cn_topic_0118921492_p1769211526491"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p136923526496"><a name="zh-cn_topic_0118921492_p136923526496"></a><a name="zh-cn_topic_0118921492_p136923526496"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1862015274410"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p6437113014125"><a name="zh-cn_topic_0118921492_p6437113014125"></a><a name="zh-cn_topic_0118921492_p6437113014125"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p114471302123"><a name="zh-cn_topic_0118921492_p114471302123"></a><a name="zh-cn_topic_0118921492_p114471302123"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p1646012304122"><a name="zh-cn_topic_0118921492_p1646012304122"></a><a name="zh-cn_topic_0118921492_p1646012304122"></a>关联的策略组合模式</p>
<a name="zh-cn_topic_0118921492_ul13466330121213"></a><a name="zh-cn_topic_0118921492_ul13466330121213"></a><ul id="zh-cn_topic_0118921492_ul13466330121213"><li>ALL</li><li>ANY</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1549719309124"><a name="zh-cn_topic_0118921492_p1549719309124"></a><a name="zh-cn_topic_0118921492_p1549719309124"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p105071430131214"><a name="zh-cn_topic_0118921492_p105071430131214"></a><a name="zh-cn_topic_0118921492_p105071430131214"></a>是</p>
</td>
</tr>
</tbody>
</table>

**表 9**  函数工作流策略后端对象模型

<a name="zh-cn_topic_0118921492_table147567512051"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row38049511555"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p58153517512"><a name="zh-cn_topic_0118921492_p58153517512"></a><a name="zh-cn_topic_0118921492_p58153517512"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p1382217511653"><a name="zh-cn_topic_0118921492_p1382217511653"></a><a name="zh-cn_topic_0118921492_p1382217511653"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p78314511252"><a name="zh-cn_topic_0118921492_p78314511252"></a><a name="zh-cn_topic_0118921492_p78314511252"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p283912511652"><a name="zh-cn_topic_0118921492_p283912511652"></a><a name="zh-cn_topic_0118921492_p283912511652"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p4848145110520"><a name="zh-cn_topic_0118921492_p4848145110520"></a><a name="zh-cn_topic_0118921492_p4848145110520"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row185719513519"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p15297184261113"><a name="zh-cn_topic_0118921492_p15297184261113"></a><a name="zh-cn_topic_0118921492_p15297184261113"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1630611425119"><a name="zh-cn_topic_0118921492_p1630611425119"></a><a name="zh-cn_topic_0118921492_p1630611425119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p173191342171116"><a name="zh-cn_topic_0118921492_p173191342171116"></a><a name="zh-cn_topic_0118921492_p173191342171116"></a>编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p8332124221118"><a name="zh-cn_topic_0118921492_p8332124221118"></a><a name="zh-cn_topic_0118921492_p8332124221118"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p163402425114"><a name="zh-cn_topic_0118921492_p163402425114"></a><a name="zh-cn_topic_0118921492_p163402425114"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row209145511055"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p14357642191114"><a name="zh-cn_topic_0118921492_p14357642191114"></a><a name="zh-cn_topic_0118921492_p14357642191114"></a>front_api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p163711542151113"><a name="zh-cn_topic_0118921492_p163711542151113"></a><a name="zh-cn_topic_0118921492_p163711542151113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p163841142111120"><a name="zh-cn_topic_0118921492_p163841142111120"></a><a name="zh-cn_topic_0118921492_p163841142111120"></a>对应的API编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p9392124217113"><a name="zh-cn_topic_0118921492_p9392124217113"></a><a name="zh-cn_topic_0118921492_p9392124217113"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p640818429111"><a name="zh-cn_topic_0118921492_p640818429111"></a><a name="zh-cn_topic_0118921492_p640818429111"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1496217512517"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1942674281120"><a name="zh-cn_topic_0118921492_p1942674281120"></a><a name="zh-cn_topic_0118921492_p1942674281120"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1043694219113"><a name="zh-cn_topic_0118921492_p1043694219113"></a><a name="zh-cn_topic_0118921492_p1043694219113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p24498429111"><a name="zh-cn_topic_0118921492_p24498429111"></a><a name="zh-cn_topic_0118921492_p24498429111"></a>策略后端名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1446634218115"><a name="zh-cn_topic_0118921492_p1446634218115"></a><a name="zh-cn_topic_0118921492_p1446634218115"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p6479194291117"><a name="zh-cn_topic_0118921492_p6479194291117"></a><a name="zh-cn_topic_0118921492_p6479194291117"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row9189520517"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p069511527499"><a name="zh-cn_topic_0118921492_p069511527499"></a><a name="zh-cn_topic_0118921492_p069511527499"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1369525218492"><a name="zh-cn_topic_0118921492_p1369525218492"></a><a name="zh-cn_topic_0118921492_p1369525218492"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p14695135254911"><a name="zh-cn_topic_0118921492_p14695135254911"></a><a name="zh-cn_topic_0118921492_p14695135254911"></a>函数版本号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1169515525492"><a name="zh-cn_topic_0118921492_p1169515525492"></a><a name="zh-cn_topic_0118921492_p1169515525492"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1696205234912"><a name="zh-cn_topic_0118921492_p1696205234912"></a><a name="zh-cn_topic_0118921492_p1696205234912"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row157495219519"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p469616525497"><a name="zh-cn_topic_0118921492_p469616525497"></a><a name="zh-cn_topic_0118921492_p469616525497"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p8696135234912"><a name="zh-cn_topic_0118921492_p8696135234912"></a><a name="zh-cn_topic_0118921492_p8696135234912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p19696115284920"><a name="zh-cn_topic_0118921492_p19696115284920"></a><a name="zh-cn_topic_0118921492_p19696115284920"></a>函数的URN</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p166964523491"><a name="zh-cn_topic_0118921492_p166964523491"></a><a name="zh-cn_topic_0118921492_p166964523491"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p669610521493"><a name="zh-cn_topic_0118921492_p669610521493"></a><a name="zh-cn_topic_0118921492_p669610521493"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row419511521259"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p36967525499"><a name="zh-cn_topic_0118921492_p36967525499"></a><a name="zh-cn_topic_0118921492_p36967525499"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1169645215492"><a name="zh-cn_topic_0118921492_p1169645215492"></a><a name="zh-cn_topic_0118921492_p1169645215492"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p869615244911"><a name="zh-cn_topic_0118921492_p869615244911"></a><a name="zh-cn_topic_0118921492_p869615244911"></a>函数类型：async|sync(异步|同步)</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p36961452204911"><a name="zh-cn_topic_0118921492_p36961452204911"></a><a name="zh-cn_topic_0118921492_p36961452204911"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1069675284917"><a name="zh-cn_topic_0118921492_p1069675284917"></a><a name="zh-cn_topic_0118921492_p1069675284917"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row729818521855"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p17697352174914"><a name="zh-cn_topic_0118921492_p17697352174914"></a><a name="zh-cn_topic_0118921492_p17697352174914"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1169775234919"><a name="zh-cn_topic_0118921492_p1169775234919"></a><a name="zh-cn_topic_0118921492_p1169775234919"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p8697852204915"><a name="zh-cn_topic_0118921492_p8697852204915"></a><a name="zh-cn_topic_0118921492_p8697852204915"></a>超时时间（1-60000），单位：毫秒</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p669775294915"><a name="zh-cn_topic_0118921492_p669775294915"></a><a name="zh-cn_topic_0118921492_p669775294915"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p19697135214914"><a name="zh-cn_topic_0118921492_p19697135214914"></a><a name="zh-cn_topic_0118921492_p19697135214914"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row7353452357"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p2318101211134"><a name="zh-cn_topic_0118921492_p2318101211134"></a><a name="zh-cn_topic_0118921492_p2318101211134"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p2333191216131"><a name="zh-cn_topic_0118921492_p2333191216131"></a><a name="zh-cn_topic_0118921492_p2333191216131"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p17355191291320"><a name="zh-cn_topic_0118921492_p17355191291320"></a><a name="zh-cn_topic_0118921492_p17355191291320"></a>关联的策略组合模式</p>
<a name="zh-cn_topic_0118921492_ul103629128139"></a><a name="zh-cn_topic_0118921492_ul103629128139"></a><ul id="zh-cn_topic_0118921492_ul103629128139"><li>ALL</li><li>ANY</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p040721281313"><a name="zh-cn_topic_0118921492_p040721281313"></a><a name="zh-cn_topic_0118921492_p040721281313"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p7421112191312"><a name="zh-cn_topic_0118921492_p7421112191312"></a><a name="zh-cn_topic_0118921492_p7421112191312"></a>是</p>
</td>
</tr>
</tbody>
</table>

**表 10**  策略后端条件对象模型

<a name="zh-cn_topic_0118921492_table35120550516"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row4570755259"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p4582185519518"><a name="zh-cn_topic_0118921492_p4582185519518"></a><a name="zh-cn_topic_0118921492_p4582185519518"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p19595055653"><a name="zh-cn_topic_0118921492_p19595055653"></a><a name="zh-cn_topic_0118921492_p19595055653"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p18611105512514"><a name="zh-cn_topic_0118921492_p18611105512514"></a><a name="zh-cn_topic_0118921492_p18611105512514"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p136234551654"><a name="zh-cn_topic_0118921492_p136234551654"></a><a name="zh-cn_topic_0118921492_p136234551654"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p2063517551153"><a name="zh-cn_topic_0118921492_p2063517551153"></a><a name="zh-cn_topic_0118921492_p2063517551153"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row76469551255"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1266719551658"><a name="zh-cn_topic_0118921492_p1266719551658"></a><a name="zh-cn_topic_0118921492_p1266719551658"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p26791155953"><a name="zh-cn_topic_0118921492_p26791155953"></a><a name="zh-cn_topic_0118921492_p26791155953"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p86904556515"><a name="zh-cn_topic_0118921492_p86904556515"></a><a name="zh-cn_topic_0118921492_p86904556515"></a>策略后端条件对象的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p17051558515"><a name="zh-cn_topic_0118921492_p17051558515"></a><a name="zh-cn_topic_0118921492_p17051558515"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p177215551515"><a name="zh-cn_topic_0118921492_p177215551515"></a><a name="zh-cn_topic_0118921492_p177215551515"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row10728175518513"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p2073965518514"><a name="zh-cn_topic_0118921492_p2073965518514"></a><a name="zh-cn_topic_0118921492_p2073965518514"></a>condition_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p175055515512"><a name="zh-cn_topic_0118921492_p175055515512"></a><a name="zh-cn_topic_0118921492_p175055515512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p11705174631510"><a name="zh-cn_topic_0118921492_p11705174631510"></a><a name="zh-cn_topic_0118921492_p11705174631510"></a>策略条件：</p>
<a name="zh-cn_topic_0118921492_ul1271254661514"></a><a name="zh-cn_topic_0118921492_ul1271254661514"></a><ul id="zh-cn_topic_0118921492_ul1271254661514"><li>exact：绝对匹配</li><li>enum：枚举</li><li>pattern：正则</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p17761855253"><a name="zh-cn_topic_0118921492_p17761855253"></a><a name="zh-cn_topic_0118921492_p17761855253"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p207892055558"><a name="zh-cn_topic_0118921492_p207892055558"></a><a name="zh-cn_topic_0118921492_p207892055558"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row157966558514"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1580917551453"><a name="zh-cn_topic_0118921492_p1580917551453"></a><a name="zh-cn_topic_0118921492_p1580917551453"></a>condition_value</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p981713551513"><a name="zh-cn_topic_0118921492_p981713551513"></a><a name="zh-cn_topic_0118921492_p981713551513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p138273551355"><a name="zh-cn_topic_0118921492_p138273551355"></a><a name="zh-cn_topic_0118921492_p138273551355"></a>策略值</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p1283920551157"><a name="zh-cn_topic_0118921492_p1283920551157"></a><a name="zh-cn_topic_0118921492_p1283920551157"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1850145512515"><a name="zh-cn_topic_0118921492_p1850145512515"></a><a name="zh-cn_topic_0118921492_p1850145512515"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row18854755456"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p148653552053"><a name="zh-cn_topic_0118921492_p148653552053"></a><a name="zh-cn_topic_0118921492_p148653552053"></a>condition_origin</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p108790551457"><a name="zh-cn_topic_0118921492_p108790551457"></a><a name="zh-cn_topic_0118921492_p108790551457"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p14407145781614"><a name="zh-cn_topic_0118921492_p14407145781614"></a><a name="zh-cn_topic_0118921492_p14407145781614"></a>策略类型：</p>
<a name="zh-cn_topic_0118921492_ul2041755781615"></a><a name="zh-cn_topic_0118921492_ul2041755781615"></a><ul id="zh-cn_topic_0118921492_ul2041755781615"><li>param：参数</li><li>source：源IP</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p590419551654"><a name="zh-cn_topic_0118921492_p590419551654"></a><a name="zh-cn_topic_0118921492_p590419551654"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p139200551057"><a name="zh-cn_topic_0118921492_p139200551057"></a><a name="zh-cn_topic_0118921492_p139200551057"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row1692616551159"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p1293513558519"><a name="zh-cn_topic_0118921492_p1293513558519"></a><a name="zh-cn_topic_0118921492_p1293513558519"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p4948115510510"><a name="zh-cn_topic_0118921492_p4948115510510"></a><a name="zh-cn_topic_0118921492_p4948115510510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p16184155119183"><a name="zh-cn_topic_0118921492_p16184155119183"></a><a name="zh-cn_topic_0118921492_p16184155119183"></a>关联的请求参数对象编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p116185613515"><a name="zh-cn_topic_0118921492_p116185613515"></a><a name="zh-cn_topic_0118921492_p116185613515"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p42685620519"><a name="zh-cn_topic_0118921492_p42685620519"></a><a name="zh-cn_topic_0118921492_p42685620519"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921492_row103310561456"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p174618561456"><a name="zh-cn_topic_0118921492_p174618561456"></a><a name="zh-cn_topic_0118921492_p174618561456"></a>policy_backend_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p205711561757"><a name="zh-cn_topic_0118921492_p205711561757"></a><a name="zh-cn_topic_0118921492_p205711561757"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p178385266186"><a name="zh-cn_topic_0118921492_p178385266186"></a><a name="zh-cn_topic_0118921492_p178385266186"></a>关联的策略后端对象编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p31214565510"><a name="zh-cn_topic_0118921492_p31214565510"></a><a name="zh-cn_topic_0118921492_p31214565510"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p191322561454"><a name="zh-cn_topic_0118921492_p191322561454"></a><a name="zh-cn_topic_0118921492_p191322561454"></a>是</p>
</td>
</tr>
</tbody>
</table>

**表 11**  认证方式参数对象模型

<a name="zh-cn_topic_0118921492_table17927144016249"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921492_row2092894072419"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0118921492_p692814013244"><a name="zh-cn_topic_0118921492_p692814013244"></a><a name="zh-cn_topic_0118921492_p692814013244"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0118921492_p6928154072413"><a name="zh-cn_topic_0118921492_p6928154072413"></a><a name="zh-cn_topic_0118921492_p6928154072413"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0118921492_p492864015248"><a name="zh-cn_topic_0118921492_p492864015248"></a><a name="zh-cn_topic_0118921492_p492864015248"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0118921492_p1492874017243"><a name="zh-cn_topic_0118921492_p1492874017243"></a><a name="zh-cn_topic_0118921492_p1492874017243"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0118921492_p11928204082413"><a name="zh-cn_topic_0118921492_p11928204082413"></a><a name="zh-cn_topic_0118921492_p11928204082413"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921492_row109281740152417"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0118921492_p59281140132410"><a name="zh-cn_topic_0118921492_p59281140132410"></a><a name="zh-cn_topic_0118921492_p59281140132410"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0118921492_p1092810400249"><a name="zh-cn_topic_0118921492_p1092810400249"></a><a name="zh-cn_topic_0118921492_p1092810400249"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0118921492_p15928340182414"><a name="zh-cn_topic_0118921492_p15928340182414"></a><a name="zh-cn_topic_0118921492_p15928340182414"></a>AppCode简易认证类型，仅在auth_type为APP时生效，默认为DISABLE：</p>
<a name="zh-cn_topic_0118921492_ul245955918358"></a><a name="zh-cn_topic_0118921492_ul245955918358"></a><ul id="zh-cn_topic_0118921492_ul245955918358"><li>DISABLE：不开启简易认证</li><li>HEADER：开启简易认证且AppCode位置在HEADER</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0118921492_p109289407244"><a name="zh-cn_topic_0118921492_p109289407244"></a><a name="zh-cn_topic_0118921492_p109289407244"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0118921492_p1992816403243"><a name="zh-cn_topic_0118921492_p1992816403243"></a><a name="zh-cn_topic_0118921492_p1992816403243"></a>-</p>
</td>
</tr>
</tbody>
</table>

