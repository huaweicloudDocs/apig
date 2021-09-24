# 删除特殊设置<a name="ZH-CN_TOPIC_0000001081837363"></a>

## 功能介绍<a name="zh-cn_topic_0225568879_section45779418"></a>

删除某个流控策略的某个特殊配置。

## URI<a name="zh-cn_topic_0225568879_section9361583"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568879_table33128920"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568879_row56178382"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568879_p54155073"><a name="zh-cn_topic_0225568879_p54155073"></a><a name="zh-cn_topic_0225568879_p54155073"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568879_p24484764"><a name="zh-cn_topic_0225568879_p24484764"></a><a name="zh-cn_topic_0225568879_p24484764"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568879_row37108872"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568879_p53028652"><a name="zh-cn_topic_0225568879_p53028652"></a><a name="zh-cn_topic_0225568879_p53028652"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568879_p353585"><a name="zh-cn_topic_0225568879_p353585"></a><a name="zh-cn_topic_0225568879_p353585"></a>/v1/{project_id}/apigw/instances/{instance_id}/throttle-specials/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568879_table28640447"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568879_row64277225"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568879_p39072761"><a name="zh-cn_topic_0225568879_p39072761"></a><a name="zh-cn_topic_0225568879_p39072761"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.33%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568879_p10777090"><a name="zh-cn_topic_0225568879_p10777090"></a><a name="zh-cn_topic_0225568879_p10777090"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.27%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568879_p529067"><a name="zh-cn_topic_0225568879_p529067"></a><a name="zh-cn_topic_0225568879_p529067"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.4%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568879_p42854428"><a name="zh-cn_topic_0225568879_p42854428"></a><a name="zh-cn_topic_0225568879_p42854428"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568879_row071316329174"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568879_p55878963"><a name="zh-cn_topic_0225568879_p55878963"></a><a name="zh-cn_topic_0225568879_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568879_p29902160"><a name="zh-cn_topic_0225568879_p29902160"></a><a name="zh-cn_topic_0225568879_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.27%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568879_p6155914"><a name="zh-cn_topic_0225568879_p6155914"></a><a name="zh-cn_topic_0225568879_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568879_p28867016"><a name="zh-cn_topic_0225568879_p28867016"></a><a name="zh-cn_topic_0225568879_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568879_row949714325177"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568879_p1780913159538"><a name="zh-cn_topic_0225568879_p1780913159538"></a><a name="zh-cn_topic_0225568879_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568879_p9809215115310"><a name="zh-cn_topic_0225568879_p9809215115310"></a><a name="zh-cn_topic_0225568879_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.27%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568879_p1280914152538"><a name="zh-cn_topic_0225568879_p1280914152538"></a><a name="zh-cn_topic_0225568879_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568879_p1880914157537"><a name="zh-cn_topic_0225568879_p1880914157537"></a><a name="zh-cn_topic_0225568879_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568879_row48656638"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568879_p48873592"><a name="zh-cn_topic_0225568879_p48873592"></a><a name="zh-cn_topic_0225568879_p48873592"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.33%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568879_p66446899"><a name="zh-cn_topic_0225568879_p66446899"></a><a name="zh-cn_topic_0225568879_p66446899"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.27%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568879_p13489751"><a name="zh-cn_topic_0225568879_p13489751"></a><a name="zh-cn_topic_0225568879_p13489751"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.4%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568879_p18928010"><a name="zh-cn_topic_0225568879_p18928010"></a><a name="zh-cn_topic_0225568879_p18928010"></a>特殊配置的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568879_section17145384"></a>

无

## 响应消息<a name="zh-cn_topic_0225568879_section46598903"></a>

无

## 状态码<a name="zh-cn_topic_0225568879_section20090736"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568879_table35281476"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568879_row8318108"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568879_p2678125"><a name="zh-cn_topic_0225568879_p2678125"></a><a name="zh-cn_topic_0225568879_p2678125"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568879_p15601604"><a name="zh-cn_topic_0225568879_p15601604"></a><a name="zh-cn_topic_0225568879_p15601604"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568879_row55770374"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568879_p21106461"><a name="zh-cn_topic_0225568879_p21106461"></a><a name="zh-cn_topic_0225568879_p21106461"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568879_p31901809"><a name="zh-cn_topic_0225568879_p31901809"></a><a name="zh-cn_topic_0225568879_p31901809"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568879_row18680829"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568879_p36752182"><a name="zh-cn_topic_0225568879_p36752182"></a><a name="zh-cn_topic_0225568879_p36752182"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568879_p439515463618"><a name="zh-cn_topic_0225568879_p439515463618"></a><a name="zh-cn_topic_0225568879_p439515463618"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568879_row15904615"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568879_p13205437"><a name="zh-cn_topic_0225568879_p13205437"></a><a name="zh-cn_topic_0225568879_p13205437"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568879_p63007447"><a name="zh-cn_topic_0225568879_p63007447"></a><a name="zh-cn_topic_0225568879_p63007447"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568879_row30196113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568879_p29966093"><a name="zh-cn_topic_0225568879_p29966093"></a><a name="zh-cn_topic_0225568879_p29966093"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568879_p11334465"><a name="zh-cn_topic_0225568879_p11334465"></a><a name="zh-cn_topic_0225568879_p11334465"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568879_row34901328"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568879_p8435340"><a name="zh-cn_topic_0225568879_p8435340"></a><a name="zh-cn_topic_0225568879_p8435340"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568879_p17426130177"><a name="zh-cn_topic_0225568879_p17426130177"></a><a name="zh-cn_topic_0225568879_p17426130177"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568879_row42456898"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568879_p16456680"><a name="zh-cn_topic_0225568879_p16456680"></a><a name="zh-cn_topic_0225568879_p16456680"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568879_p6744143"><a name="zh-cn_topic_0225568879_p6744143"></a><a name="zh-cn_topic_0225568879_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

