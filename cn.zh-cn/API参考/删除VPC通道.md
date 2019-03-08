# 删除VPC通道<a name="apig-zh-api-180713163"></a>

## 功能介绍<a name="section173482301428"></a>

删除指定的VPC通道。

## URI<a name="section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table1439319294431"></a>
<table><thead align="left"><tr id="row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p14361448204314"><a name="p14361448204314"></a><a name="p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p1936174864316"><a name="p1936174864316"></a><a name="p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1236111482435"><a name="p1236111482435"></a><a name="p1236111482435"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p11361848184318"><a name="p11361848184318"></a><a name="p11361848184318"></a>/v1.0/apigw/vpc-channels/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table18784710"></a>
<table><thead align="left"><tr id="row37287554"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p393051"><a name="p393051"></a><a name="p393051"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p31837140"><a name="p31837140"></a><a name="p31837140"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p28671509"><a name="p28671509"></a><a name="p28671509"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p40690887"><a name="p40690887"></a><a name="p40690887"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7627537"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p13850780"><a name="p13850780"></a><a name="p13850780"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p48171408"><a name="p48171408"></a><a name="p48171408"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p9569939"><a name="p9569939"></a><a name="p9569939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p36967632"><a name="p36967632"></a><a name="p36967632"></a>VPC通道的编号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section73637302425"></a>

无

## 响应消息<a name="section9395153012420"></a>

无

## 状态码<a name="section338043011426"></a>

**表 3**  返回消息说明

<a name="table1338010302424"></a>
<table><thead align="left"><tr id="row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p174881730194216"><a name="p174881730194216"></a><a name="p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p848863018429"><a name="p848863018429"></a><a name="p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p7488163084211"><a name="p7488163084211"></a><a name="p7488163084211"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p948803015424"><a name="p948803015424"></a><a name="p948803015424"></a>No Content</p>
</td>
</tr>
<tr id="row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p14488113015426"><a name="p14488113015426"></a><a name="p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p164881130154211"><a name="p164881130154211"></a><a name="p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p24883304428"><a name="p24883304428"></a><a name="p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1848810308429"><a name="p1848810308429"></a><a name="p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6488133064210"><a name="p6488133064210"></a><a name="p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p10488193018426"><a name="p10488193018426"></a><a name="p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p144883304428"><a name="p144883304428"></a><a name="p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p4488103094212"><a name="p4488103094212"></a><a name="p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p17488163014423"><a name="p17488163014423"></a><a name="p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p048813014216"><a name="p048813014216"></a><a name="p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

