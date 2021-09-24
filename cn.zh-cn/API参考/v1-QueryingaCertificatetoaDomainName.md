# 查看域名证书<a name="ZH-CN_TOPIC_0000001081976221"></a>

## 功能介绍<a name="zh-cn_topic_0225568974_section38324262122"></a>

查看域名下绑定的证书详情。

## URI<a name="zh-cn_topic_0225568974_section12832162641216"></a>

HTTP/HTTPS请求方法以及URI如下表所示

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568974_table1396111510132"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568974_row096151515139"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568974_p1422722218139"><a name="zh-cn_topic_0225568974_p1422722218139"></a><a name="zh-cn_topic_0225568974_p1422722218139"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568974_p122713225131"><a name="zh-cn_topic_0225568974_p122713225131"></a><a name="zh-cn_topic_0225568974_p122713225131"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568974_row169611815131313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568974_p15227162219132"><a name="zh-cn_topic_0225568974_p15227162219132"></a><a name="zh-cn_topic_0225568974_p15227162219132"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568974_p1667817402181"><a name="zh-cn_topic_0225568974_p1667817402181"></a><a name="zh-cn_topic_0225568974_p1667817402181"></a>/v1/{project_id}/apigw/instances/{instance_id}/api-groups/{group_id}/domains/{domain_id}/certificate/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568974_table4851459153818"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568974_row1985259143813"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568974_p12367713193420"><a name="zh-cn_topic_0225568974_p12367713193420"></a><a name="zh-cn_topic_0225568974_p12367713193420"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.580000000000002%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568974_p7367161316343"><a name="zh-cn_topic_0225568974_p7367161316343"></a><a name="zh-cn_topic_0225568974_p7367161316343"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="20.11%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568974_p93675133347"><a name="zh-cn_topic_0225568974_p93675133347"></a><a name="zh-cn_topic_0225568974_p93675133347"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="37.31%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568974_p836761317349"><a name="zh-cn_topic_0225568974_p836761317349"></a><a name="zh-cn_topic_0225568974_p836761317349"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568974_row1133784305513"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568974_p55878963"><a name="zh-cn_topic_0225568974_p55878963"></a><a name="zh-cn_topic_0225568974_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568974_p29902160"><a name="zh-cn_topic_0225568974_p29902160"></a><a name="zh-cn_topic_0225568974_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568974_p6155914"><a name="zh-cn_topic_0225568974_p6155914"></a><a name="zh-cn_topic_0225568974_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.31%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568974_p28867016"><a name="zh-cn_topic_0225568974_p28867016"></a><a name="zh-cn_topic_0225568974_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row1871244214556"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568974_p1780913159538"><a name="zh-cn_topic_0225568974_p1780913159538"></a><a name="zh-cn_topic_0225568974_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568974_p9809215115310"><a name="zh-cn_topic_0225568974_p9809215115310"></a><a name="zh-cn_topic_0225568974_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568974_p1280914152538"><a name="zh-cn_topic_0225568974_p1280914152538"></a><a name="zh-cn_topic_0225568974_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.31%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568974_p1880914157537"><a name="zh-cn_topic_0225568974_p1880914157537"></a><a name="zh-cn_topic_0225568974_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row13944152316182"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568974_p56248118"><a name="zh-cn_topic_0225568974_p56248118"></a><a name="zh-cn_topic_0225568974_p56248118"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568974_p59803701"><a name="zh-cn_topic_0225568974_p59803701"></a><a name="zh-cn_topic_0225568974_p59803701"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568974_p12261637"><a name="zh-cn_topic_0225568974_p12261637"></a><a name="zh-cn_topic_0225568974_p12261637"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.31%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568974_p53668558"><a name="zh-cn_topic_0225568974_p53668558"></a><a name="zh-cn_topic_0225568974_p53668558"></a>分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row21491627194614"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568974_p147479565365"><a name="zh-cn_topic_0225568974_p147479565365"></a><a name="zh-cn_topic_0225568974_p147479565365"></a>domain_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568974_p153301010123713"><a name="zh-cn_topic_0225568974_p153301010123713"></a><a name="zh-cn_topic_0225568974_p153301010123713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568974_p14330710143716"><a name="zh-cn_topic_0225568974_p14330710143716"></a><a name="zh-cn_topic_0225568974_p14330710143716"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.31%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568974_p9747195653615"><a name="zh-cn_topic_0225568974_p9747195653615"></a><a name="zh-cn_topic_0225568974_p9747195653615"></a>域名的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row18555915383"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568974_p111823311382"><a name="zh-cn_topic_0225568974_p111823311382"></a><a name="zh-cn_topic_0225568974_p111823311382"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="17.580000000000002%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568974_p163410335385"><a name="zh-cn_topic_0225568974_p163410335385"></a><a name="zh-cn_topic_0225568974_p163410335385"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="20.11%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568974_p83443318381"><a name="zh-cn_topic_0225568974_p83443318381"></a><a name="zh-cn_topic_0225568974_p83443318381"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="37.31%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568974_p3341333163817"><a name="zh-cn_topic_0225568974_p3341333163817"></a><a name="zh-cn_topic_0225568974_p3341333163817"></a>证书的编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568974_section14272513203411"></a>

无

## 响应消息<a name="zh-cn_topic_0225568974_section1044114111321"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568974_table34366064"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568974_row59541114"><th class="cellrowborder" valign="top" width="24.93%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568974_p58100907"><a name="zh-cn_topic_0225568974_p58100907"></a><a name="zh-cn_topic_0225568974_p58100907"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="19.23%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568974_p8553058"><a name="zh-cn_topic_0225568974_p8553058"></a><a name="zh-cn_topic_0225568974_p8553058"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.84%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568974_p21709060"><a name="zh-cn_topic_0225568974_p21709060"></a><a name="zh-cn_topic_0225568974_p21709060"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568974_row13603451"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p28137775"><a name="zh-cn_topic_0225568974_p28137775"></a><a name="zh-cn_topic_0225568974_p28137775"></a>common_name</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p64567303"><a name="zh-cn_topic_0225568974_p64567303"></a><a name="zh-cn_topic_0225568974_p64567303"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p62569068"><a name="zh-cn_topic_0225568974_p62569068"></a><a name="zh-cn_topic_0225568974_p62569068"></a>证书域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row26250702"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p45932145"><a name="zh-cn_topic_0225568974_p45932145"></a><a name="zh-cn_topic_0225568974_p45932145"></a>san</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p29516244"><a name="zh-cn_topic_0225568974_p29516244"></a><a name="zh-cn_topic_0225568974_p29516244"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p42005535"><a name="zh-cn_topic_0225568974_p42005535"></a><a name="zh-cn_topic_0225568974_p42005535"></a>SAN域名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row42505499"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p20393431"><a name="zh-cn_topic_0225568974_p20393431"></a><a name="zh-cn_topic_0225568974_p20393431"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p41255182"><a name="zh-cn_topic_0225568974_p41255182"></a><a name="zh-cn_topic_0225568974_p41255182"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p53335466"><a name="zh-cn_topic_0225568974_p53335466"></a><a name="zh-cn_topic_0225568974_p53335466"></a>证书版本</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row1597316278356"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p197412733518"><a name="zh-cn_topic_0225568974_p197412733518"></a><a name="zh-cn_topic_0225568974_p197412733518"></a>organization</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p119741127113511"><a name="zh-cn_topic_0225568974_p119741127113511"></a><a name="zh-cn_topic_0225568974_p119741127113511"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p59743278353"><a name="zh-cn_topic_0225568974_p59743278353"></a><a name="zh-cn_topic_0225568974_p59743278353"></a>公司、组织</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row819414407421"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p10195134013424"><a name="zh-cn_topic_0225568974_p10195134013424"></a><a name="zh-cn_topic_0225568974_p10195134013424"></a>organizational_unit</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p9195540204211"><a name="zh-cn_topic_0225568974_p9195540204211"></a><a name="zh-cn_topic_0225568974_p9195540204211"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p12195340194218"><a name="zh-cn_topic_0225568974_p12195340194218"></a><a name="zh-cn_topic_0225568974_p12195340194218"></a>部门</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row18379348184220"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p173791848154219"><a name="zh-cn_topic_0225568974_p173791848154219"></a><a name="zh-cn_topic_0225568974_p173791848154219"></a>locality</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p103791648174218"><a name="zh-cn_topic_0225568974_p103791648174218"></a><a name="zh-cn_topic_0225568974_p103791648174218"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p203792048114218"><a name="zh-cn_topic_0225568974_p203792048114218"></a><a name="zh-cn_topic_0225568974_p203792048114218"></a>城市</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row19955114434219"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p395614415429"><a name="zh-cn_topic_0225568974_p395614415429"></a><a name="zh-cn_topic_0225568974_p395614415429"></a>state</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p7956544144219"><a name="zh-cn_topic_0225568974_p7956544144219"></a><a name="zh-cn_topic_0225568974_p7956544144219"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p1695664412423"><a name="zh-cn_topic_0225568974_p1695664412423"></a><a name="zh-cn_topic_0225568974_p1695664412423"></a>省份</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row1237917443448"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p83807447442"><a name="zh-cn_topic_0225568974_p83807447442"></a><a name="zh-cn_topic_0225568974_p83807447442"></a>country</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p1338094424411"><a name="zh-cn_topic_0225568974_p1338094424411"></a><a name="zh-cn_topic_0225568974_p1338094424411"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p1438054424413"><a name="zh-cn_topic_0225568974_p1438054424413"></a><a name="zh-cn_topic_0225568974_p1438054424413"></a>国家</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row1531019472447"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p131074774416"><a name="zh-cn_topic_0225568974_p131074774416"></a><a name="zh-cn_topic_0225568974_p131074774416"></a>not_before</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p20996554195919"><a name="zh-cn_topic_0225568974_p20996554195919"></a><a name="zh-cn_topic_0225568974_p20996554195919"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p2310547164412"><a name="zh-cn_topic_0225568974_p2310547164412"></a><a name="zh-cn_topic_0225568974_p2310547164412"></a>证书有效期起始时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row6835102618461"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p17835326104618"><a name="zh-cn_topic_0225568974_p17835326104618"></a><a name="zh-cn_topic_0225568974_p17835326104618"></a>not_after</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p132009357462"><a name="zh-cn_topic_0225568974_p132009357462"></a><a name="zh-cn_topic_0225568974_p132009357462"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p9835132620462"><a name="zh-cn_topic_0225568974_p9835132620462"></a><a name="zh-cn_topic_0225568974_p9835132620462"></a>证书有效期截止时间</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row1275175164617"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p675185154618"><a name="zh-cn_topic_0225568974_p675185154618"></a><a name="zh-cn_topic_0225568974_p675185154618"></a>serial_number</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p3589112564711"><a name="zh-cn_topic_0225568974_p3589112564711"></a><a name="zh-cn_topic_0225568974_p3589112564711"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p5751135114615"><a name="zh-cn_topic_0225568974_p5751135114615"></a><a name="zh-cn_topic_0225568974_p5751135114615"></a>序列号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row12867115410466"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p886885418466"><a name="zh-cn_topic_0225568974_p886885418466"></a><a name="zh-cn_topic_0225568974_p886885418466"></a>issuer</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p1311443014470"><a name="zh-cn_topic_0225568974_p1311443014470"></a><a name="zh-cn_topic_0225568974_p1311443014470"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p4868115418464"><a name="zh-cn_topic_0225568974_p4868115418464"></a><a name="zh-cn_topic_0225568974_p4868115418464"></a>颁发者</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row89501546154614"><td class="cellrowborder" valign="top" width="24.93%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568974_p199501246144610"><a name="zh-cn_topic_0225568974_p199501246144610"></a><a name="zh-cn_topic_0225568974_p199501246144610"></a>signature_algorithm</p>
</td>
<td class="cellrowborder" valign="top" width="19.23%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568974_p17297103219473"><a name="zh-cn_topic_0225568974_p17297103219473"></a><a name="zh-cn_topic_0225568974_p17297103219473"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.84%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568974_p5950114674618"><a name="zh-cn_topic_0225568974_p5950114674618"></a><a name="zh-cn_topic_0225568974_p5950114674618"></a>签名算法</p>
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

## 状态码<a name="zh-cn_topic_0225568974_section2083573084114"></a>

**表 4**  返回消息说明

<a name="zh-cn_topic_0225568974_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568974_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568974_p174881730194216"><a name="zh-cn_topic_0225568974_p174881730194216"></a><a name="zh-cn_topic_0225568974_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568974_p848863018429"><a name="zh-cn_topic_0225568974_p848863018429"></a><a name="zh-cn_topic_0225568974_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568974_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568974_p7488163084211"><a name="zh-cn_topic_0225568974_p7488163084211"></a><a name="zh-cn_topic_0225568974_p7488163084211"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568974_p1397710479489"><a name="zh-cn_topic_0225568974_p1397710479489"></a><a name="zh-cn_topic_0225568974_p1397710479489"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568974_p14488113015426"><a name="zh-cn_topic_0225568974_p14488113015426"></a><a name="zh-cn_topic_0225568974_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568974_p1497764720485"><a name="zh-cn_topic_0225568974_p1497764720485"></a><a name="zh-cn_topic_0225568974_p1497764720485"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568974_p24883304428"><a name="zh-cn_topic_0225568974_p24883304428"></a><a name="zh-cn_topic_0225568974_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568974_p1848810308429"><a name="zh-cn_topic_0225568974_p1848810308429"></a><a name="zh-cn_topic_0225568974_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568974_p6488133064210"><a name="zh-cn_topic_0225568974_p6488133064210"></a><a name="zh-cn_topic_0225568974_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568974_p10488193018426"><a name="zh-cn_topic_0225568974_p10488193018426"></a><a name="zh-cn_topic_0225568974_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568974_p144883304428"><a name="zh-cn_topic_0225568974_p144883304428"></a><a name="zh-cn_topic_0225568974_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568974_p4488103094212"><a name="zh-cn_topic_0225568974_p4488103094212"></a><a name="zh-cn_topic_0225568974_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568974_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568974_p17488163014423"><a name="zh-cn_topic_0225568974_p17488163014423"></a><a name="zh-cn_topic_0225568974_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568974_p048813014216"><a name="zh-cn_topic_0225568974_p048813014216"></a><a name="zh-cn_topic_0225568974_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

