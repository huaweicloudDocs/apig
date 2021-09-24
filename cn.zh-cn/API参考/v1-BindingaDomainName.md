# 绑定域名<a name="ZH-CN_TOPIC_0000001081976219"></a>

## 功能介绍<a name="zh-cn_topic_0225568970_section173482301428"></a>

用户自定义的域名，需要CNAME到API分组的子域名上才能生效，具体方法请参见[增加CNAME类型记录集](https://support.huaweicloud.com/usermanual-dns/dns_usermanual_0010.html)。

每个API分组下最多可绑定5个域名。绑定域名后，用户可通过自定义域名调用API。

## URI<a name="zh-cn_topic_0225568970_section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568970_table1439319294431"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568970_row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568970_p14361448204314"><a name="zh-cn_topic_0225568970_p14361448204314"></a><a name="zh-cn_topic_0225568970_p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568970_p1936174864316"><a name="zh-cn_topic_0225568970_p1936174864316"></a><a name="zh-cn_topic_0225568970_p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568970_row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568970_p1236111482435"><a name="zh-cn_topic_0225568970_p1236111482435"></a><a name="zh-cn_topic_0225568970_p1236111482435"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568970_p11361848184318"><a name="zh-cn_topic_0225568970_p11361848184318"></a><a name="zh-cn_topic_0225568970_p11361848184318"></a>/v1/{project_id}/apigw/instances/{instance_id}/api-groups/{group_id}/domains</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568970_table339495"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568970_row19182484"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568970_p10277368"><a name="zh-cn_topic_0225568970_p10277368"></a><a name="zh-cn_topic_0225568970_p10277368"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568970_p27160509"><a name="zh-cn_topic_0225568970_p27160509"></a><a name="zh-cn_topic_0225568970_p27160509"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568970_p52517643"><a name="zh-cn_topic_0225568970_p52517643"></a><a name="zh-cn_topic_0225568970_p52517643"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568970_p26070665"><a name="zh-cn_topic_0225568970_p26070665"></a><a name="zh-cn_topic_0225568970_p26070665"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568970_row16106756165415"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568970_p55878963"><a name="zh-cn_topic_0225568970_p55878963"></a><a name="zh-cn_topic_0225568970_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568970_p29902160"><a name="zh-cn_topic_0225568970_p29902160"></a><a name="zh-cn_topic_0225568970_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568970_p6155914"><a name="zh-cn_topic_0225568970_p6155914"></a><a name="zh-cn_topic_0225568970_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568970_p28867016"><a name="zh-cn_topic_0225568970_p28867016"></a><a name="zh-cn_topic_0225568970_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row17547655125413"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568970_p1780913159538"><a name="zh-cn_topic_0225568970_p1780913159538"></a><a name="zh-cn_topic_0225568970_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568970_p9809215115310"><a name="zh-cn_topic_0225568970_p9809215115310"></a><a name="zh-cn_topic_0225568970_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568970_p1280914152538"><a name="zh-cn_topic_0225568970_p1280914152538"></a><a name="zh-cn_topic_0225568970_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568970_p1880914157537"><a name="zh-cn_topic_0225568970_p1880914157537"></a><a name="zh-cn_topic_0225568970_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row31349087"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568970_p56248118"><a name="zh-cn_topic_0225568970_p56248118"></a><a name="zh-cn_topic_0225568970_p56248118"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568970_p59803701"><a name="zh-cn_topic_0225568970_p59803701"></a><a name="zh-cn_topic_0225568970_p59803701"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568970_p12261637"><a name="zh-cn_topic_0225568970_p12261637"></a><a name="zh-cn_topic_0225568970_p12261637"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568970_p53668558"><a name="zh-cn_topic_0225568970_p53668558"></a><a name="zh-cn_topic_0225568970_p53668558"></a>分组的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568970_section73637302425"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568970_table1136319301429"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568970_row748813306425"><th class="cellrowborder" valign="top" width="15.46154615461546%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568970_p9488143084210"><a name="zh-cn_topic_0225568970_p9488143084210"></a><a name="zh-cn_topic_0225568970_p9488143084210"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568970_p148843017426"><a name="zh-cn_topic_0225568970_p148843017426"></a><a name="zh-cn_topic_0225568970_p148843017426"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568970_p9488830164214"><a name="zh-cn_topic_0225568970_p9488830164214"></a><a name="zh-cn_topic_0225568970_p9488830164214"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568970_p1048813014421"><a name="zh-cn_topic_0225568970_p1048813014421"></a><a name="zh-cn_topic_0225568970_p1048813014421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568970_row048883014426"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568970_p448819305424"><a name="zh-cn_topic_0225568970_p448819305424"></a><a name="zh-cn_topic_0225568970_p448819305424"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568970_p94882308421"><a name="zh-cn_topic_0225568970_p94882308421"></a><a name="zh-cn_topic_0225568970_p94882308421"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568970_p248893016423"><a name="zh-cn_topic_0225568970_p248893016423"></a><a name="zh-cn_topic_0225568970_p248893016423"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568970_p17713871468"><a name="zh-cn_topic_0225568970_p17713871468"></a><a name="zh-cn_topic_0225568970_p17713871468"></a>自定义域名。</p>
<p id="zh-cn_topic_0225568970_p948883074219"><a name="zh-cn_topic_0225568970_p948883074219"></a><a name="zh-cn_topic_0225568970_p948883074219"></a>长度为0-255位的字符串，需要符合域名规范。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
   "url_domain": "www.MyCompany.com"
}
```

## 响应消息<a name="zh-cn_topic_0225568970_section9395153012420"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568970_table7395123013420"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568970_row114881330104215"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568970_p19488153019429"><a name="zh-cn_topic_0225568970_p19488153019429"></a><a name="zh-cn_topic_0225568970_p19488153019429"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568970_p248853014422"><a name="zh-cn_topic_0225568970_p248853014422"></a><a name="zh-cn_topic_0225568970_p248853014422"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568970_p64882308421"><a name="zh-cn_topic_0225568970_p64882308421"></a><a name="zh-cn_topic_0225568970_p64882308421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568970_row12488203074215"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568970_p1448813305421"><a name="zh-cn_topic_0225568970_p1448813305421"></a><a name="zh-cn_topic_0225568970_p1448813305421"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568970_p18488163024218"><a name="zh-cn_topic_0225568970_p18488163024218"></a><a name="zh-cn_topic_0225568970_p18488163024218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568970_p94886306423"><a name="zh-cn_topic_0225568970_p94886306423"></a><a name="zh-cn_topic_0225568970_p94886306423"></a>域名的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row17488133012421"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568970_p2488113017427"><a name="zh-cn_topic_0225568970_p2488113017427"></a><a name="zh-cn_topic_0225568970_p2488113017427"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568970_p4488183013424"><a name="zh-cn_topic_0225568970_p4488183013424"></a><a name="zh-cn_topic_0225568970_p4488183013424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568970_p04888306421"><a name="zh-cn_topic_0225568970_p04888306421"></a><a name="zh-cn_topic_0225568970_p04888306421"></a>自定义域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row748812305426"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568970_p124888301424"><a name="zh-cn_topic_0225568970_p124888301424"></a><a name="zh-cn_topic_0225568970_p124888301424"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568970_p64881305424"><a name="zh-cn_topic_0225568970_p64881305424"></a><a name="zh-cn_topic_0225568970_p64881305424"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568970_p2488103044219"><a name="zh-cn_topic_0225568970_p2488103044219"></a><a name="zh-cn_topic_0225568970_p2488103044219"></a>CNAME解析状态</p>
<a name="zh-cn_topic_0225568970_ul53721145134416"></a><a name="zh-cn_topic_0225568970_ul53721145134416"></a><ul id="zh-cn_topic_0225568970_ul53721145134416"><li>1 未解析</li><li>2 解析中</li><li>3 解析成功</li><li>4 解析失败</li></ul>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "c5e0d5ba62a34d26ad5c709ae22c1a17",
	"url_domain": "www.MyCompany.com",
	"status": 3
}
```

## 状态码<a name="zh-cn_topic_0225568970_section338043011426"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568970_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568970_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568970_p174881730194216"><a name="zh-cn_topic_0225568970_p174881730194216"></a><a name="zh-cn_topic_0225568970_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568970_p848863018429"><a name="zh-cn_topic_0225568970_p848863018429"></a><a name="zh-cn_topic_0225568970_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568970_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568970_p7488163084211"><a name="zh-cn_topic_0225568970_p7488163084211"></a><a name="zh-cn_topic_0225568970_p7488163084211"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568970_p948803015424"><a name="zh-cn_topic_0225568970_p948803015424"></a><a name="zh-cn_topic_0225568970_p948803015424"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568970_p14488113015426"><a name="zh-cn_topic_0225568970_p14488113015426"></a><a name="zh-cn_topic_0225568970_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568970_p164881130154211"><a name="zh-cn_topic_0225568970_p164881130154211"></a><a name="zh-cn_topic_0225568970_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568970_p24883304428"><a name="zh-cn_topic_0225568970_p24883304428"></a><a name="zh-cn_topic_0225568970_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568970_p1848810308429"><a name="zh-cn_topic_0225568970_p1848810308429"></a><a name="zh-cn_topic_0225568970_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568970_p6488133064210"><a name="zh-cn_topic_0225568970_p6488133064210"></a><a name="zh-cn_topic_0225568970_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568970_p10488193018426"><a name="zh-cn_topic_0225568970_p10488193018426"></a><a name="zh-cn_topic_0225568970_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568970_p144883304428"><a name="zh-cn_topic_0225568970_p144883304428"></a><a name="zh-cn_topic_0225568970_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568970_p4488103094212"><a name="zh-cn_topic_0225568970_p4488103094212"></a><a name="zh-cn_topic_0225568970_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568970_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568970_p17488163014423"><a name="zh-cn_topic_0225568970_p17488163014423"></a><a name="zh-cn_topic_0225568970_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568970_p048813014216"><a name="zh-cn_topic_0225568970_p048813014216"></a><a name="zh-cn_topic_0225568970_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

