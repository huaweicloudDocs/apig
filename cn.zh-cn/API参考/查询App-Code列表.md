# 查询App Code列表<a name="apig-phapi-200226004"></a>

## 功能介绍<a name="zh-cn_topic_0118921764_section48433431"></a>

查询App Code列表。

## URI<a name="zh-cn_topic_0118921764_section33247697"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0118921764_table33538507"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921764_row26439774"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921764_p61246963"><a name="zh-cn_topic_0118921764_p61246963"></a><a name="zh-cn_topic_0118921764_p61246963"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921764_p62056956"><a name="zh-cn_topic_0118921764_p62056956"></a><a name="zh-cn_topic_0118921764_p62056956"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921764_row60557538"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921764_p6213516"><a name="zh-cn_topic_0118921764_p6213516"></a><a name="zh-cn_topic_0118921764_p6213516"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p3251109122210"><a name="p3251109122210"></a><a name="p3251109122210"></a>/v1/{project_id}/apigw/instances/{instance_id}/apps/{app_id}/app-codes/[?page_size, page_no]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0118921763_table8767205"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921763_row50080004"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0118921763_p29948539"><a name="zh-cn_topic_0118921763_p29948539"></a><a name="zh-cn_topic_0118921763_p29948539"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0118921763_p9912623"><a name="zh-cn_topic_0118921763_p9912623"></a><a name="zh-cn_topic_0118921763_p9912623"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0118921763_p64724999"><a name="zh-cn_topic_0118921763_p64724999"></a><a name="zh-cn_topic_0118921763_p64724999"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0118921763_p8233580"><a name="zh-cn_topic_0118921763_p8233580"></a><a name="zh-cn_topic_0118921763_p8233580"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1917213481870"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row14875164513717"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row943312981910"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p24341599197"><a name="p24341599197"></a><a name="p24341599197"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="p5434290195"><a name="p5434290195"></a><a name="p5434290195"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.3 "><p id="p543529161911"><a name="p543529161911"></a><a name="p543529161911"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.4 "><p id="p19435996196"><a name="p19435996196"></a><a name="p19435996196"></a>APP的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0118921764_section30793819"></a>

无

## 响应消息<a name="zh-cn_topic_0118921764_section11271404"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0118921764_table23954455"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921764_row66752668"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921764_p38257064"><a name="zh-cn_topic_0118921764_p38257064"></a><a name="zh-cn_topic_0118921764_p38257064"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921764_p11814447"><a name="zh-cn_topic_0118921764_p11814447"></a><a name="zh-cn_topic_0118921764_p11814447"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921764_p17446171"><a name="zh-cn_topic_0118921764_p17446171"></a><a name="zh-cn_topic_0118921764_p17446171"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921764_row3853780"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921764_p43720769"><a name="zh-cn_topic_0118921764_p43720769"></a><a name="zh-cn_topic_0118921764_p43720769"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921764_p51721419"><a name="zh-cn_topic_0118921764_p51721419"></a><a name="zh-cn_topic_0118921764_p51721419"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921764_p28685401"><a name="zh-cn_topic_0118921764_p28685401"></a><a name="zh-cn_topic_0118921764_p28685401"></a>符合条件的APP总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row56842021"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921764_p40801013"><a name="zh-cn_topic_0118921764_p40801013"></a><a name="zh-cn_topic_0118921764_p40801013"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921764_p16547774"><a name="zh-cn_topic_0118921764_p16547774"></a><a name="zh-cn_topic_0118921764_p16547774"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921764_p65301287"><a name="zh-cn_topic_0118921764_p65301287"></a><a name="zh-cn_topic_0118921764_p65301287"></a>本次查询返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row50840671"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921764_p24453659"><a name="zh-cn_topic_0118921764_p24453659"></a><a name="zh-cn_topic_0118921764_p24453659"></a>app_codes</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921764_p34589388"><a name="zh-cn_topic_0118921764_p34589388"></a><a name="zh-cn_topic_0118921764_p34589388"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921764_p50277082"><a name="zh-cn_topic_0118921764_p50277082"></a><a name="zh-cn_topic_0118921764_p50277082"></a>App Code列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  app\_codes参数说明

<a name="zh-cn_topic_0118921764_table49840559"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921764_row181838"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0118921764_p14728898"><a name="zh-cn_topic_0118921764_p14728898"></a><a name="zh-cn_topic_0118921764_p14728898"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0118921764_p52190083"><a name="zh-cn_topic_0118921764_p52190083"></a><a name="zh-cn_topic_0118921764_p52190083"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0118921764_p66647160"><a name="zh-cn_topic_0118921764_p66647160"></a><a name="zh-cn_topic_0118921764_p66647160"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921764_row29710857"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p59535008"><a name="zh-cn_topic_0118921758_p59535008"></a><a name="zh-cn_topic_0118921758_p59535008"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p57606383"><a name="zh-cn_topic_0118921758_p57606383"></a><a name="zh-cn_topic_0118921758_p57606383"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p35605479"><a name="zh-cn_topic_0118921758_p35605479"></a><a name="zh-cn_topic_0118921758_p35605479"></a>编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row5661128"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p52372904"><a name="zh-cn_topic_0118921758_p52372904"></a><a name="zh-cn_topic_0118921758_p52372904"></a>app_code</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p14346860"><a name="zh-cn_topic_0118921758_p14346860"></a><a name="zh-cn_topic_0118921758_p14346860"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p21245012"><a name="zh-cn_topic_0118921758_p21245012"></a><a name="zh-cn_topic_0118921758_p21245012"></a>App Code值</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row52424003"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p52575507"><a name="zh-cn_topic_0118921758_p52575507"></a><a name="zh-cn_topic_0118921758_p52575507"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p30757702"><a name="zh-cn_topic_0118921758_p30757702"></a><a name="zh-cn_topic_0118921758_p30757702"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p1284315287524"><a name="p1284315287524"></a><a name="p1284315287524"></a>APP的ID</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row45232137"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0118921758_p44372920"><a name="zh-cn_topic_0118921758_p44372920"></a><a name="zh-cn_topic_0118921758_p44372920"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0118921758_p37436804"><a name="zh-cn_topic_0118921758_p37436804"></a><a name="zh-cn_topic_0118921758_p37436804"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0118921758_p12482251"><a name="zh-cn_topic_0118921758_p12482251"></a><a name="zh-cn_topic_0118921758_p12482251"></a>创建时间</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
    "total": 4,
    "size": 4,
    "app_codes": [
        {
            "app_code": "7049bc6b5b4140b4a93340f2555641bbc4cc7179e7734baeb85a773041cbfb1a",
            "id": "5434c97d872f41a88b039a8a973e0652",
            "app_id": "db246f3f2ecd45f29ecb0f305e821fdc",
            "create_time": "2019-06-05T08:54:25Z"
        },
        {
            "app_code": "asdssdadasdsssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssssss",
            "id": "787860297c3d4e51b76fff8abd089a94",
            "app_id": "db246f3f2ecd45f29ecb0f305e821fdc",
            "create_time": "2019-06-05T04:56:51Z"
        },
        {
            "app_code": "MeOAgeemgeatouS7peiwg+ivleaooeW8j+aJp+ihjHNoZWxs6ISa5pysICAgLS0tLS0tLS3lronoo4XljIXmrovnlZnvvIzkuIvkuKrniYjmnKzlop7liqDpg6jnvbLlronoo4XljIXliKDpmaQ22222221234124",
            "id": "c7a87cdfa50b4a4eaa644901c4dddb98",
            "app_id": "db246f3f2ecd45f29ecb0f305e821fdc",
            "create_time": "2019-05-10T03:14:02Z"
        },
        {
            "app_code": "MeOAgeemgeatouS7peiwg+ivleaooeW8j+aJp+ihjHNoZWxs6ISa5pysICAgLS0tLS0tLS3lronoo4XljIXmrovnlZnvvIzkuIvkuKrniYjmnKzlop7liqDpg6jnvbLlronoo4XljIXliKDpmaQ",
            "id": "7be28fde162b4186a9a07543ca48a28e",
            "app_id": "db246f3f2ecd45f29ecb0f305e821fdc",
            "create_time": "2019-05-10T03:13:27Z"
        }
    ]
}
```

## 状态码<a name="zh-cn_topic_0118921764_section8708918"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0118921764_table10390965"></a>
<table><thead align="left"><tr id="zh-cn_topic_0118921764_row66877087"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0118921764_p48334990"><a name="zh-cn_topic_0118921764_p48334990"></a><a name="zh-cn_topic_0118921764_p48334990"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0118921764_p22820113"><a name="zh-cn_topic_0118921764_p22820113"></a><a name="zh-cn_topic_0118921764_p22820113"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0118921764_row36489873"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921764_p2889717"><a name="zh-cn_topic_0118921764_p2889717"></a><a name="zh-cn_topic_0118921764_p2889717"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921764_p32740518"><a name="zh-cn_topic_0118921764_p32740518"></a><a name="zh-cn_topic_0118921764_p32740518"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row26229206"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921764_p44190948"><a name="zh-cn_topic_0118921764_p44190948"></a><a name="zh-cn_topic_0118921764_p44190948"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921764_p22697075"><a name="zh-cn_topic_0118921764_p22697075"></a><a name="zh-cn_topic_0118921764_p22697075"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row2947091"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921764_p37387781"><a name="zh-cn_topic_0118921764_p37387781"></a><a name="zh-cn_topic_0118921764_p37387781"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921764_p8511436"><a name="zh-cn_topic_0118921764_p8511436"></a><a name="zh-cn_topic_0118921764_p8511436"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0118921764_row9494067"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0118921764_p30821972"><a name="zh-cn_topic_0118921764_p30821972"></a><a name="zh-cn_topic_0118921764_p30821972"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0118921764_p13551805"><a name="zh-cn_topic_0118921764_p13551805"></a><a name="zh-cn_topic_0118921764_p13551805"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

