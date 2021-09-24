# 查询租户配置详情<a name="ZH-CN_TOPIC_0000001082221215"></a>

## 功能介绍<a name="zh-cn_topic_0118924531_section38675465"></a>

查询某个租户的配置项及其配置值。

## URI<a name="zh-cn_topic_0118924531_section12534867"></a>

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118924531_table11067778"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924531_row47996610"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924531_p62520192"><a name="zh-cn_topic_0118924531_p62520192"></a><a name="zh-cn_topic_0118924531_p62520192"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924531_p30970795"><a name="zh-cn_topic_0118924531_p30970795"></a><a name="zh-cn_topic_0118924531_p30970795"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924531_row25606442"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924531_p60855910"><a name="zh-cn_topic_0118924531_p60855910"></a><a name="zh-cn_topic_0118924531_p60855910"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924531_p30381638"><a name="zh-cn_topic_0118924531_p30381638"></a><a name="zh-cn_topic_0118924531_p30381638"></a>/v1.0/apigw/config/project[?page_size, page_no, config_id, config_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：config\_name、config\_id、page\_size、page\_no。

URI中的参数说明如下所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924531_table153783910507"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924531_row16537139165017"><th class="cellrowborder" valign="top" width="24%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924531_p15602124115112"><a name="zh-cn_topic_0118924531_p15602124115112"></a><a name="zh-cn_topic_0118924531_p15602124115112"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924531_p7602124205118"><a name="zh-cn_topic_0118924531_p7602124205118"></a><a name="zh-cn_topic_0118924531_p7602124205118"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924531_p860284175114"><a name="zh-cn_topic_0118924531_p860284175114"></a><a name="zh-cn_topic_0118924531_p860284175114"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="46%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924531_p14602847517"><a name="zh-cn_topic_0118924531_p14602847517"></a><a name="zh-cn_topic_0118924531_p14602847517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924531_row9537239165016"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924531_p661814175111"><a name="zh-cn_topic_0118924531_p661814175111"></a><a name="zh-cn_topic_0118924531_p661814175111"></a>config_name</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924531_p1261815413514"><a name="zh-cn_topic_0118924531_p1261815413514"></a><a name="zh-cn_topic_0118924531_p1261815413514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924531_p761815415518"><a name="zh-cn_topic_0118924531_p761815415518"></a><a name="zh-cn_topic_0118924531_p761815415518"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924531_p11618184105115"><a name="zh-cn_topic_0118924531_p11618184105115"></a><a name="zh-cn_topic_0118924531_p11618184105115"></a>配置项的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row1953793911505"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924531_p18618749515"><a name="zh-cn_topic_0118924531_p18618749515"></a><a name="zh-cn_topic_0118924531_p18618749515"></a>config_id</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924531_p1061811425120"><a name="zh-cn_topic_0118924531_p1061811425120"></a><a name="zh-cn_topic_0118924531_p1061811425120"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924531_p1261816435119"><a name="zh-cn_topic_0118924531_p1261816435119"></a><a name="zh-cn_topic_0118924531_p1261816435119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924531_p186180465112"><a name="zh-cn_topic_0118924531_p186180465112"></a><a name="zh-cn_topic_0118924531_p186180465112"></a>配置项的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row1370212259535"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924531_p11547235104514"><a name="zh-cn_topic_0118924531_p11547235104514"></a><a name="zh-cn_topic_0118924531_p11547235104514"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924531_p175471935164514"><a name="zh-cn_topic_0118924531_p175471935164514"></a><a name="zh-cn_topic_0118924531_p175471935164514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924531_p6547335194519"><a name="zh-cn_topic_0118924531_p6547335194519"></a><a name="zh-cn_topic_0118924531_p6547335194519"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924531_p656353511452"><a name="zh-cn_topic_0118924531_p656353511452"></a><a name="zh-cn_topic_0118924531_p656353511452"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row4280628105311"><td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924531_p175638354457"><a name="zh-cn_topic_0118924531_p175638354457"></a><a name="zh-cn_topic_0118924531_p175638354457"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924531_p3563153515450"><a name="zh-cn_topic_0118924531_p3563153515450"></a><a name="zh-cn_topic_0118924531_p3563153515450"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924531_p13563173574511"><a name="zh-cn_topic_0118924531_p13563173574511"></a><a name="zh-cn_topic_0118924531_p13563173574511"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="46%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924531_p185631735164520"><a name="zh-cn_topic_0118924531_p185631735164520"></a><a name="zh-cn_topic_0118924531_p185631735164520"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924531_section45704940"></a>

无

## 响应消息<a name="zh-cn_topic_0118924531_section11112631"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924531_table22835098"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924531_row28471799"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924531_p24514348"><a name="zh-cn_topic_0118924531_p24514348"></a><a name="zh-cn_topic_0118924531_p24514348"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924531_p39505149"><a name="zh-cn_topic_0118924531_p39505149"></a><a name="zh-cn_topic_0118924531_p39505149"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924531_p45800532"><a name="zh-cn_topic_0118924531_p45800532"></a><a name="zh-cn_topic_0118924531_p45800532"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924531_row18855574"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p50906541"><a name="zh-cn_topic_0118924531_p50906541"></a><a name="zh-cn_topic_0118924531_p50906541"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p29789185"><a name="zh-cn_topic_0118924531_p29789185"></a><a name="zh-cn_topic_0118924531_p29789185"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p64113785"><a name="zh-cn_topic_0118924531_p64113785"></a><a name="zh-cn_topic_0118924531_p64113785"></a>查询到的配置项总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row40153158"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p31180400"><a name="zh-cn_topic_0118924531_p31180400"></a><a name="zh-cn_topic_0118924531_p31180400"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p42584499"><a name="zh-cn_topic_0118924531_p42584499"></a><a name="zh-cn_topic_0118924531_p42584499"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p26792374"><a name="zh-cn_topic_0118924531_p26792374"></a><a name="zh-cn_topic_0118924531_p26792374"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row39804775"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p2961325"><a name="zh-cn_topic_0118924531_p2961325"></a><a name="zh-cn_topic_0118924531_p2961325"></a>configs</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p38540809"><a name="zh-cn_topic_0118924531_p38540809"></a><a name="zh-cn_topic_0118924531_p38540809"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p34797792"><a name="zh-cn_topic_0118924531_p34797792"></a><a name="zh-cn_topic_0118924531_p34797792"></a>本次查询返回的配置项列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  configs参数说明

<a name="zh-cn_topic_0118924531_table44744678"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924531_row29571772"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924531_p46503322"><a name="zh-cn_topic_0118924531_p46503322"></a><a name="zh-cn_topic_0118924531_p46503322"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924531_p8672741"><a name="zh-cn_topic_0118924531_p8672741"></a><a name="zh-cn_topic_0118924531_p8672741"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924531_p31403396"><a name="zh-cn_topic_0118924531_p31403396"></a><a name="zh-cn_topic_0118924531_p31403396"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924531_row60647136"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p13470944"><a name="zh-cn_topic_0118924531_p13470944"></a><a name="zh-cn_topic_0118924531_p13470944"></a>config_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p17404652"><a name="zh-cn_topic_0118924531_p17404652"></a><a name="zh-cn_topic_0118924531_p17404652"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p490733"><a name="zh-cn_topic_0118924531_p490733"></a><a name="zh-cn_topic_0118924531_p490733"></a>配置项的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row4416605"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p22200744"><a name="zh-cn_topic_0118924531_p22200744"></a><a name="zh-cn_topic_0118924531_p22200744"></a>config_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p53429852"><a name="zh-cn_topic_0118924531_p53429852"></a><a name="zh-cn_topic_0118924531_p53429852"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p32850719"><a name="zh-cn_topic_0118924531_p32850719"></a><a name="zh-cn_topic_0118924531_p32850719"></a>配置项的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row27221023"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p57419263"><a name="zh-cn_topic_0118924531_p57419263"></a><a name="zh-cn_topic_0118924531_p57419263"></a>config_value</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p20448707"><a name="zh-cn_topic_0118924531_p20448707"></a><a name="zh-cn_topic_0118924531_p20448707"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p45732564"><a name="zh-cn_topic_0118924531_p45732564"></a><a name="zh-cn_topic_0118924531_p45732564"></a>配置值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row8939892"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p53042658"><a name="zh-cn_topic_0118924531_p53042658"></a><a name="zh-cn_topic_0118924531_p53042658"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p1488081"><a name="zh-cn_topic_0118924531_p1488081"></a><a name="zh-cn_topic_0118924531_p1488081"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p53425769"><a name="zh-cn_topic_0118924531_p53425769"></a><a name="zh-cn_topic_0118924531_p53425769"></a>对配置项的描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row11069875"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924531_p24244698"><a name="zh-cn_topic_0118924531_p24244698"></a><a name="zh-cn_topic_0118924531_p24244698"></a>config_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924531_p17663550"><a name="zh-cn_topic_0118924531_p17663550"></a><a name="zh-cn_topic_0118924531_p17663550"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924531_p21461446"><a name="zh-cn_topic_0118924531_p21461446"></a><a name="zh-cn_topic_0118924531_p21461446"></a>配置时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 3,
  "size": 3,
  "configs": [
    {
      "config_id": "1",
      "config_name": "API_NUM_LIMIT",
      "config_value": "300",
      "config_time": "2017-12-29T08: 00: 39.543642Z",
      "remark": "租户可以创建的API个数限制"
    },
    {
      "config_id": "2",
      "config_name": "APP_NUM_LIMIT",
      "config_value": "30",
      "config_time": "2017-12-29T03: 39: 03.165657Z",
      "remark": "租户可以创建的APP个数限制"
    },
    {
      "config_id": "3",
      "config_name": "APIGROUP_NUM_LIMIT",
      "config_value": "30",
      "config_time": "2017-12-29T03: 39: 03.165657Z",
      "remark": "租户可以创建的API分组个数限制"
    }
  ]
}
```

## 状态码<a name="zh-cn_topic_0118924531_section8691277"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118924531_table24119960"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924531_row8124239"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924531_p54083656"><a name="zh-cn_topic_0118924531_p54083656"></a><a name="zh-cn_topic_0118924531_p54083656"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924531_p18700021"><a name="zh-cn_topic_0118924531_p18700021"></a><a name="zh-cn_topic_0118924531_p18700021"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924531_row38306751"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924531_p15839117"><a name="zh-cn_topic_0118924531_p15839117"></a><a name="zh-cn_topic_0118924531_p15839117"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924531_p7900104"><a name="zh-cn_topic_0118924531_p7900104"></a><a name="zh-cn_topic_0118924531_p7900104"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row3992073"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924531_p54922514"><a name="zh-cn_topic_0118924531_p54922514"></a><a name="zh-cn_topic_0118924531_p54922514"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924531_p19538619"><a name="zh-cn_topic_0118924531_p19538619"></a><a name="zh-cn_topic_0118924531_p19538619"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row41629843"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924531_p16574095"><a name="zh-cn_topic_0118924531_p16574095"></a><a name="zh-cn_topic_0118924531_p16574095"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924531_p324480"><a name="zh-cn_topic_0118924531_p324480"></a><a name="zh-cn_topic_0118924531_p324480"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924531_row2920328"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924531_p35220035"><a name="zh-cn_topic_0118924531_p35220035"></a><a name="zh-cn_topic_0118924531_p35220035"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924531_p34250599"><a name="zh-cn_topic_0118924531_p34250599"></a><a name="zh-cn_topic_0118924531_p34250599"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

