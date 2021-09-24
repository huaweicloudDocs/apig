# 删除域名证书<a name="ZH-CN_TOPIC_0000001081976147"></a>

## 功能介绍<a name="zh-cn_topic_0118924570_section38324262122"></a>

如果域名证书不再需要或者已过期，则可以删除证书内容。

## URI<a name="zh-cn_topic_0118924570_section12832162641216"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924570_table1396111510132"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924570_row096151515139"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924570_p1422722218139"><a name="zh-cn_topic_0118924570_p1422722218139"></a><a name="zh-cn_topic_0118924570_p1422722218139"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924570_p122713225131"><a name="zh-cn_topic_0118924570_p122713225131"></a><a name="zh-cn_topic_0118924570_p122713225131"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924570_row169611815131313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924570_p15227162219132"><a name="zh-cn_topic_0118924570_p15227162219132"></a><a name="zh-cn_topic_0118924570_p15227162219132"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924570_p1667817402181"><a name="zh-cn_topic_0118924570_p1667817402181"></a><a name="zh-cn_topic_0118924570_p1667817402181"></a>/v1.0/apigw/api-groups/{group_id}/domains/{domain_id}/certificate/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924570_table4851459153818"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924570_row1985259143813"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924570_p12367713193420"><a name="zh-cn_topic_0118924570_p12367713193420"></a><a name="zh-cn_topic_0118924570_p12367713193420"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924570_p7367161316343"><a name="zh-cn_topic_0118924570_p7367161316343"></a><a name="zh-cn_topic_0118924570_p7367161316343"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="24%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924570_p93675133347"><a name="zh-cn_topic_0118924570_p93675133347"></a><a name="zh-cn_topic_0118924570_p93675133347"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="26%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924570_p836761317349"><a name="zh-cn_topic_0118924570_p836761317349"></a><a name="zh-cn_topic_0118924570_p836761317349"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924570_row13944152316182"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924570_p56248118"><a name="zh-cn_topic_0118924570_p56248118"></a><a name="zh-cn_topic_0118924570_p56248118"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924570_p59803701"><a name="zh-cn_topic_0118924570_p59803701"></a><a name="zh-cn_topic_0118924570_p59803701"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924570_p12261637"><a name="zh-cn_topic_0118924570_p12261637"></a><a name="zh-cn_topic_0118924570_p12261637"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924570_p53668558"><a name="zh-cn_topic_0118924570_p53668558"></a><a name="zh-cn_topic_0118924570_p53668558"></a>分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924570_row21491627194614"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924570_p147479565365"><a name="zh-cn_topic_0118924570_p147479565365"></a><a name="zh-cn_topic_0118924570_p147479565365"></a>domain_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924570_p153301010123713"><a name="zh-cn_topic_0118924570_p153301010123713"></a><a name="zh-cn_topic_0118924570_p153301010123713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924570_p14330710143716"><a name="zh-cn_topic_0118924570_p14330710143716"></a><a name="zh-cn_topic_0118924570_p14330710143716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924570_p9747195653615"><a name="zh-cn_topic_0118924570_p9747195653615"></a><a name="zh-cn_topic_0118924570_p9747195653615"></a>域名的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924570_row18555915383"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924570_p111823311382"><a name="zh-cn_topic_0118924570_p111823311382"></a><a name="zh-cn_topic_0118924570_p111823311382"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924570_p163410335385"><a name="zh-cn_topic_0118924570_p163410335385"></a><a name="zh-cn_topic_0118924570_p163410335385"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924570_p83443318381"><a name="zh-cn_topic_0118924570_p83443318381"></a><a name="zh-cn_topic_0118924570_p83443318381"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924570_p3341333163817"><a name="zh-cn_topic_0118924570_p3341333163817"></a><a name="zh-cn_topic_0118924570_p3341333163817"></a>证书的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924570_section14272513203411"></a>

无

## 响应消息<a name="zh-cn_topic_0118924570_section1044114111321"></a>

无

## 状态码<a name="zh-cn_topic_0118924570_section2083573084114"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924570_table1083533064119"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924570_row879916303414"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924570_p1979933014119"><a name="zh-cn_topic_0118924570_p1979933014119"></a><a name="zh-cn_topic_0118924570_p1979933014119"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924570_p9799153064112"><a name="zh-cn_topic_0118924570_p9799153064112"></a><a name="zh-cn_topic_0118924570_p9799153064112"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924570_row1179918309413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924570_p1997963513513"><a name="zh-cn_topic_0118924570_p1997963513513"></a><a name="zh-cn_topic_0118924570_p1997963513513"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924570_p948803015424"><a name="zh-cn_topic_0118924570_p948803015424"></a><a name="zh-cn_topic_0118924570_p948803015424"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924570_row0799133014117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924570_p1179993034116"><a name="zh-cn_topic_0118924570_p1179993034116"></a><a name="zh-cn_topic_0118924570_p1179993034116"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924570_p164881130154211"><a name="zh-cn_topic_0118924570_p164881130154211"></a><a name="zh-cn_topic_0118924570_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924570_row1879983011414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924570_p15799230134110"><a name="zh-cn_topic_0118924570_p15799230134110"></a><a name="zh-cn_topic_0118924570_p15799230134110"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924570_p1117517539434"><a name="zh-cn_topic_0118924570_p1117517539434"></a><a name="zh-cn_topic_0118924570_p1117517539434"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924570_row8799143014412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924570_p19799630144115"><a name="zh-cn_topic_0118924570_p19799630144115"></a><a name="zh-cn_topic_0118924570_p19799630144115"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924570_p18177253114318"><a name="zh-cn_topic_0118924570_p18177253114318"></a><a name="zh-cn_topic_0118924570_p18177253114318"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924570_row2799113015413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924570_p167991530204113"><a name="zh-cn_topic_0118924570_p167991530204113"></a><a name="zh-cn_topic_0118924570_p167991530204113"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924570_p12179205319431"><a name="zh-cn_topic_0118924570_p12179205319431"></a><a name="zh-cn_topic_0118924570_p12179205319431"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924570_row67991330154113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924570_p57999309411"><a name="zh-cn_topic_0118924570_p57999309411"></a><a name="zh-cn_topic_0118924570_p57999309411"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924570_p31801353174319"><a name="zh-cn_topic_0118924570_p31801353174319"></a><a name="zh-cn_topic_0118924570_p31801353174319"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

