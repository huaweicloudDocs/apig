# 注册API<a name="apig-zh-api-180713025"></a>

## 功能介绍<a name="section11821014"></a>

添加一个API，API即一个服务接口，具体的服务能力。

API分为两部分，第一部分为面向API使用者的API接口，定义了使用者如何调用这个API。第二部分面向API提供者，由API提供者定义这个API的真实的后端情况，定义了API网关如何去访问真实的后端服务。

API的真实后端服务目前支持三种类型：传统的HTTP/HTTPS形式的web后端、函数工作流、MOCK。

## URI<a name="section39280262"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table31836871"></a>
<table><thead align="left"><tr id="row66270525"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p66312269"><a name="p66312269"></a><a name="p66312269"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p2584681"><a name="p2584681"></a><a name="p2584681"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row8032634"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p46663656"><a name="p46663656"></a><a name="p46663656"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p21659802"><a name="p21659802"></a><a name="p21659802"></a>/v1.0/apigw/apis</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section17978045"></a>

**表 2**  参数说明

<a name="table9613561"></a>
<table><thead align="left"><tr id="row51426513"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p4797990"><a name="p4797990"></a><a name="p4797990"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p53092887"><a name="p53092887"></a><a name="p53092887"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p5556622"><a name="p5556622"></a><a name="p5556622"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p47433200"><a name="p47433200"></a><a name="p47433200"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16884007"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p25427355"><a name="p25427355"></a><a name="p25427355"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p46349875"><a name="p46349875"></a><a name="p46349875"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p63352408"><a name="p63352408"></a><a name="p63352408"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p31271409"><a name="p31271409"></a><a name="p31271409"></a>API所属的分组编号</p>
</td>
</tr>
<tr id="row46952608"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p45064875"><a name="p45064875"></a><a name="p45064875"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p26376263"><a name="p26376263"></a><a name="p26376263"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p56102555"><a name="p56102555"></a><a name="p56102555"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p48013136"><a name="p48013136"></a><a name="p48013136"></a>API名称</p>
<p id="p37858559"><a name="p37858559"></a><a name="p37858559"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以英文或中文开头。</p>
<div class="note" id="note690163615371"><a name="note690163615371"></a><a name="note690163615371"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p09053643719"><a name="p09053643719"></a><a name="p09053643719"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row25820024"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p11047224"><a name="p11047224"></a><a name="p11047224"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p22409969"><a name="p22409969"></a><a name="p22409969"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p3268170"><a name="p3268170"></a><a name="p3268170"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p63395179"><a name="p63395179"></a><a name="p63395179"></a>API类型：</p>
<a name="ul336530"></a><a name="ul336530"></a><ul id="ul336530"><li>1：公有API</li><li>2：私有API</li></ul>
</td>
</tr>
<tr id="row44004246"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p7574169"><a name="p7574169"></a><a name="p7574169"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p9527961"><a name="p9527961"></a><a name="p9527961"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p33567357"><a name="p33567357"></a><a name="p33567357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p34601390"><a name="p34601390"></a><a name="p34601390"></a>API的版本</p>
</td>
</tr>
<tr id="row58589356"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p48117435"><a name="p48117435"></a><a name="p48117435"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p5198195"><a name="p5198195"></a><a name="p5198195"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p18400635"><a name="p18400635"></a><a name="p18400635"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p14056443"><a name="p14056443"></a><a name="p14056443"></a>API的请求协议：</p>
<a name="ul14361951"></a><a name="ul14361951"></a><ul id="ul14361951"><li>HTTP</li><li>HTTPS</li><li>BOTH：同时支持HTTP和HTTPS</li><li>WEBSOCKET</li></ul>
<p id="p4179246"><a name="p4179246"></a><a name="p4179246"></a>默认：HTTPS</p>
</td>
</tr>
<tr id="row37613216"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p26771660"><a name="p26771660"></a><a name="p26771660"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p21020848"><a name="p21020848"></a><a name="p21020848"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p24967157"><a name="p24967157"></a><a name="p24967157"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p9073859"><a name="p9073859"></a><a name="p9073859"></a>API的请求方式：</p>
<a name="ul46261614"></a><a name="ul46261614"></a><ul id="ul46261614"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
</tr>
<tr id="row3177191"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p56025891"><a name="p56025891"></a><a name="p56025891"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p41803348"><a name="p41803348"></a><a name="p41803348"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p30628066"><a name="p30628066"></a><a name="p30628066"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p64954292"><a name="p64954292"></a><a name="p64954292"></a>API的访问地址</p>
<div class="note" id="note38431529153919"><a name="note38431529153919"></a><a name="note38431529153919"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p18843122918398"><a name="p18843122918398"></a><a name="p18843122918398"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="row51064406"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p42576202"><a name="p42576202"></a><a name="p42576202"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p26120331"><a name="p26120331"></a><a name="p26120331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p35372032"><a name="p35372032"></a><a name="p35372032"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p46562321"><a name="p46562321"></a><a name="p46562321"></a>API的匹配方式：</p>
<a name="ul8369025"></a><a name="ul8369025"></a><ul id="ul8369025"><li>SWA：前缀匹配</li><li>NORMAL：正常匹配（绝对匹配）<p id="p31111474402"><a name="p31111474402"></a><a name="p31111474402"></a>默认：NORMAL</p>
</li></ul>
</td>
</tr>
<tr id="row61222081"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p60041530"><a name="p60041530"></a><a name="p60041530"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p31525796"><a name="p31525796"></a><a name="p31525796"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p3452711"><a name="p3452711"></a><a name="p3452711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p11234154"><a name="p11234154"></a><a name="p11234154"></a>API描述</p>
<p id="p2416961"><a name="p2416961"></a><a name="p2416961"></a>字符长度不超过255</p>
<div class="note" id="note1069572664018"><a name="note1069572664018"></a><a name="note1069572664018"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p11697926124010"><a name="p11697926124010"></a><a name="p11697926124010"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row14009080"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p60993670"><a name="p60993670"></a><a name="p60993670"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p41540204"><a name="p41540204"></a><a name="p41540204"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p9313363"><a name="p9313363"></a><a name="p9313363"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p16184930"><a name="p16184930"></a><a name="p16184930"></a>API的认证方式：</p>
<a name="ul1496884"></a><a name="ul1496884"></a><ul id="ul1496884"><li>NONE：无认证</li><li>APP：APP认证</li><li>IAM：IAM认证</li></ul>
</td>
</tr>
<tr id="row23162817"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p64248927"><a name="p64248927"></a><a name="p64248927"></a>backend_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p36780609"><a name="p36780609"></a><a name="p36780609"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p26439376"><a name="p26439376"></a><a name="p26439376"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p61214707"><a name="p61214707"></a><a name="p61214707"></a>后端类型：</p>
<a name="ul65236141"></a><a name="ul65236141"></a><ul id="ul65236141"><li>HTTP：web后端</li><li>FUNCTION：函数工作流</li><li>MOCK：模拟的后端</li></ul>
</td>
</tr>
<tr id="row7589137172110"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p45893752117"><a name="p45893752117"></a><a name="p45893752117"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p105895719216"><a name="p105895719216"></a><a name="p105895719216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p18589147152113"><a name="p18589147152113"></a><a name="p18589147152113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p17891448182114"><a name="p17891448182114"></a><a name="p17891448182114"></a>标签</p>
<p id="p17589774213"><a name="p17589774213"></a><a name="p17589774213"></a>可以打servicename的标签和其他标签</p>
</td>
</tr>
<tr id="row152631022114"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p526201042116"><a name="p526201042116"></a><a name="p526201042116"></a>cors</p>
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
<tr id="row11977120131916"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p59931303198"><a name="p59931303198"></a><a name="p59931303198"></a>body_remark</p>
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
<tr id="row194617661914"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p5946166161919"><a name="p5946166161919"></a><a name="p5946166161919"></a>result_normal_sample</p>
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
<tr id="row1327418118195"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p727431112199"><a name="p727431112199"></a><a name="p727431112199"></a>result_failure_sample</p>
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
<tr id="row61097128"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p49920342"><a name="p49920342"></a><a name="p49920342"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p17015941"><a name="p17015941"></a><a name="p17015941"></a>backend_type = HTTP时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p36114013"><a name="p36114013"></a><a name="p36114013"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p39553925"><a name="p39553925"></a><a name="p39553925"></a>web后端详情</p>
</td>
</tr>
<tr id="row45108818"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p29935642"><a name="p29935642"></a><a name="p29935642"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p8867951"><a name="p8867951"></a><a name="p8867951"></a>backend_type = MOCK时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p47215416"><a name="p47215416"></a><a name="p47215416"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p66352350"><a name="p66352350"></a><a name="p66352350"></a>mock后端详情</p>
</td>
</tr>
<tr id="row52481162"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p23115734"><a name="p23115734"></a><a name="p23115734"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p60435162"><a name="p60435162"></a><a name="p60435162"></a>backend_type = FUNCTION时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p63409983"><a name="p63409983"></a><a name="p63409983"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p35935021"><a name="p35935021"></a><a name="p35935021"></a>函数工作流后端详情</p>
</td>
</tr>
<tr id="row168317015213"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p156831806524"><a name="p156831806524"></a><a name="p156831806524"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p76831801527"><a name="p76831801527"></a><a name="p76831801527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p176831903520"><a name="p176831903520"></a><a name="p176831903520"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p468350195218"><a name="p468350195218"></a><a name="p468350195218"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="row166884018355"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p06884014357"><a name="p06884014357"></a><a name="p06884014357"></a>backend_params</p>
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

**表 3**  backend\_api参数说明

<a name="table24173475"></a>
<table><thead align="left"><tr id="row27724933"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p31127089"><a name="p31127089"></a><a name="p31127089"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p38266241"><a name="p38266241"></a><a name="p38266241"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p12557789"><a name="p12557789"></a><a name="p12557789"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p10548014"><a name="p10548014"></a><a name="p10548014"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49082844"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p16287438"><a name="p16287438"></a><a name="p16287438"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1741473216910"><a name="p1741473216910"></a><a name="p1741473216910"></a>后端服务不使用VPC通道时，必选</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p24574368"><a name="p24574368"></a><a name="p24574368"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p44366800"><a name="p44366800"></a><a name="p44366800"></a>后端的Endpoint。</p>
<p id="p9406451538"><a name="p9406451538"></a><a name="p9406451538"></a>由域名（或IP地址）和端口号组成，总长度不超过255。格式为域名:端口（如：apig.huaweicloud.com:7443）。如果不写端口，则HTTPS默认端口号为443， HTTP默认端口号为80。</p>
<p id="p13446109556"><a name="p13446109556"></a><a name="p13446109556"></a>支持环境变量，使用环境变量时，每个变量名的长度为3 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="row64033799"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p19355245"><a name="p19355245"></a><a name="p19355245"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p24271019"><a name="p24271019"></a><a name="p24271019"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p19795562"><a name="p19795562"></a><a name="p19795562"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p59936722"><a name="p59936722"></a><a name="p59936722"></a>web后端版本</p>
</td>
</tr>
<tr id="row6000091"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p16245391"><a name="p16245391"></a><a name="p16245391"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p40808295"><a name="p40808295"></a><a name="p40808295"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p17137612"><a name="p17137612"></a><a name="p17137612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p45969317"><a name="p45969317"></a><a name="p45969317"></a>请求协议：</p>
<a name="ul4739707"></a><a name="ul4739707"></a><ul id="ul4739707"><li>HTTP</li><li>HTTPS</li></ul>
</td>
</tr>
<tr id="row32695023"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p31051236"><a name="p31051236"></a><a name="p31051236"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p32122210"><a name="p32122210"></a><a name="p32122210"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p51762192"><a name="p51762192"></a><a name="p51762192"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p31987990"><a name="p31987990"></a><a name="p31987990"></a>请求方式：</p>
<a name="ul47767884"></a><a name="ul47767884"></a><ul id="ul47767884"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
</tr>
<tr id="row26241179"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p45160793"><a name="p45160793"></a><a name="p45160793"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p34145627"><a name="p34145627"></a><a name="p34145627"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p14332426"><a name="p14332426"></a><a name="p14332426"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p20075853"><a name="p20075853"></a><a name="p20075853"></a>请求地址</p>
<p id="p1273516206484"><a name="p1273516206484"></a><a name="p1273516206484"></a>总长度不超过512，且满足URI规范。</p>
<p id="p144251235114414"><a name="p144251235114414"></a><a name="p144251235114414"></a>支持环境变量，使用环境变量时，每个变量名的长度为3 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”组成，且只能以英文开头。</p>
<div class="note" id="note1597012134438"><a name="note1597012134438"></a><a name="note1597012134438"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p1597171324315"><a name="p1597171324315"></a><a name="p1597171324315"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="row30294306"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p37919687"><a name="p37919687"></a><a name="p37919687"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p51595784"><a name="p51595784"></a><a name="p51595784"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p18509007"><a name="p18509007"></a><a name="p18509007"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p22834561"><a name="p22834561"></a><a name="p22834561"></a>API网关请求后端服务的超时时间，最大60000，最小为1</p>
<p id="p3397199"><a name="p3397199"></a><a name="p3397199"></a>单位：毫秒</p>
<p id="p60639412"><a name="p60639412"></a><a name="p60639412"></a>默认值：45000，请求参数值不在合法范围内时将使用默认值</p>
</td>
</tr>
<tr id="row48499315"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p36130470"><a name="p36130470"></a><a name="p36130470"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p40886937"><a name="p40886937"></a><a name="p40886937"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p23507572"><a name="p23507572"></a><a name="p23507572"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p25065184"><a name="p25065184"></a><a name="p25065184"></a>描述</p>
<p id="p18908459"><a name="p18908459"></a><a name="p18908459"></a>字符长度不超过255</p>
<div class="note" id="note14776192410444"><a name="note14776192410444"></a><a name="note14776192410444"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p197771624144419"><a name="p197771624144419"></a><a name="p197771624144419"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="row54459243"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p49122562"><a name="p49122562"></a><a name="p49122562"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p19504577"><a name="p19504577"></a><a name="p19504577"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p36366929"><a name="p36366929"></a><a name="p36366929"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p60040154"><a name="p60040154"></a><a name="p60040154"></a>是否使用VPC通道：</p>
<a name="ul17737046"></a><a name="ul17737046"></a><ul id="ul17737046"><li>1 : 使用VPC通道</li><li>2 : 不使用VPC通道</li></ul>
</td>
</tr>
<tr id="row45404886"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p53917160"><a name="p53917160"></a><a name="p53917160"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p5213863"><a name="p5213863"></a><a name="p5213863"></a>如果vpc_status=1，则这个字典类型为必填信息</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p19669754"><a name="p19669754"></a><a name="p19669754"></a>字典类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p49746250"><a name="p49746250"></a><a name="p49746250"></a>VPC通道详情</p>
</td>
</tr>
</tbody>
</table>

**表 4**  VPC通道参数说明

<a name="table26229873"></a>
<table><thead align="left"><tr id="row61659324"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p28349332"><a name="p28349332"></a><a name="p28349332"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p14594532"><a name="p14594532"></a><a name="p14594532"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p41306453"><a name="p41306453"></a><a name="p41306453"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p57488398"><a name="p57488398"></a><a name="p57488398"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26048696"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p135916441067"><a name="p135916441067"></a><a name="p135916441067"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p46332158"><a name="p46332158"></a><a name="p46332158"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p61917289"><a name="p61917289"></a><a name="p61917289"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p49244517"><a name="p49244517"></a><a name="p49244517"></a>VPC通道编号</p>
</td>
</tr>
<tr id="row63119848"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p12434084"><a name="p12434084"></a><a name="p12434084"></a>vpc_proxy_host</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p527917"><a name="p527917"></a><a name="p527917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p42761322"><a name="p42761322"></a><a name="p42761322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p41115076"><a name="p41115076"></a><a name="p41115076"></a>代理主机</p>
</td>
</tr>
</tbody>
</table>

**表 5**  mock\_info参数说明

<a name="table42337334"></a>
<table><thead align="left"><tr id="row33365929"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p18285723"><a name="p18285723"></a><a name="p18285723"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p4748581"><a name="p4748581"></a><a name="p4748581"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p49090800"><a name="p49090800"></a><a name="p49090800"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p16931876"><a name="p16931876"></a><a name="p16931876"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row29304679"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p24868836"><a name="p24868836"></a><a name="p24868836"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1109825"><a name="p1109825"></a><a name="p1109825"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p22786982"><a name="p22786982"></a><a name="p22786982"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p33806268"><a name="p33806268"></a><a name="p33806268"></a>返回结果</p>
</td>
</tr>
<tr id="row15816706"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p6084841"><a name="p6084841"></a><a name="p6084841"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p23110075"><a name="p23110075"></a><a name="p23110075"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p59976802"><a name="p59976802"></a><a name="p59976802"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p26282822"><a name="p26282822"></a><a name="p26282822"></a>版本</p>
</td>
</tr>
<tr id="row34151363"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p14797053"><a name="p14797053"></a><a name="p14797053"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p57710672"><a name="p57710672"></a><a name="p57710672"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p44052835"><a name="p44052835"></a><a name="p44052835"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p11509854"><a name="p11509854"></a><a name="p11509854"></a>描述信息</p>
<p id="p2075966"><a name="p2075966"></a><a name="p2075966"></a>长度不超过255个字符</p>
<div class="note" id="note988922210482"><a name="note988922210482"></a><a name="note988922210482"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p0889122164812"><a name="p0889122164812"></a><a name="p0889122164812"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

**表 6**  func\_info参数说明

<a name="table55289951"></a>
<table><thead align="left"><tr id="row4334171"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="p15523588"><a name="p15523588"></a><a name="p15523588"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="p49451085"><a name="p49451085"></a><a name="p49451085"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="p46114910"><a name="p46114910"></a><a name="p46114910"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="p44320224"><a name="p44320224"></a><a name="p44320224"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row33168378"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p2284117"><a name="p2284117"></a><a name="p2284117"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p50795801"><a name="p50795801"></a><a name="p50795801"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p20819180"><a name="p20819180"></a><a name="p20819180"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p8632057"><a name="p8632057"></a><a name="p8632057"></a>函数URN</p>
</td>
</tr>
<tr id="row51645464"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p22533049"><a name="p22533049"></a><a name="p22533049"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p13237646"><a name="p13237646"></a><a name="p13237646"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p65616383"><a name="p65616383"></a><a name="p65616383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p13326838"><a name="p13326838"></a><a name="p13326838"></a>调用类型:async|sync （异步|同步）</p>
</td>
</tr>
<tr id="row51588510"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p17919758"><a name="p17919758"></a><a name="p17919758"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p42214303"><a name="p42214303"></a><a name="p42214303"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p63915384"><a name="p63915384"></a><a name="p63915384"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p3582515183214"><a name="p3582515183214"></a><a name="p3582515183214"></a>API网关请求函数服务的超时时间，最大60000，最小为1</p>
<p id="p2597131514329"><a name="p2597131514329"></a><a name="p2597131514329"></a>单位：毫秒</p>
<p id="p136134155324"><a name="p136134155324"></a><a name="p136134155324"></a>默认值：45000，请求参数值不在合法范围内时将使用默认值</p>
</td>
</tr>
<tr id="row4161871"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p1567241"><a name="p1567241"></a><a name="p1567241"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p59837679"><a name="p59837679"></a><a name="p59837679"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p15013867"><a name="p15013867"></a><a name="p15013867"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p8163682"><a name="p8163682"></a><a name="p8163682"></a>版本信息</p>
</td>
</tr>
<tr id="row45744694"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p14332708"><a name="p14332708"></a><a name="p14332708"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p20098666"><a name="p20098666"></a><a name="p20098666"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p17379249"><a name="p17379249"></a><a name="p17379249"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p65541920"><a name="p65541920"></a><a name="p65541920"></a>描述信息</p>
<p id="p65657958"><a name="p65657958"></a><a name="p65657958"></a>长度不超过255个字符</p>
<div class="note" id="note962555913483"><a name="note962555913483"></a><a name="note962555913483"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="p96267594486"><a name="p96267594486"></a><a name="p96267594486"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

**表 7**  req\_params参数说明

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
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p141581516113916"><a name="p141581516113916"></a><a name="p141581516113916"></a>参数枚举值</p>
</td>
</tr>
<tr id="row878217618128"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p1778211616128"><a name="p1778211616128"></a><a name="p1778211616128"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p10782563129"><a name="p10782563129"></a><a name="p10782563129"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p178213613128"><a name="p178213613128"></a><a name="p178213613128"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p11708175481613"><a name="p11708175481613"></a><a name="p11708175481613"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row1242311108123"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p154235102129"><a name="p154235102129"></a><a name="p154235102129"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p3423141081212"><a name="p3423141081212"></a><a name="p3423141081212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1442316104122"><a name="p1442316104122"></a><a name="p1442316104122"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p542391091215"><a name="p542391091215"></a><a name="p542391091215"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row21901721131212"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9190321131218"><a name="p9190321131218"></a><a name="p9190321131218"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p7190162117128"><a name="p7190162117128"></a><a name="p7190162117128"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1619082112121"><a name="p1619082112121"></a><a name="p1619082112121"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p719062181213"><a name="p719062181213"></a><a name="p719062181213"></a>参数最小长度</p>
</td>
</tr>
<tr id="row192351217191211"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p182351717171210"><a name="p182351717171210"></a><a name="p182351717171210"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p11235151717124"><a name="p11235151717124"></a><a name="p11235151717124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p20235181721217"><a name="p20235181721217"></a><a name="p20235181721217"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p122359172126"><a name="p122359172126"></a><a name="p122359172126"></a>参数最大长度</p>
</td>
</tr>
<tr id="row222041311121"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p10220131331219"><a name="p10220131331219"></a><a name="p10220131331219"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1220131331211"><a name="p1220131331211"></a><a name="p1220131331211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1122017131128"><a name="p1122017131128"></a><a name="p1122017131128"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1722001319126"><a name="p1722001319126"></a><a name="p1722001319126"></a>正则校验规则</p>
</td>
</tr>
<tr id="row177506146139"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p197501614181317"><a name="p197501614181317"></a><a name="p197501614181317"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1975091410132"><a name="p1975091410132"></a><a name="p1975091410132"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p1275091417134"><a name="p1275091417134"></a><a name="p1275091417134"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p07501140138"><a name="p07501140138"></a><a name="p07501140138"></a>JSON校验规则</p>
</td>
</tr>
</tbody>
</table>

**表 8**  backend\_params参数说明

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
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p724735411231"><a name="p724735411231"></a><a name="p724735411231"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p1524775413233"><a name="p1524775413233"></a><a name="p1524775413233"></a>参数类别：</p>
<a name="ul1124735482312"></a><a name="ul1124735482312"></a><ul id="ul1124735482312"><li>REQUEST</li><li>CONSTANT</li><li>SYSTEM</li></ul>
</td>
</tr>
<tr id="row15261254202320"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="p9261954122310"><a name="p9261954122310"></a><a name="p9261954122310"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="p1427715452315"><a name="p1427715452315"></a><a name="p1427715452315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="p17277155419233"><a name="p17277155419233"></a><a name="p17277155419233"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="p657172452818"><a name="p657172452818"></a><a name="p657172452818"></a>参数值</p>
<p id="p110811324312"><a name="p110811324312"></a><a name="p110811324312"></a>字符长度不超过255</p>
<p id="p13947355152811"><a name="p13947355152811"></a><a name="p13947355152811"></a>类别为REQUEST时，值为req_params中的参数名称；</p>
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
    "url_domain": "xxxxxxxxxxx"
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

## 响应消息<a name="section46935561"></a>

**表 9**  参数说明

<a name="table13593802"></a>
<table><thead align="left"><tr id="row45234979"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p40154672"><a name="p40154672"></a><a name="p40154672"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p31302981"><a name="p31302981"></a><a name="p31302981"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p52513547"><a name="p52513547"></a><a name="p52513547"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row25738921"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4477896"><a name="p4477896"></a><a name="p4477896"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p27165328"><a name="p27165328"></a><a name="p27165328"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52907944"><a name="p52907944"></a><a name="p52907944"></a>API编号</p>
</td>
</tr>
<tr id="row6409449"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p49403389"><a name="p49403389"></a><a name="p49403389"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42251573"><a name="p42251573"></a><a name="p42251573"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p66934266"><a name="p66934266"></a><a name="p66934266"></a>API名称</p>
</td>
</tr>
<tr id="row65537484"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6936015"><a name="p6936015"></a><a name="p6936015"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24946322"><a name="p24946322"></a><a name="p24946322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7386173"><a name="p7386173"></a><a name="p7386173"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row66475561"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15811397"><a name="p15811397"></a><a name="p15811397"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5654748"><a name="p5654748"></a><a name="p5654748"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p55381464"><a name="p55381464"></a><a name="p55381464"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row28671136"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40660654"><a name="p40660654"></a><a name="p40660654"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p5178644"><a name="p5178644"></a><a name="p5178644"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p16817019"><a name="p16817019"></a><a name="p16817019"></a>API的状态</p>
</td>
</tr>
<tr id="row17135446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p45793889"><a name="p45793889"></a><a name="p45793889"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18317504"><a name="p18317504"></a><a name="p18317504"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p7322844"><a name="p7322844"></a><a name="p7322844"></a>API类型</p>
</td>
</tr>
<tr id="row65905596"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p36753021"><a name="p36753021"></a><a name="p36753021"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24204719"><a name="p24204719"></a><a name="p24204719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14425209"><a name="p14425209"></a><a name="p14425209"></a>API版本</p>
</td>
</tr>
<tr id="row62718023"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p46995113"><a name="p46995113"></a><a name="p46995113"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48507832"><a name="p48507832"></a><a name="p48507832"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p36820315"><a name="p36820315"></a><a name="p36820315"></a>API访问协议</p>
</td>
</tr>
<tr id="row62947384"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p65573333"><a name="p65573333"></a><a name="p65573333"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9839738"><a name="p9839738"></a><a name="p9839738"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p58821328"><a name="p58821328"></a><a name="p58821328"></a>API请求方式</p>
</td>
</tr>
<tr id="row59629909"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p65293302"><a name="p65293302"></a><a name="p65293302"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p54266141"><a name="p54266141"></a><a name="p54266141"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p33481263"><a name="p33481263"></a><a name="p33481263"></a>API访问地址</p>
</td>
</tr>
<tr id="row32895917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47323597"><a name="p47323597"></a><a name="p47323597"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8006158"><a name="p8006158"></a><a name="p8006158"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p44519063"><a name="p44519063"></a><a name="p44519063"></a>API认证方式</p>
</td>
</tr>
<tr id="row65127255"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40816288"><a name="p40816288"></a><a name="p40816288"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17785030"><a name="p17785030"></a><a name="p17785030"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p31301296"><a name="p31301296"></a><a name="p31301296"></a>API匹配方式</p>
</td>
</tr>
<tr id="row13276210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1631230"><a name="p1631230"></a><a name="p1631230"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p65020802"><a name="p65020802"></a><a name="p65020802"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p32193639"><a name="p32193639"></a><a name="p32193639"></a>API注册时间</p>
</td>
</tr>
<tr id="row21307301"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48169854"><a name="p48169854"></a><a name="p48169854"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9444107"><a name="p9444107"></a><a name="p9444107"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p26775221"><a name="p26775221"></a><a name="p26775221"></a>API修改时间</p>
</td>
</tr>
<tr id="row39650400"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57565823"><a name="p57565823"></a><a name="p57565823"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p32320111"><a name="p32320111"></a><a name="p32320111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p683352"><a name="p683352"></a><a name="p683352"></a>API描述</p>
</td>
</tr>
<tr id="row6150169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28401641"><a name="p28401641"></a><a name="p28401641"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18831557"><a name="p18831557"></a><a name="p18831557"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48961174"><a name="p48961174"></a><a name="p48961174"></a>后端类型</p>
</td>
</tr>
<tr id="row57838348"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p54394634"><a name="p54394634"></a><a name="p54394634"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p43889208"><a name="p43889208"></a><a name="p43889208"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p65364926"><a name="p65364926"></a><a name="p65364926"></a>是否需要编排</p>
</td>
</tr>
<tr id="row129911514122713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p82576192276"><a name="p82576192276"></a><a name="p82576192276"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1625711193277"><a name="p1625711193277"></a><a name="p1625711193277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p6273141922718"><a name="p6273141922718"></a><a name="p6273141922718"></a>标签</p>
</td>
</tr>
<tr id="row8835717172720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p172881819162714"><a name="p172881819162714"></a><a name="p172881819162714"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p163043196278"><a name="p163043196278"></a><a name="p163043196278"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13320121932715"><a name="p13320121932715"></a><a name="p13320121932715"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="row05086382520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p250871111256"><a name="p250871111256"></a><a name="p250871111256"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p75081711102513"><a name="p75081711102513"></a><a name="p75081711102513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1752320115253"><a name="p1752320115253"></a><a name="p1752320115253"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
</td>
</tr>
<tr id="row14117157142512"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p205704118252"><a name="p205704118252"></a><a name="p205704118252"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13570141102519"><a name="p13570141102519"></a><a name="p13570141102519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p858631112257"><a name="p858631112257"></a><a name="p858631112257"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
<tr id="row65392912259"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p0633111142512"><a name="p0633111142512"></a><a name="p0633111142512"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p063315115255"><a name="p063315115255"></a><a name="p063315115255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p116482113255"><a name="p116482113255"></a><a name="p116482113255"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="row51413426"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p3737968"><a name="p3737968"></a><a name="p3737968"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34339995"><a name="p34339995"></a><a name="p34339995"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30076186"><a name="p30076186"></a><a name="p30076186"></a>后端服务：web后端详情</p>
</td>
</tr>
<tr id="row2250221"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p48050182"><a name="p48050182"></a><a name="p48050182"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66859495"><a name="p66859495"></a><a name="p66859495"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46910009"><a name="p46910009"></a><a name="p46910009"></a>后端服务：MOCK详情</p>
</td>
</tr>
<tr id="row19536899"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p38985025"><a name="p38985025"></a><a name="p38985025"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3670467"><a name="p3670467"></a><a name="p3670467"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p28872434"><a name="p28872434"></a><a name="p28872434"></a>后端服务：函数工作流后端详情</p>
</td>
</tr>
<tr id="row10999153874010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13999938164017"><a name="p13999938164017"></a><a name="p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1999203815404"><a name="p1999203815404"></a><a name="p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p11999143884013"><a name="p11999143884013"></a><a name="p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="row14202164214407"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p420294234017"><a name="p420294234017"></a><a name="p420294234017"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17202184217401"><a name="p17202184217401"></a><a name="p17202184217401"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p112025421400"><a name="p112025421400"></a><a name="p112025421400"></a>API的后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 10**  backend\_api参数说明

<a name="table58525317"></a>
<table><thead align="left"><tr id="row19542026"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p39400239"><a name="p39400239"></a><a name="p39400239"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p37302768"><a name="p37302768"></a><a name="p37302768"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p1625399"><a name="p1625399"></a><a name="p1625399"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row64548457"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p61042544"><a name="p61042544"></a><a name="p61042544"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p45499060"><a name="p45499060"></a><a name="p45499060"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p61545244"><a name="p61545244"></a><a name="p61545244"></a>编号</p>
</td>
</tr>
<tr id="row17036289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37762203"><a name="p37762203"></a><a name="p37762203"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p38839630"><a name="p38839630"></a><a name="p38839630"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p59002305"><a name="p59002305"></a><a name="p59002305"></a>状态</p>
</td>
</tr>
<tr id="row61258698"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63007488"><a name="p63007488"></a><a name="p63007488"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3332940"><a name="p3332940"></a><a name="p3332940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12150114811818"><a name="p12150114811818"></a><a name="p12150114811818"></a>后端endpoint</p>
</td>
</tr>
<tr id="row13794225"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p43590463"><a name="p43590463"></a><a name="p43590463"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p41166589"><a name="p41166589"></a><a name="p41166589"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46159379"><a name="p46159379"></a><a name="p46159379"></a>版本</p>
</td>
</tr>
<tr id="row12781231"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p28646781"><a name="p28646781"></a><a name="p28646781"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p38687928"><a name="p38687928"></a><a name="p38687928"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46714439"><a name="p46714439"></a><a name="p46714439"></a>访问协议</p>
</td>
</tr>
<tr id="row17776770"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p30632235"><a name="p30632235"></a><a name="p30632235"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p65291932"><a name="p65291932"></a><a name="p65291932"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54155134"><a name="p54155134"></a><a name="p54155134"></a>访问方式</p>
</td>
</tr>
<tr id="row17634160"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p19080894"><a name="p19080894"></a><a name="p19080894"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2048592"><a name="p2048592"></a><a name="p2048592"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p31718287"><a name="p31718287"></a><a name="p31718287"></a>访问地址</p>
</td>
</tr>
<tr id="row17029130"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37182327"><a name="p37182327"></a><a name="p37182327"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p58978500"><a name="p58978500"></a><a name="p58978500"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12529177"><a name="p12529177"></a><a name="p12529177"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row45653735"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6965020"><a name="p6965020"></a><a name="p6965020"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p27295725"><a name="p27295725"></a><a name="p27295725"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p63470148"><a name="p63470148"></a><a name="p63470148"></a>注册时间</p>
</td>
</tr>
<tr id="row34360420"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p31730620"><a name="p31730620"></a><a name="p31730620"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p20043404"><a name="p20043404"></a><a name="p20043404"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12903037"><a name="p12903037"></a><a name="p12903037"></a>修改时间</p>
</td>
</tr>
<tr id="row49018473"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p11073390"><a name="p11073390"></a><a name="p11073390"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p24529383"><a name="p24529383"></a><a name="p24529383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p40723005"><a name="p40723005"></a><a name="p40723005"></a>描述</p>
</td>
</tr>
<tr id="row30962726"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24952849"><a name="p24952849"></a><a name="p24952849"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p7914893"><a name="p7914893"></a><a name="p7914893"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p37126593"><a name="p37126593"></a><a name="p37126593"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="row65703888"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20414732"><a name="p20414732"></a><a name="p20414732"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p42980629"><a name="p42980629"></a><a name="p42980629"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p58878930"><a name="p58878930"></a><a name="p58878930"></a>VPC通道信息</p>
</td>
</tr>
</tbody>
</table>

**表 11**  mock\_info参数说明

<a name="table60148328"></a>
<table><thead align="left"><tr id="row10756468"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p65967568"><a name="p65967568"></a><a name="p65967568"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p41772752"><a name="p41772752"></a><a name="p41772752"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p28149724"><a name="p28149724"></a><a name="p28149724"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row65535197"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6750779"><a name="p6750779"></a><a name="p6750779"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9942237"><a name="p9942237"></a><a name="p9942237"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14892"><a name="p14892"></a><a name="p14892"></a>编号</p>
</td>
</tr>
<tr id="row134031"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p10856588"><a name="p10856588"></a><a name="p10856588"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p6968425"><a name="p6968425"></a><a name="p6968425"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27571534"><a name="p27571534"></a><a name="p27571534"></a>状态</p>
</td>
</tr>
<tr id="row46817220"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p34098441"><a name="p34098441"></a><a name="p34098441"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p10510314"><a name="p10510314"></a><a name="p10510314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46029137"><a name="p46029137"></a><a name="p46029137"></a>版本</p>
</td>
</tr>
<tr id="row11609049"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p808897"><a name="p808897"></a><a name="p808897"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p65520673"><a name="p65520673"></a><a name="p65520673"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5574306"><a name="p5574306"></a><a name="p5574306"></a>返回结果</p>
</td>
</tr>
<tr id="row50168758"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p37137611"><a name="p37137611"></a><a name="p37137611"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p55356500"><a name="p55356500"></a><a name="p55356500"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p54691514"><a name="p54691514"></a><a name="p54691514"></a>注册时间</p>
</td>
</tr>
<tr id="row22461579"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7448582"><a name="p7448582"></a><a name="p7448582"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66464274"><a name="p66464274"></a><a name="p66464274"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14897110"><a name="p14897110"></a><a name="p14897110"></a>修改时间</p>
</td>
</tr>
<tr id="row66965133"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p55466713"><a name="p55466713"></a><a name="p55466713"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p63618802"><a name="p63618802"></a><a name="p63618802"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p52849343"><a name="p52849343"></a><a name="p52849343"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 12**  func\_info参数说明

<a name="table5882045"></a>
<table><thead align="left"><tr id="row61925025"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p49871117"><a name="p49871117"></a><a name="p49871117"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p13028637"><a name="p13028637"></a><a name="p13028637"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p48686649"><a name="p48686649"></a><a name="p48686649"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row51304522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p62025656"><a name="p62025656"></a><a name="p62025656"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p58022250"><a name="p58022250"></a><a name="p58022250"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p2181833"><a name="p2181833"></a><a name="p2181833"></a>编号</p>
</td>
</tr>
<tr id="row19636500"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47052705"><a name="p47052705"></a><a name="p47052705"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p53172750"><a name="p53172750"></a><a name="p53172750"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p12025475"><a name="p12025475"></a><a name="p12025475"></a>状态</p>
</td>
</tr>
<tr id="row41120417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p42419446"><a name="p42419446"></a><a name="p42419446"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13423079"><a name="p13423079"></a><a name="p13423079"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13527646"><a name="p13527646"></a><a name="p13527646"></a>版本</p>
</td>
</tr>
<tr id="row54639950"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p63759814"><a name="p63759814"></a><a name="p63759814"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64271286"><a name="p64271286"></a><a name="p64271286"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p38591687"><a name="p38591687"></a><a name="p38591687"></a>函数URN</p>
</td>
</tr>
<tr id="row11780867"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p14726184"><a name="p14726184"></a><a name="p14726184"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51970241"><a name="p51970241"></a><a name="p51970241"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p48839991"><a name="p48839991"></a><a name="p48839991"></a>调用类型:async|sync</p>
</td>
</tr>
<tr id="row36906736"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p36655611"><a name="p36655611"></a><a name="p36655611"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16314519"><a name="p16314519"></a><a name="p16314519"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p46407659"><a name="p46407659"></a><a name="p46407659"></a>注册时间</p>
</td>
</tr>
<tr id="row15015754"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8316582"><a name="p8316582"></a><a name="p8316582"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2554575"><a name="p2554575"></a><a name="p2554575"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5594028"><a name="p5594028"></a><a name="p5594028"></a>更新时间</p>
</td>
</tr>
<tr id="row50346258"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p51515097"><a name="p51515097"></a><a name="p51515097"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p11973320"><a name="p11973320"></a><a name="p11973320"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p30314888"><a name="p30314888"></a><a name="p30314888"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="row4398542"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p20737610"><a name="p20737610"></a><a name="p20737610"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p2024810"><a name="p2024810"></a><a name="p2024810"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p29791894"><a name="p29791894"></a><a name="p29791894"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 13**  req\_params参数说明

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
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p9115133544413"><a name="p9115133544413"></a><a name="p9115133544413"></a>参数枚举值</p>
</td>
</tr>
<tr id="row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p151311235144415"><a name="p151311235144415"></a><a name="p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p713112353443"><a name="p713112353443"></a><a name="p713112353443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p01464350441"><a name="p01464350441"></a><a name="p01464350441"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8146203564415"><a name="p8146203564415"></a><a name="p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p31627353442"><a name="p31627353442"></a><a name="p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p117823511445"><a name="p117823511445"></a><a name="p117823511445"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p61782355443"><a name="p61782355443"></a><a name="p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p201932035194417"><a name="p201932035194417"></a><a name="p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1119312351443"><a name="p1119312351443"></a><a name="p1119312351443"></a>参数最小长度</p>
</td>
</tr>
<tr id="row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p12209535144412"><a name="p12209535144412"></a><a name="p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12251035164419"><a name="p12251035164419"></a><a name="p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13225335194419"><a name="p13225335194419"></a><a name="p13225335194419"></a>参数最大长度</p>
</td>
</tr>
<tr id="row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52401735134413"><a name="p52401735134413"></a><a name="p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p12240153510443"><a name="p12240153510443"></a><a name="p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1256035204417"><a name="p1256035204417"></a><a name="p1256035204417"></a>正则校验规则</p>
</td>
</tr>
<tr id="row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p202561335114413"><a name="p202561335114413"></a><a name="p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16271035114412"><a name="p16271035114412"></a><a name="p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1628793511445"><a name="p1628793511445"></a><a name="p1628793511445"></a>JSON校验规则</p>
</td>
</tr>
</tbody>
</table>

**表 14**  backend\_params参数说明

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
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p34431235184418"><a name="p34431235184418"></a><a name="p34431235184418"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1044312351449"><a name="p1044312351449"></a><a name="p1044312351449"></a>参数类别</p>
</td>
</tr>
<tr id="row445983511447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5475203519440"><a name="p5475203519440"></a><a name="p5475203519440"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1449053524417"><a name="p1449053524417"></a><a name="p1449053524417"></a>Integer</p>
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
    "url_domain": "xxxxxxxxxxx",
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

## 状态码<a name="section27584683"></a>

**表 15**  返回消息说明

<a name="table64322236"></a>
<table><thead align="left"><tr id="row3387693"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p5967751"><a name="p5967751"></a><a name="p5967751"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p13625850"><a name="p13625850"></a><a name="p13625850"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row29952045"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p10196552"><a name="p10196552"></a><a name="p10196552"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p73578115452"><a name="p73578115452"></a><a name="p73578115452"></a>Created</p>
</td>
</tr>
<tr id="row51311768"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p62612511"><a name="p62612511"></a><a name="p62612511"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p38448651"><a name="p38448651"></a><a name="p38448651"></a>Bad Request</p>
</td>
</tr>
<tr id="row10493547"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p44670953"><a name="p44670953"></a><a name="p44670953"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row17325755"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p61208905"><a name="p61208905"></a><a name="p61208905"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row61006437"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p42574382"><a name="p42574382"></a><a name="p42574382"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p25972887"><a name="p25972887"></a><a name="p25972887"></a>Not Found</p>
</td>
</tr>
<tr id="row32429391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9534987"><a name="p9534987"></a><a name="p9534987"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

