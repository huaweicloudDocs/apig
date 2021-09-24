# 授权<a name="ZH-CN_TOPIC_0000001081976179"></a>

## 功能介绍<a name="zh-cn_topic_0225568843_section18879496"></a>

APP创建成功后，还不能访问API，如果想要访问某个环境上的API，需要将该API在该环境上授权给APP。授权成功后，APP即可访问该环境上的这个API。

## URI<a name="zh-cn_topic_0225568843_section35697742"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568843_table32925424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568843_row22540195"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568843_p13816501"><a name="zh-cn_topic_0225568843_p13816501"></a><a name="zh-cn_topic_0225568843_p13816501"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568843_p45394783"><a name="zh-cn_topic_0225568843_p45394783"></a><a name="zh-cn_topic_0225568843_p45394783"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568843_row53098826"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p6037662"><a name="zh-cn_topic_0225568843_p6037662"></a><a name="zh-cn_topic_0225568843_p6037662"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p19288577"><a name="zh-cn_topic_0225568843_p19288577"></a><a name="zh-cn_topic_0225568843_p19288577"></a>/v1/{project_id}/apigw/instances/{instance_id}/app-auths</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568843_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568843_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568843_p23103637"><a name="zh-cn_topic_0225568843_p23103637"></a><a name="zh-cn_topic_0225568843_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568843_p59455291"><a name="zh-cn_topic_0225568843_p59455291"></a><a name="zh-cn_topic_0225568843_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568843_p51149303"><a name="zh-cn_topic_0225568843_p51149303"></a><a name="zh-cn_topic_0225568843_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568843_p49452846"><a name="zh-cn_topic_0225568843_p49452846"></a><a name="zh-cn_topic_0225568843_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568843_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568843_p55878963"><a name="zh-cn_topic_0225568843_p55878963"></a><a name="zh-cn_topic_0225568843_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568843_p29902160"><a name="zh-cn_topic_0225568843_p29902160"></a><a name="zh-cn_topic_0225568843_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568843_p6155914"><a name="zh-cn_topic_0225568843_p6155914"></a><a name="zh-cn_topic_0225568843_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568843_p28867016"><a name="zh-cn_topic_0225568843_p28867016"></a><a name="zh-cn_topic_0225568843_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568843_p1780913159538"><a name="zh-cn_topic_0225568843_p1780913159538"></a><a name="zh-cn_topic_0225568843_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568843_p9809215115310"><a name="zh-cn_topic_0225568843_p9809215115310"></a><a name="zh-cn_topic_0225568843_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568843_p1280914152538"><a name="zh-cn_topic_0225568843_p1280914152538"></a><a name="zh-cn_topic_0225568843_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568843_p1880914157537"><a name="zh-cn_topic_0225568843_p1880914157537"></a><a name="zh-cn_topic_0225568843_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568843_section52844230"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568843_table18870942"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568843_row61645284"><th class="cellrowborder" valign="top" width="15.15%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568843_p27212147"><a name="zh-cn_topic_0225568843_p27212147"></a><a name="zh-cn_topic_0225568843_p27212147"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568843_p56700331"><a name="zh-cn_topic_0225568843_p56700331"></a><a name="zh-cn_topic_0225568843_p56700331"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="14.14%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568843_p29324083"><a name="zh-cn_topic_0225568843_p29324083"></a><a name="zh-cn_topic_0225568843_p29324083"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568843_p26440499"><a name="zh-cn_topic_0225568843_p26440499"></a><a name="zh-cn_topic_0225568843_p26440499"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568843_row61305684"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568843_p66813373"><a name="zh-cn_topic_0225568843_p66813373"></a><a name="zh-cn_topic_0225568843_p66813373"></a>api_ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568843_p43174167"><a name="zh-cn_topic_0225568843_p43174167"></a><a name="zh-cn_topic_0225568843_p43174167"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568843_p7446666"><a name="zh-cn_topic_0225568843_p7446666"></a><a name="zh-cn_topic_0225568843_p7446666"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568843_p66309053"><a name="zh-cn_topic_0225568843_p66309053"></a><a name="zh-cn_topic_0225568843_p66309053"></a>API的编号列表</p>
<p id="zh-cn_topic_0225568843_p20917660"><a name="zh-cn_topic_0225568843_p20917660"></a><a name="zh-cn_topic_0225568843_p20917660"></a>可以选择租户自己的API，也可以选择从云市场上购买的API。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row15262696"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568843_p28318893"><a name="zh-cn_topic_0225568843_p28318893"></a><a name="zh-cn_topic_0225568843_p28318893"></a>app_ids</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568843_p12129019"><a name="zh-cn_topic_0225568843_p12129019"></a><a name="zh-cn_topic_0225568843_p12129019"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568843_p42926457"><a name="zh-cn_topic_0225568843_p42926457"></a><a name="zh-cn_topic_0225568843_p42926457"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568843_p54490959"><a name="zh-cn_topic_0225568843_p54490959"></a><a name="zh-cn_topic_0225568843_p54490959"></a>APP的编号列表</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row62570841"><td class="cellrowborder" valign="top" width="15.15%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568843_p35073364"><a name="zh-cn_topic_0225568843_p35073364"></a><a name="zh-cn_topic_0225568843_p35073364"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568843_p22370211"><a name="zh-cn_topic_0225568843_p22370211"></a><a name="zh-cn_topic_0225568843_p22370211"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="14.14%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568843_p47791"><a name="zh-cn_topic_0225568843_p47791"></a><a name="zh-cn_topic_0225568843_p47791"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568843_p3871071"><a name="zh-cn_topic_0225568843_p3871071"></a><a name="zh-cn_topic_0225568843_p3871071"></a>需要授权的环境编号</p>
</td>
</tr>
</tbody>
</table>

请求参数样例：

```
{
	"api_ids": ["5bbc47e2-95b0-4a56-904e-a3cdc422f8e9",
	"6632a062-9dcf-4f18-9646-3cabb925a290"],
	"app_ids": ["14b399ac-967f-4115-bb62-c0346b4537e9"],
	"env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID"
}
```

## 响应消息<a name="zh-cn_topic_0225568843_section52524212"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568843_table109779466461"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568843_row13977174694617"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568843_p20977134604610"><a name="zh-cn_topic_0225568843_p20977134604610"></a><a name="zh-cn_topic_0225568843_p20977134604610"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568843_p16977194611469"><a name="zh-cn_topic_0225568843_p16977194611469"></a><a name="zh-cn_topic_0225568843_p16977194611469"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568843_p129778467469"><a name="zh-cn_topic_0225568843_p129778467469"></a><a name="zh-cn_topic_0225568843_p129778467469"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568843_row12977104616467"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568843_p797714467461"><a name="zh-cn_topic_0225568843_p797714467461"></a><a name="zh-cn_topic_0225568843_p797714467461"></a>--</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568843_p1597719464465"><a name="zh-cn_topic_0225568843_p1597719464465"></a><a name="zh-cn_topic_0225568843_p1597719464465"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568843_p1697714634619"><a name="zh-cn_topic_0225568843_p1697714634619"></a><a name="zh-cn_topic_0225568843_p1697714634619"></a>API与APP的授权关系列表</p>
</td>
</tr>
</tbody>
</table>

**表 5**  API与APP授权关系列表消息说明

<a name="zh-cn_topic_0225568843_table1584515573365"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568843_row6845657113616"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568843_p1845115718366"><a name="zh-cn_topic_0225568843_p1845115718366"></a><a name="zh-cn_topic_0225568843_p1845115718366"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="21%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568843_p10845145773618"><a name="zh-cn_topic_0225568843_p10845145773618"></a><a name="zh-cn_topic_0225568843_p10845145773618"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="59%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568843_p68454577363"><a name="zh-cn_topic_0225568843_p68454577363"></a><a name="zh-cn_topic_0225568843_p68454577363"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568843_row68451557183610"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568843_p17845357143613"><a name="zh-cn_topic_0225568843_p17845357143613"></a><a name="zh-cn_topic_0225568843_p17845357143613"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568843_p58451557163620"><a name="zh-cn_topic_0225568843_p58451557163620"></a><a name="zh-cn_topic_0225568843_p58451557163620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568843_p1845185743619"><a name="zh-cn_topic_0225568843_p1845185743619"></a><a name="zh-cn_topic_0225568843_p1845185743619"></a>授权关系编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row1384515716361"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568843_p16845175713610"><a name="zh-cn_topic_0225568843_p16845175713610"></a><a name="zh-cn_topic_0225568843_p16845175713610"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568843_p1784545719369"><a name="zh-cn_topic_0225568843_p1784545719369"></a><a name="zh-cn_topic_0225568843_p1784545719369"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568843_p17326141743912"><a name="zh-cn_topic_0225568843_p17326141743912"></a><a name="zh-cn_topic_0225568843_p17326141743912"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row884545753619"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568843_p28451157183610"><a name="zh-cn_topic_0225568843_p28451157183610"></a><a name="zh-cn_topic_0225568843_p28451157183610"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568843_p12845357163617"><a name="zh-cn_topic_0225568843_p12845357163617"></a><a name="zh-cn_topic_0225568843_p12845357163617"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568843_p0845175717368"><a name="zh-cn_topic_0225568843_p0845175717368"></a><a name="zh-cn_topic_0225568843_p0845175717368"></a>APP编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row1484520572361"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568843_p188451057133617"><a name="zh-cn_topic_0225568843_p188451057133617"></a><a name="zh-cn_topic_0225568843_p188451057133617"></a>auth_time</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568843_p12845125783619"><a name="zh-cn_topic_0225568843_p12845125783619"></a><a name="zh-cn_topic_0225568843_p12845125783619"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568843_p1784535714361"><a name="zh-cn_topic_0225568843_p1784535714361"></a><a name="zh-cn_topic_0225568843_p1784535714361"></a>授权时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row10845757193620"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568843_p11845105715362"><a name="zh-cn_topic_0225568843_p11845105715362"></a><a name="zh-cn_topic_0225568843_p11845105715362"></a>auth_role</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568843_p78451357163611"><a name="zh-cn_topic_0225568843_p78451357163611"></a><a name="zh-cn_topic_0225568843_p78451357163611"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568843_p1784518572363"><a name="zh-cn_topic_0225568843_p1784518572363"></a><a name="zh-cn_topic_0225568843_p1784518572363"></a>授权者：</p>
<p id="zh-cn_topic_0225568843_p1581614211435"><a name="zh-cn_topic_0225568843_p1581614211435"></a><a name="zh-cn_topic_0225568843_p1581614211435"></a>PROVIDER：API提供者授权</p>
<p id="zh-cn_topic_0225568843_p36751423104316"><a name="zh-cn_topic_0225568843_p36751423104316"></a><a name="zh-cn_topic_0225568843_p36751423104316"></a>CONSUMER：API消费者授权</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row1684517579363"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568843_p13845175710369"><a name="zh-cn_topic_0225568843_p13845175710369"></a><a name="zh-cn_topic_0225568843_p13845175710369"></a>auth_result</p>
</td>
<td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568843_p15845957143620"><a name="zh-cn_topic_0225568843_p15845957143620"></a><a name="zh-cn_topic_0225568843_p15845957143620"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="59%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568843_p38451257163612"><a name="zh-cn_topic_0225568843_p38451257163612"></a><a name="zh-cn_topic_0225568843_p38451257163612"></a>授权结果：</p>
<p id="zh-cn_topic_0225568843_p1281614113430"><a name="zh-cn_topic_0225568843_p1281614113430"></a><a name="zh-cn_topic_0225568843_p1281614113430"></a>SUCCESS：授权成功</p>
<p id="zh-cn_topic_0225568843_p18221852144311"><a name="zh-cn_topic_0225568843_p18221852144311"></a><a name="zh-cn_topic_0225568843_p18221852144311"></a>SKIPPED：跳过</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
[{
	"id": "dffcaff92d144135a9f420fcd485bbf3",
	"api_id": "8aa097b00e9843efabc9c593d11b769d",
	"app_id": "f8c6ea15-0d1b-4c5b-bd4b-911610bd3b3e",
	"auth_time": "2018-03-30T09:37:43.490197204Z",
	"auth_role": "PROVIDER",
	"auth_result": "SUCCESS"
}]
```

## 状态码<a name="zh-cn_topic_0225568843_section5836023"></a>

**表 6**  返回消息说明

<a name="zh-cn_topic_0225568843_table4431296"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568843_row6152568"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568843_p28595977"><a name="zh-cn_topic_0225568843_p28595977"></a><a name="zh-cn_topic_0225568843_p28595977"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568843_p34572832"><a name="zh-cn_topic_0225568843_p34572832"></a><a name="zh-cn_topic_0225568843_p34572832"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568843_row48935970"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p4390649"><a name="zh-cn_topic_0225568843_p4390649"></a><a name="zh-cn_topic_0225568843_p4390649"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p73578115452"><a name="zh-cn_topic_0225568843_p73578115452"></a><a name="zh-cn_topic_0225568843_p73578115452"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row46667129"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p21941106"><a name="zh-cn_topic_0225568843_p21941106"></a><a name="zh-cn_topic_0225568843_p21941106"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p32399196"><a name="zh-cn_topic_0225568843_p32399196"></a><a name="zh-cn_topic_0225568843_p32399196"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row23157315"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p63803225"><a name="zh-cn_topic_0225568843_p63803225"></a><a name="zh-cn_topic_0225568843_p63803225"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p678707"><a name="zh-cn_topic_0225568843_p678707"></a><a name="zh-cn_topic_0225568843_p678707"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row6108365"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p25015561"><a name="zh-cn_topic_0225568843_p25015561"></a><a name="zh-cn_topic_0225568843_p25015561"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p12994557"><a name="zh-cn_topic_0225568843_p12994557"></a><a name="zh-cn_topic_0225568843_p12994557"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row49842156"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p10682856"><a name="zh-cn_topic_0225568843_p10682856"></a><a name="zh-cn_topic_0225568843_p10682856"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p60005041"><a name="zh-cn_topic_0225568843_p60005041"></a><a name="zh-cn_topic_0225568843_p60005041"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row3174462"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p55804836"><a name="zh-cn_topic_0225568843_p55804836"></a><a name="zh-cn_topic_0225568843_p55804836"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p23897867"><a name="zh-cn_topic_0225568843_p23897867"></a><a name="zh-cn_topic_0225568843_p23897867"></a>Conflict</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568843_row13754214"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568843_p40349553"><a name="zh-cn_topic_0225568843_p40349553"></a><a name="zh-cn_topic_0225568843_p40349553"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568843_p14947689"><a name="zh-cn_topic_0225568843_p14947689"></a><a name="zh-cn_topic_0225568843_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

