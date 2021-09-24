# HTTP状态码<a name="ZH-CN_TOPIC_0000001082221317"></a>

常用状态码表如[表1](#zh-cn_topic_0172449737_table11812530035)所示。

**表 1**  HTTP请求状态返回码

<a name="zh-cn_topic_0172449737_table11812530035"></a>
<table><thead align="left"><tr id="zh-cn_topic_0172449737_row9812123010311"><th class="cellrowborder" valign="top" width="28.999999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0172449737_p581216302032"><a name="zh-cn_topic_0172449737_p581216302032"></a><a name="zh-cn_topic_0172449737_p581216302032"></a>返回值</p>
</th>
<th class="cellrowborder" valign="top" width="71%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0172449737_p1581214303317"><a name="zh-cn_topic_0172449737_p1581214303317"></a><a name="zh-cn_topic_0172449737_p1581214303317"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0172449737_row88125307316"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p11812430435"><a name="zh-cn_topic_0172449737_p11812430435"></a><a name="zh-cn_topic_0172449737_p11812430435"></a>200 OK</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p5812153017318"><a name="zh-cn_topic_0172449737_p5812153017318"></a><a name="zh-cn_topic_0172449737_p5812153017318"></a>处理正常。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row181212307316"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p198122302311"><a name="zh-cn_topic_0172449737_p198122302311"></a><a name="zh-cn_topic_0172449737_p198122302311"></a>204 No Content</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p4812930139"><a name="zh-cn_topic_0172449737_p4812930139"></a><a name="zh-cn_topic_0172449737_p4812930139"></a>无返回内容。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row581213305320"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p19812153018318"><a name="zh-cn_topic_0172449737_p19812153018318"></a><a name="zh-cn_topic_0172449737_p19812153018318"></a>400 Bad Request</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p1857918225217"><a name="zh-cn_topic_0172449737_p1857918225217"></a><a name="zh-cn_topic_0172449737_p1857918225217"></a>服务器未能处理请求。可能原因：</p>
<a name="zh-cn_topic_0172449737_ol11564122217211"></a><a name="zh-cn_topic_0172449737_ol11564122217211"></a><ol id="zh-cn_topic_0172449737_ol11564122217211"><li>语义有误，当前请求无法被服务器解析；</li><li>请求参数有误。</li></ol>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row781273013311"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p88121730735"><a name="zh-cn_topic_0172449737_p88121730735"></a><a name="zh-cn_topic_0172449737_p88121730735"></a>401 Unauthorized</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p138128301738"><a name="zh-cn_topic_0172449737_p138128301738"></a><a name="zh-cn_topic_0172449737_p138128301738"></a>当前请求需要用户验证。如需要用户名和密码。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row38129301312"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p12812123018318"><a name="zh-cn_topic_0172449737_p12812123018318"></a><a name="zh-cn_topic_0172449737_p12812123018318"></a>403 Forbidden</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p6812133010315"><a name="zh-cn_topic_0172449737_p6812133010315"></a><a name="zh-cn_topic_0172449737_p6812133010315"></a>对被请求页面的访问被禁止。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row8812133012318"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p188121530331"><a name="zh-cn_topic_0172449737_p188121530331"></a><a name="zh-cn_topic_0172449737_p188121530331"></a>404 Not Found</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p6812163012317"><a name="zh-cn_topic_0172449737_p6812163012317"></a><a name="zh-cn_topic_0172449737_p6812163012317"></a>请求失败，在服务器上未找到请求所希望得到的资源。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row1481212304316"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p128121930631"><a name="zh-cn_topic_0172449737_p128121930631"></a><a name="zh-cn_topic_0172449737_p128121930631"></a>405 Method Not Allowed</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p14812730536"><a name="zh-cn_topic_0172449737_p14812730536"></a><a name="zh-cn_topic_0172449737_p14812730536"></a>请求行中指定的请求方法不能被用于请求相应的资源。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row16812530536"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p981211301319"><a name="zh-cn_topic_0172449737_p981211301319"></a><a name="zh-cn_topic_0172449737_p981211301319"></a>406 Not Acceptable</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p1581217301832"><a name="zh-cn_topic_0172449737_p1581217301832"></a><a name="zh-cn_topic_0172449737_p1581217301832"></a>服务器生成的响应无法被客户端所接受。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row7812130034"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p8812630636"><a name="zh-cn_topic_0172449737_p8812630636"></a><a name="zh-cn_topic_0172449737_p8812630636"></a>407 Proxy Authentication Required</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p1812113018316"><a name="zh-cn_topic_0172449737_p1812113018316"></a><a name="zh-cn_topic_0172449737_p1812113018316"></a>用户必须首先使用代理服务器进行验证，这样请求才会被处理。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row781218301317"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p1081223013311"><a name="zh-cn_topic_0172449737_p1081223013311"></a><a name="zh-cn_topic_0172449737_p1081223013311"></a>408 Request Timeout</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p481311301632"><a name="zh-cn_topic_0172449737_p481311301632"></a><a name="zh-cn_topic_0172449737_p481311301632"></a>请求超出了服务器的等待时间。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row3813830337"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p18813153014315"><a name="zh-cn_topic_0172449737_p18813153014315"></a><a name="zh-cn_topic_0172449737_p18813153014315"></a>409 Conflict</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p138138305312"><a name="zh-cn_topic_0172449737_p138138305312"></a><a name="zh-cn_topic_0172449737_p138138305312"></a>由于和被请求的资源的当前状态之间存在冲突，请求无法完成。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row20813430832"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p8813113016319"><a name="zh-cn_topic_0172449737_p8813113016319"></a><a name="zh-cn_topic_0172449737_p8813113016319"></a>410 Gone</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p1681353016313"><a name="zh-cn_topic_0172449737_p1681353016313"></a><a name="zh-cn_topic_0172449737_p1681353016313"></a>被请求的资源在服务器上已经不再可用，并且没有任何已知的转发地址。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row1813630533"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p0813630238"><a name="zh-cn_topic_0172449737_p0813630238"></a><a name="zh-cn_topic_0172449737_p0813630238"></a>412 Precondition Failed</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p68130301535"><a name="zh-cn_topic_0172449737_p68130301535"></a><a name="zh-cn_topic_0172449737_p68130301535"></a>服务器在验证在请求的头字段中给出先决条件时，未能满足其中的一个或多个。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row4813830332"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p198131230839"><a name="zh-cn_topic_0172449737_p198131230839"></a><a name="zh-cn_topic_0172449737_p198131230839"></a>500 Internal Server Error</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p158131830431"><a name="zh-cn_topic_0172449737_p158131830431"></a><a name="zh-cn_topic_0172449737_p158131830431"></a>服务器遇到了一个未曾预料的状况，导致无法完成对请求的处理。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row581312302312"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p1081393018315"><a name="zh-cn_topic_0172449737_p1081393018315"></a><a name="zh-cn_topic_0172449737_p1081393018315"></a>501 Not Implemented</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p1681333017319"><a name="zh-cn_topic_0172449737_p1681333017319"></a><a name="zh-cn_topic_0172449737_p1681333017319"></a>请求未完成。服务器不支持所请求的功能。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row168131830135"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p481319301310"><a name="zh-cn_topic_0172449737_p481319301310"></a><a name="zh-cn_topic_0172449737_p481319301310"></a>502 Bad Gateway</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p188132300316"><a name="zh-cn_topic_0172449737_p188132300316"></a><a name="zh-cn_topic_0172449737_p188132300316"></a>请求未完成。服务器从上游服务器收到一个无效的响应。</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row158131330231"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p12813530636"><a name="zh-cn_topic_0172449737_p12813530636"></a><a name="zh-cn_topic_0172449737_p12813530636"></a>503 Service Unavailable</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p1581314301330"><a name="zh-cn_topic_0172449737_p1581314301330"></a><a name="zh-cn_topic_0172449737_p1581314301330"></a>由于服务器临时维护或者过载，服务器当前无法处理请求</p>
</td>
</tr>
<tr id="zh-cn_topic_0172449737_row98135302033"><td class="cellrowborder" valign="top" width="28.999999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0172449737_p13813183014312"><a name="zh-cn_topic_0172449737_p13813183014312"></a><a name="zh-cn_topic_0172449737_p13813183014312"></a>504 Gateway Timeout</p>
</td>
<td class="cellrowborder" valign="top" width="71%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0172449737_p1481373019313"><a name="zh-cn_topic_0172449737_p1481373019313"></a><a name="zh-cn_topic_0172449737_p1481373019313"></a>网关超时。</p>
</td>
</tr>
</tbody>
</table>

