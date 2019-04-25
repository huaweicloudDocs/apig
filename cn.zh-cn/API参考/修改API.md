# 修改API<a name="apig-zh-api-180713026"></a>

## 功能介绍<a name="section50377025"></a>

修改指定API的信息，包括后端服务信息。

## URI<a name="section50740049"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table1300090"></a>
<table><thead align="left"><tr id="row35865770"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p19446229"><a name="p19446229"></a><a name="p19446229"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p31640721"><a name="p31640721"></a><a name="p31640721"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row12761605"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p27057114"><a name="p27057114"></a><a name="p27057114"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p44142648"><a name="p44142648"></a><a name="p44142648"></a>/v1.0/apigw/apis/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table18784710"></a>
<table><thead align="left"><tr id="row37287554"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p393051"><a name="p393051"></a><a name="p393051"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p31837140"><a name="p31837140"></a><a name="p31837140"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p28671509"><a name="p28671509"></a><a name="p28671509"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p40690887"><a name="p40690887"></a><a name="p40690887"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7627537"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p13850780"><a name="p13850780"></a><a name="p13850780"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p48171408"><a name="p48171408"></a><a name="p48171408"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p9569939"><a name="p9569939"></a><a name="p9569939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p36967632"><a name="p36967632"></a><a name="p36967632"></a>API的编号，可通过查询API信息获取该编号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section54007264"></a>

**表 3**  参数说明

<a name="table41588205"></a>
<table><thead align="left"><tr id="row17423813"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p2042781"><a name="p2042781"></a><a name="p2042781"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p31247557"><a name="p31247557"></a><a name="p31247557"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p48024165"><a name="p48024165"></a><a name="p48024165"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p64752166"><a name="p64752166"></a><a name="p64752166"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10434095"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p39855401"><a name="p39855401"></a><a name="p39855401"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p7062076"><a name="p7062076"></a><a name="p7062076"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p35157263"><a name="p35157263"></a><a name="p35157263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p29166026"><a name="p29166026"></a><a name="p29166026"></a>API所属分组的编号，该值不可修改</p>
</td>
</tr>
<tr id="row55632330"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9924849"><a name="p9924849"></a><a name="p9924849"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p65715325"><a name="p65715325"></a><a name="p65715325"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p21341142"><a name="p21341142"></a><a name="p21341142"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p50910947"><a name="p50910947"></a><a name="p50910947"></a>API名称</p>
<p id="p2879096"><a name="p2879096"></a><a name="p2879096"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以英文或中文开头</p>
<div class="note" id="note10265103111316"><a name="note10265103111316"></a><a name="note10265103111316"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p54875632"><a name="p54875632"></a><a name="p54875632"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row24118641"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p7452865"><a name="p7452865"></a><a name="p7452865"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p66811165"><a name="p66811165"></a><a name="p66811165"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p42995310"><a name="p42995310"></a><a name="p42995310"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p60068124"><a name="p60068124"></a><a name="p60068124"></a>API类型：</p>
<a name="ul51356896"></a><a name="ul51356896"></a><ul id="ul51356896"><li>1：公有API</li><li>2：私有API</li></ul>
</td>
</tr>
<tr id="row59540370"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p58040647"><a name="p58040647"></a><a name="p58040647"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p3671981"><a name="p3671981"></a><a name="p3671981"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p28995051"><a name="p28995051"></a><a name="p28995051"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p66897834"><a name="p66897834"></a><a name="p66897834"></a>API的版本</p>
<p id="p924416521436"><a name="p924416521436"></a><a name="p924416521436"></a>字符长度不超过16</p>
</td>
</tr>
<tr id="row47486372"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p21190939"><a name="p21190939"></a><a name="p21190939"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p38744527"><a name="p38744527"></a><a name="p38744527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p51298983"><a name="p51298983"></a><a name="p51298983"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p61576972"><a name="p61576972"></a><a name="p61576972"></a>API的请求协议：</p>
<a name="ul31064853"></a><a name="ul31064853"></a><ul id="ul31064853"><li>HTTP</li><li>HTTPS</li><li>BOTH：同时支持HTTP和HTTPS</li><li>WEBSOCKET</li></ul>
<p id="p61941807"><a name="p61941807"></a><a name="p61941807"></a>默认：HTTPS</p>
</td>
</tr>
<tr id="row20605358"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p58421322"><a name="p58421322"></a><a name="p58421322"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p34506675"><a name="p34506675"></a><a name="p34506675"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p43577296"><a name="p43577296"></a><a name="p43577296"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p40100106"><a name="p40100106"></a><a name="p40100106"></a>API的请求方式：</p>
<a name="ul18216690"></a><a name="ul18216690"></a><ul id="ul18216690"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
</tr>
<tr id="row31204027"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p44498278"><a name="p44498278"></a><a name="p44498278"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p47590778"><a name="p47590778"></a><a name="p47590778"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p29647773"><a name="p29647773"></a><a name="p29647773"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p52659450"><a name="p52659450"></a><a name="p52659450"></a>API的访问地址</p>
<div class="note" id="note16810141640"><a name="note16810141640"></a><a name="note16810141640"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p208115144418"><a name="p208115144418"></a><a name="p208115144418"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="row55147378"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p37752640"><a name="p37752640"></a><a name="p37752640"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p38065039"><a name="p38065039"></a><a name="p38065039"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p63369351"><a name="p63369351"></a><a name="p63369351"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p32643791"><a name="p32643791"></a><a name="p32643791"></a>API的匹配方式：</p>
<a name="ul3718041"></a><a name="ul3718041"></a><ul id="ul3718041"><li>SWA：前缀匹配</li><li>NORMAL：正常匹配（绝对匹配）<p id="p62092040102910"><a name="p62092040102910"></a><a name="p62092040102910"></a>默认：NORMAL</p>
</li></ul>
</td>
</tr>
<tr id="row26098002"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p33563416"><a name="p33563416"></a><a name="p33563416"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p34282146"><a name="p34282146"></a><a name="p34282146"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p25390424"><a name="p25390424"></a><a name="p25390424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p43358500"><a name="p43358500"></a><a name="p43358500"></a>API描述</p>
<p id="p71625"><a name="p71625"></a><a name="p71625"></a>长度不超过255个字符</p>
<div class="note" id="note16618220512"><a name="note16618220512"></a><a name="note16618220512"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1468102850"><a name="p1468102850"></a><a name="p1468102850"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row60184071"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p43071573"><a name="p43071573"></a><a name="p43071573"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p66245392"><a name="p66245392"></a><a name="p66245392"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p64276511"><a name="p64276511"></a><a name="p64276511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p39014891"><a name="p39014891"></a><a name="p39014891"></a>API认证方式：</p>
<a name="ul13321616"></a><a name="ul13321616"></a><ul id="ul13321616"><li>NONE：无认证</li><li>APP：APP认证</li><li>IAM：IAM认证</li></ul>
</td>
</tr>
<tr id="row27386479"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p3712290"><a name="p3712290"></a><a name="p3712290"></a>backend_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p32260111"><a name="p32260111"></a><a name="p32260111"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p62932188"><a name="p62932188"></a><a name="p62932188"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p64342449"><a name="p64342449"></a><a name="p64342449"></a>后端类型：</p>
<a name="ul63658740"></a><a name="ul63658740"></a><ul id="ul63658740"><li>HTTP：web后端</li><li>FUNCTION：函数工作流</li><li>MOCK：mock</li></ul>
</td>
</tr>
<tr id="row1775863173118"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p45893752117"><a name="p45893752117"></a><a name="p45893752117"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p105895719216"><a name="p105895719216"></a><a name="p105895719216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p18589147152113"><a name="p18589147152113"></a><a name="p18589147152113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p17891448182114"><a name="p17891448182114"></a><a name="p17891448182114"></a>标签</p>
<p id="p17589774213"><a name="p17589774213"></a><a name="p17589774213"></a>可以打servicename的标签和其他标签</p>
</td>
</tr>
<tr id="row1182119710316"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p526201042116"><a name="p526201042116"></a><a name="p526201042116"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1426191062120"><a name="p1426191062120"></a><a name="p1426191062120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p726151042117"><a name="p726151042117"></a><a name="p726151042117"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p7213201015015"><a name="p7213201015015"></a><a name="p7213201015015"></a>是否支持跨域</p>
<a name="ul38673529507"></a><a name="ul38673529507"></a><ul id="ul38673529507"><li>TRUE：支持</li><li>FALSE：不支持</li></ul>
<p id="p17882165245011"><a name="p17882165245011"></a><a name="p17882165245011"></a>默认：FALSE</p>
</td>
</tr>
<tr id="row68451678328"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p59931303198"><a name="p59931303198"></a><a name="p59931303198"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p912844617206"><a name="p912844617206"></a><a name="p912844617206"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p79937041913"><a name="p79937041913"></a><a name="p79937041913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p148471111162112"><a name="p148471111162112"></a><a name="p148471111162112"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
<p id="p984751162120"><a name="p984751162120"></a><a name="p984751162120"></a>字符长度不超过20480</p>
<div class="note" id="note986331142110"><a name="note986331142110"></a><a name="note986331142110"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1686314115212"><a name="p1686314115212"></a><a name="p1686314115212"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row1289251118323"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p5946166161919"><a name="p5946166161919"></a><a name="p5946166161919"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p10946136161918"><a name="p10946136161918"></a><a name="p10946136161918"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p19461065195"><a name="p19461065195"></a><a name="p19461065195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p7946166193"><a name="p7946166193"></a><a name="p7946166193"></a>正常响应示例，描述API的正常返回信息</p>
<p id="p1935514810223"><a name="p1935514810223"></a><a name="p1935514810223"></a>字符长度不超过20480</p>
<div class="note" id="note1649674102319"><a name="note1649674102319"></a><a name="note1649674102319"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p165129415232"><a name="p165129415232"></a><a name="p165129415232"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row38452142325"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p727431112199"><a name="p727431112199"></a><a name="p727431112199"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p142741211171914"><a name="p142741211171914"></a><a name="p142741211171914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p18274181181910"><a name="p18274181181910"></a><a name="p18274181181910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1227471181914"><a name="p1227471181914"></a><a name="p1227471181914"></a>失败返回示例，描述API的异常返回信息</p>
<p id="p132518115249"><a name="p132518115249"></a><a name="p132518115249"></a>字符长度不超过20480</p>
<div class="note" id="note13283119202415"><a name="note13283119202415"></a><a name="note13283119202415"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p23141919202413"><a name="p23141919202413"></a><a name="p23141919202413"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row46533916"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p11150814"><a name="p11150814"></a><a name="p11150814"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p30800757"><a name="p30800757"></a><a name="p30800757"></a>backend_type = HTTP时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p11833417"><a name="p11833417"></a><a name="p11833417"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p18982721"><a name="p18982721"></a><a name="p18982721"></a>web后端详情</p>
</td>
</tr>
<tr id="row13978104"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p58484667"><a name="p58484667"></a><a name="p58484667"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p39637566"><a name="p39637566"></a><a name="p39637566"></a>backend_type = MOCK时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p56526249"><a name="p56526249"></a><a name="p56526249"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p15223461"><a name="p15223461"></a><a name="p15223461"></a>mock后端详情</p>
</td>
</tr>
<tr id="row24940840"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p6942180"><a name="p6942180"></a><a name="p6942180"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p25445741"><a name="p25445741"></a><a name="p25445741"></a>backend_type = FUNCTION时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p47839146"><a name="p47839146"></a><a name="p47839146"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p49765636"><a name="p49765636"></a><a name="p49765636"></a>函数工作流后端详情</p>
</td>
</tr>
<tr id="row16615151932917"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p156831806524"><a name="p156831806524"></a><a name="p156831806524"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p76831801527"><a name="p76831801527"></a><a name="p76831801527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p176831903520"><a name="p176831903520"></a><a name="p176831903520"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p468350195218"><a name="p468350195218"></a><a name="p468350195218"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="row1713042311290"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p06884014357"><a name="p06884014357"></a><a name="p06884014357"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p46814011357"><a name="p46814011357"></a><a name="p46814011357"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p17681640163511"><a name="p17681640163511"></a><a name="p17681640163511"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p76844033510"><a name="p76844033510"></a><a name="p76844033510"></a>API的后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  backend\_api参数说明

<a name="table40362358"></a>
<table><thead align="left"><tr id="row52890857"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p56301019"><a name="p56301019"></a><a name="p56301019"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p64088677"><a name="p64088677"></a><a name="p64088677"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p23800368"><a name="p23800368"></a><a name="p23800368"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p48781668"><a name="p48781668"></a><a name="p48781668"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row59000999"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p14351652"><a name="p14351652"></a><a name="p14351652"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1741473216910"><a name="p1741473216910"></a><a name="p1741473216910"></a>后端服务不使用VPC通道时，必选</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p7454950"><a name="p7454950"></a><a name="p7454950"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p44366800"><a name="p44366800"></a><a name="p44366800"></a>后端的Endpoint。</p>
<p id="p9406451538"><a name="p9406451538"></a><a name="p9406451538"></a>由域名（或IP地址）和端口号组成，总长度不超过255。格式为域名:端口（如：apig.huaweicloud.com:7443）。如果不写端口，则HTTPS默认端口号为443， HTTP默认端口号为80。</p>
<p id="p13446109556"><a name="p13446109556"></a><a name="p13446109556"></a>支持环境变量，使用环境变量时，每个变量名的长度为3 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="row40343362"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p46586921"><a name="p46586921"></a><a name="p46586921"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p15444219"><a name="p15444219"></a><a name="p15444219"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p43022242"><a name="p43022242"></a><a name="p43022242"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p62249606"><a name="p62249606"></a><a name="p62249606"></a>web后端版本</p>
<p id="p47092214417"><a name="p47092214417"></a><a name="p47092214417"></a>字符长度不超过16</p>
</td>
</tr>
<tr id="row14371075"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p23206461"><a name="p23206461"></a><a name="p23206461"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p675216"><a name="p675216"></a><a name="p675216"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p54692515"><a name="p54692515"></a><a name="p54692515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p908702"><a name="p908702"></a><a name="p908702"></a>请求协议：</p>
<a name="ul6405907"></a><a name="ul6405907"></a><ul id="ul6405907"><li>HTTP</li><li>HTTPS</li></ul>
</td>
</tr>
<tr id="row39395146"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p36890263"><a name="p36890263"></a><a name="p36890263"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p35321345"><a name="p35321345"></a><a name="p35321345"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p42456687"><a name="p42456687"></a><a name="p42456687"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p16439626"><a name="p16439626"></a><a name="p16439626"></a>请求方式：</p>
<a name="ul56813045"></a><a name="ul56813045"></a><ul id="ul56813045"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
</tr>
<tr id="row52269657"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p5983788"><a name="p5983788"></a><a name="p5983788"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p14924857"><a name="p14924857"></a><a name="p14924857"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p953894"><a name="p953894"></a><a name="p953894"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p10156571"><a name="p10156571"></a><a name="p10156571"></a>请求地址</p>
<div class="note" id="note198842412618"><a name="note198842412618"></a><a name="note198842412618"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p13887844620"><a name="p13887844620"></a><a name="p13887844620"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="row52675390"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p38848230"><a name="p38848230"></a><a name="p38848230"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p59698910"><a name="p59698910"></a><a name="p59698910"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p3773518"><a name="p3773518"></a><a name="p3773518"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p37219551"><a name="p37219551"></a><a name="p37219551"></a>API网关请求后端服务的超时时间，最大60000，最小为1</p>
<p id="p21072000"><a name="p21072000"></a><a name="p21072000"></a>单位：毫秒</p>
<p id="p60667237"><a name="p60667237"></a><a name="p60667237"></a>默认值：45000，请求参数值不在合法范围内时将使用默认值</p>
</td>
</tr>
<tr id="row1674569"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p1422383"><a name="p1422383"></a><a name="p1422383"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p48104235"><a name="p48104235"></a><a name="p48104235"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p4128930"><a name="p4128930"></a><a name="p4128930"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p66007934"><a name="p66007934"></a><a name="p66007934"></a>描述</p>
<p id="p2729060"><a name="p2729060"></a><a name="p2729060"></a>字符长度不超过255</p>
<div class="note" id="note932694220620"><a name="note932694220620"></a><a name="note932694220620"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p33281542563"><a name="p33281542563"></a><a name="p33281542563"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row169831"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p13756326"><a name="p13756326"></a><a name="p13756326"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p40520610"><a name="p40520610"></a><a name="p40520610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p60943938"><a name="p60943938"></a><a name="p60943938"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p37511918"><a name="p37511918"></a><a name="p37511918"></a>是否使用VPC通道：</p>
<a name="ul12506831"></a><a name="ul12506831"></a><ul id="ul12506831"><li>1 : 使用VPC通道</li><li>2 : 不使用VPC通道</li></ul>
</td>
</tr>
<tr id="row57783729"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p49970510"><a name="p49970510"></a><a name="p49970510"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p21079499"><a name="p21079499"></a><a name="p21079499"></a>如果vpc_status=1，则这个字典类型为必填信息</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p29717840"><a name="p29717840"></a><a name="p29717840"></a>字典类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p58334854"><a name="p58334854"></a><a name="p58334854"></a>VPC通道详情</p>
</td>
</tr>
</tbody>
</table>

**表 5**  VPC通道参数说明

<a name="table46198076"></a>
<table><thead align="left"><tr id="row37332224"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p4011304"><a name="p4011304"></a><a name="p4011304"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p56480221"><a name="p56480221"></a><a name="p56480221"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p11495174"><a name="p11495174"></a><a name="p11495174"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p58693900"><a name="p58693900"></a><a name="p58693900"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row56585430"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p102891318101116"><a name="p102891318101116"></a><a name="p102891318101116"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p10772440"><a name="p10772440"></a><a name="p10772440"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p152415"><a name="p152415"></a><a name="p152415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p12345675"><a name="p12345675"></a><a name="p12345675"></a>VPC通道编号</p>
</td>
</tr>
<tr id="row7409961"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p87859454111"><a name="p87859454111"></a><a name="p87859454111"></a>vpc_proxy_host</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p29937110"><a name="p29937110"></a><a name="p29937110"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p8986837"><a name="p8986837"></a><a name="p8986837"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1117285801112"><a name="p1117285801112"></a><a name="p1117285801112"></a>代理主机</p>
</td>
</tr>
<tr id="row516664612910"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p723065121617"><a name="p723065121617"></a><a name="p723065121617"></a>vpc_port</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1230135110165"><a name="p1230135110165"></a><a name="p1230135110165"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p17230851131610"><a name="p17230851131610"></a><a name="p17230851131610"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1423019510164"><a name="p1423019510164"></a><a name="p1423019510164"></a>VPC通道端口</p>
<p id="p06918365413"><a name="p06918365413"></a><a name="p06918365413"></a>私网ELB类型通道时必选，用来指定ELB实例的监听器端口</p>
</td>
</tr>
</tbody>
</table>

**表 6**  mock\_info参数说明

<a name="table33997535"></a>
<table><thead align="left"><tr id="row13765642"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p41275228"><a name="p41275228"></a><a name="p41275228"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p54959195"><a name="p54959195"></a><a name="p54959195"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p22509806"><a name="p22509806"></a><a name="p22509806"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p11355006"><a name="p11355006"></a><a name="p11355006"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row47340274"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9356979"><a name="p9356979"></a><a name="p9356979"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p19717800"><a name="p19717800"></a><a name="p19717800"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p53637945"><a name="p53637945"></a><a name="p53637945"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p49706320"><a name="p49706320"></a><a name="p49706320"></a>返回结果</p>
</td>
</tr>
<tr id="row64229608"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p35215736"><a name="p35215736"></a><a name="p35215736"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p33902377"><a name="p33902377"></a><a name="p33902377"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p61738018"><a name="p61738018"></a><a name="p61738018"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p34723596"><a name="p34723596"></a><a name="p34723596"></a>版本</p>
<p id="p20141184418"><a name="p20141184418"></a><a name="p20141184418"></a>字符长度不超过64</p>
</td>
</tr>
<tr id="row13460361"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p16547427"><a name="p16547427"></a><a name="p16547427"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p65273193"><a name="p65273193"></a><a name="p65273193"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p52637317"><a name="p52637317"></a><a name="p52637317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p35764252"><a name="p35764252"></a><a name="p35764252"></a>描述信息</p>
<p id="p33901024"><a name="p33901024"></a><a name="p33901024"></a>长度不超过255个字符</p>
<div class="note" id="note1163818251979"><a name="note1163818251979"></a><a name="note1163818251979"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p56381525274"><a name="p56381525274"></a><a name="p56381525274"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

**表 7**  func\_info参数说明

<a name="table50018966"></a>
<table><thead align="left"><tr id="row29103324"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p8559016"><a name="p8559016"></a><a name="p8559016"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p22191721"><a name="p22191721"></a><a name="p22191721"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p52699015"><a name="p52699015"></a><a name="p52699015"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p40761833"><a name="p40761833"></a><a name="p40761833"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13374200"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9568411"><a name="p9568411"></a><a name="p9568411"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p36843835"><a name="p36843835"></a><a name="p36843835"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p31560639"><a name="p31560639"></a><a name="p31560639"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p6274960"><a name="p6274960"></a><a name="p6274960"></a>函数URN</p>
</td>
</tr>
<tr id="row11043134"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p22078701"><a name="p22078701"></a><a name="p22078701"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p43544389"><a name="p43544389"></a><a name="p43544389"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p37434605"><a name="p37434605"></a><a name="p37434605"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p12304141"><a name="p12304141"></a><a name="p12304141"></a>调用类型:async|sync （异步|同步）</p>
</td>
</tr>
<tr id="row44240322"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p26696343"><a name="p26696343"></a><a name="p26696343"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p14920160"><a name="p14920160"></a><a name="p14920160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p573446"><a name="p573446"></a><a name="p573446"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p3582515183214"><a name="p3582515183214"></a><a name="p3582515183214"></a>API网关请求函数服务的超时时间，最大60000，最小为1</p>
<p id="p2597131514329"><a name="p2597131514329"></a><a name="p2597131514329"></a>单位：毫秒</p>
<p id="p136134155324"><a name="p136134155324"></a><a name="p136134155324"></a>默认值：45000，请求参数值不在合法范围内时将使用默认值</p>
</td>
</tr>
<tr id="row38552894"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p35776706"><a name="p35776706"></a><a name="p35776706"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p12232103"><a name="p12232103"></a><a name="p12232103"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p51276309"><a name="p51276309"></a><a name="p51276309"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p59740339"><a name="p59740339"></a><a name="p59740339"></a>版本信息</p>
<p id="p1036981824412"><a name="p1036981824412"></a><a name="p1036981824412"></a>字符长度不超过64</p>
</td>
</tr>
<tr id="row64163317"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p29846179"><a name="p29846179"></a><a name="p29846179"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1621438"><a name="p1621438"></a><a name="p1621438"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p64227629"><a name="p64227629"></a><a name="p64227629"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p89323561178"><a name="p89323561178"></a><a name="p89323561178"></a>描述信息</p>
<p id="p35055449"><a name="p35055449"></a><a name="p35055449"></a>长度不超过255个字符</p>
<div class="note" id="note5319001980"><a name="note5319001980"></a><a name="note5319001980"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p732040885"><a name="p732040885"></a><a name="p732040885"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

**表 8**  req\_params参数说明

<a name="table10797815193916"></a>
<table><thead align="left"><tr id="row178141315123910"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p1981481518391"><a name="p1981481518391"></a><a name="p1981481518391"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p13828101511398"><a name="p13828101511398"></a><a name="p13828101511398"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p08281415143912"><a name="p08281415143912"></a><a name="p08281415143912"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p15828131523915"><a name="p15828131523915"></a><a name="p15828131523915"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row118441515123919"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p984461512398"><a name="p984461512398"></a><a name="p984461512398"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1184451593913"><a name="p1184451593913"></a><a name="p1184451593913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1184411517393"><a name="p1184411517393"></a><a name="p1184411517393"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p18861315153916"><a name="p18861315153916"></a><a name="p18861315153916"></a>参数名称</p>
<p id="p68611515103916"><a name="p68611515103916"></a><a name="p68611515103916"></a>长度为1 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”、“.”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="row8861131510391"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p987641512396"><a name="p987641512396"></a><a name="p987641512396"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p48761915133913"><a name="p48761915133913"></a><a name="p48761915133913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p178764154394"><a name="p178764154394"></a><a name="p178764154394"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p13891161513393"><a name="p13891161513393"></a><a name="p13891161513393"></a>参数类型：</p>
<a name="ul1830218285513"></a><a name="ul1830218285513"></a><ul id="ul1830218285513"><li>STRING</li><li>NUMBER</li></ul>
</td>
</tr>
<tr id="row5891181553918"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p4891111513399"><a name="p4891111513399"></a><a name="p4891111513399"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p989171593919"><a name="p989171593919"></a><a name="p989171593919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p29076155393"><a name="p29076155393"></a><a name="p29076155393"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1490710153393"><a name="p1490710153393"></a><a name="p1490710153393"></a>参数位置：</p>
<a name="ul1690715155390"></a><a name="ul1690715155390"></a><ul id="ul1690715155390"><li>PATH</li><li>QUERY</li><li>HEADER</li></ul>
</td>
</tr>
<tr id="row159222154399"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p4922181511396"><a name="p4922181511396"></a><a name="p4922181511396"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p12939101543910"><a name="p12939101543910"></a><a name="p12939101543910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p12939101513914"><a name="p12939101513914"></a><a name="p12939101513914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1795414270226"><a name="p1795414270226"></a><a name="p1795414270226"></a>参数默认值</p>
</td>
</tr>
<tr id="row14091614391"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p301516133917"><a name="p301516133917"></a><a name="p301516133917"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p20116173911"><a name="p20116173911"></a><a name="p20116173911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p19161116173915"><a name="p19161116173915"></a><a name="p19161116173915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p3265191616229"><a name="p3265191616229"></a><a name="p3265191616229"></a>参数示例值</p>
</td>
</tr>
<tr id="row1832121613917"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p113212160395"><a name="p113212160395"></a><a name="p113212160395"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p3471216103914"><a name="p3471216103914"></a><a name="p3471216103914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p74716163396"><a name="p74716163396"></a><a name="p74716163396"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1126481992116"><a name="p1126481992116"></a><a name="p1126481992116"></a>是否必须：</p>
<a name="ul32801119142116"></a><a name="ul32801119142116"></a><ul id="ul32801119142116"><li>1：是</li><li>2：否</li></ul>
</td>
</tr>
<tr id="row36310168394"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p1363181683919"><a name="p1363181683919"></a><a name="p1363181683919"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p167919163391"><a name="p167919163391"></a><a name="p167919163391"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p47961614392"><a name="p47961614392"></a><a name="p47961614392"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1779716173917"><a name="p1779716173917"></a><a name="p1779716173917"></a>是否开启校验：</p>
<a name="ul1867752852019"></a><a name="ul1867752852019"></a><ul id="ul1867752852019"><li>1：开启校验</li><li>2：不开启校验</li></ul>
</td>
</tr>
<tr id="row7942166394"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p1894816193914"><a name="p1894816193914"></a><a name="p1894816193914"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p294171616395"><a name="p294171616395"></a><a name="p294171616395"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p8111916163917"><a name="p8111916163917"></a><a name="p8111916163917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p189891816181817"><a name="p189891816181817"></a><a name="p189891816181817"></a>描述</p>
<p id="p139892166189"><a name="p139892166189"></a><a name="p139892166189"></a>字符长度不超过255</p>
<div class="note" id="note135191711818"><a name="note135191711818"></a><a name="note135191711818"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p105317181816"><a name="p105317181816"></a><a name="p105317181816"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row13126201633917"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p1314181643914"><a name="p1314181643914"></a><a name="p1314181643914"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p814191615397"><a name="p814191615397"></a><a name="p814191615397"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p71411168392"><a name="p71411168392"></a><a name="p71411168392"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p2559522184412"><a name="p2559522184412"></a><a name="p2559522184412"></a>参数枚举值</p>
</td>
</tr>
<tr id="row878217618128"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p1778211616128"><a name="p1778211616128"></a><a name="p1778211616128"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p10782563129"><a name="p10782563129"></a><a name="p10782563129"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p178213613128"><a name="p178213613128"></a><a name="p178213613128"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p95973228446"><a name="p95973228446"></a><a name="p95973228446"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row1242311108123"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p154235102129"><a name="p154235102129"></a><a name="p154235102129"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p3423141081212"><a name="p3423141081212"></a><a name="p3423141081212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1442316104122"><a name="p1442316104122"></a><a name="p1442316104122"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p2631222104413"><a name="p2631222104413"></a><a name="p2631222104413"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row21901721131212"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9190321131218"><a name="p9190321131218"></a><a name="p9190321131218"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p7190162117128"><a name="p7190162117128"></a><a name="p7190162117128"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1619082112121"><a name="p1619082112121"></a><a name="p1619082112121"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p2668152294420"><a name="p2668152294420"></a><a name="p2668152294420"></a>参数最小长度</p>
</td>
</tr>
<tr id="row192351217191211"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p182351717171210"><a name="p182351717171210"></a><a name="p182351717171210"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p11235151717124"><a name="p11235151717124"></a><a name="p11235151717124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p20235181721217"><a name="p20235181721217"></a><a name="p20235181721217"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p3702522184416"><a name="p3702522184416"></a><a name="p3702522184416"></a>参数最大长度</p>
</td>
</tr>
<tr id="row222041311121"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p10220131331219"><a name="p10220131331219"></a><a name="p10220131331219"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1220131331211"><a name="p1220131331211"></a><a name="p1220131331211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1122017131128"><a name="p1122017131128"></a><a name="p1122017131128"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p12731822184412"><a name="p12731822184412"></a><a name="p12731822184412"></a>正则校验规则（暂不支持）</p>
</td>
</tr>
<tr id="row177506146139"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p197501614181317"><a name="p197501614181317"></a><a name="p197501614181317"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1975091410132"><a name="p1975091410132"></a><a name="p1975091410132"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1275091417134"><a name="p1275091417134"></a><a name="p1275091417134"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p57661222144411"><a name="p57661222144411"></a><a name="p57661222144411"></a>JSON校验规则（暂不支持）</p>
</td>
</tr>
</tbody>
</table>

**表 9**  backend\_params参数说明

<a name="table599625352311"></a>
<table><thead align="left"><tr id="row161185472312"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p2271054112313"><a name="p2271054112313"></a><a name="p2271054112313"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p0271154112315"><a name="p0271154112315"></a><a name="p0271154112315"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p11431854112316"><a name="p11431854112316"></a><a name="p11431854112316"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p1543354162315"><a name="p1543354162315"></a><a name="p1543354162315"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row543125416231"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p195875452310"><a name="p195875452310"></a><a name="p195875452310"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p7581354112312"><a name="p7581354112312"></a><a name="p7581354112312"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p458154112315"><a name="p458154112315"></a><a name="p458154112315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1775554132310"><a name="p1775554132310"></a><a name="p1775554132310"></a>参数名称</p>
<p id="p67518541235"><a name="p67518541235"></a><a name="p67518541235"></a>长度为1 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”、“.”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="row191211554142315"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p17121854112318"><a name="p17121854112318"></a><a name="p17121854112318"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p412115419233"><a name="p412115419233"></a><a name="p412115419233"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1213720544234"><a name="p1213720544234"></a><a name="p1213720544234"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p91371054102314"><a name="p91371054102314"></a><a name="p91371054102314"></a>参数位置：</p>
<a name="ul19137754162316"></a><a name="ul19137754162316"></a><ul id="ul19137754162316"><li>PATH</li><li>QUERY</li><li>HEADER</li></ul>
</td>
</tr>
<tr id="row15230654192316"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p12230205492317"><a name="p12230205492317"></a><a name="p12230205492317"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p10230145415237"><a name="p10230145415237"></a><a name="p10230145415237"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p724735411231"><a name="p724735411231"></a><a name="p724735411231"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1524775413233"><a name="p1524775413233"></a><a name="p1524775413233"></a>参数类别：</p>
<a name="ul1124735482312"></a><a name="ul1124735482312"></a><ul id="ul1124735482312"><li>REQUEST</li><li>CONSTANT</li><li>SYSTEM</li></ul>
</td>
</tr>
<tr id="row15261254202320"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9261954122310"><a name="p9261954122310"></a><a name="p9261954122310"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1427715452315"><a name="p1427715452315"></a><a name="p1427715452315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p17277155419233"><a name="p17277155419233"></a><a name="p17277155419233"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p657172452818"><a name="p657172452818"></a><a name="p657172452818"></a>参数值</p>
<p id="p110811324312"><a name="p110811324312"></a><a name="p110811324312"></a>字符长度不超过255</p>
<p id="p13947355152811"><a name="p13947355152811"></a><a name="p13947355152811"></a>类别为REQUEST时，值为requestParameters中的参数名称；</p>
<p id="p365913371295"><a name="p365913371295"></a><a name="p365913371295"></a>类别为CONSTANT时，值为参数真正的值；</p>
<p id="p25181013162915"><a name="p25181013162915"></a><a name="p25181013162915"></a>类别为SYSTEM时，值为网关参数名称</p>
</td>
</tr>
<tr id="row1229318545230"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p53088549232"><a name="p53088549232"></a><a name="p53088549232"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p193081654182316"><a name="p193081654182316"></a><a name="p193081654182316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p8324354112310"><a name="p8324354112310"></a><a name="p8324354112310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p183241554122314"><a name="p183241554122314"></a><a name="p183241554122314"></a>描述</p>
<p id="p2324125492316"><a name="p2324125492316"></a><a name="p2324125492316"></a>字符长度不超过255</p>
<div class="note" id="note8324854142312"><a name="note8324854142312"></a><a name="note8324854142312"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p3340125492316"><a name="p3340125492316"></a><a name="p3340125492316"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "auth_type": "app",
  "backend_api": {
    "req_method": "get",
    "req_protocol": "http",
    "req_uri": "/test",
    "timeout": 1000,
    "url_domain": "xxxxxxxxx"
  },
  "backend_params": [
    {
      "location": "query",
      "name": "project_id",
      "origin": "request",
      "value": "project_id"
    },
    {
      "location": "query",
      "name": "city",
      "origin": "request",
      "value": "city"
    }
  ],
  "backend_type": "http",
  "group_id": "f71f69876f90456ca6fd18ed012fdc11",
  "name": "test",
  "req_method": "get",
  "req_params": [
    {
      "location": "path",
      "name": "project_id",
      "required": 1,
      "type": "string"
    },
    {
      "location": "query",
      "name": "city",
      "required": 2,
      "type": "string"
    }
  ],
  "req_uri": "/test/{project_id}",
  "tag": "test",
  "type": 1,
  "result_normal_sample": "hello world!"
}
```

## 响应消息<a name="section12512296"></a>

**表 10**  参数说明

<a name="table32709465"></a>
<table><thead align="left"><tr id="row14547639"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p37508143"><a name="p37508143"></a><a name="p37508143"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p18260727"><a name="p18260727"></a><a name="p18260727"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p2723895"><a name="p2723895"></a><a name="p2723895"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row19308952"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20521281"><a name="p20521281"></a><a name="p20521281"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51611099"><a name="p51611099"></a><a name="p51611099"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p19749518"><a name="p19749518"></a><a name="p19749518"></a>API编号</p>
</td>
</tr>
<tr id="row43527936"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p36101898"><a name="p36101898"></a><a name="p36101898"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p38572608"><a name="p38572608"></a><a name="p38572608"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p37373580"><a name="p37373580"></a><a name="p37373580"></a>API名称</p>
</td>
</tr>
<tr id="row817900"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p66249969"><a name="p66249969"></a><a name="p66249969"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64647295"><a name="p64647295"></a><a name="p64647295"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1939517"><a name="p1939517"></a><a name="p1939517"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row17455653"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4621807"><a name="p4621807"></a><a name="p4621807"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p38822077"><a name="p38822077"></a><a name="p38822077"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57580536"><a name="p57580536"></a><a name="p57580536"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row48462777"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p33170882"><a name="p33170882"></a><a name="p33170882"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2486891"><a name="p2486891"></a><a name="p2486891"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p111580"><a name="p111580"></a><a name="p111580"></a>API的状态</p>
</td>
</tr>
<tr id="row1004223"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14233264"><a name="p14233264"></a><a name="p14233264"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12043774"><a name="p12043774"></a><a name="p12043774"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36021648"><a name="p36021648"></a><a name="p36021648"></a>API类型</p>
</td>
</tr>
<tr id="row55759383"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20216138"><a name="p20216138"></a><a name="p20216138"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p26894519"><a name="p26894519"></a><a name="p26894519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30972420"><a name="p30972420"></a><a name="p30972420"></a>API版本</p>
</td>
</tr>
<tr id="row10316326"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p30316071"><a name="p30316071"></a><a name="p30316071"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p39682652"><a name="p39682652"></a><a name="p39682652"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60178221"><a name="p60178221"></a><a name="p60178221"></a>API访问协议</p>
</td>
</tr>
<tr id="row4733084"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47835556"><a name="p47835556"></a><a name="p47835556"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p49474812"><a name="p49474812"></a><a name="p49474812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48036812"><a name="p48036812"></a><a name="p48036812"></a>API请求方式</p>
</td>
</tr>
<tr id="row29678129"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55118249"><a name="p55118249"></a><a name="p55118249"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35393198"><a name="p35393198"></a><a name="p35393198"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48276775"><a name="p48276775"></a><a name="p48276775"></a>API访问地址</p>
</td>
</tr>
<tr id="row31837795"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28724582"><a name="p28724582"></a><a name="p28724582"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p44989777"><a name="p44989777"></a><a name="p44989777"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20293325"><a name="p20293325"></a><a name="p20293325"></a>API认证方式</p>
</td>
</tr>
<tr id="row48422201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p29884176"><a name="p29884176"></a><a name="p29884176"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4699212"><a name="p4699212"></a><a name="p4699212"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p45091925"><a name="p45091925"></a><a name="p45091925"></a>API匹配方式</p>
</td>
</tr>
<tr id="row3174146"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55779240"><a name="p55779240"></a><a name="p55779240"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p21824591"><a name="p21824591"></a><a name="p21824591"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p22961438"><a name="p22961438"></a><a name="p22961438"></a>API注册时间</p>
</td>
</tr>
<tr id="row5326357"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28781748"><a name="p28781748"></a><a name="p28781748"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p49620240"><a name="p49620240"></a><a name="p49620240"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p59816464"><a name="p59816464"></a><a name="p59816464"></a>API修改时间</p>
</td>
</tr>
<tr id="row1477265"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52549635"><a name="p52549635"></a><a name="p52549635"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p28662029"><a name="p28662029"></a><a name="p28662029"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p39923032"><a name="p39923032"></a><a name="p39923032"></a>API描述</p>
</td>
</tr>
<tr id="row23762973"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p45752684"><a name="p45752684"></a><a name="p45752684"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14979919"><a name="p14979919"></a><a name="p14979919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5413935"><a name="p5413935"></a><a name="p5413935"></a>后端类型</p>
</td>
</tr>
<tr id="row48725417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p54444686"><a name="p54444686"></a><a name="p54444686"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47943460"><a name="p47943460"></a><a name="p47943460"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p58215058"><a name="p58215058"></a><a name="p58215058"></a>发布的环境名</p>
</td>
</tr>
<tr id="row54173482"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p25975953"><a name="p25975953"></a><a name="p25975953"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23677411"><a name="p23677411"></a><a name="p23677411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38822154"><a name="p38822154"></a><a name="p38822154"></a>发布的环境id</p>
</td>
</tr>
<tr id="row13855073"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48519138"><a name="p48519138"></a><a name="p48519138"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p37736107"><a name="p37736107"></a><a name="p37736107"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36725861"><a name="p36725861"></a><a name="p36725861"></a>发布记录的编号</p>
</td>
</tr>
<tr id="row43718035"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51499971"><a name="p51499971"></a><a name="p51499971"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10748140"><a name="p10748140"></a><a name="p10748140"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65292981"><a name="p65292981"></a><a name="p65292981"></a>是否需要编排</p>
</td>
</tr>
<tr id="row1124075772911"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p82576192276"><a name="p82576192276"></a><a name="p82576192276"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1625711193277"><a name="p1625711193277"></a><a name="p1625711193277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6273141922718"><a name="p6273141922718"></a><a name="p6273141922718"></a>标签</p>
</td>
</tr>
<tr id="row298995912296"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p172881819162714"><a name="p172881819162714"></a><a name="p172881819162714"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p163043196278"><a name="p163043196278"></a><a name="p163043196278"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13320121932715"><a name="p13320121932715"></a><a name="p13320121932715"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="row6243115683313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p105561154343"><a name="p105561154343"></a><a name="p105561154343"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p75719510345"><a name="p75719510345"></a><a name="p75719510345"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1571450346"><a name="p1571450346"></a><a name="p1571450346"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
</td>
</tr>
<tr id="row14016595335"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p106341354349"><a name="p106341354349"></a><a name="p106341354349"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1463416511341"><a name="p1463416511341"></a><a name="p1463416511341"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46509516343"><a name="p46509516343"></a><a name="p46509516343"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
<tr id="row11759163143412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19696185133419"><a name="p19696185133419"></a><a name="p19696185133419"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p369665183416"><a name="p369665183416"></a><a name="p369665183416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p77123514347"><a name="p77123514347"></a><a name="p77123514347"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="row50765917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18398585"><a name="p18398585"></a><a name="p18398585"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13890442"><a name="p13890442"></a><a name="p13890442"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p51384056"><a name="p51384056"></a><a name="p51384056"></a>后端服务：web后端详情</p>
</td>
</tr>
<tr id="row59803325"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12231169"><a name="p12231169"></a><a name="p12231169"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51200596"><a name="p51200596"></a><a name="p51200596"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53607649"><a name="p53607649"></a><a name="p53607649"></a>后端服务：MOCK详情</p>
</td>
</tr>
<tr id="row12706796"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p22617536"><a name="p22617536"></a><a name="p22617536"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20081121"><a name="p20081121"></a><a name="p20081121"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15958070"><a name="p15958070"></a><a name="p15958070"></a>后端服务：函数工作流后端详情</p>
</td>
</tr>
<tr id="row129821224203313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13999938164017"><a name="p13999938164017"></a><a name="p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1999203815404"><a name="p1999203815404"></a><a name="p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11999143884013"><a name="p11999143884013"></a><a name="p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="row1634710304331"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p420294234017"><a name="p420294234017"></a><a name="p420294234017"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17202184217401"><a name="p17202184217401"></a><a name="p17202184217401"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p112025421400"><a name="p112025421400"></a><a name="p112025421400"></a>API的后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 11**  backend\_api参数说明

<a name="table9404903"></a>
<table><thead align="left"><tr id="row24239927"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p17277099"><a name="p17277099"></a><a name="p17277099"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p57267779"><a name="p57267779"></a><a name="p57267779"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p8178536"><a name="p8178536"></a><a name="p8178536"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row58481665"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39394423"><a name="p39394423"></a><a name="p39394423"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p36831665"><a name="p36831665"></a><a name="p36831665"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30574871"><a name="p30574871"></a><a name="p30574871"></a>编号</p>
</td>
</tr>
<tr id="row6738391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8938795"><a name="p8938795"></a><a name="p8938795"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p52953824"><a name="p52953824"></a><a name="p52953824"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61401374"><a name="p61401374"></a><a name="p61401374"></a>状态</p>
</td>
</tr>
<tr id="row15741455"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p67098348"><a name="p67098348"></a><a name="p67098348"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66257126"><a name="p66257126"></a><a name="p66257126"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p15198181295"><a name="p15198181295"></a><a name="p15198181295"></a>后端endpoint</p>
</td>
</tr>
<tr id="row50171912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37393096"><a name="p37393096"></a><a name="p37393096"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8941953"><a name="p8941953"></a><a name="p8941953"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53209562"><a name="p53209562"></a><a name="p53209562"></a>版本</p>
</td>
</tr>
<tr id="row9124010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p847318"><a name="p847318"></a><a name="p847318"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1523959"><a name="p1523959"></a><a name="p1523959"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56331893"><a name="p56331893"></a><a name="p56331893"></a>访问协议</p>
</td>
</tr>
<tr id="row37224994"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p62434550"><a name="p62434550"></a><a name="p62434550"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24033753"><a name="p24033753"></a><a name="p24033753"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p577014"><a name="p577014"></a><a name="p577014"></a>访问方式</p>
</td>
</tr>
<tr id="row5193129"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17990285"><a name="p17990285"></a><a name="p17990285"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47926974"><a name="p47926974"></a><a name="p47926974"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56879651"><a name="p56879651"></a><a name="p56879651"></a>访问地址</p>
</td>
</tr>
<tr id="row42154812"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p59096651"><a name="p59096651"></a><a name="p59096651"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22099459"><a name="p22099459"></a><a name="p22099459"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p45225739"><a name="p45225739"></a><a name="p45225739"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row4378468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19111656"><a name="p19111656"></a><a name="p19111656"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p4540304"><a name="p4540304"></a><a name="p4540304"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p32220357"><a name="p32220357"></a><a name="p32220357"></a>注册时间</p>
</td>
</tr>
<tr id="row21547759"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p538082"><a name="p538082"></a><a name="p538082"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p43584661"><a name="p43584661"></a><a name="p43584661"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p40696624"><a name="p40696624"></a><a name="p40696624"></a>修改时间</p>
</td>
</tr>
<tr id="row30725300"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5721408"><a name="p5721408"></a><a name="p5721408"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p60780871"><a name="p60780871"></a><a name="p60780871"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p24303539"><a name="p24303539"></a><a name="p24303539"></a>描述</p>
</td>
</tr>
<tr id="row17405267"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p540497"><a name="p540497"></a><a name="p540497"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p43780263"><a name="p43780263"></a><a name="p43780263"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56540414"><a name="p56540414"></a><a name="p56540414"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="row39101681"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13119596"><a name="p13119596"></a><a name="p13119596"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56054331"><a name="p56054331"></a><a name="p56054331"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p44106951"><a name="p44106951"></a><a name="p44106951"></a>VPC通道信息</p>
</td>
</tr>
</tbody>
</table>

**表 12**  mock\_info参数说明

<a name="table61418239"></a>
<table><thead align="left"><tr id="row64397298"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p48798660"><a name="p48798660"></a><a name="p48798660"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p60377411"><a name="p60377411"></a><a name="p60377411"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p58732118"><a name="p58732118"></a><a name="p58732118"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row59681126"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2333018"><a name="p2333018"></a><a name="p2333018"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p54756763"><a name="p54756763"></a><a name="p54756763"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6112784"><a name="p6112784"></a><a name="p6112784"></a>编号</p>
</td>
</tr>
<tr id="row55015057"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p27034672"><a name="p27034672"></a><a name="p27034672"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42324856"><a name="p42324856"></a><a name="p42324856"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5761296"><a name="p5761296"></a><a name="p5761296"></a>状态</p>
</td>
</tr>
<tr id="row51851665"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p39235365"><a name="p39235365"></a><a name="p39235365"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p23947997"><a name="p23947997"></a><a name="p23947997"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60739618"><a name="p60739618"></a><a name="p60739618"></a>版本</p>
</td>
</tr>
<tr id="row9785652"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p54440375"><a name="p54440375"></a><a name="p54440375"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47594234"><a name="p47594234"></a><a name="p47594234"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p29927717"><a name="p29927717"></a><a name="p29927717"></a>返回结果</p>
</td>
</tr>
<tr id="row914001"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6925293"><a name="p6925293"></a><a name="p6925293"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24077828"><a name="p24077828"></a><a name="p24077828"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p4147072"><a name="p4147072"></a><a name="p4147072"></a>注册时间</p>
</td>
</tr>
<tr id="row37323656"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3317270"><a name="p3317270"></a><a name="p3317270"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p263420"><a name="p263420"></a><a name="p263420"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p21337059"><a name="p21337059"></a><a name="p21337059"></a>修改时间</p>
</td>
</tr>
<tr id="row57815806"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52568713"><a name="p52568713"></a><a name="p52568713"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p30207336"><a name="p30207336"></a><a name="p30207336"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30875140"><a name="p30875140"></a><a name="p30875140"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 13**  func\_info参数说明

<a name="table9440804"></a>
<table><thead align="left"><tr id="row1393519"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p45766225"><a name="p45766225"></a><a name="p45766225"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p16076768"><a name="p16076768"></a><a name="p16076768"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p27149827"><a name="p27149827"></a><a name="p27149827"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51652387"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p23093799"><a name="p23093799"></a><a name="p23093799"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p58658424"><a name="p58658424"></a><a name="p58658424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p53711869"><a name="p53711869"></a><a name="p53711869"></a>编号</p>
</td>
</tr>
<tr id="row13644774"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p31484949"><a name="p31484949"></a><a name="p31484949"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p144109"><a name="p144109"></a><a name="p144109"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11672853"><a name="p11672853"></a><a name="p11672853"></a>状态</p>
</td>
</tr>
<tr id="row37946814"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p53793122"><a name="p53793122"></a><a name="p53793122"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p62275626"><a name="p62275626"></a><a name="p62275626"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11160959"><a name="p11160959"></a><a name="p11160959"></a>版本</p>
</td>
</tr>
<tr id="row33339769"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p16166796"><a name="p16166796"></a><a name="p16166796"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34442079"><a name="p34442079"></a><a name="p34442079"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38344986"><a name="p38344986"></a><a name="p38344986"></a>函数URN</p>
</td>
</tr>
<tr id="row9560558"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p36207770"><a name="p36207770"></a><a name="p36207770"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p47148225"><a name="p47148225"></a><a name="p47148225"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p60909901"><a name="p60909901"></a><a name="p60909901"></a>调用类型:async|sync</p>
</td>
</tr>
<tr id="row11318205"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p44359387"><a name="p44359387"></a><a name="p44359387"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p36340561"><a name="p36340561"></a><a name="p36340561"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p57904328"><a name="p57904328"></a><a name="p57904328"></a>注册时间</p>
</td>
</tr>
<tr id="row51376907"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p779942"><a name="p779942"></a><a name="p779942"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p63175317"><a name="p63175317"></a><a name="p63175317"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16927041"><a name="p16927041"></a><a name="p16927041"></a>更新时间</p>
</td>
</tr>
<tr id="row18125641"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p58890778"><a name="p58890778"></a><a name="p58890778"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5423708"><a name="p5423708"></a><a name="p5423708"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36667190"><a name="p36667190"></a><a name="p36667190"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row61569260"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p21054174"><a name="p21054174"></a><a name="p21054174"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p27666557"><a name="p27666557"></a><a name="p27666557"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p26398640"><a name="p26398640"></a><a name="p26398640"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 14**  req\_params参数说明

<a name="table197251634194412"></a>
<table><thead align="left"><tr id="row2075603420446"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p11756234184411"><a name="p11756234184411"></a><a name="p11756234184411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p777143420447"><a name="p777143420447"></a><a name="p777143420447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p5771193415446"><a name="p5771193415446"></a><a name="p5771193415446"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row85313200454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1753320144511"><a name="p1753320144511"></a><a name="p1753320144511"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p75302015450"><a name="p75302015450"></a><a name="p75302015450"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p653162014451"><a name="p653162014451"></a><a name="p653162014451"></a>参数编号</p>
</td>
</tr>
<tr id="row8786123464413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p578618344445"><a name="p578618344445"></a><a name="p578618344445"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1480313412443"><a name="p1480313412443"></a><a name="p1480313412443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48033344445"><a name="p48033344445"></a><a name="p48033344445"></a>参数名称</p>
</td>
</tr>
<tr id="row13818193434411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p781810341448"><a name="p781810341448"></a><a name="p781810341448"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18342034114419"><a name="p18342034114419"></a><a name="p18342034114419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p083493413441"><a name="p083493413441"></a><a name="p083493413441"></a>参数类型</p>
</td>
</tr>
<tr id="row17850234124414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18865203414418"><a name="p18865203414418"></a><a name="p18865203414418"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16881203415443"><a name="p16881203415443"></a><a name="p16881203415443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p788120340445"><a name="p788120340445"></a><a name="p788120340445"></a>参数位置</p>
</td>
</tr>
<tr id="row99121534134414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18912934114419"><a name="p18912934114419"></a><a name="p18912934114419"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p139281534104415"><a name="p139281534104415"></a><a name="p139281534104415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1592853454412"><a name="p1592853454412"></a><a name="p1592853454412"></a>参数默认值</p>
</td>
</tr>
<tr id="row1594315349446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p994311348442"><a name="p994311348442"></a><a name="p994311348442"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1495973414419"><a name="p1495973414419"></a><a name="p1495973414419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1695953413449"><a name="p1695953413449"></a><a name="p1695953413449"></a>参数示例值</p>
</td>
</tr>
<tr id="row1959173474410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p2974183417445"><a name="p2974183417445"></a><a name="p2974183417445"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13974143417443"><a name="p13974143417443"></a><a name="p13974143417443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p699053414444"><a name="p699053414444"></a><a name="p699053414444"></a>是否必须</p>
</td>
</tr>
<tr id="row662354446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p66183524412"><a name="p66183524412"></a><a name="p66183524412"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p32133519447"><a name="p32133519447"></a><a name="p32133519447"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18371535124417"><a name="p18371535124417"></a><a name="p18371535124417"></a>是否开启校验</p>
</td>
</tr>
<tr id="row1053435144414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p653133513441"><a name="p653133513441"></a><a name="p653133513441"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1867183512446"><a name="p1867183512446"></a><a name="p1867183512446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p567123584420"><a name="p567123584420"></a><a name="p567123584420"></a>描述</p>
</td>
</tr>
<tr id="row7100203515443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p181002035154415"><a name="p181002035154415"></a><a name="p181002035154415"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p161151635164413"><a name="p161151635164413"></a><a name="p161151635164413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17209124910453"><a name="p17209124910453"></a><a name="p17209124910453"></a>参数枚举值</p>
</td>
</tr>
<tr id="row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p151311235144415"><a name="p151311235144415"></a><a name="p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p129607951117"><a name="p129607951117"></a><a name="p129607951117"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p192431498456"><a name="p192431498456"></a><a name="p192431498456"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8146203564415"><a name="p8146203564415"></a><a name="p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31627353442"><a name="p31627353442"></a><a name="p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1327444914518"><a name="p1327444914518"></a><a name="p1327444914518"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p61782355443"><a name="p61782355443"></a><a name="p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p201932035194417"><a name="p201932035194417"></a><a name="p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p330311493456"><a name="p330311493456"></a><a name="p330311493456"></a>参数最小长度</p>
</td>
</tr>
<tr id="row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12209535144412"><a name="p12209535144412"></a><a name="p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12251035164419"><a name="p12251035164419"></a><a name="p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9329749144513"><a name="p9329749144513"></a><a name="p9329749144513"></a>参数最大长度</p>
</td>
</tr>
<tr id="row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52401735134413"><a name="p52401735134413"></a><a name="p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12240153510443"><a name="p12240153510443"></a><a name="p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p193631549154517"><a name="p193631549154517"></a><a name="p193631549154517"></a>正则校验规则（暂不支持）</p>
</td>
</tr>
<tr id="row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p202561335114413"><a name="p202561335114413"></a><a name="p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16271035114412"><a name="p16271035114412"></a><a name="p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17400114994510"><a name="p17400114994510"></a><a name="p17400114994510"></a>JSON校验规则（暂不支持）</p>
</td>
</tr>
</tbody>
</table>

**表 15**  backend\_params参数说明

<a name="table9287113513446"></a>
<table><thead align="left"><tr id="row4302173564419"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p33182355443"><a name="p33182355443"></a><a name="p33182355443"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p14334103544415"><a name="p14334103544415"></a><a name="p14334103544415"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p19334153517444"><a name="p19334153517444"></a><a name="p19334153517444"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17142774611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47152713464"><a name="p47152713464"></a><a name="p47152713464"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1717279463"><a name="p1717279463"></a><a name="p1717279463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27122714620"><a name="p27122714620"></a><a name="p27122714620"></a>参数编号</p>
</td>
</tr>
<tr id="row2936129114713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p199361729154717"><a name="p199361729154717"></a><a name="p199361729154717"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1693652934715"><a name="p1693652934715"></a><a name="p1693652934715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1093614294475"><a name="p1093614294475"></a><a name="p1093614294475"></a>对应的请求参数编号</p>
</td>
</tr>
<tr id="row833403514441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13350143554413"><a name="p13350143554413"></a><a name="p13350143554413"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6365163554417"><a name="p6365163554417"></a><a name="p6365163554417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p036516356445"><a name="p036516356445"></a><a name="p036516356445"></a>参数名称</p>
</td>
</tr>
<tr id="row203656353443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4381103534420"><a name="p4381103534420"></a><a name="p4381103534420"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p838193504410"><a name="p838193504410"></a><a name="p838193504410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10396123516442"><a name="p10396123516442"></a><a name="p10396123516442"></a>参数位置</p>
</td>
</tr>
<tr id="row7412103554417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14271535144413"><a name="p14271535144413"></a><a name="p14271535144413"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p112891555114512"><a name="p112891555114512"></a><a name="p112891555114512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1044312351449"><a name="p1044312351449"></a><a name="p1044312351449"></a>参数类别</p>
</td>
</tr>
<tr id="row445983511447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5475203519440"><a name="p5475203519440"></a><a name="p5475203519440"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p331005594512"><a name="p331005594512"></a><a name="p331005594512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9490435144419"><a name="p9490435144419"></a><a name="p9490435144419"></a>参数值</p>
</td>
</tr>
<tr id="row7506335184410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3506935104410"><a name="p3506935104410"></a><a name="p3506935104410"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p05217356442"><a name="p05217356442"></a><a name="p05217356442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11521123517447"><a name="p11521123517447"></a><a name="p11521123517447"></a>描述</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "name": "test",
  "type": 1,
  "version": "V0.0.1",
  "req_protocol": "HTTPS",
  "req_method": "GET",
  "req_uri": "/test/{project_id}",
  "auth_type": "APP",
  "tag": "test",
  "cors": false,
  "match_mode": "NORMAL",
  "backend_type": "HTTP",
  "group_id": "f71f69876f90456ca6fd18ed012fdc11",
  "result_normal_sample": "hello world!",
  "id": "81efcfd94b8747a0b21e8c04144a4e8c",
  "status": 1,
  "arrange_necessary": 2,
  "register_time": "2018-08-15T03:41:11.0239936Z",
  "update_time": "2018-08-15T03:41:11.0239936Z",
  "group_name": "group0002",
  "backend_api": {
    "url_domain": "xxxxxxxxx",
    "req_protocol": "HTTP",
    "req_method": "GET",
    "req_uri": "/test",
    "timeout": 1000,
    "vpc_status": 2,
    "id": "3442ffd031814e3a8f133a9f1ea08453",
    "status": 1,
    "register_time": "2018-08-15T03:41:11.1019236Z",
    "update_time": "2018-08-15T03:41:11.1019236Z"
  },
  "req_params": [
    {
      "name": "project_id",
      "type": "STRING",
      "location": "PATH",
      "required": 1,
      "valid_enable": 2,
      "id": "593c5560e0924e00af08fb458f850ecb"
    },
    {
      "name": "city",
      "type": "STRING",
      "location": "QUERY",
      "required": 2,
      "valid_enable": 2,
      "id": "e0b91bc81ae54f8ea850848d782d6e1e"
    }
  ],
  "backend_params": [
    {
      "name": "project_id",
      "location": "QUERY",
      "origin": "REQUEST",
      "value": "project_id",
      "id": "44e03de2351e43a8b18ba9ec1e71d2e9",
      "req_param_id": "593c5560e0924e00af08fb458f850ecb"
    },
    {
      "name": "city",
      "location": "QUERY",
      "origin": "REQUEST",
      "value": "city",
      "id": "b60fbcb5b86f4f5c8705c445b9bd6325",
      "req_param_id": "e0b91bc81ae54f8ea850848d782d6e1e"
    }
  ]
}
```

## 状态码<a name="section16303336"></a>

**表 16**  返回消息说明

<a name="table29568396"></a>
<table><thead align="left"><tr id="row12955267"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p42743677"><a name="p42743677"></a><a name="p42743677"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p39685795"><a name="p39685795"></a><a name="p39685795"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row60432863"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p63223702"><a name="p63223702"></a><a name="p63223702"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row53398602"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p30319480"><a name="p30319480"></a><a name="p30319480"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p39958782"><a name="p39958782"></a><a name="p39958782"></a>Bad Request</p>
</td>
</tr>
<tr id="row24084722"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p4705456"><a name="p4705456"></a><a name="p4705456"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row7725748"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p21805869"><a name="p21805869"></a><a name="p21805869"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row58786678"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p64100450"><a name="p64100450"></a><a name="p64100450"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p24753987"><a name="p24753987"></a><a name="p24753987"></a>Not Found</p>
</td>
</tr>
<tr id="row21459299"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p60481678"><a name="p60481678"></a><a name="p60481678"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p68898"><a name="p68898"></a><a name="p68898"></a>Conflict</p>
</td>
</tr>
<tr id="row620082"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p50226677"><a name="p50226677"></a><a name="p50226677"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

