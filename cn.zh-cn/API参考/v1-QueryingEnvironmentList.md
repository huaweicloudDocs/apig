# 查询环境列表<a name="ZH-CN_TOPIC_0000001082135181"></a>

## 功能介绍<a name="zh-cn_topic_0225568852_section51058735"></a>

查询符合条件的环境列表。

## URI<a name="zh-cn_topic_0225568852_section56875432"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568852_table26537273"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568852_row97700"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568852_p7913769"><a name="zh-cn_topic_0225568852_p7913769"></a><a name="zh-cn_topic_0225568852_p7913769"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568852_p37035575"><a name="zh-cn_topic_0225568852_p37035575"></a><a name="zh-cn_topic_0225568852_p37035575"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568852_row47091573"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568852_p56321035"><a name="zh-cn_topic_0225568852_p56321035"></a><a name="zh-cn_topic_0225568852_p56321035"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568852_p65709986"><a name="zh-cn_topic_0225568852_p65709986"></a><a name="zh-cn_topic_0225568852_p65709986"></a>/v1/{project_id}/apigw/instances/{instance_id}/envs[?page_no, page_size,name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：name、page\_size、page\_no。

**表 2**  参数说明

<a name="zh-cn_topic_0225568852_table8687743"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568852_row22440872"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568852_p5771382"><a name="zh-cn_topic_0225568852_p5771382"></a><a name="zh-cn_topic_0225568852_p5771382"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.95%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568852_p64828808"><a name="zh-cn_topic_0225568852_p64828808"></a><a name="zh-cn_topic_0225568852_p64828808"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.77%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568852_p16642119"><a name="zh-cn_topic_0225568852_p16642119"></a><a name="zh-cn_topic_0225568852_p16642119"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="34.28%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568852_p5834394"><a name="zh-cn_topic_0225568852_p5834394"></a><a name="zh-cn_topic_0225568852_p5834394"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568852_row233893024818"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568852_p55878963"><a name="zh-cn_topic_0225568852_p55878963"></a><a name="zh-cn_topic_0225568852_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.95%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568852_p29902160"><a name="zh-cn_topic_0225568852_p29902160"></a><a name="zh-cn_topic_0225568852_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568852_p6155914"><a name="zh-cn_topic_0225568852_p6155914"></a><a name="zh-cn_topic_0225568852_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.28%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568852_p28867016"><a name="zh-cn_topic_0225568852_p28867016"></a><a name="zh-cn_topic_0225568852_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row5160173044810"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568852_p1780913159538"><a name="zh-cn_topic_0225568852_p1780913159538"></a><a name="zh-cn_topic_0225568852_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.95%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568852_p9809215115310"><a name="zh-cn_topic_0225568852_p9809215115310"></a><a name="zh-cn_topic_0225568852_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568852_p1280914152538"><a name="zh-cn_topic_0225568852_p1280914152538"></a><a name="zh-cn_topic_0225568852_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.28%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568852_p1880914157537"><a name="zh-cn_topic_0225568852_p1880914157537"></a><a name="zh-cn_topic_0225568852_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row2823914"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568852_p27410462"><a name="zh-cn_topic_0225568852_p27410462"></a><a name="zh-cn_topic_0225568852_p27410462"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20.95%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568852_p5654943"><a name="zh-cn_topic_0225568852_p5654943"></a><a name="zh-cn_topic_0225568852_p5654943"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568852_p55397204"><a name="zh-cn_topic_0225568852_p55397204"></a><a name="zh-cn_topic_0225568852_p55397204"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.28%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568852_p1186411103575"><a name="zh-cn_topic_0225568852_p1186411103575"></a><a name="zh-cn_topic_0225568852_p1186411103575"></a>环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row52134612"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568852_p62154076"><a name="zh-cn_topic_0225568852_p62154076"></a><a name="zh-cn_topic_0225568852_p62154076"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="20.95%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568852_p1315380"><a name="zh-cn_topic_0225568852_p1315380"></a><a name="zh-cn_topic_0225568852_p1315380"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568852_p39436932"><a name="zh-cn_topic_0225568852_p39436932"></a><a name="zh-cn_topic_0225568852_p39436932"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="34.28%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568852_p40274933"><a name="zh-cn_topic_0225568852_p40274933"></a><a name="zh-cn_topic_0225568852_p40274933"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row26930081"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568852_p33852966"><a name="zh-cn_topic_0225568852_p33852966"></a><a name="zh-cn_topic_0225568852_p33852966"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="20.95%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568852_p57735711"><a name="zh-cn_topic_0225568852_p57735711"></a><a name="zh-cn_topic_0225568852_p57735711"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568852_p46081013"><a name="zh-cn_topic_0225568852_p46081013"></a><a name="zh-cn_topic_0225568852_p46081013"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="34.28%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568852_p41574543"><a name="zh-cn_topic_0225568852_p41574543"></a><a name="zh-cn_topic_0225568852_p41574543"></a>页码，默认值：1</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row179311037557"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568852_p297092819498"><a name="zh-cn_topic_0225568852_p297092819498"></a><a name="zh-cn_topic_0225568852_p297092819498"></a>precise_search</p>
</td>
<td class="cellrowborder" valign="top" width="20.95%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568852_p397092812491"><a name="zh-cn_topic_0225568852_p397092812491"></a><a name="zh-cn_topic_0225568852_p397092812491"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.77%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568852_p49701728194913"><a name="zh-cn_topic_0225568852_p49701728194913"></a><a name="zh-cn_topic_0225568852_p49701728194913"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="34.28%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568852_p19970928194911"><a name="zh-cn_topic_0225568852_p19970928194911"></a><a name="zh-cn_topic_0225568852_p19970928194911"></a>指定需要精确匹配查找的参数名称，目前仅支持variable_name</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568852_section42116847"></a>

无

## 响应消息<a name="zh-cn_topic_0225568852_section56021456"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568852_table18843207"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568852_row11636316"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568852_p3017546"><a name="zh-cn_topic_0225568852_p3017546"></a><a name="zh-cn_topic_0225568852_p3017546"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568852_p43094713"><a name="zh-cn_topic_0225568852_p43094713"></a><a name="zh-cn_topic_0225568852_p43094713"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568852_p1010897"><a name="zh-cn_topic_0225568852_p1010897"></a><a name="zh-cn_topic_0225568852_p1010897"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568852_row14773817"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568852_p55828505"><a name="zh-cn_topic_0225568852_p55828505"></a><a name="zh-cn_topic_0225568852_p55828505"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568852_p25815066"><a name="zh-cn_topic_0225568852_p25815066"></a><a name="zh-cn_topic_0225568852_p25815066"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568852_p10645603"><a name="zh-cn_topic_0225568852_p10645603"></a><a name="zh-cn_topic_0225568852_p10645603"></a>符合条件的环境总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row28701571"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568852_p43125900"><a name="zh-cn_topic_0225568852_p43125900"></a><a name="zh-cn_topic_0225568852_p43125900"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568852_p3537010"><a name="zh-cn_topic_0225568852_p3537010"></a><a name="zh-cn_topic_0225568852_p3537010"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568852_p18062364"><a name="zh-cn_topic_0225568852_p18062364"></a><a name="zh-cn_topic_0225568852_p18062364"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row28343550"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568852_p14126218"><a name="zh-cn_topic_0225568852_p14126218"></a><a name="zh-cn_topic_0225568852_p14126218"></a>envs</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568852_p3373006"><a name="zh-cn_topic_0225568852_p3373006"></a><a name="zh-cn_topic_0225568852_p3373006"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568852_p4778099"><a name="zh-cn_topic_0225568852_p4778099"></a><a name="zh-cn_topic_0225568852_p4778099"></a>本次返回的环境列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  envs参数说明

<a name="zh-cn_topic_0225568852_table43002897"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568852_row40093548"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568852_p26351947"><a name="zh-cn_topic_0225568852_p26351947"></a><a name="zh-cn_topic_0225568852_p26351947"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568852_p54132987"><a name="zh-cn_topic_0225568852_p54132987"></a><a name="zh-cn_topic_0225568852_p54132987"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568852_p22695844"><a name="zh-cn_topic_0225568852_p22695844"></a><a name="zh-cn_topic_0225568852_p22695844"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568852_row26424045"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568852_p59972862"><a name="zh-cn_topic_0225568852_p59972862"></a><a name="zh-cn_topic_0225568852_p59972862"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568852_p25963648"><a name="zh-cn_topic_0225568852_p25963648"></a><a name="zh-cn_topic_0225568852_p25963648"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568852_p22680730"><a name="zh-cn_topic_0225568852_p22680730"></a><a name="zh-cn_topic_0225568852_p22680730"></a>环境ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row2799984"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568852_p25472162"><a name="zh-cn_topic_0225568852_p25472162"></a><a name="zh-cn_topic_0225568852_p25472162"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568852_p49979265"><a name="zh-cn_topic_0225568852_p49979265"></a><a name="zh-cn_topic_0225568852_p49979265"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568852_p21788660"><a name="zh-cn_topic_0225568852_p21788660"></a><a name="zh-cn_topic_0225568852_p21788660"></a>环境名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row61880217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568852_p46241670"><a name="zh-cn_topic_0225568852_p46241670"></a><a name="zh-cn_topic_0225568852_p46241670"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568852_p54587771"><a name="zh-cn_topic_0225568852_p54587771"></a><a name="zh-cn_topic_0225568852_p54587771"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568852_p59533345"><a name="zh-cn_topic_0225568852_p59533345"></a><a name="zh-cn_topic_0225568852_p59533345"></a>创建时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row66038062"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568852_p47482783"><a name="zh-cn_topic_0225568852_p47482783"></a><a name="zh-cn_topic_0225568852_p47482783"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568852_p20900246"><a name="zh-cn_topic_0225568852_p20900246"></a><a name="zh-cn_topic_0225568852_p20900246"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568852_p15198328"><a name="zh-cn_topic_0225568852_p15198328"></a><a name="zh-cn_topic_0225568852_p15198328"></a>描述信息</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"envs": [{
		"id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"name": "RELEASE",
		"remark": "生产环境",
		"create_time": "2017-12-29T03:39:03.165657Z"
	},
	{
		"id": "cca3616a-f368-4b32-9064-b2a631cb3eeb",
		"name": "DEVELOP",
		"remark": "开发环境",
		"create_time": "2017-12-28T12:50:47Z"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568852_section43507308"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568852_table40155185"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568852_row33141868"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568852_p136762"><a name="zh-cn_topic_0225568852_p136762"></a><a name="zh-cn_topic_0225568852_p136762"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568852_p11077728"><a name="zh-cn_topic_0225568852_p11077728"></a><a name="zh-cn_topic_0225568852_p11077728"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568852_row24880775"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568852_p2076886"><a name="zh-cn_topic_0225568852_p2076886"></a><a name="zh-cn_topic_0225568852_p2076886"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568852_p34010102"><a name="zh-cn_topic_0225568852_p34010102"></a><a name="zh-cn_topic_0225568852_p34010102"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row37655468"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568852_p30194056"><a name="zh-cn_topic_0225568852_p30194056"></a><a name="zh-cn_topic_0225568852_p30194056"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568852_p29799432"><a name="zh-cn_topic_0225568852_p29799432"></a><a name="zh-cn_topic_0225568852_p29799432"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row66868297"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568852_p47622971"><a name="zh-cn_topic_0225568852_p47622971"></a><a name="zh-cn_topic_0225568852_p47622971"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568852_p32255429"><a name="zh-cn_topic_0225568852_p32255429"></a><a name="zh-cn_topic_0225568852_p32255429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568852_row21863411"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568852_p26105877"><a name="zh-cn_topic_0225568852_p26105877"></a><a name="zh-cn_topic_0225568852_p26105877"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568852_p34201316"><a name="zh-cn_topic_0225568852_p34201316"></a><a name="zh-cn_topic_0225568852_p34201316"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

