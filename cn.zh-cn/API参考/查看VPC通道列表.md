# 查看VPC通道列表<a name="apig-zh-api-180713165"></a>

## 功能介绍<a name="section173482301428"></a>

查看VPC通道列表。

## URI<a name="section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table1439319294431"></a>
<table><thead align="left"><tr id="row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p14361448204314"><a name="p14361448204314"></a><a name="p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p1936174864316"><a name="p1936174864316"></a><a name="p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1236111482435"><a name="p1236111482435"></a><a name="p1236111482435"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p11361848184318"><a name="p11361848184318"></a><a name="p11361848184318"></a>/v1.0/apigw/vpc-channels[?page_size, page_no, id, name, vpc_type，project_id]</p>
</td>
</tr>
</tbody>
</table>

o

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：id、name、vpc\_type、project\_id、page\_size、page\_no。  

**表 2**  参数说明

<a name="table14832938182115"></a>
<table><thead align="left"><tr id="row1183233815217"><th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.2.5.1.1"><p id="p1683253832114"><a name="p1683253832114"></a><a name="p1683253832114"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.2"><p id="p683216382215"><a name="p683216382215"></a><a name="p683216382215"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.82178217821782%" id="mcps1.2.5.1.3"><p id="p128321138152117"><a name="p128321138152117"></a><a name="p128321138152117"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.56435643564357%" id="mcps1.2.5.1.4"><p id="p1684814382214"><a name="p1684814382214"></a><a name="p1684814382214"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row984883812115"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p15848738132116"><a name="p15848738132116"></a><a name="p15848738132116"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p5848238122115"><a name="p5848238122115"></a><a name="p5848238122115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p1184863822116"><a name="p1184863822116"></a><a name="p1184863822116"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.56435643564357%" headers="mcps1.2.5.1.4 "><p id="p5848038172114"><a name="p5848038172114"></a><a name="p5848038172114"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="row188481438132116"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p58481038112113"><a name="p58481038112113"></a><a name="p58481038112113"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p208486387214"><a name="p208486387214"></a><a name="p208486387214"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p158481838192114"><a name="p158481838192114"></a><a name="p158481838192114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.56435643564357%" headers="mcps1.2.5.1.4 "><p id="p16863163822110"><a name="p16863163822110"></a><a name="p16863163822110"></a>VPC通道的名称。</p>
</td>
</tr>
<tr id="row1386353872116"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p5863193872114"><a name="p5863193872114"></a><a name="p5863193872114"></a>vpc_type</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p3863193820216"><a name="p3863193820216"></a><a name="p3863193820216"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p3863103862115"><a name="p3863103862115"></a><a name="p3863103862115"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="43.56435643564357%" headers="mcps1.2.5.1.4 "><p id="p10863438202114"><a name="p10863438202114"></a><a name="p10863438202114"></a>VPC通道的类型。</p>
</td>
</tr>
<tr id="row1886314382217"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p1386363812218"><a name="p1386363812218"></a><a name="p1386363812218"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p5863143815215"><a name="p5863143815215"></a><a name="p5863143815215"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p6863538102114"><a name="p6863538102114"></a><a name="p6863538102114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.56435643564357%" headers="mcps1.2.5.1.4 "><p id="p1786312385217"><a name="p1786312385217"></a><a name="p1786312385217"></a>租户ID，只有管理员权限可以查询。</p>
</td>
</tr>
<tr id="row12863838172111"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p486353813212"><a name="p486353813212"></a><a name="p486353813212"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p1486363832114"><a name="p1486363832114"></a><a name="p1486363832114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p2087913381210"><a name="p2087913381210"></a><a name="p2087913381210"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="43.56435643564357%" headers="mcps1.2.5.1.4 "><p id="p7879938152118"><a name="p7879938152118"></a><a name="p7879938152118"></a>每页显示的VPC通道数量，默认值：20。</p>
</td>
</tr>
<tr id="row1879438102119"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p4879173811211"><a name="p4879173811211"></a><a name="p4879173811211"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p17879338152117"><a name="p17879338152117"></a><a name="p17879338152117"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p987933882120"><a name="p987933882120"></a><a name="p987933882120"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="43.56435643564357%" headers="mcps1.2.5.1.4 "><p id="p0879113822110"><a name="p0879113822110"></a><a name="p0879113822110"></a>页码，默认值：1。</p>
</td>
</tr>
<tr id="row167242325210"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p19672223105215"><a name="p19672223105215"></a><a name="p19672223105215"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p1367222310525"><a name="p1367222310525"></a><a name="p1367222310525"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="17.82178217821782%" headers="mcps1.2.5.1.3 "><p id="p4672142375211"><a name="p4672142375211"></a><a name="p4672142375211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.56435643564357%" headers="mcps1.2.5.1.4 "><p id="p19672182317528"><a name="p19672182317528"></a><a name="p19672182317528"></a>指定需要精确匹配查找的参数名称，目前仅支持name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section4298322"></a>

无

## 响应消息<a name="section9395153012420"></a>

**表 3**  参数说明

<a name="table7395123013420"></a>
<table><thead align="left"><tr id="row114881330104215"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p19488153019429"><a name="p19488153019429"></a><a name="p19488153019429"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="p248853014422"><a name="p248853014422"></a><a name="p248853014422"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p64882308421"><a name="p64882308421"></a><a name="p64882308421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12488203074215"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1448813305421"><a name="p1448813305421"></a><a name="p1448813305421"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p18488163024218"><a name="p18488163024218"></a><a name="p18488163024218"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p24398880"><a name="p24398880"></a><a name="p24398880"></a>符合条件的VPC通道总数。</p>
</td>
</tr>
<tr id="row17488133012421"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1585685914587"><a name="p1585685914587"></a><a name="p1585685914587"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p4488183013424"><a name="p4488183013424"></a><a name="p4488183013424"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p61344470"><a name="p61344470"></a><a name="p61344470"></a>本次查询返回的列表长度。</p>
</td>
</tr>
<tr id="row748812305426"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p19871155912585"><a name="p19871155912585"></a><a name="p19871155912585"></a>vpcs</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p64881305424"><a name="p64881305424"></a><a name="p64881305424"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p23321404"><a name="p23321404"></a><a name="p23321404"></a>本次查询到的VPC通道列表。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  VPC参数说明

<a name="table197111958323"></a>
<table><thead align="left"><tr id="row87221581128"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p372519582025"><a name="p372519582025"></a><a name="p372519582025"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="p147282582021"><a name="p147282582021"></a><a name="p147282582021"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p374210583210"><a name="p374210583210"></a><a name="p374210583210"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1174420581729"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p2074616586213"><a name="p2074616586213"></a><a name="p2074616586213"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p974815584210"><a name="p974815584210"></a><a name="p974815584210"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p875011584215"><a name="p875011584215"></a><a name="p875011584215"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="row4751658120"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1175215581922"><a name="p1175215581922"></a><a name="p1175215581922"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p87551058920"><a name="p87551058920"></a><a name="p87551058920"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p7756958726"><a name="p7756958726"></a><a name="p7756958726"></a>VPC通道的名称。</p>
</td>
</tr>
<tr id="row17757195814211"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p02495197162"><a name="p02495197162"></a><a name="p02495197162"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p16251161941619"><a name="p16251161941619"></a><a name="p16251161941619"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p5748337181118"><a name="p5748337181118"></a><a name="p5748337181118"></a>VPC通道的类型。</p>
<a name="ul4748103711119"></a><a name="ul4748103711119"></a><ul id="ul4748103711119"><li>2：API网关内置支持负载均衡功能的快速通道类型</li></ul>
</td>
</tr>
<tr id="row1670172818199"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p3847512181119"><a name="p3847512181119"></a><a name="p3847512181119"></a>member_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p18847112191114"><a name="p18847112191114"></a><a name="p18847112191114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p1399195415116"><a name="p1399195415116"></a><a name="p1399195415116"></a>VPC通道的成员类型。</p>
<a name="ul10402654141119"></a><a name="ul10402654141119"></a><ul id="ul10402654141119"><li>ip（暂不支持）</li><li>instance</li></ul>
</td>
</tr>
<tr id="row1378145815219"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p478419583211"><a name="p478419583211"></a><a name="p478419583211"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p117861358624"><a name="p117861358624"></a><a name="p117861358624"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p1678812589219"><a name="p1678812589219"></a><a name="p1678812589219"></a>VPC通道的状态。</p>
<a name="ul4789165816218"></a><a name="ul4789165816218"></a><ul id="ul4789165816218"><li>1：正常</li><li>2：异常</li></ul>
</td>
</tr>
<tr id="row079513582213"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p07971458025"><a name="p07971458025"></a><a name="p07971458025"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p77991558123"><a name="p77991558123"></a><a name="p77991558123"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p16681305"><a name="p16681305"></a><a name="p16681305"></a>VPC通道中主机的端口号。</p>
</td>
</tr>
<tr id="row188041458421"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p1180616581121"><a name="p1180616581121"></a><a name="p1180616581121"></a>balance_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p1280835813215"><a name="p1280835813215"></a><a name="p1280835813215"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p168103581629"><a name="p168103581629"></a><a name="p168103581629"></a>分发算法。</p>
<a name="ul381113585218"></a><a name="ul381113585218"></a><ul id="ul381113585218"><li>1：加权轮询（wrr）</li><li>2：加权最少连接（wleastconn）</li><li>3：源地址哈希（source）</li><li>4：URI哈希（uri）</li></ul>
</td>
</tr>
<tr id="row582114581722"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p682425815217"><a name="p682425815217"></a><a name="p682425815217"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p78261581217"><a name="p78261581217"></a><a name="p78261581217"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p1682865813210"><a name="p1682865813210"></a><a name="p1682865813210"></a>VPC通道的创建时间。</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 2,
  "size": 2,
  "vpcs": [
    {
      "name": "通道1",
      "type": 1,
      "member_type": "instance",
      "port": 8080,
      "balance_strategy": 1,
      "id": "39c62689302a48fe9f4bd7cf5c052064",
      "create_time": "2018-04-24T12:07:58Z",
      "status": 1
    },
    {
      "name": "通道2",
      "type": 2,
      "member_type": "instance",
      "port": 8088,
      "balance_strategy": 1,
      "id": "e6831cbcbe2b45bbbc6318c2892f060b",
      "create_time": "2018-04-24T11:57:03Z",
      "status": 1
    }
  ]
}
```

## 状态码<a name="section338043011426"></a>

**表 5**  返回消息说明

<a name="table1338010302424"></a>
<table><thead align="left"><tr id="row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p174881730194216"><a name="p174881730194216"></a><a name="p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p848863018429"><a name="p848863018429"></a><a name="p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p7488163084211"><a name="p7488163084211"></a><a name="p7488163084211"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p948803015424"><a name="p948803015424"></a><a name="p948803015424"></a>OK</p>
</td>
</tr>
<tr id="row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p14488113015426"><a name="p14488113015426"></a><a name="p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p164881130154211"><a name="p164881130154211"></a><a name="p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p24883304428"><a name="p24883304428"></a><a name="p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1848810308429"><a name="p1848810308429"></a><a name="p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6488133064210"><a name="p6488133064210"></a><a name="p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p10488193018426"><a name="p10488193018426"></a><a name="p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p144883304428"><a name="p144883304428"></a><a name="p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p4488103094212"><a name="p4488103094212"></a><a name="p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p17488163014423"><a name="p17488163014423"></a><a name="p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p048813014216"><a name="p048813014216"></a><a name="p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

