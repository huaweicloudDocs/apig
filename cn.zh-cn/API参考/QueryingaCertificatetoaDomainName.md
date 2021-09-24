# 查看域名证书<a name="ZH-CN_TOPIC_0000001082221227"></a>

## 功能介绍<a name="zh-cn_topic_0225502946_section38324262122"></a>

查看域名下绑定的证书详情。

## URI<a name="zh-cn_topic_0225502946_section12832162641216"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225502946_table1396111510132"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225502946_row096151515139"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225502946_p1422722218139"><a name="zh-cn_topic_0225502946_p1422722218139"></a><a name="zh-cn_topic_0225502946_p1422722218139"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225502946_p122713225131"><a name="zh-cn_topic_0225502946_p122713225131"></a><a name="zh-cn_topic_0225502946_p122713225131"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225502946_row169611815131313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225502946_p15227162219132"><a name="zh-cn_topic_0225502946_p15227162219132"></a><a name="zh-cn_topic_0225502946_p15227162219132"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225502946_p1667817402181"><a name="zh-cn_topic_0225502946_p1667817402181"></a><a name="zh-cn_topic_0225502946_p1667817402181"></a>/v1.0/apigw/api-groups/{group_id}/domains/{domain_id}/certificate/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225502946_table4851459153818"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225502946_row1985259143813"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225502946_p12367713193420"><a name="zh-cn_topic_0225502946_p12367713193420"></a><a name="zh-cn_topic_0225502946_p12367713193420"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225502946_p7367161316343"><a name="zh-cn_topic_0225502946_p7367161316343"></a><a name="zh-cn_topic_0225502946_p7367161316343"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="24%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225502946_p93675133347"><a name="zh-cn_topic_0225502946_p93675133347"></a><a name="zh-cn_topic_0225502946_p93675133347"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="26%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225502946_p836761317349"><a name="zh-cn_topic_0225502946_p836761317349"></a><a name="zh-cn_topic_0225502946_p836761317349"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225502946_row13944152316182"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225502946_p56248118"><a name="zh-cn_topic_0225502946_p56248118"></a><a name="zh-cn_topic_0225502946_p56248118"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225502946_p59803701"><a name="zh-cn_topic_0225502946_p59803701"></a><a name="zh-cn_topic_0225502946_p59803701"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225502946_p12261637"><a name="zh-cn_topic_0225502946_p12261637"></a><a name="zh-cn_topic_0225502946_p12261637"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225502946_p53668558"><a name="zh-cn_topic_0225502946_p53668558"></a><a name="zh-cn_topic_0225502946_p53668558"></a>分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row21491627194614"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225502946_p147479565365"><a name="zh-cn_topic_0225502946_p147479565365"></a><a name="zh-cn_topic_0225502946_p147479565365"></a>domain_id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225502946_p153301010123713"><a name="zh-cn_topic_0225502946_p153301010123713"></a><a name="zh-cn_topic_0225502946_p153301010123713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225502946_p14330710143716"><a name="zh-cn_topic_0225502946_p14330710143716"></a><a name="zh-cn_topic_0225502946_p14330710143716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225502946_p9747195653615"><a name="zh-cn_topic_0225502946_p9747195653615"></a><a name="zh-cn_topic_0225502946_p9747195653615"></a>域名的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row18555915383"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225502946_p111823311382"><a name="zh-cn_topic_0225502946_p111823311382"></a><a name="zh-cn_topic_0225502946_p111823311382"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225502946_p163410335385"><a name="zh-cn_topic_0225502946_p163410335385"></a><a name="zh-cn_topic_0225502946_p163410335385"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="24%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225502946_p83443318381"><a name="zh-cn_topic_0225502946_p83443318381"></a><a name="zh-cn_topic_0225502946_p83443318381"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="26%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225502946_p3341333163817"><a name="zh-cn_topic_0225502946_p3341333163817"></a><a name="zh-cn_topic_0225502946_p3341333163817"></a>证书的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225502946_section14272513203411"></a>

无

## 响应消息<a name="zh-cn_topic_0225502946_section1044114111321"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225502946_table34366064"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225502946_row59541114"><th class="cellrowborder" valign="top" width="24.93%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225502946_p58100907"><a name="zh-cn_topic_0225502946_p58100907"></a><a name="zh-cn_topic_0225502946_p58100907"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.23%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225502946_p8553058"><a name="zh-cn_topic_0225502946_p8553058"></a><a name="zh-cn_topic_0225502946_p8553058"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.84%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225502946_p21709060"><a name="zh-cn_topic_0225502946_p21709060"></a><a name="zh-cn_topic_0225502946_p21709060"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225502946_row13603451"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p28137775"><a name="zh-cn_topic_0225502946_p28137775"></a><a name="zh-cn_topic_0225502946_p28137775"></a>common_name</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p64567303"><a name="zh-cn_topic_0225502946_p64567303"></a><a name="zh-cn_topic_0225502946_p64567303"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p62569068"><a name="zh-cn_topic_0225502946_p62569068"></a><a name="zh-cn_topic_0225502946_p62569068"></a>证书域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row26250702"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p45932145"><a name="zh-cn_topic_0225502946_p45932145"></a><a name="zh-cn_topic_0225502946_p45932145"></a>san</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p29516244"><a name="zh-cn_topic_0225502946_p29516244"></a><a name="zh-cn_topic_0225502946_p29516244"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p42005535"><a name="zh-cn_topic_0225502946_p42005535"></a><a name="zh-cn_topic_0225502946_p42005535"></a>SAN域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row42505499"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p20393431"><a name="zh-cn_topic_0225502946_p20393431"></a><a name="zh-cn_topic_0225502946_p20393431"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p41255182"><a name="zh-cn_topic_0225502946_p41255182"></a><a name="zh-cn_topic_0225502946_p41255182"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p53335466"><a name="zh-cn_topic_0225502946_p53335466"></a><a name="zh-cn_topic_0225502946_p53335466"></a>证书版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row1597316278356"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p197412733518"><a name="zh-cn_topic_0225502946_p197412733518"></a><a name="zh-cn_topic_0225502946_p197412733518"></a>organization</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p119741127113511"><a name="zh-cn_topic_0225502946_p119741127113511"></a><a name="zh-cn_topic_0225502946_p119741127113511"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p59743278353"><a name="zh-cn_topic_0225502946_p59743278353"></a><a name="zh-cn_topic_0225502946_p59743278353"></a>公司、组织</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row819414407421"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p10195134013424"><a name="zh-cn_topic_0225502946_p10195134013424"></a><a name="zh-cn_topic_0225502946_p10195134013424"></a>organizational_unit</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p9195540204211"><a name="zh-cn_topic_0225502946_p9195540204211"></a><a name="zh-cn_topic_0225502946_p9195540204211"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p12195340194218"><a name="zh-cn_topic_0225502946_p12195340194218"></a><a name="zh-cn_topic_0225502946_p12195340194218"></a>部门</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row18379348184220"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p173791848154219"><a name="zh-cn_topic_0225502946_p173791848154219"></a><a name="zh-cn_topic_0225502946_p173791848154219"></a>locality</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p103791648174218"><a name="zh-cn_topic_0225502946_p103791648174218"></a><a name="zh-cn_topic_0225502946_p103791648174218"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p203792048114218"><a name="zh-cn_topic_0225502946_p203792048114218"></a><a name="zh-cn_topic_0225502946_p203792048114218"></a>城市</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row19955114434219"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p395614415429"><a name="zh-cn_topic_0225502946_p395614415429"></a><a name="zh-cn_topic_0225502946_p395614415429"></a>state</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p7956544144219"><a name="zh-cn_topic_0225502946_p7956544144219"></a><a name="zh-cn_topic_0225502946_p7956544144219"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p1695664412423"><a name="zh-cn_topic_0225502946_p1695664412423"></a><a name="zh-cn_topic_0225502946_p1695664412423"></a>省份</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row1237917443448"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p83807447442"><a name="zh-cn_topic_0225502946_p83807447442"></a><a name="zh-cn_topic_0225502946_p83807447442"></a>country</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p1338094424411"><a name="zh-cn_topic_0225502946_p1338094424411"></a><a name="zh-cn_topic_0225502946_p1338094424411"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p1438054424413"><a name="zh-cn_topic_0225502946_p1438054424413"></a><a name="zh-cn_topic_0225502946_p1438054424413"></a>国家</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row1531019472447"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p131074774416"><a name="zh-cn_topic_0225502946_p131074774416"></a><a name="zh-cn_topic_0225502946_p131074774416"></a>not_before</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p20996554195919"><a name="zh-cn_topic_0225502946_p20996554195919"></a><a name="zh-cn_topic_0225502946_p20996554195919"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p2310547164412"><a name="zh-cn_topic_0225502946_p2310547164412"></a><a name="zh-cn_topic_0225502946_p2310547164412"></a>证书有效期起始时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row6835102618461"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p17835326104618"><a name="zh-cn_topic_0225502946_p17835326104618"></a><a name="zh-cn_topic_0225502946_p17835326104618"></a>not_after</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p132009357462"><a name="zh-cn_topic_0225502946_p132009357462"></a><a name="zh-cn_topic_0225502946_p132009357462"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p9835132620462"><a name="zh-cn_topic_0225502946_p9835132620462"></a><a name="zh-cn_topic_0225502946_p9835132620462"></a>证书有效期截止时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row1275175164617"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p675185154618"><a name="zh-cn_topic_0225502946_p675185154618"></a><a name="zh-cn_topic_0225502946_p675185154618"></a>serial_number</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p3589112564711"><a name="zh-cn_topic_0225502946_p3589112564711"></a><a name="zh-cn_topic_0225502946_p3589112564711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p5751135114615"><a name="zh-cn_topic_0225502946_p5751135114615"></a><a name="zh-cn_topic_0225502946_p5751135114615"></a>序列号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row12867115410466"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p886885418466"><a name="zh-cn_topic_0225502946_p886885418466"></a><a name="zh-cn_topic_0225502946_p886885418466"></a>issuer</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p1311443014470"><a name="zh-cn_topic_0225502946_p1311443014470"></a><a name="zh-cn_topic_0225502946_p1311443014470"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p4868115418464"><a name="zh-cn_topic_0225502946_p4868115418464"></a><a name="zh-cn_topic_0225502946_p4868115418464"></a>颁发者</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row89501546154614"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225502946_p199501246144610"><a name="zh-cn_topic_0225502946_p199501246144610"></a><a name="zh-cn_topic_0225502946_p199501246144610"></a>signature_algorithm</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225502946_p17297103219473"><a name="zh-cn_topic_0225502946_p17297103219473"></a><a name="zh-cn_topic_0225502946_p17297103219473"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225502946_p5950114674618"><a name="zh-cn_topic_0225502946_p5950114674618"></a><a name="zh-cn_topic_0225502946_p5950114674618"></a>签名算法</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
    "san": [
        "xxx.xxx.xxx"
    ],
    "country": [
        "CN"
    ],
    "not_before": "2019-04-29T11:49:18Z",
    "locality": [
        "ShenZhen"
    ],
    "serial_number": "00000000000000000000000000",
    "version": 3,
    "issuer": [
        "XXX"
    ],
    "not_after": "2029-04-29T11:49:18Z",
    "organization": [
        "XXX"
    ],
    "signature_algorithm": "SHA256-RSA",
    "state": [
        "XXX"
    ],
    "common_name": "xxx.xxx.xxx",
    "organizational_unit": [
        "XXX"
    ]
}
```

## 状态码<a name="zh-cn_topic_0225502946_section2083573084114"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0225502946_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225502946_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225502946_p174881730194216"><a name="zh-cn_topic_0225502946_p174881730194216"></a><a name="zh-cn_topic_0225502946_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225502946_p848863018429"><a name="zh-cn_topic_0225502946_p848863018429"></a><a name="zh-cn_topic_0225502946_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225502946_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225502946_p7488163084211"><a name="zh-cn_topic_0225502946_p7488163084211"></a><a name="zh-cn_topic_0225502946_p7488163084211"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225502946_p1397710479489"><a name="zh-cn_topic_0225502946_p1397710479489"></a><a name="zh-cn_topic_0225502946_p1397710479489"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225502946_p14488113015426"><a name="zh-cn_topic_0225502946_p14488113015426"></a><a name="zh-cn_topic_0225502946_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225502946_p1497764720485"><a name="zh-cn_topic_0225502946_p1497764720485"></a><a name="zh-cn_topic_0225502946_p1497764720485"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225502946_p24883304428"><a name="zh-cn_topic_0225502946_p24883304428"></a><a name="zh-cn_topic_0225502946_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225502946_p1848810308429"><a name="zh-cn_topic_0225502946_p1848810308429"></a><a name="zh-cn_topic_0225502946_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225502946_p6488133064210"><a name="zh-cn_topic_0225502946_p6488133064210"></a><a name="zh-cn_topic_0225502946_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225502946_p10488193018426"><a name="zh-cn_topic_0225502946_p10488193018426"></a><a name="zh-cn_topic_0225502946_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225502946_p144883304428"><a name="zh-cn_topic_0225502946_p144883304428"></a><a name="zh-cn_topic_0225502946_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225502946_p4488103094212"><a name="zh-cn_topic_0225502946_p4488103094212"></a><a name="zh-cn_topic_0225502946_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225502946_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225502946_p17488163014423"><a name="zh-cn_topic_0225502946_p17488163014423"></a><a name="zh-cn_topic_0225502946_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225502946_p048813014216"><a name="zh-cn_topic_0225502946_p048813014216"></a><a name="zh-cn_topic_0225502946_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

