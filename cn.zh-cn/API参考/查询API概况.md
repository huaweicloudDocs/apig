# 查询API概况<a name="apig-zh-api-180713131"></a>

## 功能介绍<a name="section28347717"></a>

查询租户名下的API概况：已发布到RELEASE环境的API个数，未发布到RELEASE环境的API个数。

## URI<a name="section53802865"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table19999857"></a>
<table><thead align="left"><tr id="row42622880"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p29901289"><a name="p29901289"></a><a name="p29901289"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p6085350"><a name="p6085350"></a><a name="p6085350"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row23151360"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p63320862"><a name="p63320862"></a><a name="p63320862"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p28716201"><a name="p28716201"></a><a name="p28716201"></a>/v1.0/apigw/resources/outline/apis</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section14463741"></a>

无

## 响应消息<a name="section30712386"></a>

**表 2**  参数说明

<a name="table12714810"></a>
<table><thead align="left"><tr id="row21779198"><th class="cellrowborder" valign="top" width="24.240000000000002%" id="mcps1.2.4.1.1"><p id="p19284637"><a name="p19284637"></a><a name="p19284637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.4.1.2"><p id="p18551760"><a name="p18551760"></a><a name="p18551760"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60.61%" id="mcps1.2.4.1.3"><p id="p26297600"><a name="p26297600"></a><a name="p26297600"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18344121603916"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="p1434581618398"><a name="p1434581618398"></a><a name="p1434581618398"></a>instance_num</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.4.1.2 "><p id="p6345191653913"><a name="p6345191653913"></a><a name="p6345191653913"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="p634551693910"><a name="p634551693910"></a><a name="p634551693910"></a>API总个数</p>
</td>
</tr>
<tr id="row49730836"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="p1665909"><a name="p1665909"></a><a name="p1665909"></a>nums_off_release</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.4.1.2 "><p id="p720906"><a name="p720906"></a><a name="p720906"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="p58393403"><a name="p58393403"></a><a name="p58393403"></a>未发布到release环境的API个数</p>
</td>
</tr>
<tr id="row55778586"><td class="cellrowborder" valign="top" width="24.240000000000002%" headers="mcps1.2.4.1.1 "><p id="p21771650"><a name="p21771650"></a><a name="p21771650"></a>nums_on_release</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.4.1.2 "><p id="p18673210"><a name="p18673210"></a><a name="p18673210"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60.61%" headers="mcps1.2.4.1.3 "><p id="p36135018"><a name="p36135018"></a><a name="p36135018"></a>已发布到release环境的API个数</p>
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

## 状态码<a name="section63064810"></a>

**表 3**  返回消息说明

<a name="table15538229"></a>
<table><thead align="left"><tr id="row4507722"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p29581215"><a name="p29581215"></a><a name="p29581215"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p47268200"><a name="p47268200"></a><a name="p47268200"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3518990"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p16602744"><a name="p16602744"></a><a name="p16602744"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50988816"><a name="p50988816"></a><a name="p50988816"></a>OK</p>
</td>
</tr>
<tr id="row23805062"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p49161866"><a name="p49161866"></a><a name="p49161866"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p22688239"><a name="p22688239"></a><a name="p22688239"></a>Bad Request</p>
</td>
</tr>
<tr id="row2867565"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p30946246"><a name="p30946246"></a><a name="p30946246"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p23618003"><a name="p23618003"></a><a name="p23618003"></a>Unauthorized</p>
</td>
</tr>
<tr id="row11235441"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p37655528"><a name="p37655528"></a><a name="p37655528"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row3354822"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3305141"><a name="p3305141"></a><a name="p3305141"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

