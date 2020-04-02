# 锁定/解除锁定API分组接口<a name="apig-phapi-180713101"></a>

## 功能介绍<a name="section56552939"></a>

租户查询到自己名下待上架的API分组后，选择一个API分组并进行相关的产品发布操作，发布后，会进入云市场的审核环节，当分组进入审核环节后，租户便不可再次操作该分组。

当分组进入审核状态时，云市场需要通知API网关同步做状态的变更。当云市场审核不通过时，同样需要通知API网关解除对该分组的锁定。

## URI<a name="section39214405"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table25580828"></a>
<table><thead align="left"><tr id="row55837938"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="p26579147"><a name="p26579147"></a><a name="p26579147"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="p5427268"><a name="p5427268"></a><a name="p5427268"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row36955525"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="p40607543"><a name="p40607543"></a><a name="p40607543"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="p876673"><a name="p876673"></a><a name="p876673"></a>/v1/{project_id}/apigw/instances/{instance_id}/market/api-groups/status/{group_id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

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

**表 3**  参数说明

<a name="table3901708"></a>
<table><thead align="left"><tr id="row60617309"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p11054978"><a name="p11054978"></a><a name="p11054978"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="p23038040"><a name="p23038040"></a><a name="p23038040"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p54141958"><a name="p54141958"></a><a name="p54141958"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="p23422517"><a name="p23422517"></a><a name="p23422517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row964514516215"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row1121514457211"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row18175757"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p62950197"><a name="p62950197"></a><a name="p62950197"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="p65801173"><a name="p65801173"></a><a name="p65801173"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p28294806"><a name="p28294806"></a><a name="p28294806"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="p10177951"><a name="p10177951"></a><a name="p10177951"></a>需要审核或解除审核的API分组编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section17385329"></a>

**表 4**  参数说明

<a name="table37751912"></a>
<table><thead align="left"><tr id="row6532026"><th class="cellrowborder" valign="top" width="17.169999999999998%" id="mcps1.2.5.1.1"><p id="p59332065"><a name="p59332065"></a><a name="p59332065"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.2"><p id="p41167981"><a name="p41167981"></a><a name="p41167981"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.3"><p id="p46272198"><a name="p46272198"></a><a name="p46272198"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="52.53%" id="mcps1.2.5.1.4"><p id="p57060563"><a name="p57060563"></a><a name="p57060563"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row58502909"><td class="cellrowborder" valign="top" width="17.169999999999998%" headers="mcps1.2.5.1.1 "><p id="p41115179"><a name="p41115179"></a><a name="p41115179"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.2 "><p id="p41995206"><a name="p41995206"></a><a name="p41995206"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.3 "><p id="p46168501"><a name="p46168501"></a><a name="p46168501"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="52.53%" headers="mcps1.2.5.1.4 "><p id="p48661089"><a name="p48661089"></a><a name="p48661089"></a>分组状态：</p>
<a name="ul35296617"></a><a name="ul35296617"></a><ul id="ul35296617"><li>2：解除锁定</li><li>3：锁定状态</li></ul>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"status": 3
}
```

## 响应消息<a name="section66034445"></a>

**表 5**  参数说明

<a name="table19654592"></a>
<table><thead align="left"><tr id="row67084771"><th class="cellrowborder" valign="top" width="20.200000000000003%" id="mcps1.2.4.1.1"><p id="p65157346"><a name="p65157346"></a><a name="p65157346"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="p43253662"><a name="p43253662"></a><a name="p43253662"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="61.62%" id="mcps1.2.4.1.3"><p id="p13885694"><a name="p13885694"></a><a name="p13885694"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row50999402"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p37310923"><a name="p37310923"></a><a name="p37310923"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p2285961"><a name="p2285961"></a><a name="p2285961"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p50945163"><a name="p50945163"></a><a name="p50945163"></a>API分组编号</p>
</td>
</tr>
<tr id="row27822605"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p39038570"><a name="p39038570"></a><a name="p39038570"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p8007591"><a name="p8007591"></a><a name="p8007591"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p44635116"><a name="p44635116"></a><a name="p44635116"></a>API分组名称</p>
</td>
</tr>
<tr id="row58309879"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p25479736"><a name="p25479736"></a><a name="p25479736"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p50592767"><a name="p50592767"></a><a name="p50592767"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p4373425"><a name="p4373425"></a><a name="p4373425"></a>API分组描述</p>
</td>
</tr>
<tr id="row34110719"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p11504864"><a name="p11504864"></a><a name="p11504864"></a>update_time</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p59478793"><a name="p59478793"></a><a name="p59478793"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p53052963"><a name="p53052963"></a><a name="p53052963"></a>API分组最近更新时间</p>
</td>
</tr>
<tr id="row20904968"><td class="cellrowborder" valign="top" width="20.200000000000003%" headers="mcps1.2.4.1.1 "><p id="p15580818"><a name="p15580818"></a><a name="p15580818"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p54086728"><a name="p54086728"></a><a name="p54086728"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="61.62%" headers="mcps1.2.4.1.3 "><p id="p18948884"><a name="p18948884"></a><a name="p18948884"></a>API分组当前的状态</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": "73c58022-f20d-495a-a188-85d718647f09",
	"name": "api_group_001",
	"remark": "分组001",
	"update_time": "2017-12-28T11:57:27Z",
	"status": 3
}
```

## 状态码<a name="section22250241"></a>

**表 6**  返回消息说明

<a name="table785918"></a>
<table><thead align="left"><tr id="row35493205"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p56377346"><a name="p56377346"></a><a name="p56377346"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p3162295"><a name="p3162295"></a><a name="p3162295"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row54819357"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p11182939"><a name="p11182939"></a><a name="p11182939"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p33402906"><a name="p33402906"></a><a name="p33402906"></a>Created</p>
</td>
</tr>
<tr id="row32190706"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p57310356"><a name="p57310356"></a><a name="p57310356"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p11627275"><a name="p11627275"></a><a name="p11627275"></a>Bad Request</p>
</td>
</tr>
<tr id="row37536618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20567227"><a name="p20567227"></a><a name="p20567227"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p55332692"><a name="p55332692"></a><a name="p55332692"></a>Unauthorized</p>
</td>
</tr>
<tr id="row28232188"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p5105877"><a name="p5105877"></a><a name="p5105877"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p10922891"><a name="p10922891"></a><a name="p10922891"></a>Forbidden</p>
</td>
</tr>
<tr id="row31197156"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p43941679"><a name="p43941679"></a><a name="p43941679"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p2506251"><a name="p2506251"></a><a name="p2506251"></a>Not Found</p>
</td>
</tr>
<tr id="row22556263"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p15117982"><a name="p15117982"></a><a name="p15117982"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

