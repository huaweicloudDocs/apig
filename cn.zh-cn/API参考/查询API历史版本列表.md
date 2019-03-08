# 查询API历史版本列表<a name="apig-zh-api-180713033"></a>

## 功能介绍<a name="section6627989"></a>

查询某个API的历史版本。每个API在一个环境上最多存在10个历史版本。

## URI<a name="section59651907"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table42014202"></a>
<table><thead align="left"><tr id="row11048869"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p22543169"><a name="p22543169"></a><a name="p22543169"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p14057426"><a name="p14057426"></a><a name="p14057426"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row64909760"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p23199218"><a name="p23199218"></a><a name="p23199218"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p88529"><a name="p88529"></a><a name="p88529"></a>/v1.0/apigw/apis/publish/{api_id}[?env_id,env_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：env\_id,env\_name。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table796764"></a>
<table><thead align="left"><tr id="row53401841"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p30581871"><a name="p30581871"></a><a name="p30581871"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p61212526"><a name="p61212526"></a><a name="p61212526"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p59267606"><a name="p59267606"></a><a name="p59267606"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p35946766"><a name="p35946766"></a><a name="p35946766"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row26006910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p26184975"><a name="p26184975"></a><a name="p26184975"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p40608232"><a name="p40608232"></a><a name="p40608232"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p932530"><a name="p932530"></a><a name="p932530"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p8426133"><a name="p8426133"></a><a name="p8426133"></a>API的编号</p>
</td>
</tr>
<tr id="row123871511132316"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p038715116233"><a name="p038715116233"></a><a name="p038715116233"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p163871111162311"><a name="p163871111162311"></a><a name="p163871111162311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p123874110237"><a name="p123874110237"></a><a name="p123874110237"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p16387311102313"><a name="p16387311102313"></a><a name="p16387311102313"></a>环境的编号</p>
</td>
</tr>
<tr id="row8636813192312"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p12636013142314"><a name="p12636013142314"></a><a name="p12636013142314"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p36362134231"><a name="p36362134231"></a><a name="p36362134231"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p2636121342313"><a name="p2636121342313"></a><a name="p2636121342313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1963661313233"><a name="p1963661313233"></a><a name="p1963661313233"></a>环境的名称</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section67105121"></a>

无

## 响应消息<a name="section66805754"></a>

**表 3**  参数说明

<a name="table2981672313"></a>
<table><thead align="left"><tr id="row898177103111"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="p109837183116"><a name="p109837183116"></a><a name="p109837183116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="p1098474319"><a name="p1098474319"></a><a name="p1098474319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="p1398197193117"><a name="p1398197193117"></a><a name="p1398197193117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49812719314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p25782746"><a name="p25782746"></a><a name="p25782746"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p8027664"><a name="p8027664"></a><a name="p8027664"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p46261084"><a name="p46261084"></a><a name="p46261084"></a>满足条件的API历史版本总数</p>
</td>
</tr>
<tr id="row119827123112"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p35680577"><a name="p35680577"></a><a name="p35680577"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p4445647"><a name="p4445647"></a><a name="p4445647"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p24553101"><a name="p24553101"></a><a name="p24553101"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="row998187163114"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p48252863"><a name="p48252863"></a><a name="p48252863"></a>api_versions</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p16167821"><a name="p16167821"></a><a name="p16167821"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p34525128"><a name="p34525128"></a><a name="p34525128"></a>本次查询返回的API历史版本列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  api\_versions参数说明

<a name="table42290697"></a>
<table><thead align="left"><tr id="row54536847"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p55408512"><a name="p55408512"></a><a name="p55408512"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p58904526"><a name="p58904526"></a><a name="p58904526"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p6537312"><a name="p6537312"></a><a name="p6537312"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row59760287"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p18981672315"><a name="p18981672315"></a><a name="p18981672315"></a>version_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p209815717318"><a name="p209815717318"></a><a name="p209815717318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p8980773120"><a name="p8980773120"></a><a name="p8980773120"></a>API历史版本的ID</p>
</td>
</tr>
<tr id="row6945124117278"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p794519411278"><a name="p794519411278"></a><a name="p794519411278"></a>version_no</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p694574110271"><a name="p694574110271"></a><a name="p694574110271"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p39458412271"><a name="p39458412271"></a><a name="p39458412271"></a>API的版本号</p>
</td>
</tr>
<tr id="row52310185"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p159814710314"><a name="p159814710314"></a><a name="p159814710314"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1698871311"><a name="p1698871311"></a><a name="p1698871311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p109897153112"><a name="p109897153112"></a><a name="p109897153112"></a>API编号</p>
</td>
</tr>
<tr id="row45342804"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p129814713315"><a name="p129814713315"></a><a name="p129814713315"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13987723113"><a name="p13987723113"></a><a name="p13987723113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p109819712314"><a name="p109819712314"></a><a name="p109819712314"></a>发布的环境编号</p>
</td>
</tr>
<tr id="row143411649142719"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p143411649112717"><a name="p143411649112717"></a><a name="p143411649112717"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p3341849162714"><a name="p3341849162714"></a><a name="p3341849162714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p193411949122714"><a name="p193411949122714"></a><a name="p193411949122714"></a>发布的环境名称</p>
</td>
</tr>
<tr id="row60411917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p1098147143114"><a name="p1098147143114"></a><a name="p1098147143114"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p998197113114"><a name="p998197113114"></a><a name="p998197113114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p99816773110"><a name="p99816773110"></a><a name="p99816773110"></a>发布描述</p>
</td>
</tr>
<tr id="row41802573"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p998117163115"><a name="p998117163115"></a><a name="p998117163115"></a>publish_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p59813711317"><a name="p59813711317"></a><a name="p59813711317"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5989733118"><a name="p5989733118"></a><a name="p5989733118"></a>发布时间</p>
</td>
</tr>
<tr id="row20081233"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p15967206"><a name="p15967206"></a><a name="p15967206"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p18275332"><a name="p18275332"></a><a name="p18275332"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p81811545182511"><a name="p81811545182511"></a><a name="p81811545182511"></a>版本状态：</p>
<a name="ul0837134912255"></a><a name="ul0837134912255"></a><ul id="ul0837134912255"><li>1、当前生效中的版本</li><li>2、未生效的版本</li></ul>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 1,
  "size": 1,
  "api_versions": [
    {
      "version_id": "04c194dc7b5340ed942f2451702060da",
      "version_no": "20180722102526",
      "api_id": "acf141aa6279415088b593a4bbb55eed",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "publish_time": "2018-04-14T07:32:23Z",
      "status": 2
    }
  ]
}
```

## 状态码<a name="section67075185"></a>

**表 5**  返回消息说明

<a name="table15714732"></a>
<table><thead align="left"><tr id="row24997277"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p11513591"><a name="p11513591"></a><a name="p11513591"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p60185706"><a name="p60185706"></a><a name="p60185706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row43203997"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9862840"><a name="p9862840"></a><a name="p9862840"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p73578115452"><a name="p73578115452"></a><a name="p73578115452"></a>Created</p>
</td>
</tr>
<tr id="row9362312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20149775"><a name="p20149775"></a><a name="p20149775"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p21519099"><a name="p21519099"></a><a name="p21519099"></a>Bad Request</p>
</td>
</tr>
<tr id="row59454171"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p51058521"><a name="p51058521"></a><a name="p51058521"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p9203142078"><a name="p9203142078"></a><a name="p9203142078"></a>Unauthorized</p>
</td>
</tr>
<tr id="row43351211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p21787193"><a name="p21787193"></a><a name="p21787193"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row45172181"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p35068062"><a name="p35068062"></a><a name="p35068062"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p21940743"><a name="p21940743"></a><a name="p21940743"></a>Not Found</p>
</td>
</tr>
<tr id="row63248959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22892027"><a name="p22892027"></a><a name="p22892027"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

