# 删除VPC通道<a name="ZH-CN_TOPIC_0000001082135145"></a>

## 功能介绍<a name="zh-cn_topic_0118924575_section173482301428"></a>

删除指定的VPC通道。

## URI<a name="zh-cn_topic_0118924575_section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924575_table1439319294431"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924575_row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924575_p14361448204314"><a name="zh-cn_topic_0118924575_p14361448204314"></a><a name="zh-cn_topic_0118924575_p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924575_p1936174864316"><a name="zh-cn_topic_0118924575_p1936174864316"></a><a name="zh-cn_topic_0118924575_p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924575_row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924575_p1236111482435"><a name="zh-cn_topic_0118924575_p1236111482435"></a><a name="zh-cn_topic_0118924575_p1236111482435"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924575_p11361848184318"><a name="zh-cn_topic_0118924575_p11361848184318"></a><a name="zh-cn_topic_0118924575_p11361848184318"></a>/v1.0/apigw/vpc-channels/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924575_table18784710"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924575_row37287554"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924575_p393051"><a name="zh-cn_topic_0118924575_p393051"></a><a name="zh-cn_topic_0118924575_p393051"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924575_p31837140"><a name="zh-cn_topic_0118924575_p31837140"></a><a name="zh-cn_topic_0118924575_p31837140"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924575_p28671509"><a name="zh-cn_topic_0118924575_p28671509"></a><a name="zh-cn_topic_0118924575_p28671509"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924575_p40690887"><a name="zh-cn_topic_0118924575_p40690887"></a><a name="zh-cn_topic_0118924575_p40690887"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924575_row7627537"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924575_p13850780"><a name="zh-cn_topic_0118924575_p13850780"></a><a name="zh-cn_topic_0118924575_p13850780"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924575_p48171408"><a name="zh-cn_topic_0118924575_p48171408"></a><a name="zh-cn_topic_0118924575_p48171408"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924575_p9569939"><a name="zh-cn_topic_0118924575_p9569939"></a><a name="zh-cn_topic_0118924575_p9569939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924575_p36967632"><a name="zh-cn_topic_0118924575_p36967632"></a><a name="zh-cn_topic_0118924575_p36967632"></a>VPC通道的编号。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924575_section73637302425"></a>

无

## 响应消息<a name="zh-cn_topic_0118924575_section9395153012420"></a>

无

## 状态码<a name="zh-cn_topic_0118924575_section338043011426"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924575_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924575_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924575_p174881730194216"><a name="zh-cn_topic_0118924575_p174881730194216"></a><a name="zh-cn_topic_0118924575_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924575_p848863018429"><a name="zh-cn_topic_0118924575_p848863018429"></a><a name="zh-cn_topic_0118924575_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924575_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924575_p7488163084211"><a name="zh-cn_topic_0118924575_p7488163084211"></a><a name="zh-cn_topic_0118924575_p7488163084211"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924575_p948803015424"><a name="zh-cn_topic_0118924575_p948803015424"></a><a name="zh-cn_topic_0118924575_p948803015424"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924575_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924575_p14488113015426"><a name="zh-cn_topic_0118924575_p14488113015426"></a><a name="zh-cn_topic_0118924575_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924575_p164881130154211"><a name="zh-cn_topic_0118924575_p164881130154211"></a><a name="zh-cn_topic_0118924575_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924575_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924575_p24883304428"><a name="zh-cn_topic_0118924575_p24883304428"></a><a name="zh-cn_topic_0118924575_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924575_p1848810308429"><a name="zh-cn_topic_0118924575_p1848810308429"></a><a name="zh-cn_topic_0118924575_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924575_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924575_p6488133064210"><a name="zh-cn_topic_0118924575_p6488133064210"></a><a name="zh-cn_topic_0118924575_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924575_p10488193018426"><a name="zh-cn_topic_0118924575_p10488193018426"></a><a name="zh-cn_topic_0118924575_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924575_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924575_p144883304428"><a name="zh-cn_topic_0118924575_p144883304428"></a><a name="zh-cn_topic_0118924575_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924575_p4488103094212"><a name="zh-cn_topic_0118924575_p4488103094212"></a><a name="zh-cn_topic_0118924575_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924575_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924575_p17488163014423"><a name="zh-cn_topic_0118924575_p17488163014423"></a><a name="zh-cn_topic_0118924575_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924575_p048813014216"><a name="zh-cn_topic_0118924575_p048813014216"></a><a name="zh-cn_topic_0118924575_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

