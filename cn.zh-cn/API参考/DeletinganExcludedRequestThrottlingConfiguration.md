# 删除特殊设置<a name="ZH-CN_TOPIC_0000001081837293"></a>

## 功能介绍<a name="zh-cn_topic_0118922272_section45779418"></a>

删除某个流控策略的某个特殊配置。

## URI<a name="zh-cn_topic_0118922272_section9361583"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118922272_table33128920"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922272_row56178382"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922272_p54155073"><a name="zh-cn_topic_0118922272_p54155073"></a><a name="zh-cn_topic_0118922272_p54155073"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922272_p24484764"><a name="zh-cn_topic_0118922272_p24484764"></a><a name="zh-cn_topic_0118922272_p24484764"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922272_row37108872"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922272_p53028652"><a name="zh-cn_topic_0118922272_p53028652"></a><a name="zh-cn_topic_0118922272_p53028652"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922272_p353585"><a name="zh-cn_topic_0118922272_p353585"></a><a name="zh-cn_topic_0118922272_p353585"></a>/v1.0/apigw/throttle-specials/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118922272_table28640447"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922272_row64277225"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118922272_p39072761"><a name="zh-cn_topic_0118922272_p39072761"></a><a name="zh-cn_topic_0118922272_p39072761"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118922272_p10777090"><a name="zh-cn_topic_0118922272_p10777090"></a><a name="zh-cn_topic_0118922272_p10777090"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118922272_p529067"><a name="zh-cn_topic_0118922272_p529067"></a><a name="zh-cn_topic_0118922272_p529067"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118922272_p42854428"><a name="zh-cn_topic_0118922272_p42854428"></a><a name="zh-cn_topic_0118922272_p42854428"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922272_row48656638"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118922272_p48873592"><a name="zh-cn_topic_0118922272_p48873592"></a><a name="zh-cn_topic_0118922272_p48873592"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118922272_p66446899"><a name="zh-cn_topic_0118922272_p66446899"></a><a name="zh-cn_topic_0118922272_p66446899"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118922272_p13489751"><a name="zh-cn_topic_0118922272_p13489751"></a><a name="zh-cn_topic_0118922272_p13489751"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118922272_p18928010"><a name="zh-cn_topic_0118922272_p18928010"></a><a name="zh-cn_topic_0118922272_p18928010"></a>特殊配置的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118922272_section17145384"></a>

无

## 响应消息<a name="zh-cn_topic_0118922272_section46598903"></a>

无

## 状态码<a name="zh-cn_topic_0118922272_section20090736"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118922272_table35281476"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118922272_row8318108"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118922272_p2678125"><a name="zh-cn_topic_0118922272_p2678125"></a><a name="zh-cn_topic_0118922272_p2678125"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118922272_p15601604"><a name="zh-cn_topic_0118922272_p15601604"></a><a name="zh-cn_topic_0118922272_p15601604"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118922272_row55770374"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922272_p21106461"><a name="zh-cn_topic_0118922272_p21106461"></a><a name="zh-cn_topic_0118922272_p21106461"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922272_p31901809"><a name="zh-cn_topic_0118922272_p31901809"></a><a name="zh-cn_topic_0118922272_p31901809"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922272_row18680829"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922272_p36752182"><a name="zh-cn_topic_0118922272_p36752182"></a><a name="zh-cn_topic_0118922272_p36752182"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922272_p439515463618"><a name="zh-cn_topic_0118922272_p439515463618"></a><a name="zh-cn_topic_0118922272_p439515463618"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922272_row15904615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922272_p13205437"><a name="zh-cn_topic_0118922272_p13205437"></a><a name="zh-cn_topic_0118922272_p13205437"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922272_p63007447"><a name="zh-cn_topic_0118922272_p63007447"></a><a name="zh-cn_topic_0118922272_p63007447"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922272_row30196113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922272_p29966093"><a name="zh-cn_topic_0118922272_p29966093"></a><a name="zh-cn_topic_0118922272_p29966093"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922272_p11334465"><a name="zh-cn_topic_0118922272_p11334465"></a><a name="zh-cn_topic_0118922272_p11334465"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922272_row34901328"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922272_p8435340"><a name="zh-cn_topic_0118922272_p8435340"></a><a name="zh-cn_topic_0118922272_p8435340"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922272_p17426130177"><a name="zh-cn_topic_0118922272_p17426130177"></a><a name="zh-cn_topic_0118922272_p17426130177"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118922272_row42456898"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118922272_p16456680"><a name="zh-cn_topic_0118922272_p16456680"></a><a name="zh-cn_topic_0118922272_p16456680"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118922272_p6744143"><a name="zh-cn_topic_0118922272_p6744143"></a><a name="zh-cn_topic_0118922272_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

