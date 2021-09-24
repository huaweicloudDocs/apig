# 查询API概况<a name="ZH-CN_TOPIC_0000001081976137"></a>

## 功能介绍<a name="zh-cn_topic_0118924543_section28347717"></a>

查询租户名下的API概况：已发布到RELEASE环境的API个数，未发布到RELEASE环境的API个数。

## URI<a name="zh-cn_topic_0118924543_section53802865"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924543_table19999857"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924543_row42622880"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924543_p29901289"><a name="zh-cn_topic_0118924543_p29901289"></a><a name="zh-cn_topic_0118924543_p29901289"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924543_p6085350"><a name="zh-cn_topic_0118924543_p6085350"></a><a name="zh-cn_topic_0118924543_p6085350"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924543_row23151360"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924543_p63320862"><a name="zh-cn_topic_0118924543_p63320862"></a><a name="zh-cn_topic_0118924543_p63320862"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924543_p28716201"><a name="zh-cn_topic_0118924543_p28716201"></a><a name="zh-cn_topic_0118924543_p28716201"></a>/v1.0/apigw/resources/outline/apis</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924543_section14463741"></a>

无

## 响应消息<a name="zh-cn_topic_0118924543_section30712386"></a>

**表 2**  参数说明

<a name="zh-cn_topic_0118924543_table12714810"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924543_row21779198"><th class="cellrowborder" valign="top" width="24.240000000000002%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924543_p19284637"><a name="zh-cn_topic_0118924543_p19284637"></a><a name="zh-cn_topic_0118924543_p19284637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924543_p18551760"><a name="zh-cn_topic_0118924543_p18551760"></a><a name="zh-cn_topic_0118924543_p18551760"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60.61%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924543_p26297600"><a name="zh-cn_topic_0118924543_p26297600"></a><a name="zh-cn_topic_0118924543_p26297600"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924543_row18344121603916"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924543_p1434581618398"><a name="zh-cn_topic_0118924543_p1434581618398"></a><a name="zh-cn_topic_0118924543_p1434581618398"></a>instance_num</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924543_p6345191653913"><a name="zh-cn_topic_0118924543_p6345191653913"></a><a name="zh-cn_topic_0118924543_p6345191653913"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924543_p634551693910"><a name="zh-cn_topic_0118924543_p634551693910"></a><a name="zh-cn_topic_0118924543_p634551693910"></a>API总个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924543_row49730836"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924543_p1665909"><a name="zh-cn_topic_0118924543_p1665909"></a><a name="zh-cn_topic_0118924543_p1665909"></a>nums_off_release</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924543_p720906"><a name="zh-cn_topic_0118924543_p720906"></a><a name="zh-cn_topic_0118924543_p720906"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924543_p58393403"><a name="zh-cn_topic_0118924543_p58393403"></a><a name="zh-cn_topic_0118924543_p58393403"></a>未发布到release环境的API个数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924543_row55778586"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924543_p21771650"><a name="zh-cn_topic_0118924543_p21771650"></a><a name="zh-cn_topic_0118924543_p21771650"></a>nums_on_release</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924543_p18673210"><a name="zh-cn_topic_0118924543_p18673210"></a><a name="zh-cn_topic_0118924543_p18673210"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924543_p36135018"><a name="zh-cn_topic_0118924543_p36135018"></a><a name="zh-cn_topic_0118924543_p36135018"></a>已发布到release环境的API个数</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"instance_num": 3,"nums_off_release": 1,
	"nums_on_release": 2
}
```

## 状态码<a name="zh-cn_topic_0118924543_section63064810"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0118924543_table15538229"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924543_row4507722"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924543_p29581215"><a name="zh-cn_topic_0118924543_p29581215"></a><a name="zh-cn_topic_0118924543_p29581215"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924543_p47268200"><a name="zh-cn_topic_0118924543_p47268200"></a><a name="zh-cn_topic_0118924543_p47268200"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924543_row3518990"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924543_p16602744"><a name="zh-cn_topic_0118924543_p16602744"></a><a name="zh-cn_topic_0118924543_p16602744"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924543_p50988816"><a name="zh-cn_topic_0118924543_p50988816"></a><a name="zh-cn_topic_0118924543_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924543_row23805062"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924543_p49161866"><a name="zh-cn_topic_0118924543_p49161866"></a><a name="zh-cn_topic_0118924543_p49161866"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924543_p22688239"><a name="zh-cn_topic_0118924543_p22688239"></a><a name="zh-cn_topic_0118924543_p22688239"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924543_row2867565"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924543_p30946246"><a name="zh-cn_topic_0118924543_p30946246"></a><a name="zh-cn_topic_0118924543_p30946246"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924543_p23618003"><a name="zh-cn_topic_0118924543_p23618003"></a><a name="zh-cn_topic_0118924543_p23618003"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924543_row11235441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924543_p37655528"><a name="zh-cn_topic_0118924543_p37655528"></a><a name="zh-cn_topic_0118924543_p37655528"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924543_p13949586"><a name="zh-cn_topic_0118924543_p13949586"></a><a name="zh-cn_topic_0118924543_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924543_row3354822"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924543_p3305141"><a name="zh-cn_topic_0118924543_p3305141"></a><a name="zh-cn_topic_0118924543_p3305141"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924543_p6744143"><a name="zh-cn_topic_0118924543_p6744143"></a><a name="zh-cn_topic_0118924543_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

