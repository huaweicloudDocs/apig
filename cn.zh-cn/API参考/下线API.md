# 下线API<a name="apig-zh-api-180713029"></a>

## 功能介绍<a name="section59395644"></a>

将API从某个已发布的环境上下线，下线后，API将无法再被调用。

## URI<a name="section64798754"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table30440385"></a>
<table><thead align="left"><tr id="row5989628"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p15397832"><a name="p15397832"></a><a name="p15397832"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p39264905"><a name="p39264905"></a><a name="p39264905"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row26340775"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p53228041"><a name="p53228041"></a><a name="p53228041"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p16504088"><a name="p16504088"></a><a name="p16504088"></a>/v1.0/apigw/apis/publish/{api_id}[?env_id]</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table14319067"></a>
<table><thead align="left"><tr id="row47200048"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p65107550"><a name="p65107550"></a><a name="p65107550"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p39220237"><a name="p39220237"></a><a name="p39220237"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p22722661"><a name="p22722661"></a><a name="p22722661"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p28596237"><a name="p28596237"></a><a name="p28596237"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row34593837"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p50637422"><a name="p50637422"></a><a name="p50637422"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p7990519"><a name="p7990519"></a><a name="p7990519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p43252337"><a name="p43252337"></a><a name="p43252337"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p13778436"><a name="p13778436"></a><a name="p13778436"></a>API的编号</p>
</td>
</tr>
<tr id="row56897062"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p45259280"><a name="p45259280"></a><a name="p45259280"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p42123046"><a name="p42123046"></a><a name="p42123046"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p56523602"><a name="p56523602"></a><a name="p56523602"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p15009017"><a name="p15009017"></a><a name="p15009017"></a>环境编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section46317880"></a>

无。

## 响应消息<a name="section60760833"></a>

无

## 状态码<a name="section14207744"></a>

**表 3**  返回消息说明

<a name="table25461982"></a>
<table><thead align="left"><tr id="row64728256"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p8497375"><a name="p8497375"></a><a name="p8497375"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p17198799"><a name="p17198799"></a><a name="p17198799"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row50925496"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p31324481"><a name="p31324481"></a><a name="p31324481"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13445195614478"><a name="p13445195614478"></a><a name="p13445195614478"></a>No Content</p>
</td>
</tr>
<tr id="row18532901"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p24770038"><a name="p24770038"></a><a name="p24770038"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p60216100"><a name="p60216100"></a><a name="p60216100"></a>Bad Request</p>
</td>
</tr>
<tr id="row5073993"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p8340301"><a name="p8340301"></a><a name="p8340301"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row40281704"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p41592600"><a name="p41592600"></a><a name="p41592600"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row54907919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p18356469"><a name="p18356469"></a><a name="p18356469"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p10479027"><a name="p10479027"></a><a name="p10479027"></a>Not Found</p>
</td>
</tr>
<tr id="row27202387"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p55909770"><a name="p55909770"></a><a name="p55909770"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p32397484"><a name="p32397484"></a><a name="p32397484"></a>Conflict</p>
</td>
</tr>
<tr id="row23141906"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p62555074"><a name="p62555074"></a><a name="p62555074"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

