# 解绑域名<a name="ZH-CN_TOPIC_0000001082135141"></a>

## 功能介绍<a name="zh-cn_topic_0118924567_section2838113553510"></a>

如果API分组不再需要绑定某个自定义域名，则可以为此API分组解绑此域名。

## URI<a name="zh-cn_topic_0118924567_section1483813518355"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924567_table158813202366"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924567_row758818209365"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924567_p697919354356"><a name="zh-cn_topic_0118924567_p697919354356"></a><a name="zh-cn_topic_0118924567_p697919354356"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924567_p597913358352"><a name="zh-cn_topic_0118924567_p597913358352"></a><a name="zh-cn_topic_0118924567_p597913358352"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924567_row195883204363"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924567_p3979183510355"><a name="zh-cn_topic_0118924567_p3979183510355"></a><a name="zh-cn_topic_0118924567_p3979183510355"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924567_p09791635183515"><a name="zh-cn_topic_0118924567_p09791635183515"></a><a name="zh-cn_topic_0118924567_p09791635183515"></a>/v1.0/apigw/api-groups/{group_id}/domains/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924567_table4851459153818"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924567_row1985259143813"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924567_p12367713193420"><a name="zh-cn_topic_0118924567_p12367713193420"></a><a name="zh-cn_topic_0118924567_p12367713193420"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924567_p7367161316343"><a name="zh-cn_topic_0118924567_p7367161316343"></a><a name="zh-cn_topic_0118924567_p7367161316343"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="24%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924567_p93675133347"><a name="zh-cn_topic_0118924567_p93675133347"></a><a name="zh-cn_topic_0118924567_p93675133347"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="26%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924567_p836761317349"><a name="zh-cn_topic_0118924567_p836761317349"></a><a name="zh-cn_topic_0118924567_p836761317349"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924567_row18555915383"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924567_p111823311382"><a name="zh-cn_topic_0118924567_p111823311382"></a><a name="zh-cn_topic_0118924567_p111823311382"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924567_p163410335385"><a name="zh-cn_topic_0118924567_p163410335385"></a><a name="zh-cn_topic_0118924567_p163410335385"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924567_p83443318381"><a name="zh-cn_topic_0118924567_p83443318381"></a><a name="zh-cn_topic_0118924567_p83443318381"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924567_p3341333163817"><a name="zh-cn_topic_0118924567_p3341333163817"></a><a name="zh-cn_topic_0118924567_p3341333163817"></a>域名的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924567_row19909115531718"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924567_p8901205651717"><a name="zh-cn_topic_0118924567_p8901205651717"></a><a name="zh-cn_topic_0118924567_p8901205651717"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924567_p4901145618175"><a name="zh-cn_topic_0118924567_p4901145618175"></a><a name="zh-cn_topic_0118924567_p4901145618175"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924567_p1690118564173"><a name="zh-cn_topic_0118924567_p1690118564173"></a><a name="zh-cn_topic_0118924567_p1690118564173"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924567_p19012566171"><a name="zh-cn_topic_0118924567_p19012566171"></a><a name="zh-cn_topic_0118924567_p19012566171"></a>分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924567_section14272513203411"></a>

无

## 响应消息<a name="zh-cn_topic_0118924567_section1088543511350"></a>

无

## 状态码<a name="zh-cn_topic_0118924567_section285443523516"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924567_table178548355351"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924567_row2097913519353"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924567_p297943513357"><a name="zh-cn_topic_0118924567_p297943513357"></a><a name="zh-cn_topic_0118924567_p297943513357"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924567_p199791235183518"><a name="zh-cn_topic_0118924567_p199791235183518"></a><a name="zh-cn_topic_0118924567_p199791235183518"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924567_row13979235133511"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924567_p1997963513513"><a name="zh-cn_topic_0118924567_p1997963513513"></a><a name="zh-cn_topic_0118924567_p1997963513513"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924567_p948803015424"><a name="zh-cn_topic_0118924567_p948803015424"></a><a name="zh-cn_topic_0118924567_p948803015424"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924567_row209793352352"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924567_p297915353359"><a name="zh-cn_topic_0118924567_p297915353359"></a><a name="zh-cn_topic_0118924567_p297915353359"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924567_p164881130154211"><a name="zh-cn_topic_0118924567_p164881130154211"></a><a name="zh-cn_topic_0118924567_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924567_row697910358354"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924567_p169794352358"><a name="zh-cn_topic_0118924567_p169794352358"></a><a name="zh-cn_topic_0118924567_p169794352358"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924567_p1848810308429"><a name="zh-cn_topic_0118924567_p1848810308429"></a><a name="zh-cn_topic_0118924567_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924567_row097943523513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924567_p16979133533513"><a name="zh-cn_topic_0118924567_p16979133533513"></a><a name="zh-cn_topic_0118924567_p16979133533513"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924567_p10488193018426"><a name="zh-cn_topic_0118924567_p10488193018426"></a><a name="zh-cn_topic_0118924567_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924567_row797919352351"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924567_p1397911359350"><a name="zh-cn_topic_0118924567_p1397911359350"></a><a name="zh-cn_topic_0118924567_p1397911359350"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924567_p4488103094212"><a name="zh-cn_topic_0118924567_p4488103094212"></a><a name="zh-cn_topic_0118924567_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924567_row1979135163515"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924567_p11979153512359"><a name="zh-cn_topic_0118924567_p11979153512359"></a><a name="zh-cn_topic_0118924567_p11979153512359"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924567_p6744143"><a name="zh-cn_topic_0118924567_p6744143"></a><a name="zh-cn_topic_0118924567_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

