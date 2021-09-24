# 对象模型<a name="ZH-CN_TOPIC_0000001082135185"></a>

本节介绍流控策略的对象模型，如下表所示：

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   “操作类型”用于描述字段的属性，表示对应字段的值可进行的操作：
>    C：创建；U：更新；R：读取。
>-   “是否必选”列表示对于“操作类型”为“C”的创建操作，对应字段是否为必选字段。

**表 1**  流控对象模型

<a name="zh-cn_topic_0225568860_table5855399"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568860_row55841878"><th class="cellrowborder" valign="top" width="20.202020202020204%" id="mcps1.2.6.1.1"><p id="zh-cn_topic_0225568860_p26898301"><a name="zh-cn_topic_0225568860_p26898301"></a><a name="zh-cn_topic_0225568860_p26898301"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18181818181818%" id="mcps1.2.6.1.2"><p id="zh-cn_topic_0225568860_p31278735"><a name="zh-cn_topic_0225568860_p31278735"></a><a name="zh-cn_topic_0225568860_p31278735"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.6.1.3"><p id="zh-cn_topic_0225568860_p50549622"><a name="zh-cn_topic_0225568860_p50549622"></a><a name="zh-cn_topic_0225568860_p50549622"></a>说明</p>
</th>
<th class="cellrowborder" valign="top" width="17.17171717171717%" id="mcps1.2.6.1.4"><p id="zh-cn_topic_0225568860_p878746"><a name="zh-cn_topic_0225568860_p878746"></a><a name="zh-cn_topic_0225568860_p878746"></a>操作类型</p>
</th>
<th class="cellrowborder" valign="top" width="11.111111111111112%" id="mcps1.2.6.1.5"><p id="zh-cn_topic_0225568860_p4069602"><a name="zh-cn_topic_0225568860_p4069602"></a><a name="zh-cn_topic_0225568860_p4069602"></a>是否必选</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568860_row61202359"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p58444032"><a name="zh-cn_topic_0225568860_p58444032"></a><a name="zh-cn_topic_0225568860_p58444032"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p36346150"><a name="zh-cn_topic_0225568860_p36346150"></a><a name="zh-cn_topic_0225568860_p36346150"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p58357008"><a name="zh-cn_topic_0225568860_p58357008"></a><a name="zh-cn_topic_0225568860_p58357008"></a>流控策略的编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p29297190"><a name="zh-cn_topic_0225568860_p29297190"></a><a name="zh-cn_topic_0225568860_p29297190"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p24262226"><a name="zh-cn_topic_0225568860_p24262226"></a><a name="zh-cn_topic_0225568860_p24262226"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row17033442"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p37531591"><a name="zh-cn_topic_0225568860_p37531591"></a><a name="zh-cn_topic_0225568860_p37531591"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p20160053"><a name="zh-cn_topic_0225568860_p20160053"></a><a name="zh-cn_topic_0225568860_p20160053"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p22351571"><a name="zh-cn_topic_0225568860_p22351571"></a><a name="zh-cn_topic_0225568860_p22351571"></a>流控策略的名称</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p65646793"><a name="zh-cn_topic_0225568860_p65646793"></a><a name="zh-cn_topic_0225568860_p65646793"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p15790016"><a name="zh-cn_topic_0225568860_p15790016"></a><a name="zh-cn_topic_0225568860_p15790016"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row7892419"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p35306206"><a name="zh-cn_topic_0225568860_p35306206"></a><a name="zh-cn_topic_0225568860_p35306206"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p41230413"><a name="zh-cn_topic_0225568860_p41230413"></a><a name="zh-cn_topic_0225568860_p41230413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p51329145"><a name="zh-cn_topic_0225568860_p51329145"></a><a name="zh-cn_topic_0225568860_p51329145"></a>流控策略创建者的租户编号</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p64020041"><a name="zh-cn_topic_0225568860_p64020041"></a><a name="zh-cn_topic_0225568860_p64020041"></a>-</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p18240805"><a name="zh-cn_topic_0225568860_p18240805"></a><a name="zh-cn_topic_0225568860_p18240805"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row29949524"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p9992366"><a name="zh-cn_topic_0225568860_p9992366"></a><a name="zh-cn_topic_0225568860_p9992366"></a>api_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p4075337"><a name="zh-cn_topic_0225568860_p4075337"></a><a name="zh-cn_topic_0225568860_p4075337"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p61666893"><a name="zh-cn_topic_0225568860_p61666893"></a><a name="zh-cn_topic_0225568860_p61666893"></a>单个API流控时间内能够被访问的最大次数</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p28962400"><a name="zh-cn_topic_0225568860_p28962400"></a><a name="zh-cn_topic_0225568860_p28962400"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p64253101"><a name="zh-cn_topic_0225568860_p64253101"></a><a name="zh-cn_topic_0225568860_p64253101"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row41407000"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p65632684"><a name="zh-cn_topic_0225568860_p65632684"></a><a name="zh-cn_topic_0225568860_p65632684"></a>user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p14647181"><a name="zh-cn_topic_0225568860_p14647181"></a><a name="zh-cn_topic_0225568860_p14647181"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p45570978"><a name="zh-cn_topic_0225568860_p45570978"></a><a name="zh-cn_topic_0225568860_p45570978"></a>单个用户流控时间内能够访问的最大次数，遵循api_call_limits&gt;=user_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p261715"><a name="zh-cn_topic_0225568860_p261715"></a><a name="zh-cn_topic_0225568860_p261715"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p21198986"><a name="zh-cn_topic_0225568860_p21198986"></a><a name="zh-cn_topic_0225568860_p21198986"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row56573146"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p19022098"><a name="zh-cn_topic_0225568860_p19022098"></a><a name="zh-cn_topic_0225568860_p19022098"></a>app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p64394946"><a name="zh-cn_topic_0225568860_p64394946"></a><a name="zh-cn_topic_0225568860_p64394946"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p48608147"><a name="zh-cn_topic_0225568860_p48608147"></a><a name="zh-cn_topic_0225568860_p48608147"></a>单个APP流控时间内能个访问的最大次数，遵循user_call_limits&gt;=app_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p44945836"><a name="zh-cn_topic_0225568860_p44945836"></a><a name="zh-cn_topic_0225568860_p44945836"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p16734134"><a name="zh-cn_topic_0225568860_p16734134"></a><a name="zh-cn_topic_0225568860_p16734134"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row85441521162618"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p4949162532613"><a name="zh-cn_topic_0225568860_p4949162532613"></a><a name="zh-cn_topic_0225568860_p4949162532613"></a>ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p69491425182618"><a name="zh-cn_topic_0225568860_p69491425182618"></a><a name="zh-cn_topic_0225568860_p69491425182618"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p3949325102619"><a name="zh-cn_topic_0225568860_p3949325102619"></a><a name="zh-cn_topic_0225568860_p3949325102619"></a>单个源IP流控时间内能个访问的最大次数，遵循api_call_limits&gt;=ip_call_limits</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p2949122592615"><a name="zh-cn_topic_0225568860_p2949122592615"></a><a name="zh-cn_topic_0225568860_p2949122592615"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p59491225102615"><a name="zh-cn_topic_0225568860_p59491225102615"></a><a name="zh-cn_topic_0225568860_p59491225102615"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row16389485"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p52479907"><a name="zh-cn_topic_0225568860_p52479907"></a><a name="zh-cn_topic_0225568860_p52479907"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p23014045"><a name="zh-cn_topic_0225568860_p23014045"></a><a name="zh-cn_topic_0225568860_p23014045"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p52198339"><a name="zh-cn_topic_0225568860_p52198339"></a><a name="zh-cn_topic_0225568860_p52198339"></a>流控时长</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p207103"><a name="zh-cn_topic_0225568860_p207103"></a><a name="zh-cn_topic_0225568860_p207103"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p16775350"><a name="zh-cn_topic_0225568860_p16775350"></a><a name="zh-cn_topic_0225568860_p16775350"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row16760428"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p15417450"><a name="zh-cn_topic_0225568860_p15417450"></a><a name="zh-cn_topic_0225568860_p15417450"></a>time_unit</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p40853912"><a name="zh-cn_topic_0225568860_p40853912"></a><a name="zh-cn_topic_0225568860_p40853912"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p20832542"><a name="zh-cn_topic_0225568860_p20832542"></a><a name="zh-cn_topic_0225568860_p20832542"></a>流控时间单位，取值如下：</p>
<a name="zh-cn_topic_0225568860_ul53275154"></a><a name="zh-cn_topic_0225568860_ul53275154"></a><ul id="zh-cn_topic_0225568860_ul53275154"><li>SECOND</li><li>MINUTE</li><li>HOUR</li><li>DAY</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p42684282"><a name="zh-cn_topic_0225568860_p42684282"></a><a name="zh-cn_topic_0225568860_p42684282"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p34874806"><a name="zh-cn_topic_0225568860_p34874806"></a><a name="zh-cn_topic_0225568860_p34874806"></a>是</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row45437798"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p56582983"><a name="zh-cn_topic_0225568860_p56582983"></a><a name="zh-cn_topic_0225568860_p56582983"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p19818905"><a name="zh-cn_topic_0225568860_p19818905"></a><a name="zh-cn_topic_0225568860_p19818905"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p61827459"><a name="zh-cn_topic_0225568860_p61827459"></a><a name="zh-cn_topic_0225568860_p61827459"></a>流控策略的创建时间</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p41968302"><a name="zh-cn_topic_0225568860_p41968302"></a><a name="zh-cn_topic_0225568860_p41968302"></a>R</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p43989314"><a name="zh-cn_topic_0225568860_p43989314"></a><a name="zh-cn_topic_0225568860_p43989314"></a>-</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row60359506"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p57281813"><a name="zh-cn_topic_0225568860_p57281813"></a><a name="zh-cn_topic_0225568860_p57281813"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p9315285"><a name="zh-cn_topic_0225568860_p9315285"></a><a name="zh-cn_topic_0225568860_p9315285"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p16340601"><a name="zh-cn_topic_0225568860_p16340601"></a><a name="zh-cn_topic_0225568860_p16340601"></a>描述</p>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p48520298"><a name="zh-cn_topic_0225568860_p48520298"></a><a name="zh-cn_topic_0225568860_p48520298"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p37830031"><a name="zh-cn_topic_0225568860_p37830031"></a><a name="zh-cn_topic_0225568860_p37830031"></a>否</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568860_row10805175311599"><td class="cellrowborder" valign="top" width="20.202020202020204%" headers="mcps1.2.6.1.1 "><p id="zh-cn_topic_0225568860_p2805353155913"><a name="zh-cn_topic_0225568860_p2805353155913"></a><a name="zh-cn_topic_0225568860_p2805353155913"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="18.18181818181818%" headers="mcps1.2.6.1.2 "><p id="zh-cn_topic_0225568860_p138057534593"><a name="zh-cn_topic_0225568860_p138057534593"></a><a name="zh-cn_topic_0225568860_p138057534593"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.6.1.3 "><p id="zh-cn_topic_0225568860_p15805453105915"><a name="zh-cn_topic_0225568860_p15805453105915"></a><a name="zh-cn_topic_0225568860_p15805453105915"></a>流控策略的类型，取值如下：</p>
<a name="zh-cn_topic_0225568860_ul1043012241502"></a><a name="zh-cn_topic_0225568860_ul1043012241502"></a><ul id="zh-cn_topic_0225568860_ul1043012241502"><li>1   独享</li><li>2   共享</li></ul>
</td>
<td class="cellrowborder" valign="top" width="17.17171717171717%" headers="mcps1.2.6.1.4 "><p id="zh-cn_topic_0225568860_p5805155314596"><a name="zh-cn_topic_0225568860_p5805155314596"></a><a name="zh-cn_topic_0225568860_p5805155314596"></a>CRU</p>
</td>
<td class="cellrowborder" valign="top" width="11.111111111111112%" headers="mcps1.2.6.1.5 "><p id="zh-cn_topic_0225568860_p880516531592"><a name="zh-cn_topic_0225568860_p880516531592"></a><a name="zh-cn_topic_0225568860_p880516531592"></a>否</p>
</td>
</tr>
</tbody>
</table>

