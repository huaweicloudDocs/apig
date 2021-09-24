# 删除ACL策略<a name="ZH-CN_TOPIC_0000001081976199"></a>

## 功能介绍<a name="zh-cn_topic_0225568885_section48394544"></a>

删除指定的ACL策略， 如果存在api与该ACL策略的绑定关系，则无法删除

## URI<a name="zh-cn_topic_0225568885_section32897718"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568885_table33718846"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568885_row34578608"><th class="cellrowborder" valign="top" width="34.339999999999996%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568885_p49403825"><a name="zh-cn_topic_0225568885_p49403825"></a><a name="zh-cn_topic_0225568885_p49403825"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568885_p42286883"><a name="zh-cn_topic_0225568885_p42286883"></a><a name="zh-cn_topic_0225568885_p42286883"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568885_row2685485"><td class="cellrowborder" valign="top" width="34.339999999999996%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568885_p16197752"><a name="zh-cn_topic_0225568885_p16197752"></a><a name="zh-cn_topic_0225568885_p16197752"></a>DELETE</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568885_p36949548"><a name="zh-cn_topic_0225568885_p36949548"></a><a name="zh-cn_topic_0225568885_p36949548"></a>/v1/{project_id}/apigw/instances/{instance_id}/acls/{id}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568885_table40123375"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568885_row11290180"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568885_p42089394"><a name="zh-cn_topic_0225568885_p42089394"></a><a name="zh-cn_topic_0225568885_p42089394"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.71%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568885_p53797793"><a name="zh-cn_topic_0225568885_p53797793"></a><a name="zh-cn_topic_0225568885_p53797793"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.8%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568885_p62654009"><a name="zh-cn_topic_0225568885_p62654009"></a><a name="zh-cn_topic_0225568885_p62654009"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="38.49%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568885_p41809953"><a name="zh-cn_topic_0225568885_p41809953"></a><a name="zh-cn_topic_0225568885_p41809953"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568885_row78602219185"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568885_p55878963"><a name="zh-cn_topic_0225568885_p55878963"></a><a name="zh-cn_topic_0225568885_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.71%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568885_p29902160"><a name="zh-cn_topic_0225568885_p29902160"></a><a name="zh-cn_topic_0225568885_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.8%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568885_p6155914"><a name="zh-cn_topic_0225568885_p6155914"></a><a name="zh-cn_topic_0225568885_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.49%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568885_p28867016"><a name="zh-cn_topic_0225568885_p28867016"></a><a name="zh-cn_topic_0225568885_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568885_row1347892171817"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568885_p1780913159538"><a name="zh-cn_topic_0225568885_p1780913159538"></a><a name="zh-cn_topic_0225568885_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.71%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568885_p9809215115310"><a name="zh-cn_topic_0225568885_p9809215115310"></a><a name="zh-cn_topic_0225568885_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.8%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568885_p1280914152538"><a name="zh-cn_topic_0225568885_p1280914152538"></a><a name="zh-cn_topic_0225568885_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.49%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568885_p1880914157537"><a name="zh-cn_topic_0225568885_p1880914157537"></a><a name="zh-cn_topic_0225568885_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568885_row31163009"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568885_p41175810"><a name="zh-cn_topic_0225568885_p41175810"></a><a name="zh-cn_topic_0225568885_p41175810"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.71%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568885_p46906315"><a name="zh-cn_topic_0225568885_p46906315"></a><a name="zh-cn_topic_0225568885_p46906315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="19.8%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568885_p41315205"><a name="zh-cn_topic_0225568885_p41315205"></a><a name="zh-cn_topic_0225568885_p41315205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="38.49%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568885_p58197336"><a name="zh-cn_topic_0225568885_p58197336"></a><a name="zh-cn_topic_0225568885_p58197336"></a>ACL的ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568885_section27644012"></a>

无

## 响应消息<a name="zh-cn_topic_0225568885_section19612185101811"></a>

无

## 状态码<a name="zh-cn_topic_0225568885_section47469524"></a>

**表 3**  返回消息说明

<a name="zh-cn_topic_0225568885_table50395750"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568885_row10317805"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568885_p30435897"><a name="zh-cn_topic_0225568885_p30435897"></a><a name="zh-cn_topic_0225568885_p30435897"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568885_p49388626"><a name="zh-cn_topic_0225568885_p49388626"></a><a name="zh-cn_topic_0225568885_p49388626"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568885_row41055775"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568885_p37183497"><a name="zh-cn_topic_0225568885_p37183497"></a><a name="zh-cn_topic_0225568885_p37183497"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568885_p59073271"><a name="zh-cn_topic_0225568885_p59073271"></a><a name="zh-cn_topic_0225568885_p59073271"></a>No Content</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568885_row61897395"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568885_p47633123"><a name="zh-cn_topic_0225568885_p47633123"></a><a name="zh-cn_topic_0225568885_p47633123"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568885_p33077772"><a name="zh-cn_topic_0225568885_p33077772"></a><a name="zh-cn_topic_0225568885_p33077772"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568885_row29264493"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568885_p21613693"><a name="zh-cn_topic_0225568885_p21613693"></a><a name="zh-cn_topic_0225568885_p21613693"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568885_p5878681"><a name="zh-cn_topic_0225568885_p5878681"></a><a name="zh-cn_topic_0225568885_p5878681"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568885_row52908136"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568885_p57700610"><a name="zh-cn_topic_0225568885_p57700610"></a><a name="zh-cn_topic_0225568885_p57700610"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568885_p6744143"><a name="zh-cn_topic_0225568885_p6744143"></a><a name="zh-cn_topic_0225568885_p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

