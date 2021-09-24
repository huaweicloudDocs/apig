# 查看APP未绑定的API列表<a name="ZH-CN_TOPIC_0000001081837347"></a>

## 功能简介<a name="zh-cn_topic_0225568842_section57945658"></a>

查询指定环境上某个APP未绑定的API列表，包括自有API和从云市场购买的API。

## URI<a name="zh-cn_topic_0225568842_section51748875"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="zh-cn_topic_0225568842_table65264697"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568842_row59320654"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568842_p40243635"><a name="zh-cn_topic_0225568842_p40243635"></a><a name="zh-cn_topic_0225568842_p40243635"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568842_p38508980"><a name="zh-cn_topic_0225568842_p38508980"></a><a name="zh-cn_topic_0225568842_p38508980"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568842_row32219707"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568842_p59659437"><a name="zh-cn_topic_0225568842_p59659437"></a><a name="zh-cn_topic_0225568842_p59659437"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568842_p576244"><a name="zh-cn_topic_0225568842_p576244"></a><a name="zh-cn_topic_0225568842_p576244"></a>/v1/{project_id}/apigw/instances/{instance_id}/app-auths/unbinded-apis[?page_size, page_no, app_id, env_id, api_id, api_name, group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：** 
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。
>-   查询条件可为以下字段以及对应的值：app\_id、api\_id、api\_name、group\_id、env\_id、page\_size、page\_no。

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="zh-cn_topic_0225568842_table22390613"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568842_row15100740"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="zh-cn_topic_0225568842_p15200464"><a name="zh-cn_topic_0225568842_p15200464"></a><a name="zh-cn_topic_0225568842_p15200464"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.2"><p id="zh-cn_topic_0225568842_p23278039"><a name="zh-cn_topic_0225568842_p23278039"></a><a name="zh-cn_topic_0225568842_p23278039"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="zh-cn_topic_0225568842_p6473027"><a name="zh-cn_topic_0225568842_p6473027"></a><a name="zh-cn_topic_0225568842_p6473027"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="44.89551044895511%" id="mcps1.2.5.1.4"><p id="zh-cn_topic_0225568842_p54553212"><a name="zh-cn_topic_0225568842_p54553212"></a><a name="zh-cn_topic_0225568842_p54553212"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568842_row129168325460"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p55878963"><a name="zh-cn_topic_0225568842_p55878963"></a><a name="zh-cn_topic_0225568842_p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p29902160"><a name="zh-cn_topic_0225568842_p29902160"></a><a name="zh-cn_topic_0225568842_p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p6155914"><a name="zh-cn_topic_0225568842_p6155914"></a><a name="zh-cn_topic_0225568842_p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p28867016"><a name="zh-cn_topic_0225568842_p28867016"></a><a name="zh-cn_topic_0225568842_p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row137539327465"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p1780913159538"><a name="zh-cn_topic_0225568842_p1780913159538"></a><a name="zh-cn_topic_0225568842_p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p9809215115310"><a name="zh-cn_topic_0225568842_p9809215115310"></a><a name="zh-cn_topic_0225568842_p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p1280914152538"><a name="zh-cn_topic_0225568842_p1280914152538"></a><a name="zh-cn_topic_0225568842_p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p1880914157537"><a name="zh-cn_topic_0225568842_p1880914157537"></a><a name="zh-cn_topic_0225568842_p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row56734057"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p32055923"><a name="zh-cn_topic_0225568842_p32055923"></a><a name="zh-cn_topic_0225568842_p32055923"></a>app_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p46392961"><a name="zh-cn_topic_0225568842_p46392961"></a><a name="zh-cn_topic_0225568842_p46392961"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p66842364"><a name="zh-cn_topic_0225568842_p66842364"></a><a name="zh-cn_topic_0225568842_p66842364"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p45522379"><a name="zh-cn_topic_0225568842_p45522379"></a><a name="zh-cn_topic_0225568842_p45522379"></a>应用id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row7048230"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p34035727"><a name="zh-cn_topic_0225568842_p34035727"></a><a name="zh-cn_topic_0225568842_p34035727"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p5430464"><a name="zh-cn_topic_0225568842_p5430464"></a><a name="zh-cn_topic_0225568842_p5430464"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p37214434"><a name="zh-cn_topic_0225568842_p37214434"></a><a name="zh-cn_topic_0225568842_p37214434"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p61579164"><a name="zh-cn_topic_0225568842_p61579164"></a><a name="zh-cn_topic_0225568842_p61579164"></a>环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row17341570"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p62489940"><a name="zh-cn_topic_0225568842_p62489940"></a><a name="zh-cn_topic_0225568842_p62489940"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p28520403"><a name="zh-cn_topic_0225568842_p28520403"></a><a name="zh-cn_topic_0225568842_p28520403"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p28451302"><a name="zh-cn_topic_0225568842_p28451302"></a><a name="zh-cn_topic_0225568842_p28451302"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p22854134"><a name="zh-cn_topic_0225568842_p22854134"></a><a name="zh-cn_topic_0225568842_p22854134"></a>API分组编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row4360616"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p17665597"><a name="zh-cn_topic_0225568842_p17665597"></a><a name="zh-cn_topic_0225568842_p17665597"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p21627267"><a name="zh-cn_topic_0225568842_p21627267"></a><a name="zh-cn_topic_0225568842_p21627267"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p6978209"><a name="zh-cn_topic_0225568842_p6978209"></a><a name="zh-cn_topic_0225568842_p6978209"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p28364096"><a name="zh-cn_topic_0225568842_p28364096"></a><a name="zh-cn_topic_0225568842_p28364096"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row53950280"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p7896522"><a name="zh-cn_topic_0225568842_p7896522"></a><a name="zh-cn_topic_0225568842_p7896522"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p35638561"><a name="zh-cn_topic_0225568842_p35638561"></a><a name="zh-cn_topic_0225568842_p35638561"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p1042357"><a name="zh-cn_topic_0225568842_p1042357"></a><a name="zh-cn_topic_0225568842_p1042357"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p17322093"><a name="zh-cn_topic_0225568842_p17322093"></a><a name="zh-cn_topic_0225568842_p17322093"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row21681114"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p11339844"><a name="zh-cn_topic_0225568842_p11339844"></a><a name="zh-cn_topic_0225568842_p11339844"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p46112199"><a name="zh-cn_topic_0225568842_p46112199"></a><a name="zh-cn_topic_0225568842_p46112199"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p44100618"><a name="zh-cn_topic_0225568842_p44100618"></a><a name="zh-cn_topic_0225568842_p44100618"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p15380277"><a name="zh-cn_topic_0225568842_p15380277"></a><a name="zh-cn_topic_0225568842_p15380277"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row4204769"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="zh-cn_topic_0225568842_p5042045"><a name="zh-cn_topic_0225568842_p5042045"></a><a name="zh-cn_topic_0225568842_p5042045"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.2 "><p id="zh-cn_topic_0225568842_p5752468"><a name="zh-cn_topic_0225568842_p5752468"></a><a name="zh-cn_topic_0225568842_p5752468"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="zh-cn_topic_0225568842_p63296784"><a name="zh-cn_topic_0225568842_p63296784"></a><a name="zh-cn_topic_0225568842_p63296784"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="44.89551044895511%" headers="mcps1.2.5.1.4 "><p id="zh-cn_topic_0225568842_p26765913"><a name="zh-cn_topic_0225568842_p26765913"></a><a name="zh-cn_topic_0225568842_p26765913"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="zh-cn_topic_0225568842_section63086694"></a>

无

## 响应消息<a name="zh-cn_topic_0225568842_section9748615"></a>

**表 3**  参数说明

<a name="zh-cn_topic_0225568842_table35112378"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568842_row10083439"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568842_p11452202"><a name="zh-cn_topic_0225568842_p11452202"></a><a name="zh-cn_topic_0225568842_p11452202"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568842_p55213174"><a name="zh-cn_topic_0225568842_p55213174"></a><a name="zh-cn_topic_0225568842_p55213174"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568842_p43082106"><a name="zh-cn_topic_0225568842_p43082106"></a><a name="zh-cn_topic_0225568842_p43082106"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568842_row67098591"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p66276813"><a name="zh-cn_topic_0225568842_p66276813"></a><a name="zh-cn_topic_0225568842_p66276813"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p66821611"><a name="zh-cn_topic_0225568842_p66821611"></a><a name="zh-cn_topic_0225568842_p66821611"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p43841377"><a name="zh-cn_topic_0225568842_p43841377"></a><a name="zh-cn_topic_0225568842_p43841377"></a>符合条件的API的总数</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row59028077"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p16544923"><a name="zh-cn_topic_0225568842_p16544923"></a><a name="zh-cn_topic_0225568842_p16544923"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p65070390"><a name="zh-cn_topic_0225568842_p65070390"></a><a name="zh-cn_topic_0225568842_p65070390"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p36210213"><a name="zh-cn_topic_0225568842_p36210213"></a><a name="zh-cn_topic_0225568842_p36210213"></a>本次返回的列表长度</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row57456464"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p23461977"><a name="zh-cn_topic_0225568842_p23461977"></a><a name="zh-cn_topic_0225568842_p23461977"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p21371946"><a name="zh-cn_topic_0225568842_p21371946"></a><a name="zh-cn_topic_0225568842_p21371946"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p53406060"><a name="zh-cn_topic_0225568842_p53406060"></a><a name="zh-cn_topic_0225568842_p53406060"></a>本次返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="zh-cn_topic_0225568842_table10892494"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568842_row42715000"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="zh-cn_topic_0225568842_p37363013"><a name="zh-cn_topic_0225568842_p37363013"></a><a name="zh-cn_topic_0225568842_p37363013"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="zh-cn_topic_0225568842_p6505202"><a name="zh-cn_topic_0225568842_p6505202"></a><a name="zh-cn_topic_0225568842_p6505202"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="zh-cn_topic_0225568842_p57159335"><a name="zh-cn_topic_0225568842_p57159335"></a><a name="zh-cn_topic_0225568842_p57159335"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568842_row66503437"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p18069323"><a name="zh-cn_topic_0225568842_p18069323"></a><a name="zh-cn_topic_0225568842_p18069323"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p54329098"><a name="zh-cn_topic_0225568842_p54329098"></a><a name="zh-cn_topic_0225568842_p54329098"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p38580850"><a name="zh-cn_topic_0225568842_p38580850"></a><a name="zh-cn_topic_0225568842_p38580850"></a>API编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row11683332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p6825851"><a name="zh-cn_topic_0225568842_p6825851"></a><a name="zh-cn_topic_0225568842_p6825851"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p16023087"><a name="zh-cn_topic_0225568842_p16023087"></a><a name="zh-cn_topic_0225568842_p16023087"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p22801671"><a name="zh-cn_topic_0225568842_p22801671"></a><a name="zh-cn_topic_0225568842_p22801671"></a>API名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row3888452"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p46529230"><a name="zh-cn_topic_0225568842_p46529230"></a><a name="zh-cn_topic_0225568842_p46529230"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p10771313"><a name="zh-cn_topic_0225568842_p10771313"></a><a name="zh-cn_topic_0225568842_p10771313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p61140"><a name="zh-cn_topic_0225568842_p61140"></a><a name="zh-cn_topic_0225568842_p61140"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row550261"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p44571163"><a name="zh-cn_topic_0225568842_p44571163"></a><a name="zh-cn_topic_0225568842_p44571163"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p53494487"><a name="zh-cn_topic_0225568842_p53494487"></a><a name="zh-cn_topic_0225568842_p53494487"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p38086158"><a name="zh-cn_topic_0225568842_p38086158"></a><a name="zh-cn_topic_0225568842_p38086158"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row43301387"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p17751458"><a name="zh-cn_topic_0225568842_p17751458"></a><a name="zh-cn_topic_0225568842_p17751458"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p28581985"><a name="zh-cn_topic_0225568842_p28581985"></a><a name="zh-cn_topic_0225568842_p28581985"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p33439473"><a name="zh-cn_topic_0225568842_p33439473"></a><a name="zh-cn_topic_0225568842_p33439473"></a>API描述</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row63537654"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p46276336"><a name="zh-cn_topic_0225568842_p46276336"></a><a name="zh-cn_topic_0225568842_p46276336"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p57395755"><a name="zh-cn_topic_0225568842_p57395755"></a><a name="zh-cn_topic_0225568842_p57395755"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p18544591"><a name="zh-cn_topic_0225568842_p18544591"></a><a name="zh-cn_topic_0225568842_p18544591"></a>发布的环境名</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row32683591"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p30125210"><a name="zh-cn_topic_0225568842_p30125210"></a><a name="zh-cn_topic_0225568842_p30125210"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p24222954"><a name="zh-cn_topic_0225568842_p24222954"></a><a name="zh-cn_topic_0225568842_p24222954"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p15902238"><a name="zh-cn_topic_0225568842_p15902238"></a><a name="zh-cn_topic_0225568842_p15902238"></a>发布的环境id</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row8902417"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p50007191"><a name="zh-cn_topic_0225568842_p50007191"></a><a name="zh-cn_topic_0225568842_p50007191"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p24050677"><a name="zh-cn_topic_0225568842_p24050677"></a><a name="zh-cn_topic_0225568842_p24050677"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p1947860"><a name="zh-cn_topic_0225568842_p1947860"></a><a name="zh-cn_topic_0225568842_p1947860"></a>发布记录的编号</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row18713323316"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p587733133318"><a name="zh-cn_topic_0225568842_p587733133318"></a><a name="zh-cn_topic_0225568842_p587733133318"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p1588163353318"><a name="zh-cn_topic_0225568842_p1588163353318"></a><a name="zh-cn_topic_0225568842_p1588163353318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p188133343318"><a name="zh-cn_topic_0225568842_p188133343318"></a><a name="zh-cn_topic_0225568842_p188133343318"></a>API的认证方式</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row1130901133416"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="zh-cn_topic_0225568842_p12309171103416"><a name="zh-cn_topic_0225568842_p12309171103416"></a><a name="zh-cn_topic_0225568842_p12309171103416"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="zh-cn_topic_0225568842_p133092011193413"><a name="zh-cn_topic_0225568842_p133092011193413"></a><a name="zh-cn_topic_0225568842_p133092011193413"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="zh-cn_topic_0225568842_p113092118346"><a name="zh-cn_topic_0225568842_p113092118346"></a><a name="zh-cn_topic_0225568842_p113092118346"></a>API的访问地址</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 1,
	"size": 1,
	"apis": [{
		"id": "5bbc47e2-95b0-4a56-904e-a3cdc422f8e9",
		"name": "查询分组列表",
		"remark": "查询分组列表",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"group_name": "api_group_001",
		"run_env_name": "RELEASE",
		"run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"publish_id": "65e6fe53-1ac3-4481-ba36-9f0bc6f22057",
		"auth_type": "APP",
		"req_uri": "/test"
	}]
}
```

## 状态码<a name="zh-cn_topic_0225568842_section30909341"></a>

**表 5**  返回消息说明

<a name="zh-cn_topic_0225568842_table54370672"></a>
<table><thead align="left"><tr id="zh-cn_topic_0225568842_row45779426"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="zh-cn_topic_0225568842_p17146043"><a name="zh-cn_topic_0225568842_p17146043"></a><a name="zh-cn_topic_0225568842_p17146043"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="zh-cn_topic_0225568842_p46652212"><a name="zh-cn_topic_0225568842_p46652212"></a><a name="zh-cn_topic_0225568842_p46652212"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="zh-cn_topic_0225568842_row20732789"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568842_p1634343"><a name="zh-cn_topic_0225568842_p1634343"></a><a name="zh-cn_topic_0225568842_p1634343"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568842_p65272945"><a name="zh-cn_topic_0225568842_p65272945"></a><a name="zh-cn_topic_0225568842_p65272945"></a>OK</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row50585599"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568842_p3792865"><a name="zh-cn_topic_0225568842_p3792865"></a><a name="zh-cn_topic_0225568842_p3792865"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568842_p38786672"><a name="zh-cn_topic_0225568842_p38786672"></a><a name="zh-cn_topic_0225568842_p38786672"></a>Bad Request</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row13535731"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568842_p22652464"><a name="zh-cn_topic_0225568842_p22652464"></a><a name="zh-cn_topic_0225568842_p22652464"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568842_p22910285"><a name="zh-cn_topic_0225568842_p22910285"></a><a name="zh-cn_topic_0225568842_p22910285"></a>Unauthorized</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row4865975"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568842_p58599688"><a name="zh-cn_topic_0225568842_p58599688"></a><a name="zh-cn_topic_0225568842_p58599688"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568842_p48954253"><a name="zh-cn_topic_0225568842_p48954253"></a><a name="zh-cn_topic_0225568842_p48954253"></a>Forbidden</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row37935094"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568842_p52843813"><a name="zh-cn_topic_0225568842_p52843813"></a><a name="zh-cn_topic_0225568842_p52843813"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568842_p52490493"><a name="zh-cn_topic_0225568842_p52490493"></a><a name="zh-cn_topic_0225568842_p52490493"></a>Not Found</p>
</td>
</tr>
<tr id="zh-cn_topic_0225568842_row2652391"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="zh-cn_topic_0225568842_p13517134"><a name="zh-cn_topic_0225568842_p13517134"></a><a name="zh-cn_topic_0225568842_p13517134"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="zh-cn_topic_0225568842_p14947689"><a name="zh-cn_topic_0225568842_p14947689"></a><a name="zh-cn_topic_0225568842_p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

