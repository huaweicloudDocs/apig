# 注册API<a name="ZH-CN_TOPIC_0000001082135161"></a>

## 功能介绍<a name="zh-cn_topic_0225568815_section11821014"></a>

添加一个API，API即一个服务接口，具体的服务能力。

API分为两部分，第一部分为面向API使用者的API接口，定义了使用者如何调用这个API。第二部分面向API提供者，由API提供者定义这个API的真实的后端情况，定义了API网关如何去访问真实的后端服务。

API的真实后端服务目前支持三种类型：传统的HTTP/HTTPS形式的web后端、函数工作流、MOCK。

## URI<a name="zh-cn_topic_0225568815_section39280262"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568815_table31836871"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row66270525"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568815_p66312269"><a name="zh-cn_topic_0225568815_p66312269"></a><a name="zh-cn_topic_0225568815_p66312269"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568815_p2584681"><a name="zh-cn_topic_0225568815_p2584681"></a><a name="zh-cn_topic_0225568815_p2584681"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row8032634"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568815_p46663656"><a name="zh-cn_topic_0225568815_p46663656"></a><a name="zh-cn_topic_0225568815_p46663656"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568815_p21659802"><a name="zh-cn_topic_0225568815_p21659802"></a><a name="zh-cn_topic_0225568815_p21659802"></a>/v1/{project_id}/apigw/instances/{instance_id}/apis</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568815_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p23103637"><a name="zh-cn_topic_0225568815_p23103637"></a><a name="zh-cn_topic_0225568815_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p59455291"><a name="zh-cn_topic_0225568815_p59455291"></a><a name="zh-cn_topic_0225568815_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p51149303"><a name="zh-cn_topic_0225568815_p51149303"></a><a name="zh-cn_topic_0225568815_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p49452846"><a name="zh-cn_topic_0225568815_p49452846"></a><a name="zh-cn_topic_0225568815_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p55878963"><a name="zh-cn_topic_0225568815_p55878963"></a><a name="zh-cn_topic_0225568815_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p29902160"><a name="zh-cn_topic_0225568815_p29902160"></a><a name="zh-cn_topic_0225568815_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p6155914"><a name="zh-cn_topic_0225568815_p6155914"></a><a name="zh-cn_topic_0225568815_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p28867016"><a name="zh-cn_topic_0225568815_p28867016"></a><a name="zh-cn_topic_0225568815_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1780913159538"><a name="zh-cn_topic_0225568815_p1780913159538"></a><a name="zh-cn_topic_0225568815_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p9809215115310"><a name="zh-cn_topic_0225568815_p9809215115310"></a><a name="zh-cn_topic_0225568815_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1280914152538"><a name="zh-cn_topic_0225568815_p1280914152538"></a><a name="zh-cn_topic_0225568815_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1880914157537"><a name="zh-cn_topic_0225568815_p1880914157537"></a><a name="zh-cn_topic_0225568815_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568815_section17978045"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568815_table9613561"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row51426513"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p4797990"><a name="zh-cn_topic_0225568815_p4797990"></a><a name="zh-cn_topic_0225568815_p4797990"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p53092887"><a name="zh-cn_topic_0225568815_p53092887"></a><a name="zh-cn_topic_0225568815_p53092887"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p5556622"><a name="zh-cn_topic_0225568815_p5556622"></a><a name="zh-cn_topic_0225568815_p5556622"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p47433200"><a name="zh-cn_topic_0225568815_p47433200"></a><a name="zh-cn_topic_0225568815_p47433200"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row16884007"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p25427355"><a name="zh-cn_topic_0225568815_p25427355"></a><a name="zh-cn_topic_0225568815_p25427355"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p46349875"><a name="zh-cn_topic_0225568815_p46349875"></a><a name="zh-cn_topic_0225568815_p46349875"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p63352408"><a name="zh-cn_topic_0225568815_p63352408"></a><a name="zh-cn_topic_0225568815_p63352408"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p31271409"><a name="zh-cn_topic_0225568815_p31271409"></a><a name="zh-cn_topic_0225568815_p31271409"></a>API所属的分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row46952608"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p45064875"><a name="zh-cn_topic_0225568815_p45064875"></a><a name="zh-cn_topic_0225568815_p45064875"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p26376263"><a name="zh-cn_topic_0225568815_p26376263"></a><a name="zh-cn_topic_0225568815_p26376263"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p56102555"><a name="zh-cn_topic_0225568815_p56102555"></a><a name="zh-cn_topic_0225568815_p56102555"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p48013136"><a name="zh-cn_topic_0225568815_p48013136"></a><a name="zh-cn_topic_0225568815_p48013136"></a>API名称</p>
<p id="zh-cn_topic_0225568815_p37858559"><a name="zh-cn_topic_0225568815_p37858559"></a><a name="zh-cn_topic_0225568815_p37858559"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以英文或中文开头。</p>
<div class="note" id="zh-cn_topic_0225568815_note690163615371"><a name="zh-cn_topic_0225568815_note690163615371"></a><a name="zh-cn_topic_0225568815_note690163615371"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p09053643719"><a name="zh-cn_topic_0225568815_p09053643719"></a><a name="zh-cn_topic_0225568815_p09053643719"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row25820024"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p11047224"><a name="zh-cn_topic_0225568815_p11047224"></a><a name="zh-cn_topic_0225568815_p11047224"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p22409969"><a name="zh-cn_topic_0225568815_p22409969"></a><a name="zh-cn_topic_0225568815_p22409969"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p3268170"><a name="zh-cn_topic_0225568815_p3268170"></a><a name="zh-cn_topic_0225568815_p3268170"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p63395179"><a name="zh-cn_topic_0225568815_p63395179"></a><a name="zh-cn_topic_0225568815_p63395179"></a>API类型：</p>
<a name="zh-cn_topic_0225568815_ul336530"></a><a name="zh-cn_topic_0225568815_ul336530"></a><ul id="zh-cn_topic_0225568815_ul336530"><li>1：公有API</li><li>2：私有API</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row44004246"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p7574169"><a name="zh-cn_topic_0225568815_p7574169"></a><a name="zh-cn_topic_0225568815_p7574169"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p9527961"><a name="zh-cn_topic_0225568815_p9527961"></a><a name="zh-cn_topic_0225568815_p9527961"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p33567357"><a name="zh-cn_topic_0225568815_p33567357"></a><a name="zh-cn_topic_0225568815_p33567357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p34601390"><a name="zh-cn_topic_0225568815_p34601390"></a><a name="zh-cn_topic_0225568815_p34601390"></a>API的版本</p>
<p id="zh-cn_topic_0225568815_p5389164716429"><a name="zh-cn_topic_0225568815_p5389164716429"></a><a name="zh-cn_topic_0225568815_p5389164716429"></a>字符长度不超过16</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row58589356"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p48117435"><a name="zh-cn_topic_0225568815_p48117435"></a><a name="zh-cn_topic_0225568815_p48117435"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p5198195"><a name="zh-cn_topic_0225568815_p5198195"></a><a name="zh-cn_topic_0225568815_p5198195"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p18400635"><a name="zh-cn_topic_0225568815_p18400635"></a><a name="zh-cn_topic_0225568815_p18400635"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p14056443"><a name="zh-cn_topic_0225568815_p14056443"></a><a name="zh-cn_topic_0225568815_p14056443"></a>API的请求协议：</p>
<a name="zh-cn_topic_0225568815_ul14361951"></a><a name="zh-cn_topic_0225568815_ul14361951"></a><ul id="zh-cn_topic_0225568815_ul14361951"><li>HTTP</li><li>HTTPS</li><li>BOTH：同时支持HTTP和HTTPS</li></ul>
<p id="zh-cn_topic_0225568815_p4179246"><a name="zh-cn_topic_0225568815_p4179246"></a><a name="zh-cn_topic_0225568815_p4179246"></a>默认：HTTPS</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row37613216"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p26771660"><a name="zh-cn_topic_0225568815_p26771660"></a><a name="zh-cn_topic_0225568815_p26771660"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p21020848"><a name="zh-cn_topic_0225568815_p21020848"></a><a name="zh-cn_topic_0225568815_p21020848"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p24967157"><a name="zh-cn_topic_0225568815_p24967157"></a><a name="zh-cn_topic_0225568815_p24967157"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p9073859"><a name="zh-cn_topic_0225568815_p9073859"></a><a name="zh-cn_topic_0225568815_p9073859"></a>API的请求方式：</p>
<a name="zh-cn_topic_0225568815_ul46261614"></a><a name="zh-cn_topic_0225568815_ul46261614"></a><ul id="zh-cn_topic_0225568815_ul46261614"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row3177191"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p56025891"><a name="zh-cn_topic_0225568815_p56025891"></a><a name="zh-cn_topic_0225568815_p56025891"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p41803348"><a name="zh-cn_topic_0225568815_p41803348"></a><a name="zh-cn_topic_0225568815_p41803348"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p30628066"><a name="zh-cn_topic_0225568815_p30628066"></a><a name="zh-cn_topic_0225568815_p30628066"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p64954292"><a name="zh-cn_topic_0225568815_p64954292"></a><a name="zh-cn_topic_0225568815_p64954292"></a>API的访问地址</p>
<div class="note" id="zh-cn_topic_0225568815_note38431529153919"><a name="zh-cn_topic_0225568815_note38431529153919"></a><a name="zh-cn_topic_0225568815_note38431529153919"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p18843122918398"><a name="zh-cn_topic_0225568815_p18843122918398"></a><a name="zh-cn_topic_0225568815_p18843122918398"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row51064406"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p42576202"><a name="zh-cn_topic_0225568815_p42576202"></a><a name="zh-cn_topic_0225568815_p42576202"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p26120331"><a name="zh-cn_topic_0225568815_p26120331"></a><a name="zh-cn_topic_0225568815_p26120331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p35372032"><a name="zh-cn_topic_0225568815_p35372032"></a><a name="zh-cn_topic_0225568815_p35372032"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p46562321"><a name="zh-cn_topic_0225568815_p46562321"></a><a name="zh-cn_topic_0225568815_p46562321"></a>API的匹配方式：</p>
<a name="zh-cn_topic_0225568815_ul8369025"></a><a name="zh-cn_topic_0225568815_ul8369025"></a><ul id="zh-cn_topic_0225568815_ul8369025"><li>SWA：前缀匹配</li><li>NORMAL：正常匹配（绝对匹配）</li></ul>
<p id="zh-cn_topic_0225568815_p54641218412"><a name="zh-cn_topic_0225568815_p54641218412"></a><a name="zh-cn_topic_0225568815_p54641218412"></a>默认：NORMAL</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row61222081"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p60041530"><a name="zh-cn_topic_0225568815_p60041530"></a><a name="zh-cn_topic_0225568815_p60041530"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p31525796"><a name="zh-cn_topic_0225568815_p31525796"></a><a name="zh-cn_topic_0225568815_p31525796"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p3452711"><a name="zh-cn_topic_0225568815_p3452711"></a><a name="zh-cn_topic_0225568815_p3452711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p11234154"><a name="zh-cn_topic_0225568815_p11234154"></a><a name="zh-cn_topic_0225568815_p11234154"></a>API描述</p>
<p id="zh-cn_topic_0225568815_p2416961"><a name="zh-cn_topic_0225568815_p2416961"></a><a name="zh-cn_topic_0225568815_p2416961"></a>字符长度不超过255</p>
<div class="note" id="zh-cn_topic_0225568815_note1069572664018"><a name="zh-cn_topic_0225568815_note1069572664018"></a><a name="zh-cn_topic_0225568815_note1069572664018"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p11697926124010"><a name="zh-cn_topic_0225568815_p11697926124010"></a><a name="zh-cn_topic_0225568815_p11697926124010"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row14009080"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p60993670"><a name="zh-cn_topic_0225568815_p60993670"></a><a name="zh-cn_topic_0225568815_p60993670"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p41540204"><a name="zh-cn_topic_0225568815_p41540204"></a><a name="zh-cn_topic_0225568815_p41540204"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p9313363"><a name="zh-cn_topic_0225568815_p9313363"></a><a name="zh-cn_topic_0225568815_p9313363"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p16184930"><a name="zh-cn_topic_0225568815_p16184930"></a><a name="zh-cn_topic_0225568815_p16184930"></a>API的认证方式：</p>
<a name="zh-cn_topic_0225568815_ul1496884"></a><a name="zh-cn_topic_0225568815_ul1496884"></a><ul id="zh-cn_topic_0225568815_ul1496884"><li>NONE：无认证</li><li>APP：APP认证</li><li>IAM：IAM认证</li><li>AUTHORIZER：自定义认证</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row21088616355"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1038662319534"><a name="zh-cn_topic_0225568815_p1038662319534"></a><a name="zh-cn_topic_0225568815_p1038662319534"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p16386823125311"><a name="zh-cn_topic_0225568815_p16386823125311"></a><a name="zh-cn_topic_0225568815_p16386823125311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p3386162317532"><a name="zh-cn_topic_0225568815_p3386162317532"></a><a name="zh-cn_topic_0225568815_p3386162317532"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1386122375314"><a name="zh-cn_topic_0225568815_p1386122375314"></a><a name="zh-cn_topic_0225568815_p1386122375314"></a>认证方式参数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row201991410162820"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p18639182918193"><a name="zh-cn_topic_0225568815_p18639182918193"></a><a name="zh-cn_topic_0225568815_p18639182918193"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p18242111382911"><a name="zh-cn_topic_0225568815_p18242111382911"></a><a name="zh-cn_topic_0225568815_p18242111382911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p6795718112914"><a name="zh-cn_topic_0225568815_p6795718112914"></a><a name="zh-cn_topic_0225568815_p6795718112914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p17639829131912"><a name="zh-cn_topic_0225568815_p17639829131912"></a><a name="zh-cn_topic_0225568815_p17639829131912"></a>前端自定义认证对象的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row23162817"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p64248927"><a name="zh-cn_topic_0225568815_p64248927"></a><a name="zh-cn_topic_0225568815_p64248927"></a>backend_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p36780609"><a name="zh-cn_topic_0225568815_p36780609"></a><a name="zh-cn_topic_0225568815_p36780609"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p26439376"><a name="zh-cn_topic_0225568815_p26439376"></a><a name="zh-cn_topic_0225568815_p26439376"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p61214707"><a name="zh-cn_topic_0225568815_p61214707"></a><a name="zh-cn_topic_0225568815_p61214707"></a>后端类型：</p>
<a name="zh-cn_topic_0225568815_ul65236141"></a><a name="zh-cn_topic_0225568815_ul65236141"></a><ul id="zh-cn_topic_0225568815_ul65236141"><li>HTTP：web后端</li><li>FUNCTION：函数工作流</li><li>MOCK：模拟的后端</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7589137172110"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1732142241016"><a name="zh-cn_topic_0225568815_p1732142241016"></a><a name="zh-cn_topic_0225568815_p1732142241016"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p3321222191014"><a name="zh-cn_topic_0225568815_p3321222191014"></a><a name="zh-cn_topic_0225568815_p3321222191014"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p0329228101"><a name="zh-cn_topic_0225568815_p0329228101"></a><a name="zh-cn_topic_0225568815_p0329228101"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1832172251014"><a name="zh-cn_topic_0225568815_p1832172251014"></a><a name="zh-cn_topic_0225568815_p1832172251014"></a>服务名称标签</p>
<p id="zh-cn_topic_0225568815_p1615201832417"><a name="zh-cn_topic_0225568815_p1615201832417"></a><a name="zh-cn_topic_0225568815_p1615201832417"></a>待废弃字段</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row145864211376"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1396610102116"><a name="zh-cn_topic_0225568815_p1396610102116"></a><a name="zh-cn_topic_0225568815_p1396610102116"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p496641182113"><a name="zh-cn_topic_0225568815_p496641182113"></a><a name="zh-cn_topic_0225568815_p496641182113"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p129663117215"><a name="zh-cn_topic_0225568815_p129663117215"></a><a name="zh-cn_topic_0225568815_p129663117215"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p119661113217"><a name="zh-cn_topic_0225568815_p119661113217"></a><a name="zh-cn_topic_0225568815_p119661113217"></a>标签</p>
<p id="zh-cn_topic_0225568815_p056019015229"><a name="zh-cn_topic_0225568815_p056019015229"></a><a name="zh-cn_topic_0225568815_p056019015229"></a>包含一个服务名称标签和若干其它标签</p>
<p id="zh-cn_topic_0225568815_p125522722313"><a name="zh-cn_topic_0225568815_p125522722313"></a><a name="zh-cn_topic_0225568815_p125522722313"></a>服务名称标签非必填，必须以APIG-SN-开头</p>
<p id="zh-cn_topic_0225568815_p79633336238"><a name="zh-cn_topic_0225568815_p79633336238"></a><a name="zh-cn_topic_0225568815_p79633336238"></a>其它标签非必填，且不能以APIG-SN-开头</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row152631022114"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p526201042116"><a name="zh-cn_topic_0225568815_p526201042116"></a><a name="zh-cn_topic_0225568815_p526201042116"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1426191062120"><a name="zh-cn_topic_0225568815_p1426191062120"></a><a name="zh-cn_topic_0225568815_p1426191062120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p726151042117"><a name="zh-cn_topic_0225568815_p726151042117"></a><a name="zh-cn_topic_0225568815_p726151042117"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p7213201015015"><a name="zh-cn_topic_0225568815_p7213201015015"></a><a name="zh-cn_topic_0225568815_p7213201015015"></a>是否支持跨域</p>
<a name="zh-cn_topic_0225568815_ul38673529507"></a><a name="zh-cn_topic_0225568815_ul38673529507"></a><ul id="zh-cn_topic_0225568815_ul38673529507"><li>TRUE：支持</li><li>FALSE：不支持</li></ul>
<p id="zh-cn_topic_0225568815_p17882165245011"><a name="zh-cn_topic_0225568815_p17882165245011"></a><a name="zh-cn_topic_0225568815_p17882165245011"></a>默认：FALSE</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row11977120131916"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p59931303198"><a name="zh-cn_topic_0225568815_p59931303198"></a><a name="zh-cn_topic_0225568815_p59931303198"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p912844617206"><a name="zh-cn_topic_0225568815_p912844617206"></a><a name="zh-cn_topic_0225568815_p912844617206"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p79937041913"><a name="zh-cn_topic_0225568815_p79937041913"></a><a name="zh-cn_topic_0225568815_p79937041913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p148471111162112"><a name="zh-cn_topic_0225568815_p148471111162112"></a><a name="zh-cn_topic_0225568815_p148471111162112"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
<p id="zh-cn_topic_0225568815_p984751162120"><a name="zh-cn_topic_0225568815_p984751162120"></a><a name="zh-cn_topic_0225568815_p984751162120"></a>字符长度不超过20480</p>
<div class="note" id="zh-cn_topic_0225568815_note986331142110"><a name="zh-cn_topic_0225568815_note986331142110"></a><a name="zh-cn_topic_0225568815_note986331142110"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p1686314115212"><a name="zh-cn_topic_0225568815_p1686314115212"></a><a name="zh-cn_topic_0225568815_p1686314115212"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row194617661914"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p5946166161919"><a name="zh-cn_topic_0225568815_p5946166161919"></a><a name="zh-cn_topic_0225568815_p5946166161919"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p10946136161918"><a name="zh-cn_topic_0225568815_p10946136161918"></a><a name="zh-cn_topic_0225568815_p10946136161918"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p19461065195"><a name="zh-cn_topic_0225568815_p19461065195"></a><a name="zh-cn_topic_0225568815_p19461065195"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p7946166193"><a name="zh-cn_topic_0225568815_p7946166193"></a><a name="zh-cn_topic_0225568815_p7946166193"></a>正常响应示例，描述API的正常返回信息</p>
<p id="zh-cn_topic_0225568815_p1935514810223"><a name="zh-cn_topic_0225568815_p1935514810223"></a><a name="zh-cn_topic_0225568815_p1935514810223"></a>字符长度不超过20480</p>
<div class="note" id="zh-cn_topic_0225568815_note1649674102319"><a name="zh-cn_topic_0225568815_note1649674102319"></a><a name="zh-cn_topic_0225568815_note1649674102319"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p165129415232"><a name="zh-cn_topic_0225568815_p165129415232"></a><a name="zh-cn_topic_0225568815_p165129415232"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1327418118195"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p727431112199"><a name="zh-cn_topic_0225568815_p727431112199"></a><a name="zh-cn_topic_0225568815_p727431112199"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p142741211171914"><a name="zh-cn_topic_0225568815_p142741211171914"></a><a name="zh-cn_topic_0225568815_p142741211171914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p18274181181910"><a name="zh-cn_topic_0225568815_p18274181181910"></a><a name="zh-cn_topic_0225568815_p18274181181910"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1227471181914"><a name="zh-cn_topic_0225568815_p1227471181914"></a><a name="zh-cn_topic_0225568815_p1227471181914"></a>失败返回示例，描述API的异常返回信息</p>
<p id="zh-cn_topic_0225568815_p132518115249"><a name="zh-cn_topic_0225568815_p132518115249"></a><a name="zh-cn_topic_0225568815_p132518115249"></a>字符长度不超过20480</p>
<div class="note" id="zh-cn_topic_0225568815_note13283119202415"><a name="zh-cn_topic_0225568815_note13283119202415"></a><a name="zh-cn_topic_0225568815_note13283119202415"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p23141919202413"><a name="zh-cn_topic_0225568815_p23141919202413"></a><a name="zh-cn_topic_0225568815_p23141919202413"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row61097128"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p49920342"><a name="zh-cn_topic_0225568815_p49920342"></a><a name="zh-cn_topic_0225568815_p49920342"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p17015941"><a name="zh-cn_topic_0225568815_p17015941"></a><a name="zh-cn_topic_0225568815_p17015941"></a>backend_type = HTTP时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p36114013"><a name="zh-cn_topic_0225568815_p36114013"></a><a name="zh-cn_topic_0225568815_p36114013"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p39553925"><a name="zh-cn_topic_0225568815_p39553925"></a><a name="zh-cn_topic_0225568815_p39553925"></a>web后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row45108818"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p29935642"><a name="zh-cn_topic_0225568815_p29935642"></a><a name="zh-cn_topic_0225568815_p29935642"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p8867951"><a name="zh-cn_topic_0225568815_p8867951"></a><a name="zh-cn_topic_0225568815_p8867951"></a>backend_type = MOCK时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p47215416"><a name="zh-cn_topic_0225568815_p47215416"></a><a name="zh-cn_topic_0225568815_p47215416"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p66352350"><a name="zh-cn_topic_0225568815_p66352350"></a><a name="zh-cn_topic_0225568815_p66352350"></a>mock后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row52481162"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p23115734"><a name="zh-cn_topic_0225568815_p23115734"></a><a name="zh-cn_topic_0225568815_p23115734"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p60435162"><a name="zh-cn_topic_0225568815_p60435162"></a><a name="zh-cn_topic_0225568815_p60435162"></a>backend_type = FUNCTION时必填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p63409983"><a name="zh-cn_topic_0225568815_p63409983"></a><a name="zh-cn_topic_0225568815_p63409983"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p35935021"><a name="zh-cn_topic_0225568815_p35935021"></a><a name="zh-cn_topic_0225568815_p35935021"></a>函数工作流后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row168317015213"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p156831806524"><a name="zh-cn_topic_0225568815_p156831806524"></a><a name="zh-cn_topic_0225568815_p156831806524"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p76831801527"><a name="zh-cn_topic_0225568815_p76831801527"></a><a name="zh-cn_topic_0225568815_p76831801527"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p176831903520"><a name="zh-cn_topic_0225568815_p176831903520"></a><a name="zh-cn_topic_0225568815_p176831903520"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p468350195218"><a name="zh-cn_topic_0225568815_p468350195218"></a><a name="zh-cn_topic_0225568815_p468350195218"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row166884018355"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p06884014357"><a name="zh-cn_topic_0225568815_p06884014357"></a><a name="zh-cn_topic_0225568815_p06884014357"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p46814011357"><a name="zh-cn_topic_0225568815_p46814011357"></a><a name="zh-cn_topic_0225568815_p46814011357"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p17681640163511"><a name="zh-cn_topic_0225568815_p17681640163511"></a><a name="zh-cn_topic_0225568815_p17681640163511"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p76844033510"><a name="zh-cn_topic_0225568815_p76844033510"></a><a name="zh-cn_topic_0225568815_p76844033510"></a>API的后端参数列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row8288245503"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p52112129216"><a name="zh-cn_topic_0225568815_p52112129216"></a><a name="zh-cn_topic_0225568815_p52112129216"></a>policy_https</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p20225612162111"><a name="zh-cn_topic_0225568815_p20225612162111"></a><a name="zh-cn_topic_0225568815_p20225612162111"></a>backend_type = HTTP时选填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p42382127211"><a name="zh-cn_topic_0225568815_p42382127211"></a><a name="zh-cn_topic_0225568815_p42382127211"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p112511312102117"><a name="zh-cn_topic_0225568815_p112511312102117"></a><a name="zh-cn_topic_0225568815_p112511312102117"></a>web策略后端列表。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row4851728165015"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1027141242118"><a name="zh-cn_topic_0225568815_p1027141242118"></a><a name="zh-cn_topic_0225568815_p1027141242118"></a>policy_mocks</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p13285712192110"><a name="zh-cn_topic_0225568815_p13285712192110"></a><a name="zh-cn_topic_0225568815_p13285712192110"></a>backend_type = MOCK时选填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1930181292111"><a name="zh-cn_topic_0225568815_p1930181292111"></a><a name="zh-cn_topic_0225568815_p1930181292111"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p173121512142120"><a name="zh-cn_topic_0225568815_p173121512142120"></a><a name="zh-cn_topic_0225568815_p173121512142120"></a>mock策略后端列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row12102123185010"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p83271112142115"><a name="zh-cn_topic_0225568815_p83271112142115"></a><a name="zh-cn_topic_0225568815_p83271112142115"></a>policy_functions</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p2338191219210"><a name="zh-cn_topic_0225568815_p2338191219210"></a><a name="zh-cn_topic_0225568815_p2338191219210"></a>backend_type = FUNCTION时选填</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p18355912102115"><a name="zh-cn_topic_0225568815_p18355912102115"></a><a name="zh-cn_topic_0225568815_p18355912102115"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1536961292110"><a name="zh-cn_topic_0225568815_p1536961292110"></a><a name="zh-cn_topic_0225568815_p1536961292110"></a>函数工作流策略后端列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  backend\_api参数说明

<a name="zh-cn_topic_0225568815_table24173475"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row27724933"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p31127089"><a name="zh-cn_topic_0225568815_p31127089"></a><a name="zh-cn_topic_0225568815_p31127089"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.16%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p38266241"><a name="zh-cn_topic_0225568815_p38266241"></a><a name="zh-cn_topic_0225568815_p38266241"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.11%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p12557789"><a name="zh-cn_topic_0225568815_p12557789"></a><a name="zh-cn_topic_0225568815_p12557789"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p10548014"><a name="zh-cn_topic_0225568815_p10548014"></a><a name="zh-cn_topic_0225568815_p10548014"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row49082844"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p16287438"><a name="zh-cn_topic_0225568815_p16287438"></a><a name="zh-cn_topic_0225568815_p16287438"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1741473216910"><a name="zh-cn_topic_0225568815_p1741473216910"></a><a name="zh-cn_topic_0225568815_p1741473216910"></a>后端服务不使用VPC通道时，必选</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p24574368"><a name="zh-cn_topic_0225568815_p24574368"></a><a name="zh-cn_topic_0225568815_p24574368"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p44366800"><a name="zh-cn_topic_0225568815_p44366800"></a><a name="zh-cn_topic_0225568815_p44366800"></a>后端服务的地址。</p>
<p id="zh-cn_topic_0225568815_p9406451538"><a name="zh-cn_topic_0225568815_p9406451538"></a><a name="zh-cn_topic_0225568815_p9406451538"></a>由域名（或IP地址）和端口号组成，总长度不超过255。格式为域名:端口（如：apig.example.com:7443）。如果不写端口，则HTTPS默认端口号为443， HTTP默认端口号为80。</p>
<p id="zh-cn_topic_0225568815_p13446109556"><a name="zh-cn_topic_0225568815_p13446109556"></a><a name="zh-cn_topic_0225568815_p13446109556"></a>支持环境变量，使用环境变量时，每个变量名的长度为3 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row64033799"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p19355245"><a name="zh-cn_topic_0225568815_p19355245"></a><a name="zh-cn_topic_0225568815_p19355245"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p24271019"><a name="zh-cn_topic_0225568815_p24271019"></a><a name="zh-cn_topic_0225568815_p24271019"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p19795562"><a name="zh-cn_topic_0225568815_p19795562"></a><a name="zh-cn_topic_0225568815_p19795562"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p59936722"><a name="zh-cn_topic_0225568815_p59936722"></a><a name="zh-cn_topic_0225568815_p59936722"></a>web后端版本</p>
<p id="zh-cn_topic_0225568815_p15916160104318"><a name="zh-cn_topic_0225568815_p15916160104318"></a><a name="zh-cn_topic_0225568815_p15916160104318"></a>字符长度不超过16</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row6000091"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p16245391"><a name="zh-cn_topic_0225568815_p16245391"></a><a name="zh-cn_topic_0225568815_p16245391"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p40808295"><a name="zh-cn_topic_0225568815_p40808295"></a><a name="zh-cn_topic_0225568815_p40808295"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p17137612"><a name="zh-cn_topic_0225568815_p17137612"></a><a name="zh-cn_topic_0225568815_p17137612"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p45969317"><a name="zh-cn_topic_0225568815_p45969317"></a><a name="zh-cn_topic_0225568815_p45969317"></a>请求协议：</p>
<a name="zh-cn_topic_0225568815_ul4739707"></a><a name="zh-cn_topic_0225568815_ul4739707"></a><ul id="zh-cn_topic_0225568815_ul4739707"><li>HTTP</li><li>HTTPS</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row32695023"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p31051236"><a name="zh-cn_topic_0225568815_p31051236"></a><a name="zh-cn_topic_0225568815_p31051236"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p32122210"><a name="zh-cn_topic_0225568815_p32122210"></a><a name="zh-cn_topic_0225568815_p32122210"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p51762192"><a name="zh-cn_topic_0225568815_p51762192"></a><a name="zh-cn_topic_0225568815_p51762192"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p31987990"><a name="zh-cn_topic_0225568815_p31987990"></a><a name="zh-cn_topic_0225568815_p31987990"></a>请求方式：</p>
<a name="zh-cn_topic_0225568815_ul47767884"></a><a name="zh-cn_topic_0225568815_ul47767884"></a><ul id="zh-cn_topic_0225568815_ul47767884"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row26241179"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p45160793"><a name="zh-cn_topic_0225568815_p45160793"></a><a name="zh-cn_topic_0225568815_p45160793"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p34145627"><a name="zh-cn_topic_0225568815_p34145627"></a><a name="zh-cn_topic_0225568815_p34145627"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p14332426"><a name="zh-cn_topic_0225568815_p14332426"></a><a name="zh-cn_topic_0225568815_p14332426"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p20075853"><a name="zh-cn_topic_0225568815_p20075853"></a><a name="zh-cn_topic_0225568815_p20075853"></a>请求地址</p>
<p id="zh-cn_topic_0225568815_p1273516206484"><a name="zh-cn_topic_0225568815_p1273516206484"></a><a name="zh-cn_topic_0225568815_p1273516206484"></a>总长度不超过512，且满足URI规范。</p>
<p id="zh-cn_topic_0225568815_p144251235114414"><a name="zh-cn_topic_0225568815_p144251235114414"></a><a name="zh-cn_topic_0225568815_p144251235114414"></a>支持环境变量，使用环境变量时，每个变量名的长度为3 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”组成，且只能以英文开头。</p>
<div class="note" id="zh-cn_topic_0225568815_note1597012134438"><a name="zh-cn_topic_0225568815_note1597012134438"></a><a name="zh-cn_topic_0225568815_note1597012134438"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p1597171324315"><a name="zh-cn_topic_0225568815_p1597171324315"></a><a name="zh-cn_topic_0225568815_p1597171324315"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row30294306"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p37919687"><a name="zh-cn_topic_0225568815_p37919687"></a><a name="zh-cn_topic_0225568815_p37919687"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p51595784"><a name="zh-cn_topic_0225568815_p51595784"></a><a name="zh-cn_topic_0225568815_p51595784"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p18509007"><a name="zh-cn_topic_0225568815_p18509007"></a><a name="zh-cn_topic_0225568815_p18509007"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p22901445134415"><a name="zh-cn_topic_0225568815_p22901445134415"></a><a name="zh-cn_topic_0225568815_p22901445134415"></a>API网关请求后端服务的超时时间。超时时间最大值可以通过实例特性backend_timeout配置修改。</p>
<p id="zh-cn_topic_0225568815_p102901445134414"><a name="zh-cn_topic_0225568815_p102901445134414"></a><a name="zh-cn_topic_0225568815_p102901445134414"></a>单位：毫秒。</p>
<p id="zh-cn_topic_0225568815_p182901945154418"><a name="zh-cn_topic_0225568815_p182901945154418"></a><a name="zh-cn_topic_0225568815_p182901945154418"></a>最小值：<strong id="zh-cn_topic_0225568815_b14290645184415"><a name="zh-cn_topic_0225568815_b14290645184415"></a><a name="zh-cn_topic_0225568815_b14290645184415"></a>1</strong></p>
<p id="zh-cn_topic_0225568815_p1529054515449"><a name="zh-cn_topic_0225568815_p1529054515449"></a><a name="zh-cn_topic_0225568815_p1529054515449"></a>最大值：<strong id="zh-cn_topic_0225568815_b129015457448"><a name="zh-cn_topic_0225568815_b129015457448"></a><a name="zh-cn_topic_0225568815_b129015457448"></a>600000</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row48499315"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p36130470"><a name="zh-cn_topic_0225568815_p36130470"></a><a name="zh-cn_topic_0225568815_p36130470"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p40886937"><a name="zh-cn_topic_0225568815_p40886937"></a><a name="zh-cn_topic_0225568815_p40886937"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p23507572"><a name="zh-cn_topic_0225568815_p23507572"></a><a name="zh-cn_topic_0225568815_p23507572"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p25065184"><a name="zh-cn_topic_0225568815_p25065184"></a><a name="zh-cn_topic_0225568815_p25065184"></a>描述</p>
<p id="zh-cn_topic_0225568815_p18908459"><a name="zh-cn_topic_0225568815_p18908459"></a><a name="zh-cn_topic_0225568815_p18908459"></a>字符长度不超过255</p>
<div class="note" id="zh-cn_topic_0225568815_note14776192410444"><a name="zh-cn_topic_0225568815_note14776192410444"></a><a name="zh-cn_topic_0225568815_note14776192410444"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p197771624144419"><a name="zh-cn_topic_0225568815_p197771624144419"></a><a name="zh-cn_topic_0225568815_p197771624144419"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row54459243"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p49122562"><a name="zh-cn_topic_0225568815_p49122562"></a><a name="zh-cn_topic_0225568815_p49122562"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p19504577"><a name="zh-cn_topic_0225568815_p19504577"></a><a name="zh-cn_topic_0225568815_p19504577"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p36366929"><a name="zh-cn_topic_0225568815_p36366929"></a><a name="zh-cn_topic_0225568815_p36366929"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p60040154"><a name="zh-cn_topic_0225568815_p60040154"></a><a name="zh-cn_topic_0225568815_p60040154"></a>是否使用VPC通道：</p>
<a name="zh-cn_topic_0225568815_ul17737046"></a><a name="zh-cn_topic_0225568815_ul17737046"></a><ul id="zh-cn_topic_0225568815_ul17737046"><li>1 : 使用VPC通道</li><li>2 : 不使用VPC通道</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row45404886"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p53917160"><a name="zh-cn_topic_0225568815_p53917160"></a><a name="zh-cn_topic_0225568815_p53917160"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p5213863"><a name="zh-cn_topic_0225568815_p5213863"></a><a name="zh-cn_topic_0225568815_p5213863"></a>如果vpc_status=1，则这个字典类型为必填信息</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p19669754"><a name="zh-cn_topic_0225568815_p19669754"></a><a name="zh-cn_topic_0225568815_p19669754"></a>字典类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p49746250"><a name="zh-cn_topic_0225568815_p49746250"></a><a name="zh-cn_topic_0225568815_p49746250"></a>VPC通道详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row14763174211304"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p4426105522114"><a name="zh-cn_topic_0225568815_p4426105522114"></a><a name="zh-cn_topic_0225568815_p4426105522114"></a>authorizer_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.16%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p117759543118"><a name="zh-cn_topic_0225568815_p117759543118"></a><a name="zh-cn_topic_0225568815_p117759543118"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1754710210315"><a name="zh-cn_topic_0225568815_p1754710210315"></a><a name="zh-cn_topic_0225568815_p1754710210315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p116491557133012"><a name="zh-cn_topic_0225568815_p116491557133012"></a><a name="zh-cn_topic_0225568815_p116491557133012"></a>后端自定义认证对象的ID</p>
</td>
</tr>
</tbody>
</table>

**表 5**  VPC通道参数说明

<a name="zh-cn_topic_0225568815_table26229873"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row61659324"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p28349332"><a name="zh-cn_topic_0225568815_p28349332"></a><a name="zh-cn_topic_0225568815_p28349332"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p14594532"><a name="zh-cn_topic_0225568815_p14594532"></a><a name="zh-cn_topic_0225568815_p14594532"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p41306453"><a name="zh-cn_topic_0225568815_p41306453"></a><a name="zh-cn_topic_0225568815_p41306453"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p57488398"><a name="zh-cn_topic_0225568815_p57488398"></a><a name="zh-cn_topic_0225568815_p57488398"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row26048696"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p135916441067"><a name="zh-cn_topic_0225568815_p135916441067"></a><a name="zh-cn_topic_0225568815_p135916441067"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p46332158"><a name="zh-cn_topic_0225568815_p46332158"></a><a name="zh-cn_topic_0225568815_p46332158"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p61917289"><a name="zh-cn_topic_0225568815_p61917289"></a><a name="zh-cn_topic_0225568815_p61917289"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p49244517"><a name="zh-cn_topic_0225568815_p49244517"></a><a name="zh-cn_topic_0225568815_p49244517"></a>VPC通道编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row63119848"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p12434084"><a name="zh-cn_topic_0225568815_p12434084"></a><a name="zh-cn_topic_0225568815_p12434084"></a>vpc_proxy_host</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p527917"><a name="zh-cn_topic_0225568815_p527917"></a><a name="zh-cn_topic_0225568815_p527917"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p42761322"><a name="zh-cn_topic_0225568815_p42761322"></a><a name="zh-cn_topic_0225568815_p42761322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p41115076"><a name="zh-cn_topic_0225568815_p41115076"></a><a name="zh-cn_topic_0225568815_p41115076"></a>代理主机</p>
</td>
</tr>
</tbody>
</table>

**表 6**  mock\_info参数说明

<a name="zh-cn_topic_0225568815_table42337334"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row33365929"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p18285723"><a name="zh-cn_topic_0225568815_p18285723"></a><a name="zh-cn_topic_0225568815_p18285723"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p4748581"><a name="zh-cn_topic_0225568815_p4748581"></a><a name="zh-cn_topic_0225568815_p4748581"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p49090800"><a name="zh-cn_topic_0225568815_p49090800"></a><a name="zh-cn_topic_0225568815_p49090800"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p16931876"><a name="zh-cn_topic_0225568815_p16931876"></a><a name="zh-cn_topic_0225568815_p16931876"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row29304679"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p24868836"><a name="zh-cn_topic_0225568815_p24868836"></a><a name="zh-cn_topic_0225568815_p24868836"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1109825"><a name="zh-cn_topic_0225568815_p1109825"></a><a name="zh-cn_topic_0225568815_p1109825"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p22786982"><a name="zh-cn_topic_0225568815_p22786982"></a><a name="zh-cn_topic_0225568815_p22786982"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p33806268"><a name="zh-cn_topic_0225568815_p33806268"></a><a name="zh-cn_topic_0225568815_p33806268"></a>返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row15816706"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p6084841"><a name="zh-cn_topic_0225568815_p6084841"></a><a name="zh-cn_topic_0225568815_p6084841"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p23110075"><a name="zh-cn_topic_0225568815_p23110075"></a><a name="zh-cn_topic_0225568815_p23110075"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p59976802"><a name="zh-cn_topic_0225568815_p59976802"></a><a name="zh-cn_topic_0225568815_p59976802"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p26282822"><a name="zh-cn_topic_0225568815_p26282822"></a><a name="zh-cn_topic_0225568815_p26282822"></a>版本</p>
<p id="zh-cn_topic_0225568815_p20178612194314"><a name="zh-cn_topic_0225568815_p20178612194314"></a><a name="zh-cn_topic_0225568815_p20178612194314"></a>字符长度不超过64</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row34151363"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p14797053"><a name="zh-cn_topic_0225568815_p14797053"></a><a name="zh-cn_topic_0225568815_p14797053"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p57710672"><a name="zh-cn_topic_0225568815_p57710672"></a><a name="zh-cn_topic_0225568815_p57710672"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p44052835"><a name="zh-cn_topic_0225568815_p44052835"></a><a name="zh-cn_topic_0225568815_p44052835"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p11509854"><a name="zh-cn_topic_0225568815_p11509854"></a><a name="zh-cn_topic_0225568815_p11509854"></a>描述信息</p>
<p id="zh-cn_topic_0225568815_p2075966"><a name="zh-cn_topic_0225568815_p2075966"></a><a name="zh-cn_topic_0225568815_p2075966"></a>长度不超过255个字符</p>
<div class="note" id="zh-cn_topic_0225568815_note988922210482"><a name="zh-cn_topic_0225568815_note988922210482"></a><a name="zh-cn_topic_0225568815_note988922210482"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p0889122164812"><a name="zh-cn_topic_0225568815_p0889122164812"></a><a name="zh-cn_topic_0225568815_p0889122164812"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

**表 7**  func\_info参数说明

<a name="zh-cn_topic_0225568815_table55289951"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row4334171"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p15523588"><a name="zh-cn_topic_0225568815_p15523588"></a><a name="zh-cn_topic_0225568815_p15523588"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p49451085"><a name="zh-cn_topic_0225568815_p49451085"></a><a name="zh-cn_topic_0225568815_p49451085"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p46114910"><a name="zh-cn_topic_0225568815_p46114910"></a><a name="zh-cn_topic_0225568815_p46114910"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p44320224"><a name="zh-cn_topic_0225568815_p44320224"></a><a name="zh-cn_topic_0225568815_p44320224"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row33168378"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p2284117"><a name="zh-cn_topic_0225568815_p2284117"></a><a name="zh-cn_topic_0225568815_p2284117"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p50795801"><a name="zh-cn_topic_0225568815_p50795801"></a><a name="zh-cn_topic_0225568815_p50795801"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p20819180"><a name="zh-cn_topic_0225568815_p20819180"></a><a name="zh-cn_topic_0225568815_p20819180"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p8632057"><a name="zh-cn_topic_0225568815_p8632057"></a><a name="zh-cn_topic_0225568815_p8632057"></a>函数URN</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row51645464"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p22533049"><a name="zh-cn_topic_0225568815_p22533049"></a><a name="zh-cn_topic_0225568815_p22533049"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p13237646"><a name="zh-cn_topic_0225568815_p13237646"></a><a name="zh-cn_topic_0225568815_p13237646"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p65616383"><a name="zh-cn_topic_0225568815_p65616383"></a><a name="zh-cn_topic_0225568815_p65616383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p13326838"><a name="zh-cn_topic_0225568815_p13326838"></a><a name="zh-cn_topic_0225568815_p13326838"></a>调用类型:async|sync （异步|同步）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row51588510"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p17919758"><a name="zh-cn_topic_0225568815_p17919758"></a><a name="zh-cn_topic_0225568815_p17919758"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p42214303"><a name="zh-cn_topic_0225568815_p42214303"></a><a name="zh-cn_topic_0225568815_p42214303"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p63915384"><a name="zh-cn_topic_0225568815_p63915384"></a><a name="zh-cn_topic_0225568815_p63915384"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1947019368454"><a name="zh-cn_topic_0225568815_p1947019368454"></a><a name="zh-cn_topic_0225568815_p1947019368454"></a>API网关请求后端服务的超时时间。超时时间最大值可以通过实例特性backend_timeout配置修改。</p>
<p id="zh-cn_topic_0225568815_p2047014366451"><a name="zh-cn_topic_0225568815_p2047014366451"></a><a name="zh-cn_topic_0225568815_p2047014366451"></a>单位：毫秒。</p>
<p id="zh-cn_topic_0225568815_p547019360454"><a name="zh-cn_topic_0225568815_p547019360454"></a><a name="zh-cn_topic_0225568815_p547019360454"></a>最小值：<strong id="zh-cn_topic_0225568815_b19470113615459"><a name="zh-cn_topic_0225568815_b19470113615459"></a><a name="zh-cn_topic_0225568815_b19470113615459"></a>1</strong></p>
<p id="zh-cn_topic_0225568815_p047043664513"><a name="zh-cn_topic_0225568815_p047043664513"></a><a name="zh-cn_topic_0225568815_p047043664513"></a>最大值：<strong id="zh-cn_topic_0225568815_b1247010369456"><a name="zh-cn_topic_0225568815_b1247010369456"></a><a name="zh-cn_topic_0225568815_b1247010369456"></a>600000</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row4161871"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1567241"><a name="zh-cn_topic_0225568815_p1567241"></a><a name="zh-cn_topic_0225568815_p1567241"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p59837679"><a name="zh-cn_topic_0225568815_p59837679"></a><a name="zh-cn_topic_0225568815_p59837679"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p15013867"><a name="zh-cn_topic_0225568815_p15013867"></a><a name="zh-cn_topic_0225568815_p15013867"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p8163682"><a name="zh-cn_topic_0225568815_p8163682"></a><a name="zh-cn_topic_0225568815_p8163682"></a>版本信息</p>
<p id="zh-cn_topic_0225568815_p11713102217438"><a name="zh-cn_topic_0225568815_p11713102217438"></a><a name="zh-cn_topic_0225568815_p11713102217438"></a>字符长度不超过64</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row45744694"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p14332708"><a name="zh-cn_topic_0225568815_p14332708"></a><a name="zh-cn_topic_0225568815_p14332708"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p20098666"><a name="zh-cn_topic_0225568815_p20098666"></a><a name="zh-cn_topic_0225568815_p20098666"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p17379249"><a name="zh-cn_topic_0225568815_p17379249"></a><a name="zh-cn_topic_0225568815_p17379249"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p65541920"><a name="zh-cn_topic_0225568815_p65541920"></a><a name="zh-cn_topic_0225568815_p65541920"></a>描述信息</p>
<p id="zh-cn_topic_0225568815_p65657958"><a name="zh-cn_topic_0225568815_p65657958"></a><a name="zh-cn_topic_0225568815_p65657958"></a>长度不超过255个字符</p>
<div class="note" id="zh-cn_topic_0225568815_note962555913483"><a name="zh-cn_topic_0225568815_note962555913483"></a><a name="zh-cn_topic_0225568815_note962555913483"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p96267594486"><a name="zh-cn_topic_0225568815_p96267594486"></a><a name="zh-cn_topic_0225568815_p96267594486"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

**表 8**  req\_params参数说明

<a name="zh-cn_topic_0225568815_table10797815193916"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row178141315123910"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p1981481518391"><a name="zh-cn_topic_0225568815_p1981481518391"></a><a name="zh-cn_topic_0225568815_p1981481518391"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p13828101511398"><a name="zh-cn_topic_0225568815_p13828101511398"></a><a name="zh-cn_topic_0225568815_p13828101511398"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p08281415143912"><a name="zh-cn_topic_0225568815_p08281415143912"></a><a name="zh-cn_topic_0225568815_p08281415143912"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p15828131523915"><a name="zh-cn_topic_0225568815_p15828131523915"></a><a name="zh-cn_topic_0225568815_p15828131523915"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row118441515123919"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p984461512398"><a name="zh-cn_topic_0225568815_p984461512398"></a><a name="zh-cn_topic_0225568815_p984461512398"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1184451593913"><a name="zh-cn_topic_0225568815_p1184451593913"></a><a name="zh-cn_topic_0225568815_p1184451593913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1184411517393"><a name="zh-cn_topic_0225568815_p1184411517393"></a><a name="zh-cn_topic_0225568815_p1184411517393"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p18861315153916"><a name="zh-cn_topic_0225568815_p18861315153916"></a><a name="zh-cn_topic_0225568815_p18861315153916"></a>参数名称</p>
<p id="zh-cn_topic_0225568815_p68611515103916"><a name="zh-cn_topic_0225568815_p68611515103916"></a><a name="zh-cn_topic_0225568815_p68611515103916"></a>长度为1 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”、“.”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row8861131510391"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p987641512396"><a name="zh-cn_topic_0225568815_p987641512396"></a><a name="zh-cn_topic_0225568815_p987641512396"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p48761915133913"><a name="zh-cn_topic_0225568815_p48761915133913"></a><a name="zh-cn_topic_0225568815_p48761915133913"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p178764154394"><a name="zh-cn_topic_0225568815_p178764154394"></a><a name="zh-cn_topic_0225568815_p178764154394"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p13891161513393"><a name="zh-cn_topic_0225568815_p13891161513393"></a><a name="zh-cn_topic_0225568815_p13891161513393"></a>参数类型：</p>
<a name="zh-cn_topic_0225568815_ul1830218285513"></a><a name="zh-cn_topic_0225568815_ul1830218285513"></a><ul id="zh-cn_topic_0225568815_ul1830218285513"><li>STRING</li><li>NUMBER</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row5891181553918"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p4891111513399"><a name="zh-cn_topic_0225568815_p4891111513399"></a><a name="zh-cn_topic_0225568815_p4891111513399"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p989171593919"><a name="zh-cn_topic_0225568815_p989171593919"></a><a name="zh-cn_topic_0225568815_p989171593919"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p29076155393"><a name="zh-cn_topic_0225568815_p29076155393"></a><a name="zh-cn_topic_0225568815_p29076155393"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1490710153393"><a name="zh-cn_topic_0225568815_p1490710153393"></a><a name="zh-cn_topic_0225568815_p1490710153393"></a>参数位置：</p>
<a name="zh-cn_topic_0225568815_ul1690715155390"></a><a name="zh-cn_topic_0225568815_ul1690715155390"></a><ul id="zh-cn_topic_0225568815_ul1690715155390"><li>PATH</li><li>QUERY</li><li>HEADER</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row159222154399"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p4922181511396"><a name="zh-cn_topic_0225568815_p4922181511396"></a><a name="zh-cn_topic_0225568815_p4922181511396"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p12939101543910"><a name="zh-cn_topic_0225568815_p12939101543910"></a><a name="zh-cn_topic_0225568815_p12939101543910"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p12939101513914"><a name="zh-cn_topic_0225568815_p12939101513914"></a><a name="zh-cn_topic_0225568815_p12939101513914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1795414270226"><a name="zh-cn_topic_0225568815_p1795414270226"></a><a name="zh-cn_topic_0225568815_p1795414270226"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row14091614391"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p301516133917"><a name="zh-cn_topic_0225568815_p301516133917"></a><a name="zh-cn_topic_0225568815_p301516133917"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p20116173911"><a name="zh-cn_topic_0225568815_p20116173911"></a><a name="zh-cn_topic_0225568815_p20116173911"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p19161116173915"><a name="zh-cn_topic_0225568815_p19161116173915"></a><a name="zh-cn_topic_0225568815_p19161116173915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p3265191616229"><a name="zh-cn_topic_0225568815_p3265191616229"></a><a name="zh-cn_topic_0225568815_p3265191616229"></a>参数示例值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1832121613917"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p113212160395"><a name="zh-cn_topic_0225568815_p113212160395"></a><a name="zh-cn_topic_0225568815_p113212160395"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p3471216103914"><a name="zh-cn_topic_0225568815_p3471216103914"></a><a name="zh-cn_topic_0225568815_p3471216103914"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p74716163396"><a name="zh-cn_topic_0225568815_p74716163396"></a><a name="zh-cn_topic_0225568815_p74716163396"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1126481992116"><a name="zh-cn_topic_0225568815_p1126481992116"></a><a name="zh-cn_topic_0225568815_p1126481992116"></a>是否必须：</p>
<a name="zh-cn_topic_0225568815_ul10215132733719"></a><a name="zh-cn_topic_0225568815_ul10215132733719"></a><ul id="zh-cn_topic_0225568815_ul10215132733719"><li>1：是</li><li>2：否</li></ul>
<p id="zh-cn_topic_0225568815_p15865181819372"><a name="zh-cn_topic_0225568815_p15865181819372"></a><a name="zh-cn_topic_0225568815_p15865181819372"></a>lacation为PATH时，required默认为1，其他场景required默认为2</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row36310168394"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1363181683919"><a name="zh-cn_topic_0225568815_p1363181683919"></a><a name="zh-cn_topic_0225568815_p1363181683919"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p167919163391"><a name="zh-cn_topic_0225568815_p167919163391"></a><a name="zh-cn_topic_0225568815_p167919163391"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p47961614392"><a name="zh-cn_topic_0225568815_p47961614392"></a><a name="zh-cn_topic_0225568815_p47961614392"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1779716173917"><a name="zh-cn_topic_0225568815_p1779716173917"></a><a name="zh-cn_topic_0225568815_p1779716173917"></a>是否开启校验：</p>
<a name="zh-cn_topic_0225568815_ul15491628153915"></a><a name="zh-cn_topic_0225568815_ul15491628153915"></a><ul id="zh-cn_topic_0225568815_ul15491628153915"><li>1：开启校验</li><li>2：不开启校验</li></ul>
<p id="zh-cn_topic_0225568815_p829542314397"><a name="zh-cn_topic_0225568815_p829542314397"></a><a name="zh-cn_topic_0225568815_p829542314397"></a>默认为2</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7942166394"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1894816193914"><a name="zh-cn_topic_0225568815_p1894816193914"></a><a name="zh-cn_topic_0225568815_p1894816193914"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p294171616395"><a name="zh-cn_topic_0225568815_p294171616395"></a><a name="zh-cn_topic_0225568815_p294171616395"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p8111916163917"><a name="zh-cn_topic_0225568815_p8111916163917"></a><a name="zh-cn_topic_0225568815_p8111916163917"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p189891816181817"><a name="zh-cn_topic_0225568815_p189891816181817"></a><a name="zh-cn_topic_0225568815_p189891816181817"></a>描述</p>
<p id="zh-cn_topic_0225568815_p139892166189"><a name="zh-cn_topic_0225568815_p139892166189"></a><a name="zh-cn_topic_0225568815_p139892166189"></a>字符长度不超过255</p>
<div class="note" id="zh-cn_topic_0225568815_note135191711818"><a name="zh-cn_topic_0225568815_note135191711818"></a><a name="zh-cn_topic_0225568815_note135191711818"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p105317181816"><a name="zh-cn_topic_0225568815_p105317181816"></a><a name="zh-cn_topic_0225568815_p105317181816"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row13126201633917"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1314181643914"><a name="zh-cn_topic_0225568815_p1314181643914"></a><a name="zh-cn_topic_0225568815_p1314181643914"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p814191615397"><a name="zh-cn_topic_0225568815_p814191615397"></a><a name="zh-cn_topic_0225568815_p814191615397"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p71411168392"><a name="zh-cn_topic_0225568815_p71411168392"></a><a name="zh-cn_topic_0225568815_p71411168392"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p141581516113916"><a name="zh-cn_topic_0225568815_p141581516113916"></a><a name="zh-cn_topic_0225568815_p141581516113916"></a>参数枚举值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row878217618128"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1778211616128"><a name="zh-cn_topic_0225568815_p1778211616128"></a><a name="zh-cn_topic_0225568815_p1778211616128"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p10782563129"><a name="zh-cn_topic_0225568815_p10782563129"></a><a name="zh-cn_topic_0225568815_p10782563129"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p178213613128"><a name="zh-cn_topic_0225568815_p178213613128"></a><a name="zh-cn_topic_0225568815_p178213613128"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p11708175481613"><a name="zh-cn_topic_0225568815_p11708175481613"></a><a name="zh-cn_topic_0225568815_p11708175481613"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1242311108123"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p154235102129"><a name="zh-cn_topic_0225568815_p154235102129"></a><a name="zh-cn_topic_0225568815_p154235102129"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p3423141081212"><a name="zh-cn_topic_0225568815_p3423141081212"></a><a name="zh-cn_topic_0225568815_p3423141081212"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1442316104122"><a name="zh-cn_topic_0225568815_p1442316104122"></a><a name="zh-cn_topic_0225568815_p1442316104122"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p542391091215"><a name="zh-cn_topic_0225568815_p542391091215"></a><a name="zh-cn_topic_0225568815_p542391091215"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row21901721131212"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p9190321131218"><a name="zh-cn_topic_0225568815_p9190321131218"></a><a name="zh-cn_topic_0225568815_p9190321131218"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p7190162117128"><a name="zh-cn_topic_0225568815_p7190162117128"></a><a name="zh-cn_topic_0225568815_p7190162117128"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1619082112121"><a name="zh-cn_topic_0225568815_p1619082112121"></a><a name="zh-cn_topic_0225568815_p1619082112121"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p719062181213"><a name="zh-cn_topic_0225568815_p719062181213"></a><a name="zh-cn_topic_0225568815_p719062181213"></a>参数最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row192351217191211"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p182351717171210"><a name="zh-cn_topic_0225568815_p182351717171210"></a><a name="zh-cn_topic_0225568815_p182351717171210"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p11235151717124"><a name="zh-cn_topic_0225568815_p11235151717124"></a><a name="zh-cn_topic_0225568815_p11235151717124"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p20235181721217"><a name="zh-cn_topic_0225568815_p20235181721217"></a><a name="zh-cn_topic_0225568815_p20235181721217"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p122359172126"><a name="zh-cn_topic_0225568815_p122359172126"></a><a name="zh-cn_topic_0225568815_p122359172126"></a>参数最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row222041311121"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p10220131331219"><a name="zh-cn_topic_0225568815_p10220131331219"></a><a name="zh-cn_topic_0225568815_p10220131331219"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1220131331211"><a name="zh-cn_topic_0225568815_p1220131331211"></a><a name="zh-cn_topic_0225568815_p1220131331211"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1122017131128"><a name="zh-cn_topic_0225568815_p1122017131128"></a><a name="zh-cn_topic_0225568815_p1122017131128"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1722001319126"><a name="zh-cn_topic_0225568815_p1722001319126"></a><a name="zh-cn_topic_0225568815_p1722001319126"></a>正则校验规则（暂不支持）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row177506146139"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p197501614181317"><a name="zh-cn_topic_0225568815_p197501614181317"></a><a name="zh-cn_topic_0225568815_p197501614181317"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1975091410132"><a name="zh-cn_topic_0225568815_p1975091410132"></a><a name="zh-cn_topic_0225568815_p1975091410132"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1275091417134"><a name="zh-cn_topic_0225568815_p1275091417134"></a><a name="zh-cn_topic_0225568815_p1275091417134"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p07501140138"><a name="zh-cn_topic_0225568815_p07501140138"></a><a name="zh-cn_topic_0225568815_p07501140138"></a>JSON校验规则（暂不支持）</p>
</td>
</tr>
</tbody>
</table>

**表 9**  backend\_params参数说明

<a name="zh-cn_topic_0225568815_table599625352311"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row161185472312"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p2271054112313"><a name="zh-cn_topic_0225568815_p2271054112313"></a><a name="zh-cn_topic_0225568815_p2271054112313"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p0271154112315"><a name="zh-cn_topic_0225568815_p0271154112315"></a><a name="zh-cn_topic_0225568815_p0271154112315"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p11431854112316"><a name="zh-cn_topic_0225568815_p11431854112316"></a><a name="zh-cn_topic_0225568815_p11431854112316"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p1543354162315"><a name="zh-cn_topic_0225568815_p1543354162315"></a><a name="zh-cn_topic_0225568815_p1543354162315"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row543125416231"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p195875452310"><a name="zh-cn_topic_0225568815_p195875452310"></a><a name="zh-cn_topic_0225568815_p195875452310"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p7581354112312"><a name="zh-cn_topic_0225568815_p7581354112312"></a><a name="zh-cn_topic_0225568815_p7581354112312"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p458154112315"><a name="zh-cn_topic_0225568815_p458154112315"></a><a name="zh-cn_topic_0225568815_p458154112315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1775554132310"><a name="zh-cn_topic_0225568815_p1775554132310"></a><a name="zh-cn_topic_0225568815_p1775554132310"></a>参数名称</p>
<p id="zh-cn_topic_0225568815_p67518541235"><a name="zh-cn_topic_0225568815_p67518541235"></a><a name="zh-cn_topic_0225568815_p67518541235"></a>长度为1 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”、“.”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row191211554142315"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p17121854112318"><a name="zh-cn_topic_0225568815_p17121854112318"></a><a name="zh-cn_topic_0225568815_p17121854112318"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p412115419233"><a name="zh-cn_topic_0225568815_p412115419233"></a><a name="zh-cn_topic_0225568815_p412115419233"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1213720544234"><a name="zh-cn_topic_0225568815_p1213720544234"></a><a name="zh-cn_topic_0225568815_p1213720544234"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p91371054102314"><a name="zh-cn_topic_0225568815_p91371054102314"></a><a name="zh-cn_topic_0225568815_p91371054102314"></a>参数位置：</p>
<a name="zh-cn_topic_0225568815_ul19137754162316"></a><a name="zh-cn_topic_0225568815_ul19137754162316"></a><ul id="zh-cn_topic_0225568815_ul19137754162316"><li>PATH</li><li>QUERY</li><li>HEADER</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row15230654192316"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p12230205492317"><a name="zh-cn_topic_0225568815_p12230205492317"></a><a name="zh-cn_topic_0225568815_p12230205492317"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p10230145415237"><a name="zh-cn_topic_0225568815_p10230145415237"></a><a name="zh-cn_topic_0225568815_p10230145415237"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p724735411231"><a name="zh-cn_topic_0225568815_p724735411231"></a><a name="zh-cn_topic_0225568815_p724735411231"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1524775413233"><a name="zh-cn_topic_0225568815_p1524775413233"></a><a name="zh-cn_topic_0225568815_p1524775413233"></a>参数类别：</p>
<a name="zh-cn_topic_0225568815_ul1124735482312"></a><a name="zh-cn_topic_0225568815_ul1124735482312"></a><ul id="zh-cn_topic_0225568815_ul1124735482312"><li>REQUEST</li><li>CONSTANT</li><li>SYSTEM</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row15261254202320"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p9261954122310"><a name="zh-cn_topic_0225568815_p9261954122310"></a><a name="zh-cn_topic_0225568815_p9261954122310"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1427715452315"><a name="zh-cn_topic_0225568815_p1427715452315"></a><a name="zh-cn_topic_0225568815_p1427715452315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p17277155419233"><a name="zh-cn_topic_0225568815_p17277155419233"></a><a name="zh-cn_topic_0225568815_p17277155419233"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p657172452818"><a name="zh-cn_topic_0225568815_p657172452818"></a><a name="zh-cn_topic_0225568815_p657172452818"></a>参数值</p>
<p id="zh-cn_topic_0225568815_p110811324312"><a name="zh-cn_topic_0225568815_p110811324312"></a><a name="zh-cn_topic_0225568815_p110811324312"></a>字符长度不超过255</p>
<p id="zh-cn_topic_0225568815_p13947355152811"><a name="zh-cn_topic_0225568815_p13947355152811"></a><a name="zh-cn_topic_0225568815_p13947355152811"></a>类别为REQUEST时，值为req_params中的参数名称；</p>
<p id="zh-cn_topic_0225568815_p365913371295"><a name="zh-cn_topic_0225568815_p365913371295"></a><a name="zh-cn_topic_0225568815_p365913371295"></a>类别为CONSTANT时，值为参数真正的值；</p>
<p id="zh-cn_topic_0225568815_p25181013162915"><a name="zh-cn_topic_0225568815_p25181013162915"></a><a name="zh-cn_topic_0225568815_p25181013162915"></a>类别为SYSTEM时，值为网关参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1229318545230"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p53088549232"><a name="zh-cn_topic_0225568815_p53088549232"></a><a name="zh-cn_topic_0225568815_p53088549232"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p193081654182316"><a name="zh-cn_topic_0225568815_p193081654182316"></a><a name="zh-cn_topic_0225568815_p193081654182316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p8324354112310"><a name="zh-cn_topic_0225568815_p8324354112310"></a><a name="zh-cn_topic_0225568815_p8324354112310"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p183241554122314"><a name="zh-cn_topic_0225568815_p183241554122314"></a><a name="zh-cn_topic_0225568815_p183241554122314"></a>描述</p>
<p id="zh-cn_topic_0225568815_p2324125492316"><a name="zh-cn_topic_0225568815_p2324125492316"></a><a name="zh-cn_topic_0225568815_p2324125492316"></a>字符长度不超过255</p>
<div class="note" id="zh-cn_topic_0225568815_note8324854142312"><a name="zh-cn_topic_0225568815_note8324854142312"></a><a name="zh-cn_topic_0225568815_note8324854142312"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p3340125492316"><a name="zh-cn_topic_0225568815_p3340125492316"></a><a name="zh-cn_topic_0225568815_p3340125492316"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
</tbody>
</table>

**表 10**  policy\_https参数说明

<a name="zh-cn_topic_0225568815_table128141157246"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row7853115102415"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p0860105122414"><a name="zh-cn_topic_0225568815_p0860105122414"></a><a name="zh-cn_topic_0225568815_p0860105122414"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p1787285102417"><a name="zh-cn_topic_0225568815_p1787285102417"></a><a name="zh-cn_topic_0225568815_p1787285102417"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p9882957248"><a name="zh-cn_topic_0225568815_p9882957248"></a><a name="zh-cn_topic_0225568815_p9882957248"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p1989775112418"><a name="zh-cn_topic_0225568815_p1989775112418"></a><a name="zh-cn_topic_0225568815_p1989775112418"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row7914105182411"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p10478449260"><a name="zh-cn_topic_0225568815_p10478449260"></a><a name="zh-cn_topic_0225568815_p10478449260"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p747718413263"><a name="zh-cn_topic_0225568815_p747718413263"></a><a name="zh-cn_topic_0225568815_p747718413263"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p347620492615"><a name="zh-cn_topic_0225568815_p347620492615"></a><a name="zh-cn_topic_0225568815_p347620492615"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p10470144172613"><a name="zh-cn_topic_0225568815_p10470144172613"></a><a name="zh-cn_topic_0225568815_p10470144172613"></a>策略后端名称</p>
<p id="zh-cn_topic_0225568815_p199009132715"><a name="zh-cn_topic_0225568815_p199009132715"></a><a name="zh-cn_topic_0225568815_p199009132715"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以中文或英文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row14281461249"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p697505202410"><a name="zh-cn_topic_0225568815_p697505202410"></a><a name="zh-cn_topic_0225568815_p697505202410"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p598445112418"><a name="zh-cn_topic_0225568815_p598445112418"></a><a name="zh-cn_topic_0225568815_p598445112418"></a>后端服务不使用VPC通道时，必选</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p9993135202417"><a name="zh-cn_topic_0225568815_p9993135202417"></a><a name="zh-cn_topic_0225568815_p9993135202417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p14212632420"><a name="zh-cn_topic_0225568815_p14212632420"></a><a name="zh-cn_topic_0225568815_p14212632420"></a>策略后端的Endpoint。</p>
<p id="zh-cn_topic_0225568815_p014176182414"><a name="zh-cn_topic_0225568815_p014176182414"></a><a name="zh-cn_topic_0225568815_p014176182414"></a>由域名（或IP地址）和端口号组成，总长度不超过255。格式为域名:端口（如：apig.example.com:7443）。如果不写端口，则HTTPS默认端口号为443， HTTP默认端口号为80。</p>
<p id="zh-cn_topic_0225568815_p1520126142411"><a name="zh-cn_topic_0225568815_p1520126142411"></a><a name="zh-cn_topic_0225568815_p1520126142411"></a>支持环境变量，使用环境变量时，每个变量名的长度为3 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”组成，且只能以英文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row5823632418"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p79317692416"><a name="zh-cn_topic_0225568815_p79317692416"></a><a name="zh-cn_topic_0225568815_p79317692416"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1103068242"><a name="zh-cn_topic_0225568815_p1103068242"></a><a name="zh-cn_topic_0225568815_p1103068242"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p111510613243"><a name="zh-cn_topic_0225568815_p111510613243"></a><a name="zh-cn_topic_0225568815_p111510613243"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1512566142412"><a name="zh-cn_topic_0225568815_p1512566142412"></a><a name="zh-cn_topic_0225568815_p1512566142412"></a>请求协议：</p>
<a name="zh-cn_topic_0225568815_ul161311652420"></a><a name="zh-cn_topic_0225568815_ul161311652420"></a><ul id="zh-cn_topic_0225568815_ul161311652420"><li>HTTP</li><li>HTTPS</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1016019692418"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p8172156112420"><a name="zh-cn_topic_0225568815_p8172156112420"></a><a name="zh-cn_topic_0225568815_p8172156112420"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p71841614242"><a name="zh-cn_topic_0225568815_p71841614242"></a><a name="zh-cn_topic_0225568815_p71841614242"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1719611612247"><a name="zh-cn_topic_0225568815_p1719611612247"></a><a name="zh-cn_topic_0225568815_p1719611612247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p62054662411"><a name="zh-cn_topic_0225568815_p62054662411"></a><a name="zh-cn_topic_0225568815_p62054662411"></a>请求方式：</p>
<a name="zh-cn_topic_0225568815_ul220886152414"></a><a name="zh-cn_topic_0225568815_ul220886152414"></a><ul id="zh-cn_topic_0225568815_ul220886152414"><li>GET</li><li>POST</li><li>PUT</li><li>DELETE</li><li>HEAD</li><li>PATCH</li><li>OPTIONS</li><li>ANY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row330017619241"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p131306142416"><a name="zh-cn_topic_0225568815_p131306142416"></a><a name="zh-cn_topic_0225568815_p131306142416"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1932617672420"><a name="zh-cn_topic_0225568815_p1932617672420"></a><a name="zh-cn_topic_0225568815_p1932617672420"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1339963245"><a name="zh-cn_topic_0225568815_p1339963245"></a><a name="zh-cn_topic_0225568815_p1339963245"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p153495610242"><a name="zh-cn_topic_0225568815_p153495610242"></a><a name="zh-cn_topic_0225568815_p153495610242"></a>请求地址</p>
<p id="zh-cn_topic_0225568815_p43543618243"><a name="zh-cn_topic_0225568815_p43543618243"></a><a name="zh-cn_topic_0225568815_p43543618243"></a>总长度不超过512，且满足URI规范。</p>
<p id="zh-cn_topic_0225568815_p3361166248"><a name="zh-cn_topic_0225568815_p3361166248"></a><a name="zh-cn_topic_0225568815_p3361166248"></a>支持环境变量，使用环境变量时，每个变量名的长度为3 ~ 32位的字符串，字符串由英文字母、数字、“_”、“-”组成，且只能以英文开头。</p>
<div class="note" id="zh-cn_topic_0225568815_note12366163242"><a name="zh-cn_topic_0225568815_note12366163242"></a><a name="zh-cn_topic_0225568815_note12366163242"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568815_p19372176192416"><a name="zh-cn_topic_0225568815_p19372176192416"></a><a name="zh-cn_topic_0225568815_p19372176192416"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row12380163246"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p14390146162418"><a name="zh-cn_topic_0225568815_p14390146162418"></a><a name="zh-cn_topic_0225568815_p14390146162418"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1840117632412"><a name="zh-cn_topic_0225568815_p1840117632412"></a><a name="zh-cn_topic_0225568815_p1840117632412"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1141212642410"><a name="zh-cn_topic_0225568815_p1141212642410"></a><a name="zh-cn_topic_0225568815_p1141212642410"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p5223165234520"><a name="zh-cn_topic_0225568815_p5223165234520"></a><a name="zh-cn_topic_0225568815_p5223165234520"></a>API网关请求后端服务的超时时间。超时时间最大值可以通过实例特性backend_timeout配置修改。</p>
<p id="zh-cn_topic_0225568815_p0223052144512"><a name="zh-cn_topic_0225568815_p0223052144512"></a><a name="zh-cn_topic_0225568815_p0223052144512"></a>单位：毫秒。</p>
<p id="zh-cn_topic_0225568815_p222316520459"><a name="zh-cn_topic_0225568815_p222316520459"></a><a name="zh-cn_topic_0225568815_p222316520459"></a>最小值：<strong id="zh-cn_topic_0225568815_b132231522457"><a name="zh-cn_topic_0225568815_b132231522457"></a><a name="zh-cn_topic_0225568815_b132231522457"></a>1</strong></p>
<p id="zh-cn_topic_0225568815_p17223125284518"><a name="zh-cn_topic_0225568815_p17223125284518"></a><a name="zh-cn_topic_0225568815_p17223125284518"></a>最大值：<strong id="zh-cn_topic_0225568815_b1322385214457"><a name="zh-cn_topic_0225568815_b1322385214457"></a><a name="zh-cn_topic_0225568815_b1322385214457"></a>600000</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row155036619245"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p15131861247"><a name="zh-cn_topic_0225568815_p15131861247"></a><a name="zh-cn_topic_0225568815_p15131861247"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p852417672417"><a name="zh-cn_topic_0225568815_p852417672417"></a><a name="zh-cn_topic_0225568815_p852417672417"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p19539761241"><a name="zh-cn_topic_0225568815_p19539761241"></a><a name="zh-cn_topic_0225568815_p19539761241"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p75511166248"><a name="zh-cn_topic_0225568815_p75511166248"></a><a name="zh-cn_topic_0225568815_p75511166248"></a>是否使用VPC通道：</p>
<a name="zh-cn_topic_0225568815_ul9559969246"></a><a name="zh-cn_topic_0225568815_ul9559969246"></a><ul id="zh-cn_topic_0225568815_ul9559969246"><li>1 : 使用VPC通道</li><li>2 : 不使用VPC通道</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7591566249"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p860218612246"><a name="zh-cn_topic_0225568815_p860218612246"></a><a name="zh-cn_topic_0225568815_p860218612246"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p9617762245"><a name="zh-cn_topic_0225568815_p9617762245"></a><a name="zh-cn_topic_0225568815_p9617762245"></a>如果vpc_status=1，则这个字典类型为必填信息</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p36315618240"><a name="zh-cn_topic_0225568815_p36315618240"></a><a name="zh-cn_topic_0225568815_p36315618240"></a>字典类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p56441964245"><a name="zh-cn_topic_0225568815_p56441964245"></a><a name="zh-cn_topic_0225568815_p56441964245"></a>VPC通道详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1642019191295"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p2042071916296"><a name="zh-cn_topic_0225568815_p2042071916296"></a><a name="zh-cn_topic_0225568815_p2042071916296"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1442051942914"><a name="zh-cn_topic_0225568815_p1442051942914"></a><a name="zh-cn_topic_0225568815_p1442051942914"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p3420219162915"><a name="zh-cn_topic_0225568815_p3420219162915"></a><a name="zh-cn_topic_0225568815_p3420219162915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p17355191291320"><a name="zh-cn_topic_0225568815_p17355191291320"></a><a name="zh-cn_topic_0225568815_p17355191291320"></a>关联的策略组合模式</p>
<a name="zh-cn_topic_0225568815_ul103629128139"></a><a name="zh-cn_topic_0225568815_ul103629128139"></a><ul id="zh-cn_topic_0225568815_ul103629128139"><li>ALL</li><li>ANY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1811315118316"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p911413514319"><a name="zh-cn_topic_0225568815_p911413514319"></a><a name="zh-cn_topic_0225568815_p911413514319"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p1711485119318"><a name="zh-cn_topic_0225568815_p1711485119318"></a><a name="zh-cn_topic_0225568815_p1711485119318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p20114751123114"><a name="zh-cn_topic_0225568815_p20114751123114"></a><a name="zh-cn_topic_0225568815_p20114751123114"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p12114175115316"><a name="zh-cn_topic_0225568815_p12114175115316"></a><a name="zh-cn_topic_0225568815_p12114175115316"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1767914813115"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p9680448123119"><a name="zh-cn_topic_0225568815_p9680448123119"></a><a name="zh-cn_topic_0225568815_p9680448123119"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p2068054823119"><a name="zh-cn_topic_0225568815_p2068054823119"></a><a name="zh-cn_topic_0225568815_p2068054823119"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p13680194815319"><a name="zh-cn_topic_0225568815_p13680194815319"></a><a name="zh-cn_topic_0225568815_p13680194815319"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p36804486317"><a name="zh-cn_topic_0225568815_p36804486317"></a><a name="zh-cn_topic_0225568815_p36804486317"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 11**  policy\_mocks参数说明

<a name="zh-cn_topic_0225568815_table10870665248"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row9908116122412"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p199181613249"><a name="zh-cn_topic_0225568815_p199181613249"></a><a name="zh-cn_topic_0225568815_p199181613249"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p69300619240"><a name="zh-cn_topic_0225568815_p69300619240"></a><a name="zh-cn_topic_0225568815_p69300619240"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p394146172415"><a name="zh-cn_topic_0225568815_p394146172415"></a><a name="zh-cn_topic_0225568815_p394146172415"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p189551652411"><a name="zh-cn_topic_0225568815_p189551652411"></a><a name="zh-cn_topic_0225568815_p189551652411"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row114683612356"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p18922745143519"><a name="zh-cn_topic_0225568815_p18922745143519"></a><a name="zh-cn_topic_0225568815_p18922745143519"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p18942545113512"><a name="zh-cn_topic_0225568815_p18942545113512"></a><a name="zh-cn_topic_0225568815_p18942545113512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1295904533517"><a name="zh-cn_topic_0225568815_p1295904533517"></a><a name="zh-cn_topic_0225568815_p1295904533517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p897264510353"><a name="zh-cn_topic_0225568815_p897264510353"></a><a name="zh-cn_topic_0225568815_p897264510353"></a>策略后端名称</p>
<p id="zh-cn_topic_0225568815_p1098024533514"><a name="zh-cn_topic_0225568815_p1098024533514"></a><a name="zh-cn_topic_0225568815_p1098024533514"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以中文或英文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row196936202419"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p13980368245"><a name="zh-cn_topic_0225568815_p13980368245"></a><a name="zh-cn_topic_0225568815_p13980368245"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p179923602415"><a name="zh-cn_topic_0225568815_p179923602415"></a><a name="zh-cn_topic_0225568815_p179923602415"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p4618710246"><a name="zh-cn_topic_0225568815_p4618710246"></a><a name="zh-cn_topic_0225568815_p4618710246"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1617475244"><a name="zh-cn_topic_0225568815_p1617475244"></a><a name="zh-cn_topic_0225568815_p1617475244"></a>返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row12337122416"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1190123283614"><a name="zh-cn_topic_0225568815_p1190123283614"></a><a name="zh-cn_topic_0225568815_p1190123283614"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p19205153233617"><a name="zh-cn_topic_0225568815_p19205153233617"></a><a name="zh-cn_topic_0225568815_p19205153233617"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p162231432153614"><a name="zh-cn_topic_0225568815_p162231432153614"></a><a name="zh-cn_topic_0225568815_p162231432153614"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p162351332143612"><a name="zh-cn_topic_0225568815_p162351332143612"></a><a name="zh-cn_topic_0225568815_p162351332143612"></a>关联的策略组合模式</p>
<a name="zh-cn_topic_0225568815_ul1123923212360"></a><a name="zh-cn_topic_0225568815_ul1123923212360"></a><ul id="zh-cn_topic_0225568815_ul1123923212360"><li>ALL</li><li>ANY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row12821371241"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1429733216361"><a name="zh-cn_topic_0225568815_p1429733216361"></a><a name="zh-cn_topic_0225568815_p1429733216361"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p6316193223610"><a name="zh-cn_topic_0225568815_p6316193223610"></a><a name="zh-cn_topic_0225568815_p6316193223610"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1433273233616"><a name="zh-cn_topic_0225568815_p1433273233616"></a><a name="zh-cn_topic_0225568815_p1433273233616"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p20350163210363"><a name="zh-cn_topic_0225568815_p20350163210363"></a><a name="zh-cn_topic_0225568815_p20350163210363"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7275192383618"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p10380113214362"><a name="zh-cn_topic_0225568815_p10380113214362"></a><a name="zh-cn_topic_0225568815_p10380113214362"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p10397632143612"><a name="zh-cn_topic_0225568815_p10397632143612"></a><a name="zh-cn_topic_0225568815_p10397632143612"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p44141932173617"><a name="zh-cn_topic_0225568815_p44141932173617"></a><a name="zh-cn_topic_0225568815_p44141932173617"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p11431332143615"><a name="zh-cn_topic_0225568815_p11431332143615"></a><a name="zh-cn_topic_0225568815_p11431332143615"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 12**  policy\_functions参数说明

<a name="zh-cn_topic_0225568815_table1614912782413"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row518437192416"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p419537142413"><a name="zh-cn_topic_0225568815_p419537142413"></a><a name="zh-cn_topic_0225568815_p419537142413"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p192071677243"><a name="zh-cn_topic_0225568815_p192071677243"></a><a name="zh-cn_topic_0225568815_p192071677243"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p1522016720240"><a name="zh-cn_topic_0225568815_p1522016720240"></a><a name="zh-cn_topic_0225568815_p1522016720240"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p2023411718245"><a name="zh-cn_topic_0225568815_p2023411718245"></a><a name="zh-cn_topic_0225568815_p2023411718245"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row8404750103511"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p366915119359"><a name="zh-cn_topic_0225568815_p366915119359"></a><a name="zh-cn_topic_0225568815_p366915119359"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p568725118355"><a name="zh-cn_topic_0225568815_p568725118355"></a><a name="zh-cn_topic_0225568815_p568725118355"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p570315153515"><a name="zh-cn_topic_0225568815_p570315153515"></a><a name="zh-cn_topic_0225568815_p570315153515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1671655113352"><a name="zh-cn_topic_0225568815_p1671655113352"></a><a name="zh-cn_topic_0225568815_p1671655113352"></a>策略后端名称</p>
<p id="zh-cn_topic_0225568815_p1872635115353"><a name="zh-cn_topic_0225568815_p1872635115353"></a><a name="zh-cn_topic_0225568815_p1872635115353"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“_”组成，且只能以中文或英文开头。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1724710718245"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p182590718246"><a name="zh-cn_topic_0225568815_p182590718246"></a><a name="zh-cn_topic_0225568815_p182590718246"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p527310722416"><a name="zh-cn_topic_0225568815_p527310722416"></a><a name="zh-cn_topic_0225568815_p527310722416"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1928810715249"><a name="zh-cn_topic_0225568815_p1928810715249"></a><a name="zh-cn_topic_0225568815_p1928810715249"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1230217722411"><a name="zh-cn_topic_0225568815_p1230217722411"></a><a name="zh-cn_topic_0225568815_p1230217722411"></a>函数URN</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row73102742417"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p432318782417"><a name="zh-cn_topic_0225568815_p432318782417"></a><a name="zh-cn_topic_0225568815_p432318782417"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p7333779243"><a name="zh-cn_topic_0225568815_p7333779243"></a><a name="zh-cn_topic_0225568815_p7333779243"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p133431970246"><a name="zh-cn_topic_0225568815_p133431970246"></a><a name="zh-cn_topic_0225568815_p133431970246"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p33571571249"><a name="zh-cn_topic_0225568815_p33571571249"></a><a name="zh-cn_topic_0225568815_p33571571249"></a>调用类型:async|sync （异步|同步）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row103624772410"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1337397192420"><a name="zh-cn_topic_0225568815_p1337397192420"></a><a name="zh-cn_topic_0225568815_p1337397192420"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p143864712245"><a name="zh-cn_topic_0225568815_p143864712245"></a><a name="zh-cn_topic_0225568815_p143864712245"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p23950772412"><a name="zh-cn_topic_0225568815_p23950772412"></a><a name="zh-cn_topic_0225568815_p23950772412"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p19458115204615"><a name="zh-cn_topic_0225568815_p19458115204615"></a><a name="zh-cn_topic_0225568815_p19458115204615"></a>API网关请求后端服务的超时时间。超时时间最大值可以通过实例特性backend_timeout配置修改。</p>
<p id="zh-cn_topic_0225568815_p345812519467"><a name="zh-cn_topic_0225568815_p345812519467"></a><a name="zh-cn_topic_0225568815_p345812519467"></a>单位：毫秒。</p>
<p id="zh-cn_topic_0225568815_p84581754469"><a name="zh-cn_topic_0225568815_p84581754469"></a><a name="zh-cn_topic_0225568815_p84581754469"></a>最小值：<strong id="zh-cn_topic_0225568815_b184581452463"><a name="zh-cn_topic_0225568815_b184581452463"></a><a name="zh-cn_topic_0225568815_b184581452463"></a>1</strong></p>
<p id="zh-cn_topic_0225568815_p2458175114612"><a name="zh-cn_topic_0225568815_p2458175114612"></a><a name="zh-cn_topic_0225568815_p2458175114612"></a>最大值：<strong id="zh-cn_topic_0225568815_b1445835154618"><a name="zh-cn_topic_0225568815_b1445835154618"></a><a name="zh-cn_topic_0225568815_b1445835154618"></a>600000</strong></p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row44231071243"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p2043620717240"><a name="zh-cn_topic_0225568815_p2043620717240"></a><a name="zh-cn_topic_0225568815_p2043620717240"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p194519711241"><a name="zh-cn_topic_0225568815_p194519711241"></a><a name="zh-cn_topic_0225568815_p194519711241"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p14467197182411"><a name="zh-cn_topic_0225568815_p14467197182411"></a><a name="zh-cn_topic_0225568815_p14467197182411"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p20477157172413"><a name="zh-cn_topic_0225568815_p20477157172413"></a><a name="zh-cn_topic_0225568815_p20477157172413"></a>版本信息</p>
<p id="zh-cn_topic_0225568815_p31781824111416"><a name="zh-cn_topic_0225568815_p31781824111416"></a><a name="zh-cn_topic_0225568815_p31781824111416"></a>字符长度不超过64</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row9483476245"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p12707174493712"><a name="zh-cn_topic_0225568815_p12707174493712"></a><a name="zh-cn_topic_0225568815_p12707174493712"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p27251744103712"><a name="zh-cn_topic_0225568815_p27251744103712"></a><a name="zh-cn_topic_0225568815_p27251744103712"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p774113445374"><a name="zh-cn_topic_0225568815_p774113445374"></a><a name="zh-cn_topic_0225568815_p774113445374"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p976120448376"><a name="zh-cn_topic_0225568815_p976120448376"></a><a name="zh-cn_topic_0225568815_p976120448376"></a>关联的策略组合模式</p>
<a name="zh-cn_topic_0225568815_ul677474423716"></a><a name="zh-cn_topic_0225568815_ul677474423716"></a><ul id="zh-cn_topic_0225568815_ul677474423716"><li>ALL</li><li>ANY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1558153418371"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p10908544163715"><a name="zh-cn_topic_0225568815_p10908544163715"></a><a name="zh-cn_topic_0225568815_p10908544163715"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p19927174493713"><a name="zh-cn_topic_0225568815_p19927174493713"></a><a name="zh-cn_topic_0225568815_p19927174493713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p4941144143715"><a name="zh-cn_topic_0225568815_p4941144143715"></a><a name="zh-cn_topic_0225568815_p4941144143715"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p119628445376"><a name="zh-cn_topic_0225568815_p119628445376"></a><a name="zh-cn_topic_0225568815_p119628445376"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row4369931193716"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1899434473711"><a name="zh-cn_topic_0225568815_p1899434473711"></a><a name="zh-cn_topic_0225568815_p1899434473711"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p14911456372"><a name="zh-cn_topic_0225568815_p14911456372"></a><a name="zh-cn_topic_0225568815_p14911456372"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p424114516376"><a name="zh-cn_topic_0225568815_p424114516376"></a><a name="zh-cn_topic_0225568815_p424114516376"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p943184512374"><a name="zh-cn_topic_0225568815_p943184512374"></a><a name="zh-cn_topic_0225568815_p943184512374"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 13**  conditions参数说明

<a name="zh-cn_topic_0225568815_table375918219381"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row7823152143818"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p984312113812"><a name="zh-cn_topic_0225568815_p984312113812"></a><a name="zh-cn_topic_0225568815_p984312113812"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p88624213816"><a name="zh-cn_topic_0225568815_p88624213816"></a><a name="zh-cn_topic_0225568815_p88624213816"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p15882825385"><a name="zh-cn_topic_0225568815_p15882825385"></a><a name="zh-cn_topic_0225568815_p15882825385"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p290117218389"><a name="zh-cn_topic_0225568815_p290117218389"></a><a name="zh-cn_topic_0225568815_p290117218389"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row129131023381"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p2073965518514"><a name="zh-cn_topic_0225568815_p2073965518514"></a><a name="zh-cn_topic_0225568815_p2073965518514"></a>condition_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p175055515512"><a name="zh-cn_topic_0225568815_p175055515512"></a><a name="zh-cn_topic_0225568815_p175055515512"></a>策略类型为param时必选</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p243532112397"><a name="zh-cn_topic_0225568815_p243532112397"></a><a name="zh-cn_topic_0225568815_p243532112397"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p191180178399"><a name="zh-cn_topic_0225568815_p191180178399"></a><a name="zh-cn_topic_0225568815_p191180178399"></a>策略条件：</p>
<a name="zh-cn_topic_0225568815_ul412517178394"></a><a name="zh-cn_topic_0225568815_ul412517178394"></a><ul id="zh-cn_topic_0225568815_ul412517178394"><li>exact：绝对匹配</li><li>enum：枚举</li><li>pattern：正则</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row189876263818"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1580917551453"><a name="zh-cn_topic_0225568815_p1580917551453"></a><a name="zh-cn_topic_0225568815_p1580917551453"></a>condition_value</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p981713551513"><a name="zh-cn_topic_0225568815_p981713551513"></a><a name="zh-cn_topic_0225568815_p981713551513"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p646310215396"><a name="zh-cn_topic_0225568815_p646310215396"></a><a name="zh-cn_topic_0225568815_p646310215396"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p21921617113910"><a name="zh-cn_topic_0225568815_p21921617113910"></a><a name="zh-cn_topic_0225568815_p21921617113910"></a>策略值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row145715320389"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p148653552053"><a name="zh-cn_topic_0225568815_p148653552053"></a><a name="zh-cn_topic_0225568815_p148653552053"></a>condition_origin</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p108790551457"><a name="zh-cn_topic_0225568815_p108790551457"></a><a name="zh-cn_topic_0225568815_p108790551457"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p74929218395"><a name="zh-cn_topic_0225568815_p74929218395"></a><a name="zh-cn_topic_0225568815_p74929218395"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1021616179399"><a name="zh-cn_topic_0225568815_p1021616179399"></a><a name="zh-cn_topic_0225568815_p1021616179399"></a>策略类型：</p>
<a name="zh-cn_topic_0225568815_ul3227111717391"></a><a name="zh-cn_topic_0225568815_ul3227111717391"></a><ul id="zh-cn_topic_0225568815_ul3227111717391"><li>param：参数</li><li>source：源IP</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row51341036381"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p1293513558519"><a name="zh-cn_topic_0225568815_p1293513558519"></a><a name="zh-cn_topic_0225568815_p1293513558519"></a>req_param_name</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p4948115510510"><a name="zh-cn_topic_0225568815_p4948115510510"></a><a name="zh-cn_topic_0225568815_p4948115510510"></a>策略类型为param时必选</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p65171218399"><a name="zh-cn_topic_0225568815_p65171218399"></a><a name="zh-cn_topic_0225568815_p65171218399"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p1829011177392"><a name="zh-cn_topic_0225568815_p1829011177392"></a><a name="zh-cn_topic_0225568815_p1829011177392"></a>关联的请求参数对象名称</p>
</td>
</tr>
</tbody>
</table>

**表 14**  auth\_opt参数说明

<a name="zh-cn_topic_0225568815_table3438100125614"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row174381006567"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568815_p843813015615"><a name="zh-cn_topic_0225568815_p843813015615"></a><a name="zh-cn_topic_0225568815_p843813015615"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568815_p1643813015569"><a name="zh-cn_topic_0225568815_p1643813015569"></a><a name="zh-cn_topic_0225568815_p1643813015569"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568815_p1243840175615"><a name="zh-cn_topic_0225568815_p1243840175615"></a><a name="zh-cn_topic_0225568815_p1243840175615"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568815_p124384045617"><a name="zh-cn_topic_0225568815_p124384045617"></a><a name="zh-cn_topic_0225568815_p124384045617"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row04387035614"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568815_p14438106562"><a name="zh-cn_topic_0225568815_p14438106562"></a><a name="zh-cn_topic_0225568815_p14438106562"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568815_p743912095610"><a name="zh-cn_topic_0225568815_p743912095610"></a><a name="zh-cn_topic_0225568815_p743912095610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568815_p1043911075619"><a name="zh-cn_topic_0225568815_p1043911075619"></a><a name="zh-cn_topic_0225568815_p1043911075619"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568815_p15928340182414"><a name="zh-cn_topic_0225568815_p15928340182414"></a><a name="zh-cn_topic_0225568815_p15928340182414"></a>AppCode简易认证类型，仅在auth_type为APP时生效，默认为DISABLE：</p>
<a name="zh-cn_topic_0225568815_ul245955918358"></a><a name="zh-cn_topic_0225568815_ul245955918358"></a><ul id="zh-cn_topic_0225568815_ul245955918358"><li>DISABLE：不开启简易认证</li><li>HEADER：开启简易认证且AppCode位置在HEADER</li></ul>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "auth_type": "app",
  "auth_opt": {
    "app_code_auth_type": "HEADER"
  },
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
  "tags": ["APIG-SN-test", "test"],
  "type": 1,
  "result_normal_sample": "hello world!"
}
```

## 响应消息<a name="zh-cn_topic_0225568815_section46935561"></a>

**表 15**  参数说明

<a name="zh-cn_topic_0225568815_table13593802"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row45234979"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p40154672"><a name="zh-cn_topic_0225568815_p40154672"></a><a name="zh-cn_topic_0225568815_p40154672"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p31302981"><a name="zh-cn_topic_0225568815_p31302981"></a><a name="zh-cn_topic_0225568815_p31302981"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p52513547"><a name="zh-cn_topic_0225568815_p52513547"></a><a name="zh-cn_topic_0225568815_p52513547"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row25738921"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p4477896"><a name="zh-cn_topic_0225568815_p4477896"></a><a name="zh-cn_topic_0225568815_p4477896"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p27165328"><a name="zh-cn_topic_0225568815_p27165328"></a><a name="zh-cn_topic_0225568815_p27165328"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p52907944"><a name="zh-cn_topic_0225568815_p52907944"></a><a name="zh-cn_topic_0225568815_p52907944"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row6409449"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p49403389"><a name="zh-cn_topic_0225568815_p49403389"></a><a name="zh-cn_topic_0225568815_p49403389"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p42251573"><a name="zh-cn_topic_0225568815_p42251573"></a><a name="zh-cn_topic_0225568815_p42251573"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p66934266"><a name="zh-cn_topic_0225568815_p66934266"></a><a name="zh-cn_topic_0225568815_p66934266"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row65537484"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p6936015"><a name="zh-cn_topic_0225568815_p6936015"></a><a name="zh-cn_topic_0225568815_p6936015"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p24946322"><a name="zh-cn_topic_0225568815_p24946322"></a><a name="zh-cn_topic_0225568815_p24946322"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p7386173"><a name="zh-cn_topic_0225568815_p7386173"></a><a name="zh-cn_topic_0225568815_p7386173"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row66475561"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p15811397"><a name="zh-cn_topic_0225568815_p15811397"></a><a name="zh-cn_topic_0225568815_p15811397"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p5654748"><a name="zh-cn_topic_0225568815_p5654748"></a><a name="zh-cn_topic_0225568815_p5654748"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p55381464"><a name="zh-cn_topic_0225568815_p55381464"></a><a name="zh-cn_topic_0225568815_p55381464"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row28671136"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p40660654"><a name="zh-cn_topic_0225568815_p40660654"></a><a name="zh-cn_topic_0225568815_p40660654"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p5178644"><a name="zh-cn_topic_0225568815_p5178644"></a><a name="zh-cn_topic_0225568815_p5178644"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p16817019"><a name="zh-cn_topic_0225568815_p16817019"></a><a name="zh-cn_topic_0225568815_p16817019"></a>API的状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17135446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p45793889"><a name="zh-cn_topic_0225568815_p45793889"></a><a name="zh-cn_topic_0225568815_p45793889"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p18317504"><a name="zh-cn_topic_0225568815_p18317504"></a><a name="zh-cn_topic_0225568815_p18317504"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p7322844"><a name="zh-cn_topic_0225568815_p7322844"></a><a name="zh-cn_topic_0225568815_p7322844"></a>API类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row65905596"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p36753021"><a name="zh-cn_topic_0225568815_p36753021"></a><a name="zh-cn_topic_0225568815_p36753021"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p24204719"><a name="zh-cn_topic_0225568815_p24204719"></a><a name="zh-cn_topic_0225568815_p24204719"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p14425209"><a name="zh-cn_topic_0225568815_p14425209"></a><a name="zh-cn_topic_0225568815_p14425209"></a>API版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row62718023"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p46995113"><a name="zh-cn_topic_0225568815_p46995113"></a><a name="zh-cn_topic_0225568815_p46995113"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p48507832"><a name="zh-cn_topic_0225568815_p48507832"></a><a name="zh-cn_topic_0225568815_p48507832"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p36820315"><a name="zh-cn_topic_0225568815_p36820315"></a><a name="zh-cn_topic_0225568815_p36820315"></a>API访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row62947384"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p65573333"><a name="zh-cn_topic_0225568815_p65573333"></a><a name="zh-cn_topic_0225568815_p65573333"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p9839738"><a name="zh-cn_topic_0225568815_p9839738"></a><a name="zh-cn_topic_0225568815_p9839738"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p58821328"><a name="zh-cn_topic_0225568815_p58821328"></a><a name="zh-cn_topic_0225568815_p58821328"></a>API请求方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row59629909"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p65293302"><a name="zh-cn_topic_0225568815_p65293302"></a><a name="zh-cn_topic_0225568815_p65293302"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p54266141"><a name="zh-cn_topic_0225568815_p54266141"></a><a name="zh-cn_topic_0225568815_p54266141"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p33481263"><a name="zh-cn_topic_0225568815_p33481263"></a><a name="zh-cn_topic_0225568815_p33481263"></a>API访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row32895917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p47323597"><a name="zh-cn_topic_0225568815_p47323597"></a><a name="zh-cn_topic_0225568815_p47323597"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p8006158"><a name="zh-cn_topic_0225568815_p8006158"></a><a name="zh-cn_topic_0225568815_p8006158"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p44519063"><a name="zh-cn_topic_0225568815_p44519063"></a><a name="zh-cn_topic_0225568815_p44519063"></a>API认证方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row196085403616"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p45549491969"><a name="zh-cn_topic_0225568815_p45549491969"></a><a name="zh-cn_topic_0225568815_p45549491969"></a>auth_opt</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p19554194910611"><a name="zh-cn_topic_0225568815_p19554194910611"></a><a name="zh-cn_topic_0225568815_p19554194910611"></a>字段数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p155541490617"><a name="zh-cn_topic_0225568815_p155541490617"></a><a name="zh-cn_topic_0225568815_p155541490617"></a>API认证方式参数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row65127255"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p40816288"><a name="zh-cn_topic_0225568815_p40816288"></a><a name="zh-cn_topic_0225568815_p40816288"></a>match_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p17785030"><a name="zh-cn_topic_0225568815_p17785030"></a><a name="zh-cn_topic_0225568815_p17785030"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p31301296"><a name="zh-cn_topic_0225568815_p31301296"></a><a name="zh-cn_topic_0225568815_p31301296"></a>API匹配方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row13276210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1631230"><a name="zh-cn_topic_0225568815_p1631230"></a><a name="zh-cn_topic_0225568815_p1631230"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p65020802"><a name="zh-cn_topic_0225568815_p65020802"></a><a name="zh-cn_topic_0225568815_p65020802"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p32193639"><a name="zh-cn_topic_0225568815_p32193639"></a><a name="zh-cn_topic_0225568815_p32193639"></a>API注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row21307301"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p48169854"><a name="zh-cn_topic_0225568815_p48169854"></a><a name="zh-cn_topic_0225568815_p48169854"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p9444107"><a name="zh-cn_topic_0225568815_p9444107"></a><a name="zh-cn_topic_0225568815_p9444107"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p26775221"><a name="zh-cn_topic_0225568815_p26775221"></a><a name="zh-cn_topic_0225568815_p26775221"></a>API修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row39650400"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p57565823"><a name="zh-cn_topic_0225568815_p57565823"></a><a name="zh-cn_topic_0225568815_p57565823"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p32320111"><a name="zh-cn_topic_0225568815_p32320111"></a><a name="zh-cn_topic_0225568815_p32320111"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p683352"><a name="zh-cn_topic_0225568815_p683352"></a><a name="zh-cn_topic_0225568815_p683352"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row6150169"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p28401641"><a name="zh-cn_topic_0225568815_p28401641"></a><a name="zh-cn_topic_0225568815_p28401641"></a>bakend_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p18831557"><a name="zh-cn_topic_0225568815_p18831557"></a><a name="zh-cn_topic_0225568815_p18831557"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p48961174"><a name="zh-cn_topic_0225568815_p48961174"></a><a name="zh-cn_topic_0225568815_p48961174"></a>后端类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row57838348"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p54394634"><a name="zh-cn_topic_0225568815_p54394634"></a><a name="zh-cn_topic_0225568815_p54394634"></a>arrange_necessary</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p43889208"><a name="zh-cn_topic_0225568815_p43889208"></a><a name="zh-cn_topic_0225568815_p43889208"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p65364926"><a name="zh-cn_topic_0225568815_p65364926"></a><a name="zh-cn_topic_0225568815_p65364926"></a>是否需要编排</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row129911514122713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p82576192276"><a name="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p82576192276"></a><a name="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p82576192276"></a>tag</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p1625711193277"><a name="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p1625711193277"></a><a name="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p1625711193277"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p6273141922718"><a name="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p6273141922718"></a><a name="zh-cn_topic_0225568815_zh-cn_topic_0118921493_p6273141922718"></a>服务名称标签，待废弃字段</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row724717266414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p5689175210267"><a name="zh-cn_topic_0225568815_p5689175210267"></a><a name="zh-cn_topic_0225568815_p5689175210267"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p969065252610"><a name="zh-cn_topic_0225568815_p969065252610"></a><a name="zh-cn_topic_0225568815_p969065252610"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p10599103122713"><a name="zh-cn_topic_0225568815_p10599103122713"></a><a name="zh-cn_topic_0225568815_p10599103122713"></a>标签</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row8835717172720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p172881819162714"><a name="zh-cn_topic_0225568815_p172881819162714"></a><a name="zh-cn_topic_0225568815_p172881819162714"></a>cors</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p163043196278"><a name="zh-cn_topic_0225568815_p163043196278"></a><a name="zh-cn_topic_0225568815_p163043196278"></a>Bool</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p13320121932715"><a name="zh-cn_topic_0225568815_p13320121932715"></a><a name="zh-cn_topic_0225568815_p13320121932715"></a>是否支持跨域访问</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row05086382520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p250871111256"><a name="zh-cn_topic_0225568815_p250871111256"></a><a name="zh-cn_topic_0225568815_p250871111256"></a>body_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p75081711102513"><a name="zh-cn_topic_0225568815_p75081711102513"></a><a name="zh-cn_topic_0225568815_p75081711102513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1752320115253"><a name="zh-cn_topic_0225568815_p1752320115253"></a><a name="zh-cn_topic_0225568815_p1752320115253"></a>API请求体描述，可以是请求体示例、媒体类型、参数等信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row14117157142512"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p205704118252"><a name="zh-cn_topic_0225568815_p205704118252"></a><a name="zh-cn_topic_0225568815_p205704118252"></a>result_normal_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p13570141102519"><a name="zh-cn_topic_0225568815_p13570141102519"></a><a name="zh-cn_topic_0225568815_p13570141102519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p858631112257"><a name="zh-cn_topic_0225568815_p858631112257"></a><a name="zh-cn_topic_0225568815_p858631112257"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row65392912259"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p0633111142512"><a name="zh-cn_topic_0225568815_p0633111142512"></a><a name="zh-cn_topic_0225568815_p0633111142512"></a>result_failure_sample</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p063315115255"><a name="zh-cn_topic_0225568815_p063315115255"></a><a name="zh-cn_topic_0225568815_p063315115255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p116482113255"><a name="zh-cn_topic_0225568815_p116482113255"></a><a name="zh-cn_topic_0225568815_p116482113255"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row51413426"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p3737968"><a name="zh-cn_topic_0225568815_p3737968"></a><a name="zh-cn_topic_0225568815_p3737968"></a>backend_api</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p34339995"><a name="zh-cn_topic_0225568815_p34339995"></a><a name="zh-cn_topic_0225568815_p34339995"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p30076186"><a name="zh-cn_topic_0225568815_p30076186"></a><a name="zh-cn_topic_0225568815_p30076186"></a>后端服务：web后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row2250221"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p48050182"><a name="zh-cn_topic_0225568815_p48050182"></a><a name="zh-cn_topic_0225568815_p48050182"></a>mock_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p66859495"><a name="zh-cn_topic_0225568815_p66859495"></a><a name="zh-cn_topic_0225568815_p66859495"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p46910009"><a name="zh-cn_topic_0225568815_p46910009"></a><a name="zh-cn_topic_0225568815_p46910009"></a>后端服务：MOCK详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row19536899"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p38985025"><a name="zh-cn_topic_0225568815_p38985025"></a><a name="zh-cn_topic_0225568815_p38985025"></a>func_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p3670467"><a name="zh-cn_topic_0225568815_p3670467"></a><a name="zh-cn_topic_0225568815_p3670467"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p28872434"><a name="zh-cn_topic_0225568815_p28872434"></a><a name="zh-cn_topic_0225568815_p28872434"></a>后端服务：函数工作流后端详情</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row10999153874010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p13999938164017"><a name="zh-cn_topic_0225568815_p13999938164017"></a><a name="zh-cn_topic_0225568815_p13999938164017"></a>req_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1999203815404"><a name="zh-cn_topic_0225568815_p1999203815404"></a><a name="zh-cn_topic_0225568815_p1999203815404"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p11999143884013"><a name="zh-cn_topic_0225568815_p11999143884013"></a><a name="zh-cn_topic_0225568815_p11999143884013"></a>API的请求参数列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row14202164214407"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p420294234017"><a name="zh-cn_topic_0225568815_p420294234017"></a><a name="zh-cn_topic_0225568815_p420294234017"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p17202184217401"><a name="zh-cn_topic_0225568815_p17202184217401"></a><a name="zh-cn_topic_0225568815_p17202184217401"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p112025421400"><a name="zh-cn_topic_0225568815_p112025421400"></a><a name="zh-cn_topic_0225568815_p112025421400"></a>API的后端参数列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row15628145672517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p09691119194418"><a name="zh-cn_topic_0225568815_p09691119194418"></a><a name="zh-cn_topic_0225568815_p09691119194418"></a>policy_https</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p698531944420"><a name="zh-cn_topic_0225568815_p698531944420"></a><a name="zh-cn_topic_0225568815_p698531944420"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p142392054413"><a name="zh-cn_topic_0225568815_p142392054413"></a><a name="zh-cn_topic_0225568815_p142392054413"></a>web策略后端列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7901259152520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p450102034414"><a name="zh-cn_topic_0225568815_p450102034414"></a><a name="zh-cn_topic_0225568815_p450102034414"></a>policy_mocks</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p966720104412"><a name="zh-cn_topic_0225568815_p966720104412"></a><a name="zh-cn_topic_0225568815_p966720104412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p01071207449"><a name="zh-cn_topic_0225568815_p01071207449"></a><a name="zh-cn_topic_0225568815_p01071207449"></a>mock策略后端列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row2898103112612"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p18136122016449"><a name="zh-cn_topic_0225568815_p18136122016449"></a><a name="zh-cn_topic_0225568815_p18136122016449"></a>policy_functions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p715582011444"><a name="zh-cn_topic_0225568815_p715582011444"></a><a name="zh-cn_topic_0225568815_p715582011444"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p819162074416"><a name="zh-cn_topic_0225568815_p819162074416"></a><a name="zh-cn_topic_0225568815_p819162074416"></a>函数工作流策略后端列表</p>
</td>
</tr>
</tbody>
</table>

**表 16**  backend\_api参数说明

<a name="zh-cn_topic_0225568815_table58525317"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row19542026"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p39400239"><a name="zh-cn_topic_0225568815_p39400239"></a><a name="zh-cn_topic_0225568815_p39400239"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p37302768"><a name="zh-cn_topic_0225568815_p37302768"></a><a name="zh-cn_topic_0225568815_p37302768"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p1625399"><a name="zh-cn_topic_0225568815_p1625399"></a><a name="zh-cn_topic_0225568815_p1625399"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row64548457"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p61042544"><a name="zh-cn_topic_0225568815_p61042544"></a><a name="zh-cn_topic_0225568815_p61042544"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p45499060"><a name="zh-cn_topic_0225568815_p45499060"></a><a name="zh-cn_topic_0225568815_p45499060"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p61545244"><a name="zh-cn_topic_0225568815_p61545244"></a><a name="zh-cn_topic_0225568815_p61545244"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17036289"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p37762203"><a name="zh-cn_topic_0225568815_p37762203"></a><a name="zh-cn_topic_0225568815_p37762203"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p38839630"><a name="zh-cn_topic_0225568815_p38839630"></a><a name="zh-cn_topic_0225568815_p38839630"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p59002305"><a name="zh-cn_topic_0225568815_p59002305"></a><a name="zh-cn_topic_0225568815_p59002305"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row61258698"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p63007488"><a name="zh-cn_topic_0225568815_p63007488"></a><a name="zh-cn_topic_0225568815_p63007488"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p3332940"><a name="zh-cn_topic_0225568815_p3332940"></a><a name="zh-cn_topic_0225568815_p3332940"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p12150114811818"><a name="zh-cn_topic_0225568815_p12150114811818"></a><a name="zh-cn_topic_0225568815_p12150114811818"></a>后端endpoint</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row13794225"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p43590463"><a name="zh-cn_topic_0225568815_p43590463"></a><a name="zh-cn_topic_0225568815_p43590463"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p41166589"><a name="zh-cn_topic_0225568815_p41166589"></a><a name="zh-cn_topic_0225568815_p41166589"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p46159379"><a name="zh-cn_topic_0225568815_p46159379"></a><a name="zh-cn_topic_0225568815_p46159379"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row12781231"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p28646781"><a name="zh-cn_topic_0225568815_p28646781"></a><a name="zh-cn_topic_0225568815_p28646781"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p38687928"><a name="zh-cn_topic_0225568815_p38687928"></a><a name="zh-cn_topic_0225568815_p38687928"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p46714439"><a name="zh-cn_topic_0225568815_p46714439"></a><a name="zh-cn_topic_0225568815_p46714439"></a>访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17776770"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p30632235"><a name="zh-cn_topic_0225568815_p30632235"></a><a name="zh-cn_topic_0225568815_p30632235"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p65291932"><a name="zh-cn_topic_0225568815_p65291932"></a><a name="zh-cn_topic_0225568815_p65291932"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p54155134"><a name="zh-cn_topic_0225568815_p54155134"></a><a name="zh-cn_topic_0225568815_p54155134"></a>访问方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17634160"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p19080894"><a name="zh-cn_topic_0225568815_p19080894"></a><a name="zh-cn_topic_0225568815_p19080894"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p2048592"><a name="zh-cn_topic_0225568815_p2048592"></a><a name="zh-cn_topic_0225568815_p2048592"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p31718287"><a name="zh-cn_topic_0225568815_p31718287"></a><a name="zh-cn_topic_0225568815_p31718287"></a>访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17029130"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p37182327"><a name="zh-cn_topic_0225568815_p37182327"></a><a name="zh-cn_topic_0225568815_p37182327"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p58978500"><a name="zh-cn_topic_0225568815_p58978500"></a><a name="zh-cn_topic_0225568815_p58978500"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p12529177"><a name="zh-cn_topic_0225568815_p12529177"></a><a name="zh-cn_topic_0225568815_p12529177"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row45653735"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p6965020"><a name="zh-cn_topic_0225568815_p6965020"></a><a name="zh-cn_topic_0225568815_p6965020"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p27295725"><a name="zh-cn_topic_0225568815_p27295725"></a><a name="zh-cn_topic_0225568815_p27295725"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p63470148"><a name="zh-cn_topic_0225568815_p63470148"></a><a name="zh-cn_topic_0225568815_p63470148"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row34360420"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p31730620"><a name="zh-cn_topic_0225568815_p31730620"></a><a name="zh-cn_topic_0225568815_p31730620"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p20043404"><a name="zh-cn_topic_0225568815_p20043404"></a><a name="zh-cn_topic_0225568815_p20043404"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p12903037"><a name="zh-cn_topic_0225568815_p12903037"></a><a name="zh-cn_topic_0225568815_p12903037"></a>修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row49018473"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p11073390"><a name="zh-cn_topic_0225568815_p11073390"></a><a name="zh-cn_topic_0225568815_p11073390"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p24529383"><a name="zh-cn_topic_0225568815_p24529383"></a><a name="zh-cn_topic_0225568815_p24529383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p40723005"><a name="zh-cn_topic_0225568815_p40723005"></a><a name="zh-cn_topic_0225568815_p40723005"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row30962726"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p24952849"><a name="zh-cn_topic_0225568815_p24952849"></a><a name="zh-cn_topic_0225568815_p24952849"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p7914893"><a name="zh-cn_topic_0225568815_p7914893"></a><a name="zh-cn_topic_0225568815_p7914893"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p37126593"><a name="zh-cn_topic_0225568815_p37126593"></a><a name="zh-cn_topic_0225568815_p37126593"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row65703888"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p20414732"><a name="zh-cn_topic_0225568815_p20414732"></a><a name="zh-cn_topic_0225568815_p20414732"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p42980629"><a name="zh-cn_topic_0225568815_p42980629"></a><a name="zh-cn_topic_0225568815_p42980629"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p58878930"><a name="zh-cn_topic_0225568815_p58878930"></a><a name="zh-cn_topic_0225568815_p58878930"></a>VPC通道信息</p>
</td>
</tr>
</tbody>
</table>

**表 17**  mock\_info参数说明

<a name="zh-cn_topic_0225568815_table60148328"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row10756468"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p65967568"><a name="zh-cn_topic_0225568815_p65967568"></a><a name="zh-cn_topic_0225568815_p65967568"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p41772752"><a name="zh-cn_topic_0225568815_p41772752"></a><a name="zh-cn_topic_0225568815_p41772752"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p28149724"><a name="zh-cn_topic_0225568815_p28149724"></a><a name="zh-cn_topic_0225568815_p28149724"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row65535197"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p6750779"><a name="zh-cn_topic_0225568815_p6750779"></a><a name="zh-cn_topic_0225568815_p6750779"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p9942237"><a name="zh-cn_topic_0225568815_p9942237"></a><a name="zh-cn_topic_0225568815_p9942237"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p14892"><a name="zh-cn_topic_0225568815_p14892"></a><a name="zh-cn_topic_0225568815_p14892"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row134031"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p10856588"><a name="zh-cn_topic_0225568815_p10856588"></a><a name="zh-cn_topic_0225568815_p10856588"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p6968425"><a name="zh-cn_topic_0225568815_p6968425"></a><a name="zh-cn_topic_0225568815_p6968425"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p27571534"><a name="zh-cn_topic_0225568815_p27571534"></a><a name="zh-cn_topic_0225568815_p27571534"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row46817220"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p34098441"><a name="zh-cn_topic_0225568815_p34098441"></a><a name="zh-cn_topic_0225568815_p34098441"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p10510314"><a name="zh-cn_topic_0225568815_p10510314"></a><a name="zh-cn_topic_0225568815_p10510314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p46029137"><a name="zh-cn_topic_0225568815_p46029137"></a><a name="zh-cn_topic_0225568815_p46029137"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row11609049"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p808897"><a name="zh-cn_topic_0225568815_p808897"></a><a name="zh-cn_topic_0225568815_p808897"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p65520673"><a name="zh-cn_topic_0225568815_p65520673"></a><a name="zh-cn_topic_0225568815_p65520673"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p5574306"><a name="zh-cn_topic_0225568815_p5574306"></a><a name="zh-cn_topic_0225568815_p5574306"></a>返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row50168758"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p37137611"><a name="zh-cn_topic_0225568815_p37137611"></a><a name="zh-cn_topic_0225568815_p37137611"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p55356500"><a name="zh-cn_topic_0225568815_p55356500"></a><a name="zh-cn_topic_0225568815_p55356500"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p54691514"><a name="zh-cn_topic_0225568815_p54691514"></a><a name="zh-cn_topic_0225568815_p54691514"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row22461579"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p7448582"><a name="zh-cn_topic_0225568815_p7448582"></a><a name="zh-cn_topic_0225568815_p7448582"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p66464274"><a name="zh-cn_topic_0225568815_p66464274"></a><a name="zh-cn_topic_0225568815_p66464274"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p14897110"><a name="zh-cn_topic_0225568815_p14897110"></a><a name="zh-cn_topic_0225568815_p14897110"></a>修改时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row66965133"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p55466713"><a name="zh-cn_topic_0225568815_p55466713"></a><a name="zh-cn_topic_0225568815_p55466713"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p63618802"><a name="zh-cn_topic_0225568815_p63618802"></a><a name="zh-cn_topic_0225568815_p63618802"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p52849343"><a name="zh-cn_topic_0225568815_p52849343"></a><a name="zh-cn_topic_0225568815_p52849343"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 18**  func\_info参数说明

<a name="zh-cn_topic_0225568815_table5882045"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row61925025"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p49871117"><a name="zh-cn_topic_0225568815_p49871117"></a><a name="zh-cn_topic_0225568815_p49871117"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p13028637"><a name="zh-cn_topic_0225568815_p13028637"></a><a name="zh-cn_topic_0225568815_p13028637"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p48686649"><a name="zh-cn_topic_0225568815_p48686649"></a><a name="zh-cn_topic_0225568815_p48686649"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row51304522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p62025656"><a name="zh-cn_topic_0225568815_p62025656"></a><a name="zh-cn_topic_0225568815_p62025656"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p58022250"><a name="zh-cn_topic_0225568815_p58022250"></a><a name="zh-cn_topic_0225568815_p58022250"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p2181833"><a name="zh-cn_topic_0225568815_p2181833"></a><a name="zh-cn_topic_0225568815_p2181833"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row19636500"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p47052705"><a name="zh-cn_topic_0225568815_p47052705"></a><a name="zh-cn_topic_0225568815_p47052705"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p53172750"><a name="zh-cn_topic_0225568815_p53172750"></a><a name="zh-cn_topic_0225568815_p53172750"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p12025475"><a name="zh-cn_topic_0225568815_p12025475"></a><a name="zh-cn_topic_0225568815_p12025475"></a>状态</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row41120417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p42419446"><a name="zh-cn_topic_0225568815_p42419446"></a><a name="zh-cn_topic_0225568815_p42419446"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p13423079"><a name="zh-cn_topic_0225568815_p13423079"></a><a name="zh-cn_topic_0225568815_p13423079"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p13527646"><a name="zh-cn_topic_0225568815_p13527646"></a><a name="zh-cn_topic_0225568815_p13527646"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row54639950"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p63759814"><a name="zh-cn_topic_0225568815_p63759814"></a><a name="zh-cn_topic_0225568815_p63759814"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p64271286"><a name="zh-cn_topic_0225568815_p64271286"></a><a name="zh-cn_topic_0225568815_p64271286"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p38591687"><a name="zh-cn_topic_0225568815_p38591687"></a><a name="zh-cn_topic_0225568815_p38591687"></a>函数URN</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row11780867"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p14726184"><a name="zh-cn_topic_0225568815_p14726184"></a><a name="zh-cn_topic_0225568815_p14726184"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p51970241"><a name="zh-cn_topic_0225568815_p51970241"></a><a name="zh-cn_topic_0225568815_p51970241"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p48839991"><a name="zh-cn_topic_0225568815_p48839991"></a><a name="zh-cn_topic_0225568815_p48839991"></a>调用类型:async|sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row36906736"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p36655611"><a name="zh-cn_topic_0225568815_p36655611"></a><a name="zh-cn_topic_0225568815_p36655611"></a>register_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p16314519"><a name="zh-cn_topic_0225568815_p16314519"></a><a name="zh-cn_topic_0225568815_p16314519"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p46407659"><a name="zh-cn_topic_0225568815_p46407659"></a><a name="zh-cn_topic_0225568815_p46407659"></a>注册时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row15015754"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p8316582"><a name="zh-cn_topic_0225568815_p8316582"></a><a name="zh-cn_topic_0225568815_p8316582"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p2554575"><a name="zh-cn_topic_0225568815_p2554575"></a><a name="zh-cn_topic_0225568815_p2554575"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p5594028"><a name="zh-cn_topic_0225568815_p5594028"></a><a name="zh-cn_topic_0225568815_p5594028"></a>更新时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row50346258"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p51515097"><a name="zh-cn_topic_0225568815_p51515097"></a><a name="zh-cn_topic_0225568815_p51515097"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p11973320"><a name="zh-cn_topic_0225568815_p11973320"></a><a name="zh-cn_topic_0225568815_p11973320"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p30314888"><a name="zh-cn_topic_0225568815_p30314888"></a><a name="zh-cn_topic_0225568815_p30314888"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row4398542"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p20737610"><a name="zh-cn_topic_0225568815_p20737610"></a><a name="zh-cn_topic_0225568815_p20737610"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p2024810"><a name="zh-cn_topic_0225568815_p2024810"></a><a name="zh-cn_topic_0225568815_p2024810"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p29791894"><a name="zh-cn_topic_0225568815_p29791894"></a><a name="zh-cn_topic_0225568815_p29791894"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 19**  req\_params参数说明

<a name="zh-cn_topic_0225568815_table197251634194412"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row2075603420446"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p11756234184411"><a name="zh-cn_topic_0225568815_p11756234184411"></a><a name="zh-cn_topic_0225568815_p11756234184411"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p777143420447"><a name="zh-cn_topic_0225568815_p777143420447"></a><a name="zh-cn_topic_0225568815_p777143420447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p5771193415446"><a name="zh-cn_topic_0225568815_p5771193415446"></a><a name="zh-cn_topic_0225568815_p5771193415446"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row85313200454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1753320144511"><a name="zh-cn_topic_0225568815_p1753320144511"></a><a name="zh-cn_topic_0225568815_p1753320144511"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p75302015450"><a name="zh-cn_topic_0225568815_p75302015450"></a><a name="zh-cn_topic_0225568815_p75302015450"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p653162014451"><a name="zh-cn_topic_0225568815_p653162014451"></a><a name="zh-cn_topic_0225568815_p653162014451"></a>参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row8786123464413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p578618344445"><a name="zh-cn_topic_0225568815_p578618344445"></a><a name="zh-cn_topic_0225568815_p578618344445"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1480313412443"><a name="zh-cn_topic_0225568815_p1480313412443"></a><a name="zh-cn_topic_0225568815_p1480313412443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p48033344445"><a name="zh-cn_topic_0225568815_p48033344445"></a><a name="zh-cn_topic_0225568815_p48033344445"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row13818193434411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p781810341448"><a name="zh-cn_topic_0225568815_p781810341448"></a><a name="zh-cn_topic_0225568815_p781810341448"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p18342034114419"><a name="zh-cn_topic_0225568815_p18342034114419"></a><a name="zh-cn_topic_0225568815_p18342034114419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p083493413441"><a name="zh-cn_topic_0225568815_p083493413441"></a><a name="zh-cn_topic_0225568815_p083493413441"></a>参数类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17850234124414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p18865203414418"><a name="zh-cn_topic_0225568815_p18865203414418"></a><a name="zh-cn_topic_0225568815_p18865203414418"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p16881203415443"><a name="zh-cn_topic_0225568815_p16881203415443"></a><a name="zh-cn_topic_0225568815_p16881203415443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p788120340445"><a name="zh-cn_topic_0225568815_p788120340445"></a><a name="zh-cn_topic_0225568815_p788120340445"></a>参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row99121534134414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p18912934114419"><a name="zh-cn_topic_0225568815_p18912934114419"></a><a name="zh-cn_topic_0225568815_p18912934114419"></a>default_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p139281534104415"><a name="zh-cn_topic_0225568815_p139281534104415"></a><a name="zh-cn_topic_0225568815_p139281534104415"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1592853454412"><a name="zh-cn_topic_0225568815_p1592853454412"></a><a name="zh-cn_topic_0225568815_p1592853454412"></a>参数默认值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1594315349446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p994311348442"><a name="zh-cn_topic_0225568815_p994311348442"></a><a name="zh-cn_topic_0225568815_p994311348442"></a>sample_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1495973414419"><a name="zh-cn_topic_0225568815_p1495973414419"></a><a name="zh-cn_topic_0225568815_p1495973414419"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1695953413449"><a name="zh-cn_topic_0225568815_p1695953413449"></a><a name="zh-cn_topic_0225568815_p1695953413449"></a>参数示例值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1959173474410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p2974183417445"><a name="zh-cn_topic_0225568815_p2974183417445"></a><a name="zh-cn_topic_0225568815_p2974183417445"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p13974143417443"><a name="zh-cn_topic_0225568815_p13974143417443"></a><a name="zh-cn_topic_0225568815_p13974143417443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p699053414444"><a name="zh-cn_topic_0225568815_p699053414444"></a><a name="zh-cn_topic_0225568815_p699053414444"></a>是否必须</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row662354446"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p66183524412"><a name="zh-cn_topic_0225568815_p66183524412"></a><a name="zh-cn_topic_0225568815_p66183524412"></a>valid_enable</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p32133519447"><a name="zh-cn_topic_0225568815_p32133519447"></a><a name="zh-cn_topic_0225568815_p32133519447"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p18371535124417"><a name="zh-cn_topic_0225568815_p18371535124417"></a><a name="zh-cn_topic_0225568815_p18371535124417"></a>是否开启校验</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1053435144414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p653133513441"><a name="zh-cn_topic_0225568815_p653133513441"></a><a name="zh-cn_topic_0225568815_p653133513441"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1867183512446"><a name="zh-cn_topic_0225568815_p1867183512446"></a><a name="zh-cn_topic_0225568815_p1867183512446"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p567123584420"><a name="zh-cn_topic_0225568815_p567123584420"></a><a name="zh-cn_topic_0225568815_p567123584420"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7100203515443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p181002035154415"><a name="zh-cn_topic_0225568815_p181002035154415"></a><a name="zh-cn_topic_0225568815_p181002035154415"></a>enumerations</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p161151635164413"><a name="zh-cn_topic_0225568815_p161151635164413"></a><a name="zh-cn_topic_0225568815_p161151635164413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p2559522184412"><a name="zh-cn_topic_0225568815_p2559522184412"></a><a name="zh-cn_topic_0225568815_p2559522184412"></a>参数枚举值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row121151635204414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p151311235144415"><a name="zh-cn_topic_0225568815_p151311235144415"></a><a name="zh-cn_topic_0225568815_p151311235144415"></a>min_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p713112353443"><a name="zh-cn_topic_0225568815_p713112353443"></a><a name="zh-cn_topic_0225568815_p713112353443"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p95973228446"><a name="zh-cn_topic_0225568815_p95973228446"></a><a name="zh-cn_topic_0225568815_p95973228446"></a>参数最小值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row01461435194417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p8146203564415"><a name="zh-cn_topic_0225568815_p8146203564415"></a><a name="zh-cn_topic_0225568815_p8146203564415"></a>max_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p31627353442"><a name="zh-cn_topic_0225568815_p31627353442"></a><a name="zh-cn_topic_0225568815_p31627353442"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p2631222104413"><a name="zh-cn_topic_0225568815_p2631222104413"></a><a name="zh-cn_topic_0225568815_p2631222104413"></a>参数最大值（参数类型为NUMBER时有效）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1717853574413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p61782355443"><a name="zh-cn_topic_0225568815_p61782355443"></a><a name="zh-cn_topic_0225568815_p61782355443"></a>min_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p201932035194417"><a name="zh-cn_topic_0225568815_p201932035194417"></a><a name="zh-cn_topic_0225568815_p201932035194417"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p2668152294420"><a name="zh-cn_topic_0225568815_p2668152294420"></a><a name="zh-cn_topic_0225568815_p2668152294420"></a>参数最小长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1220912352444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p12209535144412"><a name="zh-cn_topic_0225568815_p12209535144412"></a><a name="zh-cn_topic_0225568815_p12209535144412"></a>max_size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p12251035164419"><a name="zh-cn_topic_0225568815_p12251035164419"></a><a name="zh-cn_topic_0225568815_p12251035164419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p3702522184416"><a name="zh-cn_topic_0225568815_p3702522184416"></a><a name="zh-cn_topic_0225568815_p3702522184416"></a>参数最大长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1422523519444"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p52401735134413"><a name="zh-cn_topic_0225568815_p52401735134413"></a><a name="zh-cn_topic_0225568815_p52401735134413"></a>regular</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p12240153510443"><a name="zh-cn_topic_0225568815_p12240153510443"></a><a name="zh-cn_topic_0225568815_p12240153510443"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p12731822184412"><a name="zh-cn_topic_0225568815_p12731822184412"></a><a name="zh-cn_topic_0225568815_p12731822184412"></a>正则校验规则（暂不支持）</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row12561435124410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p202561335114413"><a name="zh-cn_topic_0225568815_p202561335114413"></a><a name="zh-cn_topic_0225568815_p202561335114413"></a>json_schema</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p16271035114412"><a name="zh-cn_topic_0225568815_p16271035114412"></a><a name="zh-cn_topic_0225568815_p16271035114412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p57661222144411"><a name="zh-cn_topic_0225568815_p57661222144411"></a><a name="zh-cn_topic_0225568815_p57661222144411"></a>JSON校验规则（暂不支持）</p>
</td>
</tr>
</tbody>
</table>

**表 20**  backend\_params参数说明

<a name="zh-cn_topic_0225568815_table9287113513446"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row4302173564419"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p33182355443"><a name="zh-cn_topic_0225568815_p33182355443"></a><a name="zh-cn_topic_0225568815_p33182355443"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p14334103544415"><a name="zh-cn_topic_0225568815_p14334103544415"></a><a name="zh-cn_topic_0225568815_p14334103544415"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p19334153517444"><a name="zh-cn_topic_0225568815_p19334153517444"></a><a name="zh-cn_topic_0225568815_p19334153517444"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row17142774611"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p47152713464"><a name="zh-cn_topic_0225568815_p47152713464"></a><a name="zh-cn_topic_0225568815_p47152713464"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1717279463"><a name="zh-cn_topic_0225568815_p1717279463"></a><a name="zh-cn_topic_0225568815_p1717279463"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p27122714620"><a name="zh-cn_topic_0225568815_p27122714620"></a><a name="zh-cn_topic_0225568815_p27122714620"></a>参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row2936129114713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p199361729154717"><a name="zh-cn_topic_0225568815_p199361729154717"></a><a name="zh-cn_topic_0225568815_p199361729154717"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1693652934715"><a name="zh-cn_topic_0225568815_p1693652934715"></a><a name="zh-cn_topic_0225568815_p1693652934715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1093614294475"><a name="zh-cn_topic_0225568815_p1093614294475"></a><a name="zh-cn_topic_0225568815_p1093614294475"></a>对应的请求参数编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row833403514441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p13350143554413"><a name="zh-cn_topic_0225568815_p13350143554413"></a><a name="zh-cn_topic_0225568815_p13350143554413"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p6365163554417"><a name="zh-cn_topic_0225568815_p6365163554417"></a><a name="zh-cn_topic_0225568815_p6365163554417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p036516356445"><a name="zh-cn_topic_0225568815_p036516356445"></a><a name="zh-cn_topic_0225568815_p036516356445"></a>参数名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row203656353443"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p4381103534420"><a name="zh-cn_topic_0225568815_p4381103534420"></a><a name="zh-cn_topic_0225568815_p4381103534420"></a>location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p838193504410"><a name="zh-cn_topic_0225568815_p838193504410"></a><a name="zh-cn_topic_0225568815_p838193504410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p10396123516442"><a name="zh-cn_topic_0225568815_p10396123516442"></a><a name="zh-cn_topic_0225568815_p10396123516442"></a>参数位置</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7412103554417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p14271535144413"><a name="zh-cn_topic_0225568815_p14271535144413"></a><a name="zh-cn_topic_0225568815_p14271535144413"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p34431235184418"><a name="zh-cn_topic_0225568815_p34431235184418"></a><a name="zh-cn_topic_0225568815_p34431235184418"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1044312351449"><a name="zh-cn_topic_0225568815_p1044312351449"></a><a name="zh-cn_topic_0225568815_p1044312351449"></a>参数类别</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row445983511447"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p5475203519440"><a name="zh-cn_topic_0225568815_p5475203519440"></a><a name="zh-cn_topic_0225568815_p5475203519440"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1449053524417"><a name="zh-cn_topic_0225568815_p1449053524417"></a><a name="zh-cn_topic_0225568815_p1449053524417"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p9490435144419"><a name="zh-cn_topic_0225568815_p9490435144419"></a><a name="zh-cn_topic_0225568815_p9490435144419"></a>参数值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row7506335184410"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p3506935104410"><a name="zh-cn_topic_0225568815_p3506935104410"></a><a name="zh-cn_topic_0225568815_p3506935104410"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p05217356442"><a name="zh-cn_topic_0225568815_p05217356442"></a><a name="zh-cn_topic_0225568815_p05217356442"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p11521123517447"><a name="zh-cn_topic_0225568815_p11521123517447"></a><a name="zh-cn_topic_0225568815_p11521123517447"></a>描述</p>
</td>
</tr>
</tbody>
</table>

**表 21**  policy\_https参数说明

<a name="zh-cn_topic_0225568815_table1883393417451"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row12893173494517"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p1491393413454"><a name="zh-cn_topic_0225568815_p1491393413454"></a><a name="zh-cn_topic_0225568815_p1491393413454"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p3930134144518"><a name="zh-cn_topic_0225568815_p3930134144518"></a><a name="zh-cn_topic_0225568815_p3930134144518"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p1394693410456"><a name="zh-cn_topic_0225568815_p1394693410456"></a><a name="zh-cn_topic_0225568815_p1394693410456"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row129661334174520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1997923418453"><a name="zh-cn_topic_0225568815_p1997923418453"></a><a name="zh-cn_topic_0225568815_p1997923418453"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p699316349457"><a name="zh-cn_topic_0225568815_p699316349457"></a><a name="zh-cn_topic_0225568815_p699316349457"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1176354455"><a name="zh-cn_topic_0225568815_p1176354455"></a><a name="zh-cn_topic_0225568815_p1176354455"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row191173534519"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p729183516457"><a name="zh-cn_topic_0225568815_p729183516457"></a><a name="zh-cn_topic_0225568815_p729183516457"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p5442035114515"><a name="zh-cn_topic_0225568815_p5442035114515"></a><a name="zh-cn_topic_0225568815_p5442035114515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p105673584520"><a name="zh-cn_topic_0225568815_p105673584520"></a><a name="zh-cn_topic_0225568815_p105673584520"></a>策略后端名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row19611535114513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p20805354452"><a name="zh-cn_topic_0225568815_p20805354452"></a><a name="zh-cn_topic_0225568815_p20805354452"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p09323564519"><a name="zh-cn_topic_0225568815_p09323564519"></a><a name="zh-cn_topic_0225568815_p09323564519"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p131089355454"><a name="zh-cn_topic_0225568815_p131089355454"></a><a name="zh-cn_topic_0225568815_p131089355454"></a>策略后端endpoint</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row141732035194520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p11921135124512"><a name="zh-cn_topic_0225568815_p11921135124512"></a><a name="zh-cn_topic_0225568815_p11921135124512"></a>req_protocol</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p2209173510459"><a name="zh-cn_topic_0225568815_p2209173510459"></a><a name="zh-cn_topic_0225568815_p2209173510459"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p2223153513453"><a name="zh-cn_topic_0225568815_p2223153513453"></a><a name="zh-cn_topic_0225568815_p2223153513453"></a>访问协议</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row102311835144513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p142451635144514"><a name="zh-cn_topic_0225568815_p142451635144514"></a><a name="zh-cn_topic_0225568815_p142451635144514"></a>req_method</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p926153519453"><a name="zh-cn_topic_0225568815_p926153519453"></a><a name="zh-cn_topic_0225568815_p926153519453"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p0276135124514"><a name="zh-cn_topic_0225568815_p0276135124514"></a><a name="zh-cn_topic_0225568815_p0276135124514"></a>访问方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row9284735204514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1629817356452"><a name="zh-cn_topic_0225568815_p1629817356452"></a><a name="zh-cn_topic_0225568815_p1629817356452"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p2313183554516"><a name="zh-cn_topic_0225568815_p2313183554516"></a><a name="zh-cn_topic_0225568815_p2313183554516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p123341135134516"><a name="zh-cn_topic_0225568815_p123341135134516"></a><a name="zh-cn_topic_0225568815_p123341135134516"></a>访问地址</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row20342535194519"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p8362535154510"><a name="zh-cn_topic_0225568815_p8362535154510"></a><a name="zh-cn_topic_0225568815_p8362535154510"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p12378193514459"><a name="zh-cn_topic_0225568815_p12378193514459"></a><a name="zh-cn_topic_0225568815_p12378193514459"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p123951235114514"><a name="zh-cn_topic_0225568815_p123951235114514"></a><a name="zh-cn_topic_0225568815_p123951235114514"></a>访问超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1159233518458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p20614163564511"><a name="zh-cn_topic_0225568815_p20614163564511"></a><a name="zh-cn_topic_0225568815_p20614163564511"></a>vpc_status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p9632143519451"><a name="zh-cn_topic_0225568815_p9632143519451"></a><a name="zh-cn_topic_0225568815_p9632143519451"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p56481835124516"><a name="zh-cn_topic_0225568815_p56481835124516"></a><a name="zh-cn_topic_0225568815_p56481835124516"></a>是否使用VPC通道</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row765613353459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p19673193519458"><a name="zh-cn_topic_0225568815_p19673193519458"></a><a name="zh-cn_topic_0225568815_p19673193519458"></a>vpc_info</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p0690203524511"><a name="zh-cn_topic_0225568815_p0690203524511"></a><a name="zh-cn_topic_0225568815_p0690203524511"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p20706143594518"><a name="zh-cn_topic_0225568815_p20706143594518"></a><a name="zh-cn_topic_0225568815_p20706143594518"></a>VPC通道信息</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row33971122125919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p7397722115911"><a name="zh-cn_topic_0225568815_p7397722115911"></a><a name="zh-cn_topic_0225568815_p7397722115911"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p14397142235915"><a name="zh-cn_topic_0225568815_p14397142235915"></a><a name="zh-cn_topic_0225568815_p14397142235915"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p143978228592"><a name="zh-cn_topic_0225568815_p143978228592"></a><a name="zh-cn_topic_0225568815_p143978228592"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17521289599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p181451844918"><a name="zh-cn_topic_0225568815_p181451844918"></a><a name="zh-cn_topic_0225568815_p181451844918"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p178501852715"><a name="zh-cn_topic_0225568815_p178501852715"></a><a name="zh-cn_topic_0225568815_p178501852715"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1091214598110"><a name="zh-cn_topic_0225568815_p1091214598110"></a><a name="zh-cn_topic_0225568815_p1091214598110"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row62321736195919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p131741744219"><a name="zh-cn_topic_0225568815_p131741744219"></a><a name="zh-cn_topic_0225568815_p131741744219"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1487855214114"><a name="zh-cn_topic_0225568815_p1487855214114"></a><a name="zh-cn_topic_0225568815_p1487855214114"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p3947175912116"><a name="zh-cn_topic_0225568815_p3947175912116"></a><a name="zh-cn_topic_0225568815_p3947175912116"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 22**  policy\_mocks参数说明

<a name="zh-cn_topic_0225568815_table12725183513454"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row15764635144513"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p378211357456"><a name="zh-cn_topic_0225568815_p378211357456"></a><a name="zh-cn_topic_0225568815_p378211357456"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p58001135104513"><a name="zh-cn_topic_0225568815_p58001135104513"></a><a name="zh-cn_topic_0225568815_p58001135104513"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p981853512455"><a name="zh-cn_topic_0225568815_p981853512455"></a><a name="zh-cn_topic_0225568815_p981853512455"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row2835103534513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p6852143510458"><a name="zh-cn_topic_0225568815_p6852143510458"></a><a name="zh-cn_topic_0225568815_p6852143510458"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p2866103524515"><a name="zh-cn_topic_0225568815_p2866103524515"></a><a name="zh-cn_topic_0225568815_p2866103524515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1587913519457"><a name="zh-cn_topic_0225568815_p1587913519457"></a><a name="zh-cn_topic_0225568815_p1587913519457"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row8887123534513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p15538921331"><a name="zh-cn_topic_0225568815_p15538921331"></a><a name="zh-cn_topic_0225568815_p15538921331"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p135591025311"><a name="zh-cn_topic_0225568815_p135591025311"></a><a name="zh-cn_topic_0225568815_p135591025311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p105814212311"><a name="zh-cn_topic_0225568815_p105814212311"></a><a name="zh-cn_topic_0225568815_p105814212311"></a>策略后端名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row119183644517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1737133612459"><a name="zh-cn_topic_0225568815_p1737133612459"></a><a name="zh-cn_topic_0225568815_p1737133612459"></a>result_content</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p13522036104518"><a name="zh-cn_topic_0225568815_p13522036104518"></a><a name="zh-cn_topic_0225568815_p13522036104518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p116953674519"><a name="zh-cn_topic_0225568815_p116953674519"></a><a name="zh-cn_topic_0225568815_p116953674519"></a>返回结果</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1780193618456"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p129375499320"><a name="zh-cn_topic_0225568815_p129375499320"></a><a name="zh-cn_topic_0225568815_p129375499320"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p20959149733"><a name="zh-cn_topic_0225568815_p20959149733"></a><a name="zh-cn_topic_0225568815_p20959149733"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p49808491431"><a name="zh-cn_topic_0225568815_p49808491431"></a><a name="zh-cn_topic_0225568815_p49808491431"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row914193684515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p21155015317"><a name="zh-cn_topic_0225568815_p21155015317"></a><a name="zh-cn_topic_0225568815_p21155015317"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1631135010319"><a name="zh-cn_topic_0225568815_p1631135010319"></a><a name="zh-cn_topic_0225568815_p1631135010319"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p95105016320"><a name="zh-cn_topic_0225568815_p95105016320"></a><a name="zh-cn_topic_0225568815_p95105016320"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row220083616456"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p19851150935"><a name="zh-cn_topic_0225568815_p19851150935"></a><a name="zh-cn_topic_0225568815_p19851150935"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p191021350934"><a name="zh-cn_topic_0225568815_p191021350934"></a><a name="zh-cn_topic_0225568815_p191021350934"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p21240503312"><a name="zh-cn_topic_0225568815_p21240503312"></a><a name="zh-cn_topic_0225568815_p21240503312"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 23**  policy\_functions参数说明

<a name="zh-cn_topic_0225568815_table11274103664518"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row14323123615458"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p12336163614453"><a name="zh-cn_topic_0225568815_p12336163614453"></a><a name="zh-cn_topic_0225568815_p12336163614453"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p3348163613458"><a name="zh-cn_topic_0225568815_p3348163613458"></a><a name="zh-cn_topic_0225568815_p3348163613458"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p136353684510"><a name="zh-cn_topic_0225568815_p136353684510"></a><a name="zh-cn_topic_0225568815_p136353684510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row438373613454"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p193981361454"><a name="zh-cn_topic_0225568815_p193981361454"></a><a name="zh-cn_topic_0225568815_p193981361454"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p10414336164515"><a name="zh-cn_topic_0225568815_p10414336164515"></a><a name="zh-cn_topic_0225568815_p10414336164515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1543203615456"><a name="zh-cn_topic_0225568815_p1543203615456"></a><a name="zh-cn_topic_0225568815_p1543203615456"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1844443611451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p145173216411"><a name="zh-cn_topic_0225568815_p145173216411"></a><a name="zh-cn_topic_0225568815_p145173216411"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p125371217420"><a name="zh-cn_topic_0225568815_p125371217420"></a><a name="zh-cn_topic_0225568815_p125371217420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p15581212410"><a name="zh-cn_topic_0225568815_p15581212410"></a><a name="zh-cn_topic_0225568815_p15581212410"></a>策略后端名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row450233644511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p25201036164517"><a name="zh-cn_topic_0225568815_p25201036164517"></a><a name="zh-cn_topic_0225568815_p25201036164517"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p16541736164516"><a name="zh-cn_topic_0225568815_p16541736164516"></a><a name="zh-cn_topic_0225568815_p16541736164516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p16558133684511"><a name="zh-cn_topic_0225568815_p16558133684511"></a><a name="zh-cn_topic_0225568815_p16558133684511"></a>版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row45685369453"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p45841936134516"><a name="zh-cn_topic_0225568815_p45841936134516"></a><a name="zh-cn_topic_0225568815_p45841936134516"></a>function_urn</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p25991036114518"><a name="zh-cn_topic_0225568815_p25991036114518"></a><a name="zh-cn_topic_0225568815_p25991036114518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p6618133614456"><a name="zh-cn_topic_0225568815_p6618133614456"></a><a name="zh-cn_topic_0225568815_p6618133614456"></a>函数URN</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row56281362452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1364419365459"><a name="zh-cn_topic_0225568815_p1364419365459"></a><a name="zh-cn_topic_0225568815_p1364419365459"></a>invocation_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p19665236114517"><a name="zh-cn_topic_0225568815_p19665236114517"></a><a name="zh-cn_topic_0225568815_p19665236114517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1968233654519"><a name="zh-cn_topic_0225568815_p1968233654519"></a><a name="zh-cn_topic_0225568815_p1968233654519"></a>调用类型:async|sync</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row108137365458"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1183073613455"><a name="zh-cn_topic_0225568815_p1183073613455"></a><a name="zh-cn_topic_0225568815_p1183073613455"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1484712366457"><a name="zh-cn_topic_0225568815_p1484712366457"></a><a name="zh-cn_topic_0225568815_p1484712366457"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1687010368458"><a name="zh-cn_topic_0225568815_p1687010368458"></a><a name="zh-cn_topic_0225568815_p1687010368458"></a>超时时间，单位：毫秒</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1288018362459"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p125311657249"><a name="zh-cn_topic_0225568815_p125311657249"></a><a name="zh-cn_topic_0225568815_p125311657249"></a>effect_mode</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p165491576420"><a name="zh-cn_topic_0225568815_p165491576420"></a><a name="zh-cn_topic_0225568815_p165491576420"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p556795712420"><a name="zh-cn_topic_0225568815_p556795712420"></a><a name="zh-cn_topic_0225568815_p556795712420"></a>关联的策略组合模式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row14199172719419"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p259219571446"><a name="zh-cn_topic_0225568815_p259219571446"></a><a name="zh-cn_topic_0225568815_p259219571446"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p160916576412"><a name="zh-cn_topic_0225568815_p160916576412"></a><a name="zh-cn_topic_0225568815_p160916576412"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p17627257149"><a name="zh-cn_topic_0225568815_p17627257149"></a><a name="zh-cn_topic_0225568815_p17627257149"></a>策略条件列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row107283241048"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p66684572045"><a name="zh-cn_topic_0225568815_p66684572045"></a><a name="zh-cn_topic_0225568815_p66684572045"></a>backend_params</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p126865574411"><a name="zh-cn_topic_0225568815_p126865574411"></a><a name="zh-cn_topic_0225568815_p126865574411"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p17025579410"><a name="zh-cn_topic_0225568815_p17025579410"></a><a name="zh-cn_topic_0225568815_p17025579410"></a>后端参数列表</p>
</td>
</tr>
</tbody>
</table>

**表 24**  conditions参数说明

<a name="zh-cn_topic_0225568815_table54445157"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row01061051953"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p121240513510"><a name="zh-cn_topic_0225568815_p121240513510"></a><a name="zh-cn_topic_0225568815_p121240513510"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p0145557515"><a name="zh-cn_topic_0225568815_p0145557515"></a><a name="zh-cn_topic_0225568815_p0145557515"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p4166752511"><a name="zh-cn_topic_0225568815_p4166752511"></a><a name="zh-cn_topic_0225568815_p4166752511"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row1618417512511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p719835852"><a name="zh-cn_topic_0225568815_p719835852"></a><a name="zh-cn_topic_0225568815_p719835852"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p16224185456"><a name="zh-cn_topic_0225568815_p16224185456"></a><a name="zh-cn_topic_0225568815_p16224185456"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p102391557519"><a name="zh-cn_topic_0225568815_p102391557519"></a><a name="zh-cn_topic_0225568815_p102391557519"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row82501551858"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1796083474"><a name="zh-cn_topic_0225568815_p1796083474"></a><a name="zh-cn_topic_0225568815_p1796083474"></a>condition_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p18804202017712"><a name="zh-cn_topic_0225568815_p18804202017712"></a><a name="zh-cn_topic_0225568815_p18804202017712"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p382342012717"><a name="zh-cn_topic_0225568815_p382342012717"></a><a name="zh-cn_topic_0225568815_p382342012717"></a>策略条件</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row123301257513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p181491444714"><a name="zh-cn_topic_0225568815_p181491444714"></a><a name="zh-cn_topic_0225568815_p181491444714"></a>condition_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1492819201073"><a name="zh-cn_topic_0225568815_p1492819201073"></a><a name="zh-cn_topic_0225568815_p1492819201073"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1994462016716"><a name="zh-cn_topic_0225568815_p1994462016716"></a><a name="zh-cn_topic_0225568815_p1994462016716"></a>策略值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1040955655"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p12230841573"><a name="zh-cn_topic_0225568815_p12230841573"></a><a name="zh-cn_topic_0225568815_p12230841573"></a>condition_origin</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p197610207714"><a name="zh-cn_topic_0225568815_p197610207714"></a><a name="zh-cn_topic_0225568815_p197610207714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1999642015720"><a name="zh-cn_topic_0225568815_p1999642015720"></a><a name="zh-cn_topic_0225568815_p1999642015720"></a>策略类型</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1247645451"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p193881741373"><a name="zh-cn_topic_0225568815_p193881741373"></a><a name="zh-cn_topic_0225568815_p193881741373"></a>req_param_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p1575921679"><a name="zh-cn_topic_0225568815_p1575921679"></a><a name="zh-cn_topic_0225568815_p1575921679"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1396172120712"><a name="zh-cn_topic_0225568815_p1396172120712"></a><a name="zh-cn_topic_0225568815_p1396172120712"></a>关联的请求参数对象名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row455495755"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p15751853519"><a name="zh-cn_topic_0225568815_p15751853519"></a><a name="zh-cn_topic_0225568815_p15751853519"></a>req_param_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p10599451451"><a name="zh-cn_topic_0225568815_p10599451451"></a><a name="zh-cn_topic_0225568815_p10599451451"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p5617455515"><a name="zh-cn_topic_0225568815_p5617455515"></a><a name="zh-cn_topic_0225568815_p5617455515"></a>关联的请求参数对象编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row1862912512520"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p176461751659"><a name="zh-cn_topic_0225568815_p176461751659"></a><a name="zh-cn_topic_0225568815_p176461751659"></a>req_param_location</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p146711652057"><a name="zh-cn_topic_0225568815_p146711652057"></a><a name="zh-cn_topic_0225568815_p146711652057"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p869795651"><a name="zh-cn_topic_0225568815_p869795651"></a><a name="zh-cn_topic_0225568815_p869795651"></a>关联的请求参数对象位置</p>
</td>
</tr>
</tbody>
</table>

**表 25**  auth\_opt参数说明

<a name="zh-cn_topic_0225568815_table3296221173715"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row829715213377"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568815_p17297192173718"><a name="zh-cn_topic_0225568815_p17297192173718"></a><a name="zh-cn_topic_0225568815_p17297192173718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568815_p9297821143718"><a name="zh-cn_topic_0225568815_p9297821143718"></a><a name="zh-cn_topic_0225568815_p9297821143718"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568815_p4297152163717"><a name="zh-cn_topic_0225568815_p4297152163717"></a><a name="zh-cn_topic_0225568815_p4297152163717"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row4297421123717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568815_p1848964315375"><a name="zh-cn_topic_0225568815_p1848964315375"></a><a name="zh-cn_topic_0225568815_p1848964315375"></a>app_code_auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568815_p4489164310372"><a name="zh-cn_topic_0225568815_p4489164310372"></a><a name="zh-cn_topic_0225568815_p4489164310372"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568815_p1948934316376"><a name="zh-cn_topic_0225568815_p1948934316376"></a><a name="zh-cn_topic_0225568815_p1948934316376"></a>AppCode简易认证类型</p>
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
  "req_uri": "/test/{tenant_id}",
  "auth_type": "APP",
  "auth_opt": {
    "app_code_auth_type": "HEADER"
  },
  "tags": ["APIG-SN-test", "test"],
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
      "name": "tenant_id",
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
      "name": "tenant_id",
      "location": "QUERY",
      "origin": "REQUEST",
      "value": "tenant_id",
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
  ],
  "policy_https": [{
    "conditions": [{
      "id": "44e03de2351e43a8b18ba9ec1e71d2e9",
      "condition_type": "pattern",
      "condition_value": "^[0-9]$",
      "condition_origin": "param",
      "req_param_name": "project_id",
      "req_param_id": "b60fbcb5b86f4f5c8705c445b9sda325",
      "req_param_location": "PATH"
    }],
    "backend_params": [{
      "name": "project_id",
      "value": "bbbb",
      "location": "QUERY",
      "origin": "REQUEST",
      "id": "44e03de2351e43a8b18ba9ec1e71d2e8",
      "req_param_id": "593c5560e0924e00af08fb458f850ecb"
    }],
    "effect_mode": "ANY",
    "id": "44e03de2351e43a8b18ba9ec1e71d2e8",
    "name": "policy001",
    "req_method": "GET",
    "req_protocol": "http",
    "req_uri": "/test/policy",
    "timeout": 10000,
    "url_domain": "xxxxxxxxxxx",
    "vpc_status": 2
  }]
}
```

## 状态码<a name="zh-cn_topic_0225568815_section27584683"></a>

**表 26**  返回消息说明

<a name="zh-cn_topic_0225568815_table64322236"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568815_row3387693"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568815_p5967751"><a name="zh-cn_topic_0225568815_p5967751"></a><a name="zh-cn_topic_0225568815_p5967751"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568815_p13625850"><a name="zh-cn_topic_0225568815_p13625850"></a><a name="zh-cn_topic_0225568815_p13625850"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568815_row29952045"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568815_p10196552"><a name="zh-cn_topic_0225568815_p10196552"></a><a name="zh-cn_topic_0225568815_p10196552"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568815_p73578115452"><a name="zh-cn_topic_0225568815_p73578115452"></a><a name="zh-cn_topic_0225568815_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row51311768"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568815_p62612511"><a name="zh-cn_topic_0225568815_p62612511"></a><a name="zh-cn_topic_0225568815_p62612511"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568815_p38448651"><a name="zh-cn_topic_0225568815_p38448651"></a><a name="zh-cn_topic_0225568815_p38448651"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row10493547"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568815_p44670953"><a name="zh-cn_topic_0225568815_p44670953"></a><a name="zh-cn_topic_0225568815_p44670953"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568815_p9203142078"><a name="zh-cn_topic_0225568815_p9203142078"></a><a name="zh-cn_topic_0225568815_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row17325755"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568815_p61208905"><a name="zh-cn_topic_0225568815_p61208905"></a><a name="zh-cn_topic_0225568815_p61208905"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568815_p13949586"><a name="zh-cn_topic_0225568815_p13949586"></a><a name="zh-cn_topic_0225568815_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row61006437"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568815_p42574382"><a name="zh-cn_topic_0225568815_p42574382"></a><a name="zh-cn_topic_0225568815_p42574382"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568815_p25972887"><a name="zh-cn_topic_0225568815_p25972887"></a><a name="zh-cn_topic_0225568815_p25972887"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568815_row32429391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568815_p9534987"><a name="zh-cn_topic_0225568815_p9534987"></a><a name="zh-cn_topic_0225568815_p9534987"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568815_p14947689"><a name="zh-cn_topic_0225568815_p14947689"></a><a name="zh-cn_topic_0225568815_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

