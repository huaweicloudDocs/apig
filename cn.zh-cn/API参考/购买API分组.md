# 购买API分组<a name="apig-phapi-180713105"></a>

## 功能介绍<a name="section39474715"></a>

租户在云市场购买一个API分组。

租户购买了一个API分组之后，会默认为该API分组绑定一个系统创建的APP，租户可通过该APP调用该分组下的所有公有且认证方式为APP认证并已发布到RELEASE环境的API。

## URI<a name="section19728122"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table52422860"></a>
<table><thead align="left"><tr id="row16282296"><th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.1"><p id="p43797605"><a name="p43797605"></a><a name="p43797605"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.2.3.1.2"><p id="p57945135"><a name="p57945135"></a><a name="p57945135"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row63044349"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.1 "><p id="p6318648"><a name="p6318648"></a><a name="p6318648"></a>post</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.2.3.1.2 "><p id="p42048455"><a name="p42048455"></a><a name="p42048455"></a>/v1/{project_id}/apigw/instances/{instance_id}/market/api-groups/purchase</p>
</td>
</tr>
</tbody>
</table>

**表 2**  Head参数信息

<a name="table1077685961811"></a>
<table><thead align="left"><tr id="row6776145921810"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p87761159141817"><a name="p87761159141817"></a><a name="p87761159141817"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="p4776175919185"><a name="p4776175919185"></a><a name="p4776175919185"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="p677610599186"><a name="p677610599186"></a><a name="p677610599186"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="p1177635911817"><a name="p1177635911817"></a><a name="p1177635911817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row177635917187"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p18981357121915"><a name="p18981357121915"></a><a name="p18981357121915"></a>X-Domain-Id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p1877615911184"><a name="p1877615911184"></a><a name="p1877615911184"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p11776115931813"><a name="p11776115931813"></a><a name="p11776115931813"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p877695917180"><a name="p877695917180"></a><a name="p877695917180"></a>租户的DomainId</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section11605164214474"></a>

**表 3**  参数说明

<a name="table14769194213479"></a>
<table><thead align="left"><tr id="row476614254715"><th class="cellrowborder" valign="top" width="19%" id="mcps1.2.5.1.1"><p id="p18765204214719"><a name="p18765204214719"></a><a name="p18765204214719"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p2765164214475"><a name="p2765164214475"></a><a name="p2765164214475"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.3"><p id="p127653422474"><a name="p127653422474"></a><a name="p127653422474"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="53%" id="mcps1.2.5.1.4"><p id="p1376611426479"><a name="p1376611426479"></a><a name="p1376611426479"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row4126248182213"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row104640475226"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row37661742114712"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p27666426479"><a name="p27666426479"></a><a name="p27666426479"></a>order_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p576694215475"><a name="p576694215475"></a><a name="p576694215475"></a>预付费套餐包必须</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p13766042184715"><a name="p13766042184715"></a><a name="p13766042184715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p1076654224718"><a name="p1076654224718"></a><a name="p1076654224718"></a>云市场的订购编号，保证幂等性，如果重复订购，调用APIG的接口时，该字段保持不变，云市场可根据自身业务需求决定该字段需要存放的值</p>
</td>
</tr>
<tr id="row2076604212471"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p1576614425472"><a name="p1576614425472"></a><a name="p1576614425472"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p13766144234718"><a name="p13766144234718"></a><a name="p13766144234718"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p107661042114714"><a name="p107661042114714"></a><a name="p107661042114714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p1766104218475"><a name="p1766104218475"></a><a name="p1766104218475"></a>购买的API分组编号</p>
</td>
</tr>
<tr id="row4767174274712"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p177665425479"><a name="p177665425479"></a><a name="p177665425479"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p3767114212474"><a name="p3767114212474"></a><a name="p3767114212474"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p117673428474"><a name="p117673428474"></a><a name="p117673428474"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p1767194219474"><a name="p1767194219474"></a><a name="p1767194219474"></a>生效时间，取秒数</p>
</td>
</tr>
<tr id="row1767194244710"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p2767134219478"><a name="p2767134219478"></a><a name="p2767134219478"></a>expire_time</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p1767164284713"><a name="p1767164284713"></a><a name="p1767164284713"></a>非后付费按需必须</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p117674426477"><a name="p117674426477"></a><a name="p117674426477"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p2076774274720"><a name="p2076774274720"></a><a name="p2076774274720"></a>过期时间，取秒数</p>
</td>
</tr>
<tr id="row1476764244713"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p1876774213479"><a name="p1876774213479"></a><a name="p1876774213479"></a>req_quota</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p1767442174711"><a name="p1767442174711"></a><a name="p1767442174711"></a>预付费套餐包必须</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p47671142174712"><a name="p47671142174712"></a><a name="p47671142174712"></a>Long</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p177671542124711"><a name="p177671542124711"></a><a name="p177671542124711"></a>购买的请求次数</p>
</td>
</tr>
<tr id="row376914224719"><td class="cellrowborder" valign="top" width="19%" headers="mcps1.2.5.1.1 "><p id="p8767642174719"><a name="p8767642174719"></a><a name="p8767642174719"></a>order_type</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p5767154204716"><a name="p5767154204716"></a><a name="p5767154204716"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.3 "><p id="p107691442184710"><a name="p107691442184710"></a><a name="p107691442184710"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="53%" headers="mcps1.2.5.1.4 "><p id="p197691429477"><a name="p197691429477"></a><a name="p197691429477"></a>计费类型：</p>
<a name="ul6769242134712"></a><a name="ul6769242134712"></a><ul id="ul6769242134712"><li>1：预付费套餐包</li><li>2：后付费包周期</li><li>3：后付费按需</li></ul>
</td>
</tr>
</tbody>
</table>

请求参数样例：

```
{
	"expire_time": "1549874100",
	"group_id": "73c58022-f20d-495a-a188-85d718647f09",
	"order_id": "12v58023-e20f-084b-b299-74c618647e98",
	"req_quota": 1000000000,
	"start_time": "1518338100",
	"order_type": 1
}
```

## 响应消息<a name="section629654012486"></a>

**表 4**  参数说明

<a name="table15776164224719"></a>
<table><thead align="left"><tr id="row2772104284712"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p4772154254714"><a name="p4772154254714"></a><a name="p4772154254714"></a>参数名</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p277213425474"><a name="p277213425474"></a><a name="p277213425474"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p3772742134717"><a name="p3772742134717"></a><a name="p3772742134717"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1977204264720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p877216426473"><a name="p877216426473"></a><a name="p877216426473"></a>purchase_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1277254217477"><a name="p1277254217477"></a><a name="p1277254217477"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p477244217474"><a name="p477244217474"></a><a name="p477244217474"></a>资源编号（订购关系编号）</p>
</td>
</tr>
<tr id="row1477224216475"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17772134224712"><a name="p17772134224712"></a><a name="p17772134224712"></a>order_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57721342164715"><a name="p57721342164715"></a><a name="p57721342164715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17772104212474"><a name="p17772104212474"></a><a name="p17772104212474"></a>云市场的订购编号</p>
</td>
</tr>
<tr id="row1577310425478"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8773642154711"><a name="p8773642154711"></a><a name="p8773642154711"></a>start_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p1477314244719"><a name="p1477314244719"></a><a name="p1477314244719"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1477384224711"><a name="p1477384224711"></a><a name="p1477384224711"></a>生效时间</p>
</td>
</tr>
<tr id="row2773642124718"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p5773142104714"><a name="p5773142104714"></a><a name="p5773142104714"></a>expire_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p13773184212470"><a name="p13773184212470"></a><a name="p13773184212470"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p3773104218476"><a name="p3773104218476"></a><a name="p3773104218476"></a>过期时间</p>
</td>
</tr>
<tr id="row1777524204713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p177731422478"><a name="p177731422478"></a><a name="p177731422478"></a>req_quota</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p117751042114712"><a name="p117751042114712"></a><a name="p117751042114712"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p5775104213472"><a name="p5775104213472"></a><a name="p5775104213472"></a>购买的请求次数</p>
</td>
</tr>
<tr id="row1477654284718"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p177574294710"><a name="p177574294710"></a><a name="p177574294710"></a>order_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p87751942194712"><a name="p87751942194712"></a><a name="p87751942194712"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p07751142144714"><a name="p07751142144714"></a><a name="p07751142144714"></a>计费类型：</p>
<a name="ul97769424475"></a><a name="ul97769424475"></a><ul id="ul97769424475"><li>1：预付费套餐包</li><li>2：后付费包周期</li><li>3：后付费按需</li></ul>
</td>
</tr>
<tr id="row187761942184715"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p107761242184717"><a name="p107761242184717"></a><a name="p107761242184717"></a>app_key</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9776942114717"><a name="p9776942114717"></a><a name="p9776942114717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p10776842114712"><a name="p10776842114712"></a><a name="p10776842114712"></a>云市场分配的APP的app_key</p>
</td>
</tr>
<tr id="row16776742174717"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p9776134214714"><a name="p9776134214714"></a><a name="p9776134214714"></a>app_secret</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p16776842134715"><a name="p16776842134715"></a><a name="p16776842134715"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p377694210470"><a name="p377694210470"></a><a name="p377694210470"></a>云市场分配的APP的app_secret</p>
</td>
</tr>
<tr id="row117761342154713"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p57768425479"><a name="p57768425479"></a><a name="p57768425479"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p137764421479"><a name="p137764421479"></a><a name="p137764421479"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p20776154294712"><a name="p20776154294712"></a><a name="p20776154294712"></a>API分组编号</p>
</td>
</tr>
</tbody>
</table>

响应参数示例：

```
{
	"order_id": "12v58023-e20f-084b-b299-74c618647e98",
	"group_id": "73c58022-f20d-495a-a188-85d718647f09",
	"start_time": "2017-12-31T00:00:00Z",
	"expire_time": "2018-12-31T00:00:00Z",
	"req_quota": 1000000000,
	"order_type": 1,
	"purchase_id": "3f30d49b-220f-4b11-9e94-c2fd3c1cc587",
	"app_key": "1b6137af-3f1d-4cac-b894-ac1700af5f03",
	"app_secret": "******"
}
```

## 状态码<a name="section18408172011482"></a>

**表 5**  返回消息说明

<a name="table1777194274714"></a>
<table><thead align="left"><tr id="row167706423477"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p5770154294718"><a name="p5770154294718"></a><a name="p5770154294718"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p87708425476"><a name="p87708425476"></a><a name="p87708425476"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5770134211472"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p19770242154712"><a name="p19770242154712"></a><a name="p19770242154712"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p7770144214716"><a name="p7770144214716"></a><a name="p7770144214716"></a>Created</p>
</td>
</tr>
<tr id="row2077124219476"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p2077010426477"><a name="p2077010426477"></a><a name="p2077010426477"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p187703427470"><a name="p187703427470"></a><a name="p187703427470"></a>Bad Request</p>
</td>
</tr>
<tr id="row18771142164720"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p7771104214470"><a name="p7771104214470"></a><a name="p7771104214470"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1771114219477"><a name="p1771114219477"></a><a name="p1771114219477"></a>Unauthorized</p>
</td>
</tr>
<tr id="row1377164210473"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p3771144284711"><a name="p3771144284711"></a><a name="p3771144284711"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p377174214712"><a name="p377174214712"></a><a name="p377174214712"></a>Forbidden</p>
</td>
</tr>
<tr id="row1577194214474"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1577124218477"><a name="p1577124218477"></a><a name="p1577124218477"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

