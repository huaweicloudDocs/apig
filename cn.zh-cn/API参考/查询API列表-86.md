# 查询API列表<a name="apig-phapi-180911221"></a>

## 功能介绍<a name="section39474715"></a>

查询某个已上架的API分组下的API。这些API需要满足以下规则方可被查询到：

-   API的认证方式为APP认证
-   API的类型是公有的
-   API已经发布到RELEASE环境

## URI<a name="section21728667"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table810618"></a>
<table><thead align="left"><tr id="row24350089"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p26200207"><a name="p26200207"></a><a name="p26200207"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p41842029"><a name="p41842029"></a><a name="p41842029"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row33761228"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p50304980"><a name="p50304980"></a><a name="p50304980"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p48171564"><a name="p48171564"></a><a name="p48171564"></a>/v1/{project_id}/apigw/instances/{instance_id}/market/apis[?group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：group\_id。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table57467174"></a>
<table><thead align="left"><tr id="row58385281"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p31587325"><a name="p31587325"></a><a name="p31587325"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p8436529"><a name="p8436529"></a><a name="p8436529"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p12270278"><a name="p12270278"></a><a name="p12270278"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p54368484"><a name="p54368484"></a><a name="p54368484"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row172921835112417"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row18778123482417"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row41771058"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p28012504"><a name="p28012504"></a><a name="p28012504"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p54420351"><a name="p54420351"></a><a name="p54420351"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p45972302"><a name="p45972302"></a><a name="p45972302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p554519551264"><a name="p554519551264"></a><a name="p554519551264"></a>API分组编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section61340275"></a>

无

## 响应消息<a name="section2506351"></a>

**表 3**  API列表

<a name="table33988889"></a>
<table><thead align="left"><tr id="row2774919"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p23441890"><a name="p23441890"></a><a name="p23441890"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p19744913"><a name="p19744913"></a><a name="p19744913"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p55834109"><a name="p55834109"></a><a name="p55834109"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26268941"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p47409449"><a name="p47409449"></a><a name="p47409449"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p14960186"><a name="p14960186"></a><a name="p14960186"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p56189101885"><a name="p56189101885"></a><a name="p56189101885"></a>API的编号</p>
</td>
</tr>
<tr id="row34340333"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p66431616588"><a name="p66431616588"></a><a name="p66431616588"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18581172016812"><a name="p18581172016812"></a><a name="p18581172016812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1214317241381"><a name="p1214317241381"></a><a name="p1214317241381"></a>API的名称</p>
</td>
</tr>
<tr id="row7948700"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1612813012812"><a name="p1612813012812"></a><a name="p1612813012812"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p102061935782"><a name="p102061935782"></a><a name="p102061935782"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p0956538582"><a name="p0956538582"></a><a name="p0956538582"></a>API的描述</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
[
  {
    "id": "0e51b689e0784bc884f43756bbf34fa5",
    "name": "market_api01",
    "remark": "market_api01"
  }
]
```

## 状态码<a name="section15191564"></a>

**表 4**  返回消息说明

<a name="table7632062"></a>
<table><thead align="left"><tr id="row29647066"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p52602177"><a name="p52602177"></a><a name="p52602177"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p32917907"><a name="p32917907"></a><a name="p32917907"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49104826"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p18067998"><a name="p18067998"></a><a name="p18067998"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p54221734"><a name="p54221734"></a><a name="p54221734"></a>OK</p>
</td>
</tr>
<tr id="row18233563"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p523669"><a name="p523669"></a><a name="p523669"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p42417256"><a name="p42417256"></a><a name="p42417256"></a>Bad Request</p>
</td>
</tr>
<tr id="row46210986"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p52102356"><a name="p52102356"></a><a name="p52102356"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p59541290"><a name="p59541290"></a><a name="p59541290"></a>Unauthorized</p>
</td>
</tr>
<tr id="row66109570"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p53274950"><a name="p53274950"></a><a name="p53274950"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

