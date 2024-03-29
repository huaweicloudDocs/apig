# 绑定域名证书<a name="ZH-CN_TOPIC_0000001082135217"></a>

## 功能介绍<a name="zh-cn_topic_0225568972_section5819630194117"></a>

如果创建API时，“定义API请求”使用HTTPS请求协议，那么在独立域名中需要添加SSL证书。

本章节主要介绍为特定域名绑定证书。

## URI<a name="zh-cn_topic_0225568972_section881973019417"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568972_table773935944313"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568972_row10739259144317"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568972_p442710812449"><a name="zh-cn_topic_0225568972_p442710812449"></a><a name="zh-cn_topic_0225568972_p442710812449"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568972_p1642778124420"><a name="zh-cn_topic_0225568972_p1642778124420"></a><a name="zh-cn_topic_0225568972_p1642778124420"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568972_row17739559204316"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568972_p10427198164415"><a name="zh-cn_topic_0225568972_p10427198164415"></a><a name="zh-cn_topic_0225568972_p10427198164415"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568972_p104271789444"><a name="zh-cn_topic_0225568972_p104271789444"></a><a name="zh-cn_topic_0225568972_p104271789444"></a>/v1/{project_id}/apigw/instances/{instance_id}/api-groups/{group_id}/domains/{domain_id}/certificate</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568972_table339495"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568972_row19182484"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568972_p10277368"><a name="zh-cn_topic_0225568972_p10277368"></a><a name="zh-cn_topic_0225568972_p10277368"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568972_p27160509"><a name="zh-cn_topic_0225568972_p27160509"></a><a name="zh-cn_topic_0225568972_p27160509"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568972_p52517643"><a name="zh-cn_topic_0225568972_p52517643"></a><a name="zh-cn_topic_0225568972_p52517643"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568972_p26070665"><a name="zh-cn_topic_0225568972_p26070665"></a><a name="zh-cn_topic_0225568972_p26070665"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568972_row1827901965516"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568972_p55878963"><a name="zh-cn_topic_0225568972_p55878963"></a><a name="zh-cn_topic_0225568972_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568972_p29902160"><a name="zh-cn_topic_0225568972_p29902160"></a><a name="zh-cn_topic_0225568972_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568972_p6155914"><a name="zh-cn_topic_0225568972_p6155914"></a><a name="zh-cn_topic_0225568972_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568972_p28867016"><a name="zh-cn_topic_0225568972_p28867016"></a><a name="zh-cn_topic_0225568972_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row166876181554"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568972_p1780913159538"><a name="zh-cn_topic_0225568972_p1780913159538"></a><a name="zh-cn_topic_0225568972_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568972_p9809215115310"><a name="zh-cn_topic_0225568972_p9809215115310"></a><a name="zh-cn_topic_0225568972_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568972_p1280914152538"><a name="zh-cn_topic_0225568972_p1280914152538"></a><a name="zh-cn_topic_0225568972_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568972_p1880914157537"><a name="zh-cn_topic_0225568972_p1880914157537"></a><a name="zh-cn_topic_0225568972_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row31349087"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568972_p56248118"><a name="zh-cn_topic_0225568972_p56248118"></a><a name="zh-cn_topic_0225568972_p56248118"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568972_p59803701"><a name="zh-cn_topic_0225568972_p59803701"></a><a name="zh-cn_topic_0225568972_p59803701"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568972_p12261637"><a name="zh-cn_topic_0225568972_p12261637"></a><a name="zh-cn_topic_0225568972_p12261637"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568972_p53668558"><a name="zh-cn_topic_0225568972_p53668558"></a><a name="zh-cn_topic_0225568972_p53668558"></a>分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row67461856163611"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568972_p147479565365"><a name="zh-cn_topic_0225568972_p147479565365"></a><a name="zh-cn_topic_0225568972_p147479565365"></a>domain_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568972_p153301010123713"><a name="zh-cn_topic_0225568972_p153301010123713"></a><a name="zh-cn_topic_0225568972_p153301010123713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568972_p14330710143716"><a name="zh-cn_topic_0225568972_p14330710143716"></a><a name="zh-cn_topic_0225568972_p14330710143716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568972_p9747195653615"><a name="zh-cn_topic_0225568972_p9747195653615"></a><a name="zh-cn_topic_0225568972_p9747195653615"></a>域名的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568972_section1681914308419"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568972_table2819133012418"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568972_row1879911301414"><th class="cellrowborder" valign="top" width="15.46154615461546%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568972_p19799163014416"><a name="zh-cn_topic_0225568972_p19799163014416"></a><a name="zh-cn_topic_0225568972_p19799163014416"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568972_p17799930184111"><a name="zh-cn_topic_0225568972_p17799930184111"></a><a name="zh-cn_topic_0225568972_p17799930184111"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568972_p0799930174117"><a name="zh-cn_topic_0225568972_p0799930174117"></a><a name="zh-cn_topic_0225568972_p0799930174117"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568972_p1079953034114"><a name="zh-cn_topic_0225568972_p1079953034114"></a><a name="zh-cn_topic_0225568972_p1079953034114"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568972_row10799530204120"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568972_p177999309417"><a name="zh-cn_topic_0225568972_p177999309417"></a><a name="zh-cn_topic_0225568972_p177999309417"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568972_p4799153015411"><a name="zh-cn_topic_0225568972_p4799153015411"></a><a name="zh-cn_topic_0225568972_p4799153015411"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568972_p8799113094114"><a name="zh-cn_topic_0225568972_p8799113094114"></a><a name="zh-cn_topic_0225568972_p8799113094114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568972_p948883074219"><a name="zh-cn_topic_0225568972_p948883074219"></a><a name="zh-cn_topic_0225568972_p948883074219"></a>证书名称。</p>
<p id="zh-cn_topic_0225568972_p1471110513547"><a name="zh-cn_topic_0225568972_p1471110513547"></a><a name="zh-cn_topic_0225568972_p1471110513547"></a>长度为4 ~ 50位的字符串，字符串由中文、英文字母、数字、"_"组成，且只能以英文或中文开头。</p>
<div class="note" id="zh-cn_topic_0225568972_note15331931175"><a name="zh-cn_topic_0225568972_note15331931175"></a><a name="zh-cn_topic_0225568972_note15331931175"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568972_p1833153875"><a name="zh-cn_topic_0225568972_p1833153875"></a><a name="zh-cn_topic_0225568972_p1833153875"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row3799123014411"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568972_p0799193019417"><a name="zh-cn_topic_0225568972_p0799193019417"></a><a name="zh-cn_topic_0225568972_p0799193019417"></a>cert_content</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568972_p197994309418"><a name="zh-cn_topic_0225568972_p197994309418"></a><a name="zh-cn_topic_0225568972_p197994309418"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568972_p1779910304414"><a name="zh-cn_topic_0225568972_p1779910304414"></a><a name="zh-cn_topic_0225568972_p1779910304414"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568972_p579933024118"><a name="zh-cn_topic_0225568972_p579933024118"></a><a name="zh-cn_topic_0225568972_p579933024118"></a>证书内容。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row13799330124117"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568972_p479983074111"><a name="zh-cn_topic_0225568972_p479983074111"></a><a name="zh-cn_topic_0225568972_p479983074111"></a>private_key</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568972_p27991530114111"><a name="zh-cn_topic_0225568972_p27991530114111"></a><a name="zh-cn_topic_0225568972_p27991530114111"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568972_p2079910304412"><a name="zh-cn_topic_0225568972_p2079910304412"></a><a name="zh-cn_topic_0225568972_p2079910304412"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568972_p13799730104112"><a name="zh-cn_topic_0225568972_p13799730104112"></a><a name="zh-cn_topic_0225568972_p13799730104112"></a>私钥内容。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"cert_content": "example",
	"name": "test_ssl",
	"private_key": "example"
}
```

## 响应消息<a name="zh-cn_topic_0225568972_section1583533015411"></a>

**表 4**  参数说明

<a name="zh-cn_topic_0225568972_table178351830144116"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568972_row14799153017414"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568972_p18799133011416"><a name="zh-cn_topic_0225568972_p18799133011416"></a><a name="zh-cn_topic_0225568972_p18799133011416"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568972_p279903013414"><a name="zh-cn_topic_0225568972_p279903013414"></a><a name="zh-cn_topic_0225568972_p279903013414"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568972_p679993010416"><a name="zh-cn_topic_0225568972_p679993010416"></a><a name="zh-cn_topic_0225568972_p679993010416"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568972_row3799113014417"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568972_p2799530194111"><a name="zh-cn_topic_0225568972_p2799530194111"></a><a name="zh-cn_topic_0225568972_p2799530194111"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568972_p37991530184114"><a name="zh-cn_topic_0225568972_p37991530184114"></a><a name="zh-cn_topic_0225568972_p37991530184114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568972_p15799203014414"><a name="zh-cn_topic_0225568972_p15799203014414"></a><a name="zh-cn_topic_0225568972_p15799203014414"></a>自定义域名的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row8799143015416"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568972_p9799103011416"><a name="zh-cn_topic_0225568972_p9799103011416"></a><a name="zh-cn_topic_0225568972_p9799103011416"></a>url_domain</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568972_p479943064119"><a name="zh-cn_topic_0225568972_p479943064119"></a><a name="zh-cn_topic_0225568972_p479943064119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568972_p1779913016410"><a name="zh-cn_topic_0225568972_p1779913016410"></a><a name="zh-cn_topic_0225568972_p1779913016410"></a>自定义域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row27991830124111"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568972_p47991130184118"><a name="zh-cn_topic_0225568972_p47991130184118"></a><a name="zh-cn_topic_0225568972_p47991130184118"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568972_p67991430114113"><a name="zh-cn_topic_0225568972_p67991430114113"></a><a name="zh-cn_topic_0225568972_p67991430114113"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568972_p1979915302419"><a name="zh-cn_topic_0225568972_p1979915302419"></a><a name="zh-cn_topic_0225568972_p1979915302419"></a>解析状态值</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row179913034114"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568972_p1179903094117"><a name="zh-cn_topic_0225568972_p1179903094117"></a><a name="zh-cn_topic_0225568972_p1179903094117"></a>ssl_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568972_p1979993013416"><a name="zh-cn_topic_0225568972_p1979993013416"></a><a name="zh-cn_topic_0225568972_p1979993013416"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568972_p1679983012413"><a name="zh-cn_topic_0225568972_p1679983012413"></a><a name="zh-cn_topic_0225568972_p1679983012413"></a>证书的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row17799730134117"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568972_p8799193015410"><a name="zh-cn_topic_0225568972_p8799193015410"></a><a name="zh-cn_topic_0225568972_p8799193015410"></a>ssl_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568972_p6799430144112"><a name="zh-cn_topic_0225568972_p6799430144112"></a><a name="zh-cn_topic_0225568972_p6799430144112"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568972_p779903014419"><a name="zh-cn_topic_0225568972_p779903014419"></a><a name="zh-cn_topic_0225568972_p779903014419"></a>证书的名称</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"id": " b9be707660c5406394f8973e087bae20",
	"url_domain": "www.example.com",
	"status": 3,
	"ssl_id ": "0a515af69f4e4dcca84fbf85f68c0e27",
	"ssl_name": "证书"
}
```

## 状态码<a name="zh-cn_topic_0225568972_section2083573084114"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568972_table1083533064119"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568972_row879916303414"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568972_p1979933014119"><a name="zh-cn_topic_0225568972_p1979933014119"></a><a name="zh-cn_topic_0225568972_p1979933014119"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568972_p9799153064112"><a name="zh-cn_topic_0225568972_p9799153064112"></a><a name="zh-cn_topic_0225568972_p9799153064112"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568972_row1179918309413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568972_p0799163011418"><a name="zh-cn_topic_0225568972_p0799163011418"></a><a name="zh-cn_topic_0225568972_p0799163011418"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568972_p948803015424"><a name="zh-cn_topic_0225568972_p948803015424"></a><a name="zh-cn_topic_0225568972_p948803015424"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row0799133014117"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568972_p1179993034116"><a name="zh-cn_topic_0225568972_p1179993034116"></a><a name="zh-cn_topic_0225568972_p1179993034116"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568972_p164881130154211"><a name="zh-cn_topic_0225568972_p164881130154211"></a><a name="zh-cn_topic_0225568972_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row1879983011414"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568972_p15799230134110"><a name="zh-cn_topic_0225568972_p15799230134110"></a><a name="zh-cn_topic_0225568972_p15799230134110"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568972_p1848810308429"><a name="zh-cn_topic_0225568972_p1848810308429"></a><a name="zh-cn_topic_0225568972_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row8799143014412"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568972_p19799630144115"><a name="zh-cn_topic_0225568972_p19799630144115"></a><a name="zh-cn_topic_0225568972_p19799630144115"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568972_p10488193018426"><a name="zh-cn_topic_0225568972_p10488193018426"></a><a name="zh-cn_topic_0225568972_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row2799113015413"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568972_p167991530204113"><a name="zh-cn_topic_0225568972_p167991530204113"></a><a name="zh-cn_topic_0225568972_p167991530204113"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568972_p4488103094212"><a name="zh-cn_topic_0225568972_p4488103094212"></a><a name="zh-cn_topic_0225568972_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568972_row67991330154113"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568972_p57999309411"><a name="zh-cn_topic_0225568972_p57999309411"></a><a name="zh-cn_topic_0225568972_p57999309411"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568972_p048813014216"><a name="zh-cn_topic_0225568972_p048813014216"></a><a name="zh-cn_topic_0225568972_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

