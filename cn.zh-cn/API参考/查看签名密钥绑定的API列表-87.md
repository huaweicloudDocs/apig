# 查看签名密钥绑定的API列表<a name="apig-phapi-180713143"></a>

## 功能介绍<a name="section7363686"></a>

查询某个签名密钥上已经绑定的API列表。

## URI<a name="section66273177"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及

<a name="table999197"></a>
<table><thead align="left"><tr id="row49370350"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p39575399"><a name="p39575399"></a><a name="p39575399"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p51490749"><a name="p51490749"></a><a name="p51490749"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row10001111"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p4783645"><a name="p4783645"></a><a name="p4783645"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p51931001"><a name="p51931001"></a><a name="p51931001"></a><span id="ph677261824511"><a name="ph677261824511"></a><a name="ph677261824511"></a>/v1/{project_id}/apigw/instances/{instance_id}</span>/sign-bindings/binded-apis[?page_size, page_no, sign_id ,env_id, api_id, api_name, group_id]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：sign\_id、env\_id、api\_id、api\_name、group\_id、page\_size、page\_no。  

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table11268757"></a>
<table><thead align="left"><tr id="row61242453"><th class="cellrowborder" valign="top" width="24.48755124487551%" id="mcps1.2.5.1.1"><p id="p61691636"><a name="p61691636"></a><a name="p61691636"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.348265173482652%" id="mcps1.2.5.1.2"><p id="p30966608"><a name="p30966608"></a><a name="p30966608"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="15.308469153084694%" id="mcps1.2.5.1.3"><p id="p25267280"><a name="p25267280"></a><a name="p25267280"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="42.85571442855714%" id="mcps1.2.5.1.4"><p id="p33383772"><a name="p33383772"></a><a name="p33383772"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1127843405112"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row470333314515"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row19731037"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p54710203"><a name="p54710203"></a><a name="p54710203"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p2341469"><a name="p2341469"></a><a name="p2341469"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p55441324"><a name="p55441324"></a><a name="p55441324"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p61562255"><a name="p61562255"></a><a name="p61562255"></a>签名密钥编号</p>
</td>
</tr>
<tr id="row17189388"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p50163177"><a name="p50163177"></a><a name="p50163177"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p36685518"><a name="p36685518"></a><a name="p36685518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p18736996"><a name="p18736996"></a><a name="p18736996"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p41301714"><a name="p41301714"></a><a name="p41301714"></a>环境编号</p>
</td>
</tr>
<tr id="row36171114"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p44179153"><a name="p44179153"></a><a name="p44179153"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p21741603"><a name="p21741603"></a><a name="p21741603"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p16239434"><a name="p16239434"></a><a name="p16239434"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p40325806"><a name="p40325806"></a><a name="p40325806"></a>API编号</p>
</td>
</tr>
<tr id="row27387938"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p3830507"><a name="p3830507"></a><a name="p3830507"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p41835685"><a name="p41835685"></a><a name="p41835685"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p33247352"><a name="p33247352"></a><a name="p33247352"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p8680971"><a name="p8680971"></a><a name="p8680971"></a>API名称</p>
</td>
</tr>
<tr id="row11019876"><td class="cellrowborder" valign="top" width="24.48755124487551%" headers="mcps1.2.5.1.1 "><p id="p20194746"><a name="p20194746"></a><a name="p20194746"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="17.348265173482652%" headers="mcps1.2.5.1.2 "><p id="p25161766"><a name="p25161766"></a><a name="p25161766"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="15.308469153084694%" headers="mcps1.2.5.1.3 "><p id="p24837133"><a name="p24837133"></a><a name="p24837133"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="42.85571442855714%" headers="mcps1.2.5.1.4 "><p id="p65650777"><a name="p65650777"></a><a name="p65650777"></a>API分组编号</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section59587687"></a>

无

## 响应消息<a name="section61873308"></a>

**表 3**  参数说明

<a name="table4657576"></a>
<table><thead align="left"><tr id="row50783217"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p19799895"><a name="p19799895"></a><a name="p19799895"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="p60287699"><a name="p60287699"></a><a name="p60287699"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p51465418"><a name="p51465418"></a><a name="p51465418"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7949350"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p39917647"><a name="p39917647"></a><a name="p39917647"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p12103980"><a name="p12103980"></a><a name="p12103980"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p40898342"><a name="p40898342"></a><a name="p40898342"></a>本次查询满足条件的API总数</p>
</td>
</tr>
<tr id="row32540761"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p18555976"><a name="p18555976"></a><a name="p18555976"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p26639112"><a name="p26639112"></a><a name="p26639112"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p10284481"><a name="p10284481"></a><a name="p10284481"></a>本次查询返回的API列表长度</p>
</td>
</tr>
<tr id="row25451466"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p48302826"><a name="p48302826"></a><a name="p48302826"></a>bindings</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p20214806"><a name="p20214806"></a><a name="p20214806"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p26786615"><a name="p26786615"></a><a name="p26786615"></a>本次查询返回的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  bindings参数说明

<a name="table22232245"></a>
<table><thead align="left"><tr id="row66251318"><th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.1"><p id="p64756531"><a name="p64756531"></a><a name="p64756531"></a><strong id="b45937869"><a name="b45937869"></a><a name="b45937869"></a>参数</strong></p>
</th>
<th class="cellrowborder" valign="top" width="16.16%" id="mcps1.2.4.1.2"><p id="p29979902"><a name="p29979902"></a><a name="p29979902"></a><strong id="b1383662"><a name="b1383662"></a><a name="b1383662"></a>类型</strong></p>
</th>
<th class="cellrowborder" valign="top" width="65.66%" id="mcps1.2.4.1.3"><p id="p44967804"><a name="p44967804"></a><a name="p44967804"></a><strong id="b2057060"><a name="b2057060"></a><a name="b2057060"></a>说明</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row32404203"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p7494749"><a name="p7494749"></a><a name="p7494749"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p3094948"><a name="p3094948"></a><a name="p3094948"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p49364264"><a name="p49364264"></a><a name="p49364264"></a>绑定关系的ID</p>
</td>
</tr>
<tr id="row41625196"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p16197717"><a name="p16197717"></a><a name="p16197717"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p36946735"><a name="p36946735"></a><a name="p36946735"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p39895586"><a name="p39895586"></a><a name="p39895586"></a>API编号</p>
</td>
</tr>
<tr id="row23515956"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p25744254"><a name="p25744254"></a><a name="p25744254"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p4909812"><a name="p4909812"></a><a name="p4909812"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p62150528"><a name="p62150528"></a><a name="p62150528"></a>API名称</p>
</td>
</tr>
<tr id="row22483840"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p9251781"><a name="p9251781"></a><a name="p9251781"></a>api_remark</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p11196819"><a name="p11196819"></a><a name="p11196819"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p34527121"><a name="p34527121"></a><a name="p34527121"></a>API描述</p>
</td>
</tr>
<tr id="row42308633"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p4447267"><a name="p4447267"></a><a name="p4447267"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p24684337"><a name="p24684337"></a><a name="p24684337"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p53274284"><a name="p53274284"></a><a name="p53274284"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row9706509"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p48029782"><a name="p48029782"></a><a name="p48029782"></a>api_type</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p65207103"><a name="p65207103"></a><a name="p65207103"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p47283952"><a name="p47283952"></a><a name="p47283952"></a>API类型</p>
</td>
</tr>
<tr id="row22902387"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p43154084"><a name="p43154084"></a><a name="p43154084"></a>sign_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p5819954"><a name="p5819954"></a><a name="p5819954"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p1654276"><a name="p1654276"></a><a name="p1654276"></a>签名密钥的编号</p>
</td>
</tr>
<tr id="row14888491"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p65117086"><a name="p65117086"></a><a name="p65117086"></a>sign_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p39992651"><a name="p39992651"></a><a name="p39992651"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p18179288"><a name="p18179288"></a><a name="p18179288"></a>签名密钥的名称</p>
</td>
</tr>
<tr id="row29395866"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p32254939"><a name="p32254939"></a><a name="p32254939"></a>sign_key</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p62513232"><a name="p62513232"></a><a name="p62513232"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p30407009"><a name="p30407009"></a><a name="p30407009"></a>签名密钥的key</p>
</td>
</tr>
<tr id="row5227632"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p20785080"><a name="p20785080"></a><a name="p20785080"></a>sign_secret</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p5869904"><a name="p5869904"></a><a name="p5869904"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p5700192"><a name="p5700192"></a><a name="p5700192"></a>签名密钥的密钥</p>
</td>
</tr>
<tr id="row51301733"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p61799709"><a name="p61799709"></a><a name="p61799709"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p39720546"><a name="p39720546"></a><a name="p39720546"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p63247643"><a name="p63247643"></a><a name="p63247643"></a>API所属环境的编号</p>
</td>
</tr>
<tr id="row32357879"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p3742522"><a name="p3742522"></a><a name="p3742522"></a>env_name</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p34708837"><a name="p34708837"></a><a name="p34708837"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p59952417"><a name="p59952417"></a><a name="p59952417"></a>API所属环境的名称</p>
</td>
</tr>
<tr id="row2700845"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p17441860"><a name="p17441860"></a><a name="p17441860"></a>binding_time</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p3504576"><a name="p3504576"></a><a name="p3504576"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p15435273"><a name="p15435273"></a><a name="p15435273"></a>绑定时间</p>
</td>
</tr>
<tr id="row18871194793313"><td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.1 "><p id="p2871144711339"><a name="p2871144711339"></a><a name="p2871144711339"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.16%" headers="mcps1.2.4.1.2 "><p id="p187144773318"><a name="p187144773318"></a><a name="p187144773318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="65.66%" headers="mcps1.2.4.1.3 "><p id="p1587134723312"><a name="p1587134723312"></a><a name="p1587134723312"></a>API的发布编号</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "total": 2,
  "size": 2,
  "bindings": [
    {
      "id": "4588ec6f5dab4f67b298dc693f58029e",
      "api_id": "d85c502a-f916-47e8-bba0-50537a2d1af2",
      "api_name": "aaa",
      "api_remark": "",
      "group_name": "asd",
      "api_type": 1,
      "sign_id": "3a793b65a9034bdfae08924f149bfb4a",
      "sign_name": "signature01",
      "sign_key": "abcd_1234",
      "sign_secret": "******",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "binding_time": "2018-02-07T07:08:51Z",
      "publish_id": "3a793b65a9034bdfae08924f149bfsda"
    },
    {
      "id": "d8426fb090e442c4a56a35e451bea085",
      "api_id": "3c6769c6-ec61-4b45-b478-c60310dbaa1b",
      "api_name": "bbb",
      "api_remark": "",
      "group_name": "asd",
      "api_type": 1,
      "sign_id": "3a793b65a9034bdfae08924f149bfb4a",
      "sign_name": "signature01",
      "sign_key": "abcd_1234",
      "sign_secret": "******",
      "env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
      "env_name": "RELEASE",
      "binding_time": "2018-02-07T03:17:26Z",
      "publish_id": "3a793b65a9034bdfae08924f149bfsda"
    }
  ]
}
```

## 状态码<a name="section66527135"></a>

**表 5**  返回消息说明

<a name="table2146877"></a>
<table><thead align="left"><tr id="row2324594"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p54074401"><a name="p54074401"></a><a name="p54074401"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p27335413"><a name="p27335413"></a><a name="p27335413"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row63292345"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p26406346"><a name="p26406346"></a><a name="p26406346"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p58539320"><a name="p58539320"></a><a name="p58539320"></a>OK</p>
</td>
</tr>
<tr id="row57091837"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p61036097"><a name="p61036097"></a><a name="p61036097"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p44976788"><a name="p44976788"></a><a name="p44976788"></a>Bad Request</p>
</td>
</tr>
<tr id="row2137916"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p38953516"><a name="p38953516"></a><a name="p38953516"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p1118208"><a name="p1118208"></a><a name="p1118208"></a>Unauthorized</p>
</td>
</tr>
<tr id="row10063875"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9867561"><a name="p9867561"></a><a name="p9867561"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p61074983"><a name="p61074983"></a><a name="p61074983"></a>Forbidden</p>
</td>
</tr>
<tr id="row12803943"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p30486494"><a name="p30486494"></a><a name="p30486494"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p15296380"><a name="p15296380"></a><a name="p15296380"></a>Not Found</p>
</td>
</tr>
<tr id="row11620166"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p1709366"><a name="p1709366"></a><a name="p1709366"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p6744143"><a name="p6744143"></a><a name="p6744143"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

