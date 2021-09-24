# 创建VPC通道<a name="ZH-CN_TOPIC_0000001081837391"></a>

## 功能介绍<a name="zh-cn_topic_0225568977_section173482301428"></a>

在API网关中创建连接私有VPC资源的通道，并在创建API时将后端节点配置为使用这些VPC通道，以便API网关直接访问私有VPC资源。

>![](public_sys-resources/icon-note.gif) **说明：** 
>每个用户最多创建30个VPC通道。

## URI<a name="zh-cn_topic_0225568977_section1336323014423"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568977_table1439319294431"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568977_row1393229154314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568977_p14361448204314"><a name="zh-cn_topic_0225568977_p14361448204314"></a><a name="zh-cn_topic_0225568977_p14361448204314"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568977_p1936174864316"><a name="zh-cn_topic_0225568977_p1936174864316"></a><a name="zh-cn_topic_0225568977_p1936174864316"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568977_row8393122914436"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568977_p1236111482435"><a name="zh-cn_topic_0225568977_p1236111482435"></a><a name="zh-cn_topic_0225568977_p1236111482435"></a>POST</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568977_p11361848184318"><a name="zh-cn_topic_0225568977_p11361848184318"></a><a name="zh-cn_topic_0225568977_p11361848184318"></a>/v1/{project_id}/apigw/instances/{instance_id}/vpc-channels</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568977_table38510415"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568977_row62423067"><th class="cellrowborder" valign="top" width="23.46765323467653%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568977_p23103637"><a name="zh-cn_topic_0225568977_p23103637"></a><a name="zh-cn_topic_0225568977_p23103637"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568977_p59455291"><a name="zh-cn_topic_0225568977_p59455291"></a><a name="zh-cn_topic_0225568977_p59455291"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568977_p51149303"><a name="zh-cn_topic_0225568977_p51149303"></a><a name="zh-cn_topic_0225568977_p51149303"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="41.835816418358164%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568977_p49452846"><a name="zh-cn_topic_0225568977_p49452846"></a><a name="zh-cn_topic_0225568977_p49452846"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568977_row46257610"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p55878963"><a name="zh-cn_topic_0225568977_p55878963"></a><a name="zh-cn_topic_0225568977_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p29902160"><a name="zh-cn_topic_0225568977_p29902160"></a><a name="zh-cn_topic_0225568977_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p6155914"><a name="zh-cn_topic_0225568977_p6155914"></a><a name="zh-cn_topic_0225568977_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p28867016"><a name="zh-cn_topic_0225568977_p28867016"></a><a name="zh-cn_topic_0225568977_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row7809161535314"><td class="cellrowborder" valign="top" width="23.46765323467653%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p1780913159538"><a name="zh-cn_topic_0225568977_p1780913159538"></a><a name="zh-cn_topic_0225568977_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p9809215115310"><a name="zh-cn_topic_0225568977_p9809215115310"></a><a name="zh-cn_topic_0225568977_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p1280914152538"><a name="zh-cn_topic_0225568977_p1280914152538"></a><a name="zh-cn_topic_0225568977_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="41.835816418358164%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p1880914157537"><a name="zh-cn_topic_0225568977_p1880914157537"></a><a name="zh-cn_topic_0225568977_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568977_section73637302425"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568977_table1136319301429"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568977_row748813306425"><th class="cellrowborder" valign="top" width="15.46154615461546%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568977_p9488143084210"><a name="zh-cn_topic_0225568977_p9488143084210"></a><a name="zh-cn_topic_0225568977_p9488143084210"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568977_p148843017426"><a name="zh-cn_topic_0225568977_p148843017426"></a><a name="zh-cn_topic_0225568977_p148843017426"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568977_p9488830164214"><a name="zh-cn_topic_0225568977_p9488830164214"></a><a name="zh-cn_topic_0225568977_p9488830164214"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568977_p1048813014421"><a name="zh-cn_topic_0225568977_p1048813014421"></a><a name="zh-cn_topic_0225568977_p1048813014421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568977_row2012102914318"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p9051148"><a name="zh-cn_topic_0225568977_p9051148"></a><a name="zh-cn_topic_0225568977_p9051148"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p62054412"><a name="zh-cn_topic_0225568977_p62054412"></a><a name="zh-cn_topic_0225568977_p62054412"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p12740424339"><a name="zh-cn_topic_0225568977_p12740424339"></a><a name="zh-cn_topic_0225568977_p12740424339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p13931103183318"><a name="zh-cn_topic_0225568977_p13931103183318"></a><a name="zh-cn_topic_0225568977_p13931103183318"></a>VPC通道的名称。</p>
<p id="zh-cn_topic_0225568977_p37858559"><a name="zh-cn_topic_0225568977_p37858559"></a><a name="zh-cn_topic_0225568977_p37858559"></a>长度为3 ~ 64位的字符串，字符串由中文、英文字母、数字、“-”、“_”组成，且只能以英文或中文开头。</p>
<div class="note" id="zh-cn_topic_0225568977_note690163615371"><a name="zh-cn_topic_0225568977_note690163615371"></a><a name="zh-cn_topic_0225568977_note690163615371"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568977_p09053643719"><a name="zh-cn_topic_0225568977_p09053643719"></a><a name="zh-cn_topic_0225568977_p09053643719"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row81211629183115"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p4509019"><a name="zh-cn_topic_0225568977_p4509019"></a><a name="zh-cn_topic_0225568977_p4509019"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p29686297"><a name="zh-cn_topic_0225568977_p29686297"></a><a name="zh-cn_topic_0225568977_p29686297"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p82741042143312"><a name="zh-cn_topic_0225568977_p82741042143312"></a><a name="zh-cn_topic_0225568977_p82741042143312"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p139319318333"><a name="zh-cn_topic_0225568977_p139319318333"></a><a name="zh-cn_topic_0225568977_p139319318333"></a>VPC通道的类型。</p>
<a name="zh-cn_topic_0225568977_ul4250115615505"></a><a name="zh-cn_topic_0225568977_ul4250115615505"></a><ul id="zh-cn_topic_0225568977_ul4250115615505"><li>2：API网关内置支持负载均衡功能的快速通道类型</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row13314191535217"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p19314131517528"><a name="zh-cn_topic_0225568977_p19314131517528"></a><a name="zh-cn_topic_0225568977_p19314131517528"></a>member_type</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p123141715125216"><a name="zh-cn_topic_0225568977_p123141715125216"></a><a name="zh-cn_topic_0225568977_p123141715125216"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p17315151575211"><a name="zh-cn_topic_0225568977_p17315151575211"></a><a name="zh-cn_topic_0225568977_p17315151575211"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p1137783455312"><a name="zh-cn_topic_0225568977_p1137783455312"></a><a name="zh-cn_topic_0225568977_p1137783455312"></a>VPC通道的成员类型。</p>
<a name="zh-cn_topic_0225568977_ul123771834145313"></a><a name="zh-cn_topic_0225568977_ul123771834145313"></a><ul id="zh-cn_topic_0225568977_ul123771834145313"><li>ip（暂不支持）</li><li>instance</li></ul>
<p id="zh-cn_topic_0225568977_p5561134685210"><a name="zh-cn_topic_0225568977_p5561134685210"></a><a name="zh-cn_topic_0225568977_p5561134685210"></a>仅VPC通道类型为2时有效，缺省为instance。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row1612192923111"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p49099023"><a name="zh-cn_topic_0225568977_p49099023"></a><a name="zh-cn_topic_0225568977_p49099023"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p17597936"><a name="zh-cn_topic_0225568977_p17597936"></a><a name="zh-cn_topic_0225568977_p17597936"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p929014217338"><a name="zh-cn_topic_0225568977_p929014217338"></a><a name="zh-cn_topic_0225568977_p929014217338"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p49461931193318"><a name="zh-cn_topic_0225568977_p49461931193318"></a><a name="zh-cn_topic_0225568977_p49461931193318"></a>VPC通道中主机的端口号。</p>
<p id="zh-cn_topic_0225568977_p97191632173515"><a name="zh-cn_topic_0225568977_p97191632173515"></a><a name="zh-cn_topic_0225568977_p97191632173515"></a>取值范围1 ~ 65535，仅VPC通道类型为2时有效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row17121132912318"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p192983401416"><a name="zh-cn_topic_0225568977_p192983401416"></a><a name="zh-cn_topic_0225568977_p192983401416"></a>balance_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p182985416144"><a name="zh-cn_topic_0225568977_p182985416144"></a><a name="zh-cn_topic_0225568977_p182985416144"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p6290114214331"><a name="zh-cn_topic_0225568977_p6290114214331"></a><a name="zh-cn_topic_0225568977_p6290114214331"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p13616155945512"><a name="zh-cn_topic_0225568977_p13616155945512"></a><a name="zh-cn_topic_0225568977_p13616155945512"></a>分发算法。</p>
<a name="zh-cn_topic_0225568977_ul46161059145520"></a><a name="zh-cn_topic_0225568977_ul46161059145520"></a><ul id="zh-cn_topic_0225568977_ul46161059145520"><li>1：加权轮询（wrr）</li><li>2：加权最少连接（wleastconn）</li><li>3：源地址哈希（source）</li><li>4：URI哈希（uri）</li></ul>
<p id="zh-cn_topic_0225568977_p5946153116333"><a name="zh-cn_topic_0225568977_p5946153116333"></a><a name="zh-cn_topic_0225568977_p5946153116333"></a>仅VPC通道类型为2时有效，缺省为1。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row91212298312"><td class="cellrowborder" valign="top" width="15.46154615461546%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p8845107161418"><a name="zh-cn_topic_0225568977_p8845107161418"></a><a name="zh-cn_topic_0225568977_p8845107161418"></a>vpc_health_config</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p188451179141"><a name="zh-cn_topic_0225568977_p188451179141"></a><a name="zh-cn_topic_0225568977_p188451179141"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p122908425332"><a name="zh-cn_topic_0225568977_p122908425332"></a><a name="zh-cn_topic_0225568977_p122908425332"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p8946531183318"><a name="zh-cn_topic_0225568977_p8946531183318"></a><a name="zh-cn_topic_0225568977_p8946531183318"></a>健康检查详情，仅VPC通道类型为2时有效。</p>
</td>
</tr>
</tbody>
</table>

**表 4**  健康检查详情

<a name="zh-cn_topic_0225568977_table56131171473"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568977_row1561341712474"><th class="cellrowborder" valign="top" width="15.151515151515152%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568977_p11613171794715"><a name="zh-cn_topic_0225568977_p11613171794715"></a><a name="zh-cn_topic_0225568977_p11613171794715"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.131313131313133%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568977_p1461341719471"><a name="zh-cn_topic_0225568977_p1461341719471"></a><a name="zh-cn_topic_0225568977_p1461341719471"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.131313131313133%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568977_p1361310173475"><a name="zh-cn_topic_0225568977_p1361310173475"></a><a name="zh-cn_topic_0225568977_p1361310173475"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.58585858585859%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568977_p1962861718474"><a name="zh-cn_topic_0225568977_p1962861718474"></a><a name="zh-cn_topic_0225568977_p1962861718474"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568977_row46281317124714"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p1562871714717"><a name="zh-cn_topic_0225568977_p1562871714717"></a><a name="zh-cn_topic_0225568977_p1562871714717"></a>protocol</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p146282176479"><a name="zh-cn_topic_0225568977_p146282176479"></a><a name="zh-cn_topic_0225568977_p146282176479"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p1862819174475"><a name="zh-cn_topic_0225568977_p1862819174475"></a><a name="zh-cn_topic_0225568977_p1862819174475"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><div class="p" id="zh-cn_topic_0225568977_p1935373174812"><a name="zh-cn_topic_0225568977_p1935373174812"></a><a name="zh-cn_topic_0225568977_p1935373174812"></a>使用以下协议，对VPC中主机执行健康检查。<a name="zh-cn_topic_0225568977_ul19904951155719"></a><a name="zh-cn_topic_0225568977_ul19904951155719"></a><ul id="zh-cn_topic_0225568977_ul19904951155719"><li>TCP</li><li>HTTP</li><li>HTTPS</li></ul>
</div>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row7628217124717"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p0628171711477"><a name="zh-cn_topic_0225568977_p0628171711477"></a><a name="zh-cn_topic_0225568977_p0628171711477"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p1782432775013"><a name="zh-cn_topic_0225568977_p1782432775013"></a><a name="zh-cn_topic_0225568977_p1782432775013"></a>protocol = http时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p10644017184710"><a name="zh-cn_topic_0225568977_p10644017184710"></a><a name="zh-cn_topic_0225568977_p10644017184710"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p15591010195011"><a name="zh-cn_topic_0225568977_p15591010195011"></a><a name="zh-cn_topic_0225568977_p15591010195011"></a>健康检查时的目标路径。</p>
<div class="note" id="zh-cn_topic_0225568977_note38431529153919"><a name="zh-cn_topic_0225568977_note38431529153919"></a><a name="zh-cn_topic_0225568977_note38431529153919"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568977_p18843122918398"><a name="zh-cn_topic_0225568977_p18843122918398"></a><a name="zh-cn_topic_0225568977_p18843122918398"></a>需要服从URI规范。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row10644151704717"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p46440172472"><a name="zh-cn_topic_0225568977_p46440172472"></a><a name="zh-cn_topic_0225568977_p46440172472"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p14644181754720"><a name="zh-cn_topic_0225568977_p14644181754720"></a><a name="zh-cn_topic_0225568977_p14644181754720"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p19644617104710"><a name="zh-cn_topic_0225568977_p19644617104710"></a><a name="zh-cn_topic_0225568977_p19644617104710"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p78214132565"><a name="zh-cn_topic_0225568977_p78214132565"></a><a name="zh-cn_topic_0225568977_p78214132565"></a>健康检查的目标端口，缺省时为VPC中主机的端口号。</p>
<p id="zh-cn_topic_0225568977_p2782317155411"><a name="zh-cn_topic_0225568977_p2782317155411"></a><a name="zh-cn_topic_0225568977_p2782317155411"></a>取值范围1 ~ 65535。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row56601917164716"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p76604177474"><a name="zh-cn_topic_0225568977_p76604177474"></a><a name="zh-cn_topic_0225568977_p76604177474"></a>threshold_normal</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p4660117134717"><a name="zh-cn_topic_0225568977_p4660117134717"></a><a name="zh-cn_topic_0225568977_p4660117134717"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p196608172477"><a name="zh-cn_topic_0225568977_p196608172477"></a><a name="zh-cn_topic_0225568977_p196608172477"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p1315411125313"><a name="zh-cn_topic_0225568977_p1315411125313"></a><a name="zh-cn_topic_0225568977_p1315411125313"></a>正常阈值。</p>
<p id="zh-cn_topic_0225568977_p1798813185617"><a name="zh-cn_topic_0225568977_p1798813185617"></a><a name="zh-cn_topic_0225568977_p1798813185617"></a>判定VPC通道中主机正常的依据为：连续检查<em id="zh-cn_topic_0225568977_i421224922811"><a name="zh-cn_topic_0225568977_i421224922811"></a><a name="zh-cn_topic_0225568977_i421224922811"></a>x</em>成功，x为您设置的正常阈值。</p>
<p id="zh-cn_topic_0225568977_p35225297513"><a name="zh-cn_topic_0225568977_p35225297513"></a><a name="zh-cn_topic_0225568977_p35225297513"></a>取值范围2 ~ 10</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row1266061794714"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p196601017124713"><a name="zh-cn_topic_0225568977_p196601017124713"></a><a name="zh-cn_topic_0225568977_p196601017124713"></a>threshold_abnormal</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p206601417154713"><a name="zh-cn_topic_0225568977_p206601417154713"></a><a name="zh-cn_topic_0225568977_p206601417154713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p56601117104714"><a name="zh-cn_topic_0225568977_p56601117104714"></a><a name="zh-cn_topic_0225568977_p56601117104714"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p1898161316565"><a name="zh-cn_topic_0225568977_p1898161316565"></a><a name="zh-cn_topic_0225568977_p1898161316565"></a>异常阙值。</p>
<p id="zh-cn_topic_0225568977_p79167352531"><a name="zh-cn_topic_0225568977_p79167352531"></a><a name="zh-cn_topic_0225568977_p79167352531"></a>判定VPC通道中主机异常的依据为：连续检查<em id="zh-cn_topic_0225568977_i37296135294"><a name="zh-cn_topic_0225568977_i37296135294"></a><a name="zh-cn_topic_0225568977_i37296135294"></a>x失败</em>，x为您设置的异常阈值。</p>
<p id="zh-cn_topic_0225568977_p1865194916514"><a name="zh-cn_topic_0225568977_p1865194916514"></a><a name="zh-cn_topic_0225568977_p1865194916514"></a>取值范围2 ~ 10。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row7675121714474"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p66751817104717"><a name="zh-cn_topic_0225568977_p66751817104717"></a><a name="zh-cn_topic_0225568977_p66751817104717"></a>time_out</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p367521764713"><a name="zh-cn_topic_0225568977_p367521764713"></a><a name="zh-cn_topic_0225568977_p367521764713"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p36751017184719"><a name="zh-cn_topic_0225568977_p36751017184719"></a><a name="zh-cn_topic_0225568977_p36751017184719"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p1511311311562"><a name="zh-cn_topic_0225568977_p1511311311562"></a><a name="zh-cn_topic_0225568977_p1511311311562"></a>超时时间：检查期间，无响应的时间，单位为秒。必须小于time_interval字段取值。</p>
<p id="zh-cn_topic_0225568977_p6100155285117"><a name="zh-cn_topic_0225568977_p6100155285117"></a><a name="zh-cn_topic_0225568977_p6100155285117"></a>取值范围2 ~ 30。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row146754172472"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p2675171734717"><a name="zh-cn_topic_0225568977_p2675171734717"></a><a name="zh-cn_topic_0225568977_p2675171734717"></a>time_interval</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p18675111734711"><a name="zh-cn_topic_0225568977_p18675111734711"></a><a name="zh-cn_topic_0225568977_p18675111734711"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p26751317174716"><a name="zh-cn_topic_0225568977_p26751317174716"></a><a name="zh-cn_topic_0225568977_p26751317174716"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p958312467512"><a name="zh-cn_topic_0225568977_p958312467512"></a><a name="zh-cn_topic_0225568977_p958312467512"></a>间隔时间：连续两次检查的间隔时间，单位为秒。必须大于time_out字段取值。</p>
<p id="zh-cn_topic_0225568977_p106781254125110"><a name="zh-cn_topic_0225568977_p106781254125110"></a><a name="zh-cn_topic_0225568977_p106781254125110"></a>取值范围5 ~ 300。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row927095444819"><td class="cellrowborder" valign="top" width="15.151515151515152%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p1027035412488"><a name="zh-cn_topic_0225568977_p1027035412488"></a><a name="zh-cn_topic_0225568977_p1027035412488"></a>http_code</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p7270195418482"><a name="zh-cn_topic_0225568977_p7270195418482"></a><a name="zh-cn_topic_0225568977_p7270195418482"></a>protocol = http时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.131313131313133%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p9270135474815"><a name="zh-cn_topic_0225568977_p9270135474815"></a><a name="zh-cn_topic_0225568977_p9270135474815"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.58585858585859%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p15281310185519"><a name="zh-cn_topic_0225568977_p15281310185519"></a><a name="zh-cn_topic_0225568977_p15281310185519"></a>检查目标HTTP响应时，判断成功使用的HTTP响应码。</p>
<p id="zh-cn_topic_0225568977_p1144417511111"><a name="zh-cn_topic_0225568977_p1144417511111"></a><a name="zh-cn_topic_0225568977_p1144417511111"></a>取值范围为100到599之前的任意整数值，支持如下三种格式：</p>
<a name="zh-cn_topic_0225568977_ul343965120114"></a><a name="zh-cn_topic_0225568977_ul343965120114"></a><ul id="zh-cn_topic_0225568977_ul343965120114"><li>多个值，如：200,201,202</li><li>一系列值，如：200-299</li><li>组合值，如：201,202,210-299</li></ul>
</td>
</tr>
</tbody>
</table>

**表 5**  后端实例列表

<a name="zh-cn_topic_0225568977_table6144132024717"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568977_row15144122054719"><th class="cellrowborder" valign="top" width="15.52155215521552%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568977_p41441620124712"><a name="zh-cn_topic_0225568977_p41441620124712"></a><a name="zh-cn_topic_0225568977_p41441620124712"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="13.34133413341334%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568977_p14144820104719"><a name="zh-cn_topic_0225568977_p14144820104719"></a><a name="zh-cn_topic_0225568977_p14144820104719"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13.4013401340134%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568977_p71601720114710"><a name="zh-cn_topic_0225568977_p71601720114710"></a><a name="zh-cn_topic_0225568977_p71601720114710"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="57.73577357735774%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568977_p1716072074719"><a name="zh-cn_topic_0225568977_p1716072074719"></a><a name="zh-cn_topic_0225568977_p1716072074719"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568977_row816019209472"><td class="cellrowborder" valign="top" width="15.52155215521552%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p11160192010473"><a name="zh-cn_topic_0225568977_p11160192010473"></a><a name="zh-cn_topic_0225568977_p11160192010473"></a>instance_name</p>
</td>
<td class="cellrowborder" valign="top" width="13.34133413341334%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p916052018474"><a name="zh-cn_topic_0225568977_p916052018474"></a><a name="zh-cn_topic_0225568977_p916052018474"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p1916032024714"><a name="zh-cn_topic_0225568977_p1916032024714"></a><a name="zh-cn_topic_0225568977_p1916032024714"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p64172706"><a name="zh-cn_topic_0225568977_p64172706"></a><a name="zh-cn_topic_0225568977_p64172706"></a>后端实例的名称。</p>
<p id="zh-cn_topic_0225568977_p7024991"><a name="zh-cn_topic_0225568977_p7024991"></a><a name="zh-cn_topic_0225568977_p7024991"></a>支持汉字，英文，数字，“-”,“_”,“.”，1 ~ 64字符。</p>
<div class="note" id="zh-cn_topic_0225568977_note1155910113419"><a name="zh-cn_topic_0225568977_note1155910113419"></a><a name="zh-cn_topic_0225568977_note1155910113419"></a><span class="notetitle"> 说明： </span><div class="notebody"><p id="zh-cn_topic_0225568977_p1559011141"><a name="zh-cn_topic_0225568977_p1559011141"></a><a name="zh-cn_topic_0225568977_p1559011141"></a>中文字符必须为UTF-8或者unicode编码。</p>
</div></div>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row171743206475"><td class="cellrowborder" valign="top" width="15.52155215521552%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p31740206478"><a name="zh-cn_topic_0225568977_p31740206478"></a><a name="zh-cn_topic_0225568977_p31740206478"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="13.34133413341334%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p1174162084716"><a name="zh-cn_topic_0225568977_p1174162084716"></a><a name="zh-cn_topic_0225568977_p1174162084716"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p1217432012470"><a name="zh-cn_topic_0225568977_p1217432012470"></a><a name="zh-cn_topic_0225568977_p1217432012470"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p1825072175810"><a name="zh-cn_topic_0225568977_p1825072175810"></a><a name="zh-cn_topic_0225568977_p1825072175810"></a>后端实例的编号。</p>
<p id="zh-cn_topic_0225568977_p1647171815547"><a name="zh-cn_topic_0225568977_p1647171815547"></a><a name="zh-cn_topic_0225568977_p1647171815547"></a>支持英文，数字，“-”,“_”，1 ~ 64字符。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row4191162015475"><td class="cellrowborder" valign="top" width="15.52155215521552%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568977_p17191112094711"><a name="zh-cn_topic_0225568977_p17191112094711"></a><a name="zh-cn_topic_0225568977_p17191112094711"></a>weight</p>
</td>
<td class="cellrowborder" valign="top" width="13.34133413341334%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568977_p131911920174712"><a name="zh-cn_topic_0225568977_p131911920174712"></a><a name="zh-cn_topic_0225568977_p131911920174712"></a>type = 2时必选</p>
</td>
<td class="cellrowborder" valign="top" width="13.4013401340134%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568977_p161911220194720"><a name="zh-cn_topic_0225568977_p161911220194720"></a><a name="zh-cn_topic_0225568977_p161911220194720"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="57.73577357735774%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568977_p1133512255618"><a name="zh-cn_topic_0225568977_p1133512255618"></a><a name="zh-cn_topic_0225568977_p1133512255618"></a>权重值。</p>
<p id="zh-cn_topic_0225568977_p4191102016478"><a name="zh-cn_topic_0225568977_p4191102016478"></a><a name="zh-cn_topic_0225568977_p4191102016478"></a>权重值越大，转发到该后端实例的请求数量越多。</p>
<p id="zh-cn_topic_0225568977_p17922913115812"><a name="zh-cn_topic_0225568977_p17922913115812"></a><a name="zh-cn_topic_0225568977_p17922913115812"></a>取值范围1 ~ 100，仅VPC通道类型为2时有效。</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
  "balance_strategy": 1,
  "name": "vpc_001",
  "port": 15565,
  "type": 2,
  "member_type": "instance",
  "vpc_health_config": {
    "http_code": "205",
    "path": "/hc",
    "port": 15563,
    "protocol": "http",
    "threshold_abnormal": 5,
    "threshold_normal": 5,
    "time_interval": 200,
    "time_out": 30
  },
  "vpc_instances": [
    {
      "instance_id": "instance01",
      "instance_name": "instance_name01",
      "weight": 10
    }
  ]
}
```

## 响应消息<a name="zh-cn_topic_0225568977_section9395153012420"></a>

**表 6**  参数说明

<a name="zh-cn_topic_0225568977_table7395123013420"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568977_row114881330104215"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568977_p19488153019429"><a name="zh-cn_topic_0225568977_p19488153019429"></a><a name="zh-cn_topic_0225568977_p19488153019429"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568977_p248853014422"><a name="zh-cn_topic_0225568977_p248853014422"></a><a name="zh-cn_topic_0225568977_p248853014422"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568977_p64882308421"><a name="zh-cn_topic_0225568977_p64882308421"></a><a name="zh-cn_topic_0225568977_p64882308421"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568977_row12488203074215"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p1448813305421"><a name="zh-cn_topic_0225568977_p1448813305421"></a><a name="zh-cn_topic_0225568977_p1448813305421"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p18488163024218"><a name="zh-cn_topic_0225568977_p18488163024218"></a><a name="zh-cn_topic_0225568977_p18488163024218"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p25696563"><a name="zh-cn_topic_0225568977_p25696563"></a><a name="zh-cn_topic_0225568977_p25696563"></a>VPC通道的编号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row17488133012421"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p1585685914587"><a name="zh-cn_topic_0225568977_p1585685914587"></a><a name="zh-cn_topic_0225568977_p1585685914587"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p4488183013424"><a name="zh-cn_topic_0225568977_p4488183013424"></a><a name="zh-cn_topic_0225568977_p4488183013424"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p60351493"><a name="zh-cn_topic_0225568977_p60351493"></a><a name="zh-cn_topic_0225568977_p60351493"></a>VPC通道的名称。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row748812305426"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p19871155912585"><a name="zh-cn_topic_0225568977_p19871155912585"></a><a name="zh-cn_topic_0225568977_p19871155912585"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p64881305424"><a name="zh-cn_topic_0225568977_p64881305424"></a><a name="zh-cn_topic_0225568977_p64881305424"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p5748337181118"><a name="zh-cn_topic_0225568977_p5748337181118"></a><a name="zh-cn_topic_0225568977_p5748337181118"></a>VPC通道的类型。</p>
<a name="zh-cn_topic_0225568977_ul4748103711119"></a><a name="zh-cn_topic_0225568977_ul4748103711119"></a><ul id="zh-cn_topic_0225568977_ul4748103711119"><li>2：API网关内置支持负载均衡功能的快速通道类型</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row1684761218111"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p3847512181119"><a name="zh-cn_topic_0225568977_p3847512181119"></a><a name="zh-cn_topic_0225568977_p3847512181119"></a>member_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p18847112191114"><a name="zh-cn_topic_0225568977_p18847112191114"></a><a name="zh-cn_topic_0225568977_p18847112191114"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p1399195415116"><a name="zh-cn_topic_0225568977_p1399195415116"></a><a name="zh-cn_topic_0225568977_p1399195415116"></a>VPC通道的成员类型。</p>
<a name="zh-cn_topic_0225568977_ul10402654141119"></a><a name="zh-cn_topic_0225568977_ul10402654141119"></a><ul id="zh-cn_topic_0225568977_ul10402654141119"><li>ip（暂不支持）</li><li>instance</li></ul>
<p id="zh-cn_topic_0225568977_p1041115410113"><a name="zh-cn_topic_0225568977_p1041115410113"></a><a name="zh-cn_topic_0225568977_p1041115410113"></a>仅VPC通道类型为2时有效。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row138095017017"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p14809406014"><a name="zh-cn_topic_0225568977_p14809406014"></a><a name="zh-cn_topic_0225568977_p14809406014"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p5809305016"><a name="zh-cn_topic_0225568977_p5809305016"></a><a name="zh-cn_topic_0225568977_p5809305016"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p12663581620"><a name="zh-cn_topic_0225568977_p12663581620"></a><a name="zh-cn_topic_0225568977_p12663581620"></a>VPC通道的状态。</p>
<a name="zh-cn_topic_0225568977_ul15791839184416"></a><a name="zh-cn_topic_0225568977_ul15791839184416"></a><ul id="zh-cn_topic_0225568977_ul15791839184416"><li>1：正常</li><li>2：异常</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row31998111201"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p151995112018"><a name="zh-cn_topic_0225568977_p151995112018"></a><a name="zh-cn_topic_0225568977_p151995112018"></a>port</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p15199011306"><a name="zh-cn_topic_0225568977_p15199011306"></a><a name="zh-cn_topic_0225568977_p15199011306"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p16681305"><a name="zh-cn_topic_0225568977_p16681305"></a><a name="zh-cn_topic_0225568977_p16681305"></a>VPC通道中主机的端口号。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row05591488016"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p135594817016"><a name="zh-cn_topic_0225568977_p135594817016"></a><a name="zh-cn_topic_0225568977_p135594817016"></a>balance_strategy</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p14559178309"><a name="zh-cn_topic_0225568977_p14559178309"></a><a name="zh-cn_topic_0225568977_p14559178309"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p22981401418"><a name="zh-cn_topic_0225568977_p22981401418"></a><a name="zh-cn_topic_0225568977_p22981401418"></a>分发算法。</p>
<a name="zh-cn_topic_0225568977_ul31881612450"></a><a name="zh-cn_topic_0225568977_ul31881612450"></a><ul id="zh-cn_topic_0225568977_ul31881612450"><li>1：加权轮询（wrr）</li><li>2：加权最少连接（wleastconn）</li><li>3：源地址哈希（source）</li><li>4：URI哈希（uri）</li></ul>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row109961654185911"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568977_p19996135415590"><a name="zh-cn_topic_0225568977_p19996135415590"></a><a name="zh-cn_topic_0225568977_p19996135415590"></a>create_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568977_p20996554195919"><a name="zh-cn_topic_0225568977_p20996554195919"></a><a name="zh-cn_topic_0225568977_p20996554195919"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568977_p198451273146"><a name="zh-cn_topic_0225568977_p198451273146"></a><a name="zh-cn_topic_0225568977_p198451273146"></a>VPC通道的创建时间。</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "name": "vpc_001",
  "type": 2,
  "member_type": "instance",
  "port": 15565,
  "balance_strategy": 1,
  "id": "c3e6a7d85d9e47be89dfcc3cd37405d7",
  "create_time": "2018-07-27T12:30:48.027484Z",
  "status": 1
}
```

## 状态码<a name="zh-cn_topic_0225568977_section338043011426"></a>

**表 7**  返回消息说明

<a name="zh-cn_topic_0225568977_table1338010302424"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568977_row048810308426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568977_p174881730194216"><a name="zh-cn_topic_0225568977_p174881730194216"></a><a name="zh-cn_topic_0225568977_p174881730194216"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568977_p848863018429"><a name="zh-cn_topic_0225568977_p848863018429"></a><a name="zh-cn_topic_0225568977_p848863018429"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568977_row94881130104218"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568977_p7488163084211"><a name="zh-cn_topic_0225568977_p7488163084211"></a><a name="zh-cn_topic_0225568977_p7488163084211"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568977_p948803015424"><a name="zh-cn_topic_0225568977_p948803015424"></a><a name="zh-cn_topic_0225568977_p948803015424"></a>Created</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row1948893004211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568977_p14488113015426"><a name="zh-cn_topic_0225568977_p14488113015426"></a><a name="zh-cn_topic_0225568977_p14488113015426"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568977_p164881130154211"><a name="zh-cn_topic_0225568977_p164881130154211"></a><a name="zh-cn_topic_0225568977_p164881130154211"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row9488173084210"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568977_p24883304428"><a name="zh-cn_topic_0225568977_p24883304428"></a><a name="zh-cn_topic_0225568977_p24883304428"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568977_p1848810308429"><a name="zh-cn_topic_0225568977_p1848810308429"></a><a name="zh-cn_topic_0225568977_p1848810308429"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row1488230194211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568977_p6488133064210"><a name="zh-cn_topic_0225568977_p6488133064210"></a><a name="zh-cn_topic_0225568977_p6488133064210"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568977_p10488193018426"><a name="zh-cn_topic_0225568977_p10488193018426"></a><a name="zh-cn_topic_0225568977_p10488193018426"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row174882030134217"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568977_p144883304428"><a name="zh-cn_topic_0225568977_p144883304428"></a><a name="zh-cn_topic_0225568977_p144883304428"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568977_p4488103094212"><a name="zh-cn_topic_0225568977_p4488103094212"></a><a name="zh-cn_topic_0225568977_p4488103094212"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568977_row5488183024215"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568977_p17488163014423"><a name="zh-cn_topic_0225568977_p17488163014423"></a><a name="zh-cn_topic_0225568977_p17488163014423"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568977_p048813014216"><a name="zh-cn_topic_0225568977_p048813014216"></a><a name="zh-cn_topic_0225568977_p048813014216"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

