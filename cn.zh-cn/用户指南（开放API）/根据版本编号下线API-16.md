# 根据版本编号下线API<a name="apig-phapi-180911216"></a>

## 功能介绍<a name="section59395644"></a>

对某个生效中的API版本进行下线操作，下线后，API在该版本生效的环境中将不再能够被调用。

该接口供FunctionGraph服务使用。

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
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p16504088"><a name="p16504088"></a><a name="p16504088"></a><span id="ph131289353412"><a name="ph131289353412"></a><a name="ph131289353412"></a>/v1/{project_id}/apigw/instances/{instance_id}</span>/apis/versions/{version_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table14319067"></a>
<table><thead align="left"><tr id="row47200048"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p65107550"><a name="p65107550"></a><a name="p65107550"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.950000000000001%" id="mcps1.2.5.1.2"><p id="p39220237"><a name="p39220237"></a><a name="p39220237"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.3"><p id="p22722661"><a name="p22722661"></a><a name="p22722661"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.699999999999996%" id="mcps1.2.5.1.4"><p id="p28596237"><a name="p28596237"></a><a name="p28596237"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16588184511195"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.950000000000001%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.699999999999996%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row5188345121915"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.950000000000001%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.699999999999996%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row34593837"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p50637422"><a name="p50637422"></a><a name="p50637422"></a>version_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.950000000000001%" headers="mcps1.2.5.1.2 "><p id="p7990519"><a name="p7990519"></a><a name="p7990519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.3 "><p id="p43252337"><a name="p43252337"></a><a name="p43252337"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.699999999999996%" headers="mcps1.2.5.1.4 "><p id="p13778436"><a name="p13778436"></a><a name="p13778436"></a>API版本的编号</p>
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
<tr id="row23141906"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p62555074"><a name="p62555074"></a><a name="p62555074"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

