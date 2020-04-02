# 创建App Code<a name="apig-phapi-200226001"></a>

## 功能介绍<a name="zh-cn_topic_0118921764_section48433431"></a>

App Code为APP应用下的子模块，创建App Code之后，可以实现简易的APP认证。

## URI<a name="section3288343175318"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921764_table33538507"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921764_row26439774"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921764_p61246963"><a name="zh-cn_topic_0118921764_p61246963"></a><a name="zh-cn_topic_0118921764_p61246963"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921764_p62056956"><a name="zh-cn_topic_0118921764_p62056956"></a><a name="zh-cn_topic_0118921764_p62056956"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921764_row60557538"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921764_p6213516"><a name="zh-cn_topic_0118921764_p6213516"></a><a name="zh-cn_topic_0118921764_p6213516"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921764_p33532770"><a name="zh-cn_topic_0118921764_p33532770"></a><a name="zh-cn_topic_0118921764_p33532770"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps/{app_id}/app-codes</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921763_table8767205"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row50080004"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921763_p29948539"><a name="zh-cn_topic_0118921763_p29948539"></a><a name="zh-cn_topic_0118921763_p29948539"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921763_p9912623"><a name="zh-cn_topic_0118921763_p9912623"></a><a name="zh-cn_topic_0118921763_p9912623"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921763_p64724999"><a name="zh-cn_topic_0118921763_p64724999"></a><a name="zh-cn_topic_0118921763_p64724999"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921763_p8233580"><a name="zh-cn_topic_0118921763_p8233580"></a><a name="zh-cn_topic_0118921763_p8233580"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1122717391119"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row84904365114"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row943312981910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p24341599197"><a name="p24341599197"></a><a name="p24341599197"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p5434290195"><a name="p5434290195"></a><a name="p5434290195"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p543529161911"><a name="p543529161911"></a><a name="p543529161911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p19435996196"><a name="p19435996196"></a><a name="p19435996196"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section6311133695620"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921758_table12551817"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921758_row63926902"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921758_p10696570"><a name="zh-cn_topic_0118921758_p10696570"></a><a name="zh-cn_topic_0118921758_p10696570"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.13%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921758_p61115871"><a name="zh-cn_topic_0118921758_p61115871"></a><a name="zh-cn_topic_0118921758_p61115871"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921758_p51438541"><a name="zh-cn_topic_0118921758_p51438541"></a><a name="zh-cn_topic_0118921758_p51438541"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.58%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921758_p5772267"><a name="zh-cn_topic_0118921758_p5772267"></a><a name="zh-cn_topic_0118921758_p5772267"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921758_row64900449"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118921758_p22445016"><a name="zh-cn_topic_0118921758_p22445016"></a><a name="zh-cn_topic_0118921758_p22445016"></a>app_code</p>
</td>
<td class="cellrowborder" valign="top" width="13.13%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118921758_p6106999"><a name="zh-cn_topic_0118921758_p6106999"></a><a name="zh-cn_topic_0118921758_p6106999"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118921758_p24904935"><a name="zh-cn_topic_0118921758_p24904935"></a><a name="zh-cn_topic_0118921758_p24904935"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.58%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118921758_p4033872"><a name="zh-cn_topic_0118921758_p4033872"></a><a name="zh-cn_topic_0118921758_p4033872"></a>APP的名称</p>
<p id="zh-cn_topic_0118921758_p55011617"><a name="zh-cn_topic_0118921758_p55011617"></a><a name="zh-cn_topic_0118921758_p55011617"></a>支持英文，+_!@#$%+/=，且只能以英文和+、/开头，64-180个字符。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "app_code": "GjOD3g80AABuuFeEJpVQADBlAjBh3UzC7W+gr4VJBB5BtJ4fdVOQoSvoji3gFxUDb5pWBz9wUcw9+8/bFZ1B/4pq29wCMQC0pQWX6zTndljDEl99As1pw+WntAU9xcq+ffagoH6zDpKUvdxV6Ezj8LcCcPZN6BU="
}
```

## 响应消息<a name="zh-cn_topic_0118921758_section15267056"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0118921758_table20910139"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921758_row9919741"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921758_p65301594"><a name="zh-cn_topic_0118921758_p65301594"></a><a name="zh-cn_topic_0118921758_p65301594"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921758_p54937751"><a name="zh-cn_topic_0118921758_p54937751"></a><a name="zh-cn_topic_0118921758_p54937751"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921758_p20772828"><a name="zh-cn_topic_0118921758_p20772828"></a><a name="zh-cn_topic_0118921758_p20772828"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921758_row4877522"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p59535008"><a name="zh-cn_topic_0118921758_p59535008"></a><a name="zh-cn_topic_0118921758_p59535008"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p57606383"><a name="zh-cn_topic_0118921758_p57606383"></a><a name="zh-cn_topic_0118921758_p57606383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p35605479"><a name="zh-cn_topic_0118921758_p35605479"></a><a name="zh-cn_topic_0118921758_p35605479"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row52013857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p52372904"><a name="zh-cn_topic_0118921758_p52372904"></a><a name="zh-cn_topic_0118921758_p52372904"></a>app_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p14346860"><a name="zh-cn_topic_0118921758_p14346860"></a><a name="zh-cn_topic_0118921758_p14346860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p21245012"><a name="zh-cn_topic_0118921758_p21245012"></a><a name="zh-cn_topic_0118921758_p21245012"></a>App Code值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row56987385"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p52575507"><a name="zh-cn_topic_0118921758_p52575507"></a><a name="zh-cn_topic_0118921758_p52575507"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p30757702"><a name="zh-cn_topic_0118921758_p30757702"></a><a name="zh-cn_topic_0118921758_p30757702"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1284315287524"><a name="p1284315287524"></a><a name="p1284315287524"></a>APP的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row8004354"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p44372920"><a name="zh-cn_topic_0118921758_p44372920"></a><a name="zh-cn_topic_0118921758_p44372920"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p37436804"><a name="zh-cn_topic_0118921758_p37436804"></a><a name="zh-cn_topic_0118921758_p37436804"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p12482251"><a name="zh-cn_topic_0118921758_p12482251"></a><a name="zh-cn_topic_0118921758_p12482251"></a>创建时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
    "app_code": "GjOD3g80AABuuFeEJpVQADBlAjBh3UzC7W+gr4VJBB5BtJ4fdVOQoSvoji3gFxUDb5pWBz9wUcw9+8/bFZ1B/4pq29wCMQC0pQWX6zTndljDEl99As1pw+WntAU9xcq+ffagoH6zDpKUvdxV6Ezj8LcCcPZN6BU=",
    "id": "2fb07c4391d0401696ed345dd1229158",
    "app_id": "db246f3f2ecd45f29ecb0f305e821fdc",
    "create_time": "2019-06-05T04:57:14.470987604Z"
}
```

## 状态码<a name="zh-cn_topic_0118921758_section38979041"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118921758_table665003"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921758_row9107269"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921758_p66600187"><a name="zh-cn_topic_0118921758_p66600187"></a><a name="zh-cn_topic_0118921758_p66600187"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921758_p25906037"><a name="zh-cn_topic_0118921758_p25906037"></a><a name="zh-cn_topic_0118921758_p25906037"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921758_row18014235"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921758_p49866967"><a name="zh-cn_topic_0118921758_p49866967"></a><a name="zh-cn_topic_0118921758_p49866967"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921758_p12692494"><a name="zh-cn_topic_0118921758_p12692494"></a><a name="zh-cn_topic_0118921758_p12692494"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row47123588"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921758_p58914306"><a name="zh-cn_topic_0118921758_p58914306"></a><a name="zh-cn_topic_0118921758_p58914306"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921758_p7329456"><a name="zh-cn_topic_0118921758_p7329456"></a><a name="zh-cn_topic_0118921758_p7329456"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row65965104"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921758_p41573226"><a name="zh-cn_topic_0118921758_p41573226"></a><a name="zh-cn_topic_0118921758_p41573226"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921758_p9203142078"><a name="zh-cn_topic_0118921758_p9203142078"></a><a name="zh-cn_topic_0118921758_p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row40784364"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921758_p15199212"><a name="zh-cn_topic_0118921758_p15199212"></a><a name="zh-cn_topic_0118921758_p15199212"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921758_p13949586"><a name="zh-cn_topic_0118921758_p13949586"></a><a name="zh-cn_topic_0118921758_p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921758_row7263502"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921758_p51472750"><a name="zh-cn_topic_0118921758_p51472750"></a><a name="zh-cn_topic_0118921758_p51472750"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921758_p8543194"><a name="zh-cn_topic_0118921758_p8543194"></a><a name="zh-cn_topic_0118921758_p8543194"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

