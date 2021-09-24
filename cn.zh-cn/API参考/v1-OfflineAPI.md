# 下线API<a name="ZH-CN_TOPIC_0000001082135163"></a>

## 功能介绍<a name="zh-cn_topic_0225568820_section59395644"></a>

将API从某个已发布的环境上下线，下线后，API将无法再被调用。

## URI<a name="zh-cn_topic_0225568820_section64798754"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568820_table30440385"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568820_row5989628"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568820_p15397832"><a name="zh-cn_topic_0225568820_p15397832"></a><a name="zh-cn_topic_0225568820_p15397832"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568820_p39264905"><a name="zh-cn_topic_0225568820_p39264905"></a><a name="zh-cn_topic_0225568820_p39264905"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568820_row26340775"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p53228041"><a name="zh-cn_topic_0225568820_p53228041"></a><a name="zh-cn_topic_0225568820_p53228041"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p16504088"><a name="zh-cn_topic_0225568820_p16504088"></a><a name="zh-cn_topic_0225568820_p16504088"></a>/v1/{project_id}/apigw/instances/{instance_id}/apis/publish/{api_id}[?env_id]</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568820_table14319067"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568820_row47200048"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568820_p65107550"><a name="zh-cn_topic_0225568820_p65107550"></a><a name="zh-cn_topic_0225568820_p65107550"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.83%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568820_p39220237"><a name="zh-cn_topic_0225568820_p39220237"></a><a name="zh-cn_topic_0225568820_p39220237"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.32%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568820_p22722661"><a name="zh-cn_topic_0225568820_p22722661"></a><a name="zh-cn_topic_0225568820_p22722661"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="39.85%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568820_p28596237"><a name="zh-cn_topic_0225568820_p28596237"></a><a name="zh-cn_topic_0225568820_p28596237"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568820_row47017119181"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568820_p55878963"><a name="zh-cn_topic_0225568820_p55878963"></a><a name="zh-cn_topic_0225568820_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568820_p29902160"><a name="zh-cn_topic_0225568820_p29902160"></a><a name="zh-cn_topic_0225568820_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568820_p6155914"><a name="zh-cn_topic_0225568820_p6155914"></a><a name="zh-cn_topic_0225568820_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.85%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568820_p28867016"><a name="zh-cn_topic_0225568820_p28867016"></a><a name="zh-cn_topic_0225568820_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row688860131818"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568820_p1780913159538"><a name="zh-cn_topic_0225568820_p1780913159538"></a><a name="zh-cn_topic_0225568820_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568820_p9809215115310"><a name="zh-cn_topic_0225568820_p9809215115310"></a><a name="zh-cn_topic_0225568820_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568820_p1280914152538"><a name="zh-cn_topic_0225568820_p1280914152538"></a><a name="zh-cn_topic_0225568820_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.85%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568820_p1880914157537"><a name="zh-cn_topic_0225568820_p1880914157537"></a><a name="zh-cn_topic_0225568820_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row34593837"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568820_p50637422"><a name="zh-cn_topic_0225568820_p50637422"></a><a name="zh-cn_topic_0225568820_p50637422"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568820_p7990519"><a name="zh-cn_topic_0225568820_p7990519"></a><a name="zh-cn_topic_0225568820_p7990519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568820_p43252337"><a name="zh-cn_topic_0225568820_p43252337"></a><a name="zh-cn_topic_0225568820_p43252337"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.85%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568820_p13778436"><a name="zh-cn_topic_0225568820_p13778436"></a><a name="zh-cn_topic_0225568820_p13778436"></a>API的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row56897062"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568820_p45259280"><a name="zh-cn_topic_0225568820_p45259280"></a><a name="zh-cn_topic_0225568820_p45259280"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.83%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568820_p42123046"><a name="zh-cn_topic_0225568820_p42123046"></a><a name="zh-cn_topic_0225568820_p42123046"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.32%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568820_p56523602"><a name="zh-cn_topic_0225568820_p56523602"></a><a name="zh-cn_topic_0225568820_p56523602"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="39.85%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568820_p15009017"><a name="zh-cn_topic_0225568820_p15009017"></a><a name="zh-cn_topic_0225568820_p15009017"></a>环境编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568820_section46317880"></a>

无。

## 响应消息<a name="zh-cn_topic_0225568820_section60760833"></a>

无

## 状态码<a name="zh-cn_topic_0225568820_section14207744"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568820_table25461982"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568820_row64728256"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568820_p8497375"><a name="zh-cn_topic_0225568820_p8497375"></a><a name="zh-cn_topic_0225568820_p8497375"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568820_p17198799"><a name="zh-cn_topic_0225568820_p17198799"></a><a name="zh-cn_topic_0225568820_p17198799"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568820_row50925496"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p31324481"><a name="zh-cn_topic_0225568820_p31324481"></a><a name="zh-cn_topic_0225568820_p31324481"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p13445195614478"><a name="zh-cn_topic_0225568820_p13445195614478"></a><a name="zh-cn_topic_0225568820_p13445195614478"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row18532901"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p24770038"><a name="zh-cn_topic_0225568820_p24770038"></a><a name="zh-cn_topic_0225568820_p24770038"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p60216100"><a name="zh-cn_topic_0225568820_p60216100"></a><a name="zh-cn_topic_0225568820_p60216100"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row5073993"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p8340301"><a name="zh-cn_topic_0225568820_p8340301"></a><a name="zh-cn_topic_0225568820_p8340301"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p9203142078"><a name="zh-cn_topic_0225568820_p9203142078"></a><a name="zh-cn_topic_0225568820_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row40281704"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p41592600"><a name="zh-cn_topic_0225568820_p41592600"></a><a name="zh-cn_topic_0225568820_p41592600"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p13949586"><a name="zh-cn_topic_0225568820_p13949586"></a><a name="zh-cn_topic_0225568820_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row54907919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p18356469"><a name="zh-cn_topic_0225568820_p18356469"></a><a name="zh-cn_topic_0225568820_p18356469"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p10479027"><a name="zh-cn_topic_0225568820_p10479027"></a><a name="zh-cn_topic_0225568820_p10479027"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row27202387"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p55909770"><a name="zh-cn_topic_0225568820_p55909770"></a><a name="zh-cn_topic_0225568820_p55909770"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p32397484"><a name="zh-cn_topic_0225568820_p32397484"></a><a name="zh-cn_topic_0225568820_p32397484"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568820_row23141906"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568820_p62555074"><a name="zh-cn_topic_0225568820_p62555074"></a><a name="zh-cn_topic_0225568820_p62555074"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568820_p14947689"><a name="zh-cn_topic_0225568820_p14947689"></a><a name="zh-cn_topic_0225568820_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

