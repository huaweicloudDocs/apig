# 创建流控策略<a name="ZH-CN_TOPIC_0000001081837355"></a>

## 功能介绍<a name="zh-cn_topic_0225568861_section20764951"></a>

当API上线后，系统会默认给每个API提供一个流控策略，API提供者可以根据自身API的服务能力及负载情况变更这个流控策略。

流控策略即限制API在一定长度的时间内，能够允许被访问的最大次数。

## URI<a name="zh-cn_topic_0225568861_section52666834"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568861_table44188448"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568861_row14412546"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568861_p26565558"><a name="zh-cn_topic_0225568861_p26565558"></a><a name="zh-cn_topic_0225568861_p26565558"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568861_p4326583"><a name="zh-cn_topic_0225568861_p4326583"></a><a name="zh-cn_topic_0225568861_p4326583"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568861_row14908908"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568861_p66770877"><a name="zh-cn_topic_0225568861_p66770877"></a><a name="zh-cn_topic_0225568861_p66770877"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568861_p39731988"><a name="zh-cn_topic_0225568861_p39731988"></a><a name="zh-cn_topic_0225568861_p39731988"></a>/v1/{project_id}/apigw/instances/{instance_id}/throttles</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568861_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568861_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568861_p23103637"><a name="zh-cn_topic_0225568861_p23103637"></a><a name="zh-cn_topic_0225568861_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568861_p59455291"><a name="zh-cn_topic_0225568861_p59455291"></a><a name="zh-cn_topic_0225568861_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568861_p51149303"><a name="zh-cn_topic_0225568861_p51149303"></a><a name="zh-cn_topic_0225568861_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568861_p49452846"><a name="zh-cn_topic_0225568861_p49452846"></a><a name="zh-cn_topic_0225568861_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568861_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p55878963"><a name="zh-cn_topic_0225568861_p55878963"></a><a name="zh-cn_topic_0225568861_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p29902160"><a name="zh-cn_topic_0225568861_p29902160"></a><a name="zh-cn_topic_0225568861_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p6155914"><a name="zh-cn_topic_0225568861_p6155914"></a><a name="zh-cn_topic_0225568861_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p28867016"><a name="zh-cn_topic_0225568861_p28867016"></a><a name="zh-cn_topic_0225568861_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p1780913159538"><a name="zh-cn_topic_0225568861_p1780913159538"></a><a name="zh-cn_topic_0225568861_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p9809215115310"><a name="zh-cn_topic_0225568861_p9809215115310"></a><a name="zh-cn_topic_0225568861_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p1280914152538"><a name="zh-cn_topic_0225568861_p1280914152538"></a><a name="zh-cn_topic_0225568861_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p1880914157537"><a name="zh-cn_topic_0225568861_p1880914157537"></a><a name="zh-cn_topic_0225568861_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568861_section4239459"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568861_table64174422"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568861_row65905982"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568861_p36784311"><a name="zh-cn_topic_0225568861_p36784311"></a><a name="zh-cn_topic_0225568861_p36784311"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="11.110000000000001%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568861_p26739213"><a name="zh-cn_topic_0225568861_p26739213"></a><a name="zh-cn_topic_0225568861_p26739213"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="27.46%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568861_p18392615"><a name="zh-cn_topic_0225568861_p18392615"></a><a name="zh-cn_topic_0225568861_p18392615"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.26%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568861_p13406829"><a name="zh-cn_topic_0225568861_p13406829"></a><a name="zh-cn_topic_0225568861_p13406829"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568861_row12211401"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p49599392"><a name="zh-cn_topic_0225568861_p49599392"></a><a name="zh-cn_topic_0225568861_p49599392"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p58127836"><a name="zh-cn_topic_0225568861_p58127836"></a><a name="zh-cn_topic_0225568861_p58127836"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p10734309"><a name="zh-cn_topic_0225568861_p10734309"></a><a name="zh-cn_topic_0225568861_p10734309"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p64172706"><a name="zh-cn_topic_0225568861_p64172706"></a><a name="zh-cn_topic_0225568861_p64172706"></a>流控策略名称。</p>
<p id="zh-cn_topic_0225568861_p7024991"><a name="zh-cn_topic_0225568861_p7024991"></a><a name="zh-cn_topic_0225568861_p7024991"></a>支持汉字，英文，数字，下划线，且只能以英文和汉字开头，3 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0225568861_note1155910113419"><a name="zh-cn_topic_0225568861_note1155910113419"></a><a name="zh-cn_topic_0225568861_note1155910113419"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568861_p1559011141"><a name="zh-cn_topic_0225568861_p1559011141"></a><a name="zh-cn_topic_0225568861_p1559011141"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row48701856"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p52536224"><a name="zh-cn_topic_0225568861_p52536224"></a><a name="zh-cn_topic_0225568861_p52536224"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p27575724"><a name="zh-cn_topic_0225568861_p27575724"></a><a name="zh-cn_topic_0225568861_p27575724"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p19041197"><a name="zh-cn_topic_0225568861_p19041197"></a><a name="zh-cn_topic_0225568861_p19041197"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p65942027"><a name="zh-cn_topic_0225568861_p65942027"></a><a name="zh-cn_topic_0225568861_p65942027"></a>API流量限制是指时长内一个API能够被访问的次数上限。该值不超过系统默认配额限制，系统默认配额为200tps，用户可根据实际情况修改该系统默认配额。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row21791516"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p20282335"><a name="zh-cn_topic_0225568861_p20282335"></a><a name="zh-cn_topic_0225568861_p20282335"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p32256476"><a name="zh-cn_topic_0225568861_p32256476"></a><a name="zh-cn_topic_0225568861_p32256476"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p62637753"><a name="zh-cn_topic_0225568861_p62637753"></a><a name="zh-cn_topic_0225568861_p62637753"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p40493214"><a name="zh-cn_topic_0225568861_p40493214"></a><a name="zh-cn_topic_0225568861_p40493214"></a>用户流量限制是指一个API在时长之内每一个用户能访问的次数上限，该数值不超过API流量限制值。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row58762201"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p62117818"><a name="zh-cn_topic_0225568861_p62117818"></a><a name="zh-cn_topic_0225568861_p62117818"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p65487393"><a name="zh-cn_topic_0225568861_p65487393"></a><a name="zh-cn_topic_0225568861_p65487393"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p2878579"><a name="zh-cn_topic_0225568861_p2878579"></a><a name="zh-cn_topic_0225568861_p2878579"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p31838362"><a name="zh-cn_topic_0225568861_p31838362"></a><a name="zh-cn_topic_0225568861_p31838362"></a>APP流量限制是指一个API在时长之内被每个APP访问的次数上限，该数值不超过用户流量限制值。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row1415542572716"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p787433222711"><a name="zh-cn_topic_0225568861_p787433222711"></a><a name="zh-cn_topic_0225568861_p787433222711"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p787443219272"><a name="zh-cn_topic_0225568861_p787443219272"></a><a name="zh-cn_topic_0225568861_p787443219272"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p288943212278"><a name="zh-cn_topic_0225568861_p288943212278"></a><a name="zh-cn_topic_0225568861_p288943212278"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p18889193272718"><a name="zh-cn_topic_0225568861_p18889193272718"></a><a name="zh-cn_topic_0225568861_p18889193272718"></a>源IP流量限制是指一个API在时长之内被每个IP访问的次数上限，该数值不超过API流量限制值。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row57608434"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p35771579"><a name="zh-cn_topic_0225568861_p35771579"></a><a name="zh-cn_topic_0225568861_p35771579"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p11816821"><a name="zh-cn_topic_0225568861_p11816821"></a><a name="zh-cn_topic_0225568861_p11816821"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p17638472"><a name="zh-cn_topic_0225568861_p17638472"></a><a name="zh-cn_topic_0225568861_p17638472"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p19430107"><a name="zh-cn_topic_0225568861_p19430107"></a><a name="zh-cn_topic_0225568861_p19430107"></a>流量控制的时长单位。与“流量限制次数”配合使用，表示单位时间内的API请求次数上限。输入的值不超过2147483647。正整数。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row4577802"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p35257718"><a name="zh-cn_topic_0225568861_p35257718"></a><a name="zh-cn_topic_0225568861_p35257718"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p37302877"><a name="zh-cn_topic_0225568861_p37302877"></a><a name="zh-cn_topic_0225568861_p37302877"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p1634217"><a name="zh-cn_topic_0225568861_p1634217"></a><a name="zh-cn_topic_0225568861_p1634217"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p65262786"><a name="zh-cn_topic_0225568861_p65262786"></a><a name="zh-cn_topic_0225568861_p65262786"></a>流控的时间单位：</p>
<a name="zh-cn_topic_0225568861_ul50353255"></a><a name="zh-cn_topic_0225568861_ul50353255"></a><ul id="zh-cn_topic_0225568861_ul50353255"><li>SECOND</li><li>MINUTE</li><li>HOUR</li><li>DAY</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row51166460"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p50842565"><a name="zh-cn_topic_0225568861_p50842565"></a><a name="zh-cn_topic_0225568861_p50842565"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p24607062"><a name="zh-cn_topic_0225568861_p24607062"></a><a name="zh-cn_topic_0225568861_p24607062"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p47015000"><a name="zh-cn_topic_0225568861_p47015000"></a><a name="zh-cn_topic_0225568861_p47015000"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p50118642"><a name="zh-cn_topic_0225568861_p50118642"></a><a name="zh-cn_topic_0225568861_p50118642"></a>流控策略描述</p>
<p id="zh-cn_topic_0225568861_p29268538"><a name="zh-cn_topic_0225568861_p29268538"></a><a name="zh-cn_topic_0225568861_p29268538"></a>字符长度不超过255。</p>
<div class="note" id="zh-cn_topic_0225568861_note670734010419"><a name="zh-cn_topic_0225568861_note670734010419"></a><a name="zh-cn_topic_0225568861_note670734010419"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568861_p6707240049"><a name="zh-cn_topic_0225568861_p6707240049"></a><a name="zh-cn_topic_0225568861_p6707240049"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row9409521748"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p134091124420"><a name="zh-cn_topic_0225568861_p134091124420"></a><a name="zh-cn_topic_0225568861_p134091124420"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p14091327416"><a name="zh-cn_topic_0225568861_p14091327416"></a><a name="zh-cn_topic_0225568861_p14091327416"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p64091925413"><a name="zh-cn_topic_0225568861_p64091925413"></a><a name="zh-cn_topic_0225568861_p64091925413"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p15805453105915"><a name="zh-cn_topic_0225568861_p15805453105915"></a><a name="zh-cn_topic_0225568861_p15805453105915"></a>流控策略的类型，取值如下：</p>
<a name="zh-cn_topic_0225568861_ul1043012241502"></a><a name="zh-cn_topic_0225568861_ul1043012241502"></a><ul id="zh-cn_topic_0225568861_ul1043012241502"><li>1：独享，表示绑定到流控策略的单个API流控时间内能够被调用多少次。</li><li>2：共享，表示绑定到流控策略的所有API流控时间内能够被调用多少次。</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row18816116144517"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568861_p189261354175913"><a name="zh-cn_topic_0225568861_p189261354175913"></a><a name="zh-cn_topic_0225568861_p189261354175913"></a>enable_adaptive_control</p>
</td>
<td class="cellrowborder" valign="top" width="11.110000000000001%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568861_p792615541592"><a name="zh-cn_topic_0225568861_p792615541592"></a><a name="zh-cn_topic_0225568861_p792615541592"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="27.46%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568861_p15926654165919"><a name="zh-cn_topic_0225568861_p15926654165919"></a><a name="zh-cn_topic_0225568861_p15926654165919"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568861_p173718104565"><a name="zh-cn_topic_0225568861_p173718104565"></a><a name="zh-cn_topic_0225568861_p173718104565"></a>是否开启动态流控：</p>
<a name="zh-cn_topic_0225568861_ul173711210185620"></a><a name="zh-cn_topic_0225568861_ul173711210185620"></a><ul id="zh-cn_topic_0225568861_ul173711210185620"><li>TRUE</li><li>FALSE</li></ul>
<p id="zh-cn_topic_0225568861_p209261544595"><a name="zh-cn_topic_0225568861_p209261544595"></a><a name="zh-cn_topic_0225568861_p209261544595"></a>暂不支持</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"api_call_limits": 800,
	"user_call_limits": 500,
	"app_call_limits": 300,
        "ip_call_limits": 600,
	"name": "每秒800次",
	"remark": "API每秒800次，用户500次，APP300次，IP600次",
	"time_interval": 1,
	"time_unit": "SECOND"
}
```

## 响应消息<a name="zh-cn_topic_0225568861_section7851859"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568861_table25797343"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568861_row59012107"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568861_p15251357"><a name="zh-cn_topic_0225568861_p15251357"></a><a name="zh-cn_topic_0225568861_p15251357"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568861_p27400391"><a name="zh-cn_topic_0225568861_p27400391"></a><a name="zh-cn_topic_0225568861_p27400391"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568861_p4839218"><a name="zh-cn_topic_0225568861_p4839218"></a><a name="zh-cn_topic_0225568861_p4839218"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568861_row56432390"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p7620841"><a name="zh-cn_topic_0225568861_p7620841"></a><a name="zh-cn_topic_0225568861_p7620841"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p13308422"><a name="zh-cn_topic_0225568861_p13308422"></a><a name="zh-cn_topic_0225568861_p13308422"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p4240387"><a name="zh-cn_topic_0225568861_p4240387"></a><a name="zh-cn_topic_0225568861_p4240387"></a>流控策略的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row38163485"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p4234574"><a name="zh-cn_topic_0225568861_p4234574"></a><a name="zh-cn_topic_0225568861_p4234574"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p7456179"><a name="zh-cn_topic_0225568861_p7456179"></a><a name="zh-cn_topic_0225568861_p7456179"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p67079604"><a name="zh-cn_topic_0225568861_p67079604"></a><a name="zh-cn_topic_0225568861_p67079604"></a>流控策略的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row66845531"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p45778963"><a name="zh-cn_topic_0225568861_p45778963"></a><a name="zh-cn_topic_0225568861_p45778963"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p17108507"><a name="zh-cn_topic_0225568861_p17108507"></a><a name="zh-cn_topic_0225568861_p17108507"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p43611803"><a name="zh-cn_topic_0225568861_p43611803"></a><a name="zh-cn_topic_0225568861_p43611803"></a>单个API流控时间内能够被访问的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row56961912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p50512160"><a name="zh-cn_topic_0225568861_p50512160"></a><a name="zh-cn_topic_0225568861_p50512160"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p64953173"><a name="zh-cn_topic_0225568861_p64953173"></a><a name="zh-cn_topic_0225568861_p64953173"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p26715646"><a name="zh-cn_topic_0225568861_p26715646"></a><a name="zh-cn_topic_0225568861_p26715646"></a>单个用户流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row39114226"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p14135717"><a name="zh-cn_topic_0225568861_p14135717"></a><a name="zh-cn_topic_0225568861_p14135717"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p4142400"><a name="zh-cn_topic_0225568861_p4142400"></a><a name="zh-cn_topic_0225568861_p4142400"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p67098988"><a name="zh-cn_topic_0225568861_p67098988"></a><a name="zh-cn_topic_0225568861_p67098988"></a>单个APP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row145194716337"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p71235716345"><a name="zh-cn_topic_0225568861_p71235716345"></a><a name="zh-cn_topic_0225568861_p71235716345"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p612135773413"><a name="zh-cn_topic_0225568861_p612135773413"></a><a name="zh-cn_topic_0225568861_p612135773413"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p12122573347"><a name="zh-cn_topic_0225568861_p12122573347"></a><a name="zh-cn_topic_0225568861_p12122573347"></a>单个IP流控时间内能够访问API的次数限制</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row67019984"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p59909591"><a name="zh-cn_topic_0225568861_p59909591"></a><a name="zh-cn_topic_0225568861_p59909591"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p20838723"><a name="zh-cn_topic_0225568861_p20838723"></a><a name="zh-cn_topic_0225568861_p20838723"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p10215036"><a name="zh-cn_topic_0225568861_p10215036"></a><a name="zh-cn_topic_0225568861_p10215036"></a>流控的时长</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row24826465"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p64786615"><a name="zh-cn_topic_0225568861_p64786615"></a><a name="zh-cn_topic_0225568861_p64786615"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p13224462"><a name="zh-cn_topic_0225568861_p13224462"></a><a name="zh-cn_topic_0225568861_p13224462"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p64548493"><a name="zh-cn_topic_0225568861_p64548493"></a><a name="zh-cn_topic_0225568861_p64548493"></a>流控的时间单位</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row44065532"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p12538315"><a name="zh-cn_topic_0225568861_p12538315"></a><a name="zh-cn_topic_0225568861_p12538315"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p8970583"><a name="zh-cn_topic_0225568861_p8970583"></a><a name="zh-cn_topic_0225568861_p8970583"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p55528583"><a name="zh-cn_topic_0225568861_p55528583"></a><a name="zh-cn_topic_0225568861_p55528583"></a>描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row29995200"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p13692130"><a name="zh-cn_topic_0225568861_p13692130"></a><a name="zh-cn_topic_0225568861_p13692130"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p35320732"><a name="zh-cn_topic_0225568861_p35320732"></a><a name="zh-cn_topic_0225568861_p35320732"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p42407063"><a name="zh-cn_topic_0225568861_p42407063"></a><a name="zh-cn_topic_0225568861_p42407063"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row46119252"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p44671955"><a name="zh-cn_topic_0225568861_p44671955"></a><a name="zh-cn_topic_0225568861_p44671955"></a>is_include_special_throttle</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p61658598"><a name="zh-cn_topic_0225568861_p61658598"></a><a name="zh-cn_topic_0225568861_p61658598"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p191931644142414"><a name="zh-cn_topic_0225568861_p191931644142414"></a><a name="zh-cn_topic_0225568861_p191931644142414"></a>是否包含特殊流控配置：</p>
<a name="zh-cn_topic_0225568861_ul107800420518"></a><a name="zh-cn_topic_0225568861_ul107800420518"></a><ul id="zh-cn_topic_0225568861_ul107800420518"><li>1：包含</li><li>2：不包含</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row9948932860"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p89481832869"><a name="zh-cn_topic_0225568861_p89481832869"></a><a name="zh-cn_topic_0225568861_p89481832869"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p29484325618"><a name="zh-cn_topic_0225568861_p29484325618"></a><a name="zh-cn_topic_0225568861_p29484325618"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p19018411067"><a name="zh-cn_topic_0225568861_p19018411067"></a><a name="zh-cn_topic_0225568861_p19018411067"></a>流控策略的类型，取值如下：</p>
<a name="zh-cn_topic_0225568861_ul129012411663"></a><a name="zh-cn_topic_0225568861_ul129012411663"></a><ul id="zh-cn_topic_0225568861_ul129012411663"><li>1：独享</li><li>2：共享</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row179111394718"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p14797139472"><a name="zh-cn_topic_0225568861_p14797139472"></a><a name="zh-cn_topic_0225568861_p14797139472"></a>bind_num</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p147913137471"><a name="zh-cn_topic_0225568861_p147913137471"></a><a name="zh-cn_topic_0225568861_p147913137471"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p11798139474"><a name="zh-cn_topic_0225568861_p11798139474"></a><a name="zh-cn_topic_0225568861_p11798139474"></a>流控绑定的API数量</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row127701016204716"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568861_p19770121614477"><a name="zh-cn_topic_0225568861_p19770121614477"></a><a name="zh-cn_topic_0225568861_p19770121614477"></a>enable_adaptive_control</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568861_p27566352475"><a name="zh-cn_topic_0225568861_p27566352475"></a><a name="zh-cn_topic_0225568861_p27566352475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568861_p13499124885712"><a name="zh-cn_topic_0225568861_p13499124885712"></a><a name="zh-cn_topic_0225568861_p13499124885712"></a>是否开启动态流控：</p>
<a name="zh-cn_topic_0225568861_ul349924895712"></a><a name="zh-cn_topic_0225568861_ul349924895712"></a><ul id="zh-cn_topic_0225568861_ul349924895712"><li>TRUE</li><li>FALSE</li></ul>
<p id="zh-cn_topic_0225568861_p549964814575"><a name="zh-cn_topic_0225568861_p549964814575"></a><a name="zh-cn_topic_0225568861_p549964814575"></a>暂不支持</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "0325b671-2d50-4614-9868-22102262695d",
	"name": "每秒800次",
	"api_call_limits": 800,
	"user_call_limits": 500,
	"app_call_limits": 300,
        "ip_call_limits": 600,
	"time_interval": 1,
	"time_unit": "SECOND",
	"create_time": "2017-12-29T01:55:59.9904225Z",
	"remark": "API每秒800次，用户500次，APP300次，IP600次",
	"is_inclu_special_throttle": 2,
        "type":1,
	"bind_num": 0,
        "enable_adaptive_control": "FALSE"
}
```

## 状态码<a name="zh-cn_topic_0225568861_section38155131"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568861_table17723792"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568861_row9500439"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568861_p31338096"><a name="zh-cn_topic_0225568861_p31338096"></a><a name="zh-cn_topic_0225568861_p31338096"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568861_p55357882"><a name="zh-cn_topic_0225568861_p55357882"></a><a name="zh-cn_topic_0225568861_p55357882"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568861_row54803485"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568861_p9897280"><a name="zh-cn_topic_0225568861_p9897280"></a><a name="zh-cn_topic_0225568861_p9897280"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568861_p63482187"><a name="zh-cn_topic_0225568861_p63482187"></a><a name="zh-cn_topic_0225568861_p63482187"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row34468775"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568861_p40507427"><a name="zh-cn_topic_0225568861_p40507427"></a><a name="zh-cn_topic_0225568861_p40507427"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568861_p59876122"><a name="zh-cn_topic_0225568861_p59876122"></a><a name="zh-cn_topic_0225568861_p59876122"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row2014192"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568861_p28931886"><a name="zh-cn_topic_0225568861_p28931886"></a><a name="zh-cn_topic_0225568861_p28931886"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568861_p61781404"><a name="zh-cn_topic_0225568861_p61781404"></a><a name="zh-cn_topic_0225568861_p61781404"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568861_row19161724"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568861_p8595830"><a name="zh-cn_topic_0225568861_p8595830"></a><a name="zh-cn_topic_0225568861_p8595830"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568861_p14947689"><a name="zh-cn_topic_0225568861_p14947689"></a><a name="zh-cn_topic_0225568861_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

