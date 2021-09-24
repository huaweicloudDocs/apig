# 根据版本编号下线API<a name="ZH-CN_TOPIC_0000001081837263"></a>

## 功能介绍<a name="zh-cn_topic_0127545882_section59395644"></a>

对某个生效中的API版本进行下线操作，下线后，API在该版本生效的环境中将不再能够被调用。

该接口供FunctionGraph服务使用。

## URI<a name="zh-cn_topic_0127545882_section64798754"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0127545882_table30440385"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127545882_row5989628"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127545882_p15397832"><a name="zh-cn_topic_0127545882_p15397832"></a><a name="zh-cn_topic_0127545882_p15397832"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127545882_p39264905"><a name="zh-cn_topic_0127545882_p39264905"></a><a name="zh-cn_topic_0127545882_p39264905"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127545882_row26340775"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127545882_p53228041"><a name="zh-cn_topic_0127545882_p53228041"></a><a name="zh-cn_topic_0127545882_p53228041"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127545882_p16504088"><a name="zh-cn_topic_0127545882_p16504088"></a><a name="zh-cn_topic_0127545882_p16504088"></a>/v1.0/apigw/apis/versions/{version_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0127545882_table14319067"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127545882_row47200048"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0127545882_p65107550"><a name="zh-cn_topic_0127545882_p65107550"></a><a name="zh-cn_topic_0127545882_p65107550"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0127545882_p39220237"><a name="zh-cn_topic_0127545882_p39220237"></a><a name="zh-cn_topic_0127545882_p39220237"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0127545882_p22722661"><a name="zh-cn_topic_0127545882_p22722661"></a><a name="zh-cn_topic_0127545882_p22722661"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0127545882_p28596237"><a name="zh-cn_topic_0127545882_p28596237"></a><a name="zh-cn_topic_0127545882_p28596237"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127545882_row34593837"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0127545882_p50637422"><a name="zh-cn_topic_0127545882_p50637422"></a><a name="zh-cn_topic_0127545882_p50637422"></a>version_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0127545882_p7990519"><a name="zh-cn_topic_0127545882_p7990519"></a><a name="zh-cn_topic_0127545882_p7990519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0127545882_p43252337"><a name="zh-cn_topic_0127545882_p43252337"></a><a name="zh-cn_topic_0127545882_p43252337"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0127545882_p13778436"><a name="zh-cn_topic_0127545882_p13778436"></a><a name="zh-cn_topic_0127545882_p13778436"></a>API版本的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0127545882_section46317880"></a>

无。

## 响应消息<a name="zh-cn_topic_0127545882_section60760833"></a>

无

## 状态码<a name="zh-cn_topic_0127545882_section14207744"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0127545882_table25461982"></a>
<table><thead align="left"><tr id="zh-cn_topic_0127545882_row64728256"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0127545882_p8497375"><a name="zh-cn_topic_0127545882_p8497375"></a><a name="zh-cn_topic_0127545882_p8497375"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0127545882_p17198799"><a name="zh-cn_topic_0127545882_p17198799"></a><a name="zh-cn_topic_0127545882_p17198799"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0127545882_row50925496"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127545882_p31324481"><a name="zh-cn_topic_0127545882_p31324481"></a><a name="zh-cn_topic_0127545882_p31324481"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127545882_p13445195614478"><a name="zh-cn_topic_0127545882_p13445195614478"></a><a name="zh-cn_topic_0127545882_p13445195614478"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0127545882_row18532901"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127545882_p24770038"><a name="zh-cn_topic_0127545882_p24770038"></a><a name="zh-cn_topic_0127545882_p24770038"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127545882_p60216100"><a name="zh-cn_topic_0127545882_p60216100"></a><a name="zh-cn_topic_0127545882_p60216100"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0127545882_row5073993"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127545882_p8340301"><a name="zh-cn_topic_0127545882_p8340301"></a><a name="zh-cn_topic_0127545882_p8340301"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127545882_p9203142078"><a name="zh-cn_topic_0127545882_p9203142078"></a><a name="zh-cn_topic_0127545882_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0127545882_row40281704"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127545882_p41592600"><a name="zh-cn_topic_0127545882_p41592600"></a><a name="zh-cn_topic_0127545882_p41592600"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127545882_p13949586"><a name="zh-cn_topic_0127545882_p13949586"></a><a name="zh-cn_topic_0127545882_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0127545882_row54907919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127545882_p18356469"><a name="zh-cn_topic_0127545882_p18356469"></a><a name="zh-cn_topic_0127545882_p18356469"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127545882_p10479027"><a name="zh-cn_topic_0127545882_p10479027"></a><a name="zh-cn_topic_0127545882_p10479027"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0127545882_row23141906"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0127545882_p62555074"><a name="zh-cn_topic_0127545882_p62555074"></a><a name="zh-cn_topic_0127545882_p62555074"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0127545882_p14947689"><a name="zh-cn_topic_0127545882_p14947689"></a><a name="zh-cn_topic_0127545882_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

