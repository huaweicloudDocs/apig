# 查询分组详情<a name="ZH-CN_TOPIC_0000001082221213"></a>

## 功能介绍<a name="zh-cn_topic_0118924523_section15513853"></a>

查询已购买的指定分组的详情。

## URI<a name="zh-cn_topic_0118924523_section5406953"></a>

HTTP/HTTPS请求方法以及URI如下表1所示

**表 1**  HTTP/HTTPS请求方法及URI

<a name="zh-cn_topic_0118924523_table61361165"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924523_row31500276"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924523_p1385538"><a name="zh-cn_topic_0118924523_p1385538"></a><a name="zh-cn_topic_0118924523_p1385538"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924523_p45119720"><a name="zh-cn_topic_0118924523_p45119720"></a><a name="zh-cn_topic_0118924523_p45119720"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924523_row30818703"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924523_p13287006"><a name="zh-cn_topic_0118924523_p13287006"></a><a name="zh-cn_topic_0118924523_p13287006"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924523_p2505726"><a name="zh-cn_topic_0118924523_p2505726"></a><a name="zh-cn_topic_0118924523_p2505726"></a>/v1.0/apigw/purchases/groups/{purchase_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118924523_table22551540"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924523_row16521053"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118924523_p63136955"><a name="zh-cn_topic_0118924523_p63136955"></a><a name="zh-cn_topic_0118924523_p63136955"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118924523_p13819741"><a name="zh-cn_topic_0118924523_p13819741"></a><a name="zh-cn_topic_0118924523_p13819741"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118924523_p45657260"><a name="zh-cn_topic_0118924523_p45657260"></a><a name="zh-cn_topic_0118924523_p45657260"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118924523_p7250575"><a name="zh-cn_topic_0118924523_p7250575"></a><a name="zh-cn_topic_0118924523_p7250575"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924523_row50425711"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0118924523_p1932019184374"><a name="zh-cn_topic_0118924523_p1932019184374"></a><a name="zh-cn_topic_0118924523_p1932019184374"></a>purchase_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0118924523_p63500868"><a name="zh-cn_topic_0118924523_p63500868"></a><a name="zh-cn_topic_0118924523_p63500868"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0118924523_p43296649"><a name="zh-cn_topic_0118924523_p43296649"></a><a name="zh-cn_topic_0118924523_p43296649"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0118924523_p16867183216377"><a name="zh-cn_topic_0118924523_p16867183216377"></a><a name="zh-cn_topic_0118924523_p16867183216377"></a>订购关系编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118924523_section48662582"></a>

无

## 响应消息<a name="zh-cn_topic_0118924523_section49355104"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118924523_table58595317"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924523_row16765496"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118924523_p15827946"><a name="zh-cn_topic_0118924523_p15827946"></a><a name="zh-cn_topic_0118924523_p15827946"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118924523_p6995273"><a name="zh-cn_topic_0118924523_p6995273"></a><a name="zh-cn_topic_0118924523_p6995273"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118924523_p29746236"><a name="zh-cn_topic_0118924523_p29746236"></a><a name="zh-cn_topic_0118924523_p29746236"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924523_row60634924"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p12481792"><a name="zh-cn_topic_0118924523_p12481792"></a><a name="zh-cn_topic_0118924523_p12481792"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p4392225"><a name="zh-cn_topic_0118924523_p4392225"></a><a name="zh-cn_topic_0118924523_p4392225"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p20225910"><a name="zh-cn_topic_0118924523_p20225910"></a><a name="zh-cn_topic_0118924523_p20225910"></a>订购关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row47815463"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p47847334"><a name="zh-cn_topic_0118924523_p47847334"></a><a name="zh-cn_topic_0118924523_p47847334"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p50428878"><a name="zh-cn_topic_0118924523_p50428878"></a><a name="zh-cn_topic_0118924523_p50428878"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p58207302"><a name="zh-cn_topic_0118924523_p58207302"></a><a name="zh-cn_topic_0118924523_p58207302"></a>分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row54103671"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p20321259"><a name="zh-cn_topic_0118924523_p20321259"></a><a name="zh-cn_topic_0118924523_p20321259"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p35409283"><a name="zh-cn_topic_0118924523_p35409283"></a><a name="zh-cn_topic_0118924523_p35409283"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p49579688"><a name="zh-cn_topic_0118924523_p49579688"></a><a name="zh-cn_topic_0118924523_p49579688"></a>分组名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row43564010"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p39023949"><a name="zh-cn_topic_0118924523_p39023949"></a><a name="zh-cn_topic_0118924523_p39023949"></a>group_remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p6823280"><a name="zh-cn_topic_0118924523_p6823280"></a><a name="zh-cn_topic_0118924523_p6823280"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p15814779"><a name="zh-cn_topic_0118924523_p15814779"></a><a name="zh-cn_topic_0118924523_p15814779"></a>分组描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row8115287"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p53358547"><a name="zh-cn_topic_0118924523_p53358547"></a><a name="zh-cn_topic_0118924523_p53358547"></a>order_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p27075018"><a name="zh-cn_topic_0118924523_p27075018"></a><a name="zh-cn_topic_0118924523_p27075018"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p45592870"><a name="zh-cn_topic_0118924523_p45592870"></a><a name="zh-cn_topic_0118924523_p45592870"></a>订购时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row7682654"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p18315212"><a name="zh-cn_topic_0118924523_p18315212"></a><a name="zh-cn_topic_0118924523_p18315212"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p7137170"><a name="zh-cn_topic_0118924523_p7137170"></a><a name="zh-cn_topic_0118924523_p7137170"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p41239897"><a name="zh-cn_topic_0118924523_p41239897"></a><a name="zh-cn_topic_0118924523_p41239897"></a>生效时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row35614756"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p66222991"><a name="zh-cn_topic_0118924523_p66222991"></a><a name="zh-cn_topic_0118924523_p66222991"></a>expire_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p62462030"><a name="zh-cn_topic_0118924523_p62462030"></a><a name="zh-cn_topic_0118924523_p62462030"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p26259658"><a name="zh-cn_topic_0118924523_p26259658"></a><a name="zh-cn_topic_0118924523_p26259658"></a>过期时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row35010330"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p17264443"><a name="zh-cn_topic_0118924523_p17264443"></a><a name="zh-cn_topic_0118924523_p17264443"></a>group_domains</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p56242637"><a name="zh-cn_topic_0118924523_p56242637"></a><a name="zh-cn_topic_0118924523_p56242637"></a>[]String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p59359735"><a name="zh-cn_topic_0118924523_p59359735"></a><a name="zh-cn_topic_0118924523_p59359735"></a>分组访问域名列表，查询详情时返回</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row64475573"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p55138935"><a name="zh-cn_topic_0118924523_p55138935"></a><a name="zh-cn_topic_0118924523_p55138935"></a>quota_left</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p37068774"><a name="zh-cn_topic_0118924523_p37068774"></a><a name="zh-cn_topic_0118924523_p37068774"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p49780713"><a name="zh-cn_topic_0118924523_p49780713"></a><a name="zh-cn_topic_0118924523_p49780713"></a>剩余访问次数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row45373238"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p51353651"><a name="zh-cn_topic_0118924523_p51353651"></a><a name="zh-cn_topic_0118924523_p51353651"></a>quota_used</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p66005048"><a name="zh-cn_topic_0118924523_p66005048"></a><a name="zh-cn_topic_0118924523_p66005048"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p44808686"><a name="zh-cn_topic_0118924523_p44808686"></a><a name="zh-cn_topic_0118924523_p44808686"></a>已使用访问次数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row624995"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p50624612"><a name="zh-cn_topic_0118924523_p50624612"></a><a name="zh-cn_topic_0118924523_p50624612"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p6952939"><a name="zh-cn_topic_0118924523_p6952939"></a><a name="zh-cn_topic_0118924523_p6952939"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p26317149"><a name="zh-cn_topic_0118924523_p26317149"></a><a name="zh-cn_topic_0118924523_p26317149"></a>生成的APP的key</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row35527755"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118924523_p59175883"><a name="zh-cn_topic_0118924523_p59175883"></a><a name="zh-cn_topic_0118924523_p59175883"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118924523_p28517228"><a name="zh-cn_topic_0118924523_p28517228"></a><a name="zh-cn_topic_0118924523_p28517228"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118924523_p28194133"><a name="zh-cn_topic_0118924523_p28194133"></a><a name="zh-cn_topic_0118924523_p28194133"></a>生成的APP的secret</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "id": "3f30d49b-220f-4b11-9e94-c2fd3c1cc587",
  "group_id": "73c58022-f20d-495a-a188-85d718647f09",
  "group_name": "api_group_001",
  "group_remark": "分组001",
  "group_domains": [
    "test.market.example.com"
  ],
  "quota_used": 0,
  "quota_left": 2000000000,
  "order_time": "2018-01-02T10: 51: 26Z",
  "start_time": "2018-01-01T00: 00: 00Z",
  "expire_time": "2019-01-01T00: 00: 00Z",
  "app_key": "0e242685-661d-4254-a8bb-be9a92b04785",
  "app_secret": "******"
}
```

## 状态码<a name="zh-cn_topic_0118924523_section35310062"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0118924523_table65467683"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118924523_row62252322"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118924523_p9273323"><a name="zh-cn_topic_0118924523_p9273323"></a><a name="zh-cn_topic_0118924523_p9273323"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118924523_p12941733"><a name="zh-cn_topic_0118924523_p12941733"></a><a name="zh-cn_topic_0118924523_p12941733"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118924523_row41647480"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924523_p18002699"><a name="zh-cn_topic_0118924523_p18002699"></a><a name="zh-cn_topic_0118924523_p18002699"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924523_p50988816"><a name="zh-cn_topic_0118924523_p50988816"></a><a name="zh-cn_topic_0118924523_p50988816"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row37739194"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924523_p36975910"><a name="zh-cn_topic_0118924523_p36975910"></a><a name="zh-cn_topic_0118924523_p36975910"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924523_p42258701"><a name="zh-cn_topic_0118924523_p42258701"></a><a name="zh-cn_topic_0118924523_p42258701"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row44783995"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924523_p3625001"><a name="zh-cn_topic_0118924523_p3625001"></a><a name="zh-cn_topic_0118924523_p3625001"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924523_p25189639"><a name="zh-cn_topic_0118924523_p25189639"></a><a name="zh-cn_topic_0118924523_p25189639"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row25380159"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924523_p42527017"><a name="zh-cn_topic_0118924523_p42527017"></a><a name="zh-cn_topic_0118924523_p42527017"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924523_p22136343"><a name="zh-cn_topic_0118924523_p22136343"></a><a name="zh-cn_topic_0118924523_p22136343"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0118924523_row65009363"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118924523_p31267075"><a name="zh-cn_topic_0118924523_p31267075"></a><a name="zh-cn_topic_0118924523_p31267075"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118924523_p15296380"><a name="zh-cn_topic_0118924523_p15296380"></a><a name="zh-cn_topic_0118924523_p15296380"></a>Not Found</p>
</td>
</tr>
</tbody>
</table>

