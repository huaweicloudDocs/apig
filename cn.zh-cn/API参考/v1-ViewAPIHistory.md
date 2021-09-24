# 查询API历史版本列表<a name="ZH-CN_TOPIC_0000001082135165"></a>

## 功能介绍<a name="zh-cn_topic_0225568825_section6627989"></a>

查询某个API的历史版本。每个API在一个环境上最多存在10个历史版本。

## URI<a name="zh-cn_topic_0225568825_section59651907"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568825_table42014202"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568825_row11048869"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568825_p22543169"><a name="zh-cn_topic_0225568825_p22543169"></a><a name="zh-cn_topic_0225568825_p22543169"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568825_p14057426"><a name="zh-cn_topic_0225568825_p14057426"></a><a name="zh-cn_topic_0225568825_p14057426"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568825_row64909760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568825_p23199218"><a name="zh-cn_topic_0225568825_p23199218"></a><a name="zh-cn_topic_0225568825_p23199218"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568825_p88529"><a name="zh-cn_topic_0225568825_p88529"></a><a name="zh-cn_topic_0225568825_p88529"></a>/v1/{project_id}/apigw/instances/{instance_id}/apis/publish/{api_id}[?env_id,env_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：env\_id,env\_name。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568825_table796764"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568825_row53401841"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568825_p30581871"><a name="zh-cn_topic_0225568825_p30581871"></a><a name="zh-cn_topic_0225568825_p30581871"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568825_p61212526"><a name="zh-cn_topic_0225568825_p61212526"></a><a name="zh-cn_topic_0225568825_p61212526"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="16.41%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568825_p59267606"><a name="zh-cn_topic_0225568825_p59267606"></a><a name="zh-cn_topic_0225568825_p59267606"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.589999999999996%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568825_p35946766"><a name="zh-cn_topic_0225568825_p35946766"></a><a name="zh-cn_topic_0225568825_p35946766"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568825_row1149913412198"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568825_p55878963"><a name="zh-cn_topic_0225568825_p55878963"></a><a name="zh-cn_topic_0225568825_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568825_p29902160"><a name="zh-cn_topic_0225568825_p29902160"></a><a name="zh-cn_topic_0225568825_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.41%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568825_p6155914"><a name="zh-cn_topic_0225568825_p6155914"></a><a name="zh-cn_topic_0225568825_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.589999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568825_p28867016"><a name="zh-cn_topic_0225568825_p28867016"></a><a name="zh-cn_topic_0225568825_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row12941133181910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568825_p1780913159538"><a name="zh-cn_topic_0225568825_p1780913159538"></a><a name="zh-cn_topic_0225568825_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568825_p9809215115310"><a name="zh-cn_topic_0225568825_p9809215115310"></a><a name="zh-cn_topic_0225568825_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.41%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568825_p1280914152538"><a name="zh-cn_topic_0225568825_p1280914152538"></a><a name="zh-cn_topic_0225568825_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.589999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568825_p1880914157537"><a name="zh-cn_topic_0225568825_p1880914157537"></a><a name="zh-cn_topic_0225568825_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row26006910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568825_p26184975"><a name="zh-cn_topic_0225568825_p26184975"></a><a name="zh-cn_topic_0225568825_p26184975"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568825_p40608232"><a name="zh-cn_topic_0225568825_p40608232"></a><a name="zh-cn_topic_0225568825_p40608232"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="16.41%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568825_p932530"><a name="zh-cn_topic_0225568825_p932530"></a><a name="zh-cn_topic_0225568825_p932530"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.589999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568825_p8426133"><a name="zh-cn_topic_0225568825_p8426133"></a><a name="zh-cn_topic_0225568825_p8426133"></a>API的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row123871511132316"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568825_p038715116233"><a name="zh-cn_topic_0225568825_p038715116233"></a><a name="zh-cn_topic_0225568825_p038715116233"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568825_p163871111162311"><a name="zh-cn_topic_0225568825_p163871111162311"></a><a name="zh-cn_topic_0225568825_p163871111162311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.41%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568825_p123874110237"><a name="zh-cn_topic_0225568825_p123874110237"></a><a name="zh-cn_topic_0225568825_p123874110237"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.589999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568825_p16387311102313"><a name="zh-cn_topic_0225568825_p16387311102313"></a><a name="zh-cn_topic_0225568825_p16387311102313"></a>环境的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row8636813192312"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568825_p12636013142314"><a name="zh-cn_topic_0225568825_p12636013142314"></a><a name="zh-cn_topic_0225568825_p12636013142314"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="17%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568825_p36362134231"><a name="zh-cn_topic_0225568825_p36362134231"></a><a name="zh-cn_topic_0225568825_p36362134231"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="16.41%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568825_p2636121342313"><a name="zh-cn_topic_0225568825_p2636121342313"></a><a name="zh-cn_topic_0225568825_p2636121342313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.589999999999996%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568825_p1963661313233"><a name="zh-cn_topic_0225568825_p1963661313233"></a><a name="zh-cn_topic_0225568825_p1963661313233"></a>环境的名称</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568825_section67105121"></a>

无

## 响应消息<a name="zh-cn_topic_0225568825_section66805754"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568825_table2981672313"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568825_row898177103111"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568825_p109837183116"><a name="zh-cn_topic_0225568825_p109837183116"></a><a name="zh-cn_topic_0225568825_p109837183116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568825_p1098474319"><a name="zh-cn_topic_0225568825_p1098474319"></a><a name="zh-cn_topic_0225568825_p1098474319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568825_p1398197193117"><a name="zh-cn_topic_0225568825_p1398197193117"></a><a name="zh-cn_topic_0225568825_p1398197193117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568825_row49812719314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p25782746"><a name="zh-cn_topic_0225568825_p25782746"></a><a name="zh-cn_topic_0225568825_p25782746"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p8027664"><a name="zh-cn_topic_0225568825_p8027664"></a><a name="zh-cn_topic_0225568825_p8027664"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p46261084"><a name="zh-cn_topic_0225568825_p46261084"></a><a name="zh-cn_topic_0225568825_p46261084"></a>满足条件的API历史版本总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row119827123112"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p35680577"><a name="zh-cn_topic_0225568825_p35680577"></a><a name="zh-cn_topic_0225568825_p35680577"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p4445647"><a name="zh-cn_topic_0225568825_p4445647"></a><a name="zh-cn_topic_0225568825_p4445647"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p24553101"><a name="zh-cn_topic_0225568825_p24553101"></a><a name="zh-cn_topic_0225568825_p24553101"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row998187163114"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p48252863"><a name="zh-cn_topic_0225568825_p48252863"></a><a name="zh-cn_topic_0225568825_p48252863"></a>api_versions</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p16167821"><a name="zh-cn_topic_0225568825_p16167821"></a><a name="zh-cn_topic_0225568825_p16167821"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p34525128"><a name="zh-cn_topic_0225568825_p34525128"></a><a name="zh-cn_topic_0225568825_p34525128"></a>本次查询返回的API历史版本列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  api\_versions参数说明

<a name="zh-cn_topic_0225568825_table42290697"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568825_row54536847"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568825_p55408512"><a name="zh-cn_topic_0225568825_p55408512"></a><a name="zh-cn_topic_0225568825_p55408512"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568825_p58904526"><a name="zh-cn_topic_0225568825_p58904526"></a><a name="zh-cn_topic_0225568825_p58904526"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568825_p6537312"><a name="zh-cn_topic_0225568825_p6537312"></a><a name="zh-cn_topic_0225568825_p6537312"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568825_row59760287"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p18981672315"><a name="zh-cn_topic_0225568825_p18981672315"></a><a name="zh-cn_topic_0225568825_p18981672315"></a>version_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p209815717318"><a name="zh-cn_topic_0225568825_p209815717318"></a><a name="zh-cn_topic_0225568825_p209815717318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p8980773120"><a name="zh-cn_topic_0225568825_p8980773120"></a><a name="zh-cn_topic_0225568825_p8980773120"></a>API历史版本的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row6945124117278"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p794519411278"><a name="zh-cn_topic_0225568825_p794519411278"></a><a name="zh-cn_topic_0225568825_p794519411278"></a>version_no</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p694574110271"><a name="zh-cn_topic_0225568825_p694574110271"></a><a name="zh-cn_topic_0225568825_p694574110271"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p39458412271"><a name="zh-cn_topic_0225568825_p39458412271"></a><a name="zh-cn_topic_0225568825_p39458412271"></a>API的版本号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row52310185"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p159814710314"><a name="zh-cn_topic_0225568825_p159814710314"></a><a name="zh-cn_topic_0225568825_p159814710314"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p1698871311"><a name="zh-cn_topic_0225568825_p1698871311"></a><a name="zh-cn_topic_0225568825_p1698871311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p109897153112"><a name="zh-cn_topic_0225568825_p109897153112"></a><a name="zh-cn_topic_0225568825_p109897153112"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row45342804"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p129814713315"><a name="zh-cn_topic_0225568825_p129814713315"></a><a name="zh-cn_topic_0225568825_p129814713315"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p13987723113"><a name="zh-cn_topic_0225568825_p13987723113"></a><a name="zh-cn_topic_0225568825_p13987723113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p109819712314"><a name="zh-cn_topic_0225568825_p109819712314"></a><a name="zh-cn_topic_0225568825_p109819712314"></a>发布的环境编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row143411649142719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p143411649112717"><a name="zh-cn_topic_0225568825_p143411649112717"></a><a name="zh-cn_topic_0225568825_p143411649112717"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p3341849162714"><a name="zh-cn_topic_0225568825_p3341849162714"></a><a name="zh-cn_topic_0225568825_p3341849162714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p193411949122714"><a name="zh-cn_topic_0225568825_p193411949122714"></a><a name="zh-cn_topic_0225568825_p193411949122714"></a>发布的环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row60411917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p1098147143114"><a name="zh-cn_topic_0225568825_p1098147143114"></a><a name="zh-cn_topic_0225568825_p1098147143114"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p998197113114"><a name="zh-cn_topic_0225568825_p998197113114"></a><a name="zh-cn_topic_0225568825_p998197113114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p99816773110"><a name="zh-cn_topic_0225568825_p99816773110"></a><a name="zh-cn_topic_0225568825_p99816773110"></a>发布描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row41802573"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p998117163115"><a name="zh-cn_topic_0225568825_p998117163115"></a><a name="zh-cn_topic_0225568825_p998117163115"></a>publish_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p59813711317"><a name="zh-cn_topic_0225568825_p59813711317"></a><a name="zh-cn_topic_0225568825_p59813711317"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p5989733118"><a name="zh-cn_topic_0225568825_p5989733118"></a><a name="zh-cn_topic_0225568825_p5989733118"></a>发布时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row20081233"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568825_p15967206"><a name="zh-cn_topic_0225568825_p15967206"></a><a name="zh-cn_topic_0225568825_p15967206"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568825_p18275332"><a name="zh-cn_topic_0225568825_p18275332"></a><a name="zh-cn_topic_0225568825_p18275332"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568825_p81811545182511"><a name="zh-cn_topic_0225568825_p81811545182511"></a><a name="zh-cn_topic_0225568825_p81811545182511"></a>版本状态：</p>
<a name="zh-cn_topic_0225568825_ul0837134912255"></a><a name="zh-cn_topic_0225568825_ul0837134912255"></a><ul id="zh-cn_topic_0225568825_ul0837134912255"><li>1、当前生效中的版本</li><li>2、未生效的版本</li></ul>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 1,
  "size": 1,
  "api_versions": [
    {
      "version_id": "04c194dc7b5340ed942f2451702060da",
      "version_no": "20180722102526",
      "api_id": "acf141aa6279415088b593a4bbb55eed",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "publish_time": "2018-04-14T07:32:23Z",
      "status": 2
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0225568825_section67075185"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568825_table15714732"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568825_row24997277"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568825_p11513591"><a name="zh-cn_topic_0225568825_p11513591"></a><a name="zh-cn_topic_0225568825_p11513591"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568825_p60185706"><a name="zh-cn_topic_0225568825_p60185706"></a><a name="zh-cn_topic_0225568825_p60185706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568825_row43203997"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568825_p9862840"><a name="zh-cn_topic_0225568825_p9862840"></a><a name="zh-cn_topic_0225568825_p9862840"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568825_p73578115452"><a name="zh-cn_topic_0225568825_p73578115452"></a><a name="zh-cn_topic_0225568825_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row9362312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568825_p20149775"><a name="zh-cn_topic_0225568825_p20149775"></a><a name="zh-cn_topic_0225568825_p20149775"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568825_p21519099"><a name="zh-cn_topic_0225568825_p21519099"></a><a name="zh-cn_topic_0225568825_p21519099"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row59454171"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568825_p51058521"><a name="zh-cn_topic_0225568825_p51058521"></a><a name="zh-cn_topic_0225568825_p51058521"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568825_p9203142078"><a name="zh-cn_topic_0225568825_p9203142078"></a><a name="zh-cn_topic_0225568825_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row43351211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568825_p21787193"><a name="zh-cn_topic_0225568825_p21787193"></a><a name="zh-cn_topic_0225568825_p21787193"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568825_p13949586"><a name="zh-cn_topic_0225568825_p13949586"></a><a name="zh-cn_topic_0225568825_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row45172181"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568825_p35068062"><a name="zh-cn_topic_0225568825_p35068062"></a><a name="zh-cn_topic_0225568825_p35068062"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568825_p21940743"><a name="zh-cn_topic_0225568825_p21940743"></a><a name="zh-cn_topic_0225568825_p21940743"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568825_row63248959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568825_p22892027"><a name="zh-cn_topic_0225568825_p22892027"></a><a name="zh-cn_topic_0225568825_p22892027"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568825_p14947689"><a name="zh-cn_topic_0225568825_p14947689"></a><a name="zh-cn_topic_0225568825_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

