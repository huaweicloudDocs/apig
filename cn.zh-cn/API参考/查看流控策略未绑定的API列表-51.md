# 查看流控策略未绑定的API列表<a name="apig-phapi-180713071"></a>

## 功能介绍<a name="section4541287"></a>

查询所有未绑定到该流控策略上的自有API列表。需要API已经发布，未发布的API不予展示。

## URI<a name="section40871586"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1**  HTTP/HTTPS请求方法以及URI

<a name="table17929243"></a>
<table><thead align="left"><tr id="row17167268"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p48371431"><a name="p48371431"></a><a name="p48371431"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p25771876"><a name="p25771876"></a><a name="p25771876"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row7147201"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p42052390"><a name="p42052390"></a><a name="p42052390"></a>GET</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p50800444"><a name="p50800444"></a><a name="p50800444"></a>/v1/{project_id}/apigw/instances/{instance_id}/throttle-bindings/unbinded-apis[?page_size, page_no, throttle_id, group_id, env_id, api_id, api_name]</p>
</td>
</tr>
</tbody>
</table>

>![](public_sys-resources/icon-note.gif) **说明：**   
>-   可以在URI后面用‘?’和‘&’添加不同的查询条件组合。  
>-   查询条件可为以下字段以及对应的值：group\_id、env\_id、throttle\_id、api\_id、api\_name、page\_size、page\_no。  

## 请求消息<a name="section32299958"></a>

**表 2**  参数说明

<a name="table12842929"></a>
<table><thead align="left"><tr id="row39349454"><th class="cellrowborder" valign="top" width="25%" id="mcps1.2.5.1.1"><p id="p33189219"><a name="p33189219"></a><a name="p33189219"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="18.04%" id="mcps1.2.5.1.2"><p id="p3972204"><a name="p3972204"></a><a name="p3972204"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="21.89%" id="mcps1.2.5.1.3"><p id="p53313106"><a name="p53313106"></a><a name="p53313106"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="35.07%" id="mcps1.2.5.1.4"><p id="p23394300"><a name="p23394300"></a><a name="p23394300"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row414493711502"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p55878963"><a name="p55878963"></a><a name="p55878963"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p29902160"><a name="p29902160"></a><a name="p29902160"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p6155914"><a name="p6155914"></a><a name="p6155914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p28867016"><a name="p28867016"></a><a name="p28867016"></a>项目ID。可从控制台“我的凭证”中获取region下项目ID，管理员权限可查询。</p>
</td>
</tr>
<tr id="row4983113615501"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p1780913159538"><a name="p1780913159538"></a><a name="p1780913159538"></a>instance_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p9809215115310"><a name="p9809215115310"></a><a name="p9809215115310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p1280914152538"><a name="p1280914152538"></a><a name="p1280914152538"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p1880914157537"><a name="p1880914157537"></a><a name="p1880914157537"></a>实例ID，可从API网关控制台的专享版实例信息中获取。</p>
</td>
</tr>
<tr id="row15890130"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p12032190"><a name="p12032190"></a><a name="p12032190"></a>throttle_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p35083301"><a name="p35083301"></a><a name="p35083301"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p23175153"><a name="p23175153"></a><a name="p23175153"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p65248138"><a name="p65248138"></a><a name="p65248138"></a>流控策略的编号</p>
</td>
</tr>
<tr id="row50362335"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p52817301"><a name="p52817301"></a><a name="p52817301"></a>env_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p50342988"><a name="p50342988"></a><a name="p50342988"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p51250219"><a name="p51250219"></a><a name="p51250219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p57627099"><a name="p57627099"></a><a name="p57627099"></a>环境的编号</p>
</td>
</tr>
<tr id="row48881849"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p6821"><a name="p6821"></a><a name="p6821"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p552501"><a name="p552501"></a><a name="p552501"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p44752593"><a name="p44752593"></a><a name="p44752593"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p1081442"><a name="p1081442"></a><a name="p1081442"></a>API分组编号</p>
</td>
</tr>
<tr id="row9732986"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p50174421"><a name="p50174421"></a><a name="p50174421"></a>api_id</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p37596313"><a name="p37596313"></a><a name="p37596313"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p25402476"><a name="p25402476"></a><a name="p25402476"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p44334713"><a name="p44334713"></a><a name="p44334713"></a>API编号</p>
</td>
</tr>
<tr id="row63468100"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p40642456"><a name="p40642456"></a><a name="p40642456"></a>api_name</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p3704633"><a name="p3704633"></a><a name="p3704633"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p31639822"><a name="p31639822"></a><a name="p31639822"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p12688767"><a name="p12688767"></a><a name="p12688767"></a>API名称</p>
</td>
</tr>
<tr id="row47090046"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p56197414"><a name="p56197414"></a><a name="p56197414"></a>page_size</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p55696670"><a name="p55696670"></a><a name="p55696670"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p15136398"><a name="p15136398"></a><a name="p15136398"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p18088735"><a name="p18088735"></a><a name="p18088735"></a>每页显示的条数，默认值：20</p>
</td>
</tr>
<tr id="row28580891"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.2.5.1.1 "><p id="p33350848"><a name="p33350848"></a><a name="p33350848"></a>page_no</p>
</td>
<td class="cellrowborder" valign="top" width="18.04%" headers="mcps1.2.5.1.2 "><p id="p17064153"><a name="p17064153"></a><a name="p17064153"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="21.89%" headers="mcps1.2.5.1.3 "><p id="p40019151"><a name="p40019151"></a><a name="p40019151"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="35.07%" headers="mcps1.2.5.1.4 "><p id="p20325769"><a name="p20325769"></a><a name="p20325769"></a>页码，默认值：1</p>
</td>
</tr>
</tbody>
</table>

## 响应消息<a name="section66159830"></a>

**表 3**  参数说明

<a name="table35267323"></a>
<table><thead align="left"><tr id="row2437493"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p63219260"><a name="p63219260"></a><a name="p63219260"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p20486464"><a name="p20486464"></a><a name="p20486464"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p48790888"><a name="p48790888"></a><a name="p48790888"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row59747869"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7739206"><a name="p7739206"></a><a name="p7739206"></a>total</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p22895948"><a name="p22895948"></a><a name="p22895948"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p42632470"><a name="p42632470"></a><a name="p42632470"></a>满足查询条件的API的总个数</p>
</td>
</tr>
<tr id="row48147912"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7666804"><a name="p7666804"></a><a name="p7666804"></a>size</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p17031384"><a name="p17031384"></a><a name="p17031384"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p37364893"><a name="p37364893"></a><a name="p37364893"></a>当前查询到的列表长度</p>
</td>
</tr>
<tr id="row739723"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p59917636"><a name="p59917636"></a><a name="p59917636"></a>apis</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p21490353"><a name="p21490353"></a><a name="p21490353"></a>字典数据类型</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p62997051"><a name="p62997051"></a><a name="p62997051"></a>当前查询到的API列表</p>
</td>
</tr>
</tbody>
</table>

**表 4**  apis参数说明

<a name="table30102550"></a>
<table><thead align="left"><tr id="row47773471"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.1"><p id="p44445903"><a name="p44445903"></a><a name="p44445903"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="20%" id="mcps1.2.4.1.2"><p id="p43348363"><a name="p43348363"></a><a name="p43348363"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="60%" id="mcps1.2.4.1.3"><p id="p21556540"><a name="p21556540"></a><a name="p21556540"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1249354"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p34088860"><a name="p34088860"></a><a name="p34088860"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9734299"><a name="p9734299"></a><a name="p9734299"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p50280750"><a name="p50280750"></a><a name="p50280750"></a>API编号</p>
</td>
</tr>
<tr id="row49873571"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p13227440"><a name="p13227440"></a><a name="p13227440"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p64789701"><a name="p64789701"></a><a name="p64789701"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p13474443"><a name="p13474443"></a><a name="p13474443"></a>API名称</p>
</td>
</tr>
<tr id="row54161128"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24975225"><a name="p24975225"></a><a name="p24975225"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p9727376"><a name="p9727376"></a><a name="p9727376"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p49719954"><a name="p49719954"></a><a name="p49719954"></a>API所属分组的编号</p>
</td>
</tr>
<tr id="row44826408"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p7060408"><a name="p7060408"></a><a name="p7060408"></a>group_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p35022185"><a name="p35022185"></a><a name="p35022185"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p18224738"><a name="p18224738"></a><a name="p18224738"></a>API所属分组的名称</p>
</td>
</tr>
<tr id="row15125437"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17200889"><a name="p17200889"></a><a name="p17200889"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p51094765"><a name="p51094765"></a><a name="p51094765"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p45035330"><a name="p45035330"></a><a name="p45035330"></a>API类型</p>
</td>
</tr>
<tr id="row17619504"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p17893702"><a name="p17893702"></a><a name="p17893702"></a>remark</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p40103794"><a name="p40103794"></a><a name="p40103794"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p27181849"><a name="p27181849"></a><a name="p27181849"></a>API描述</p>
</td>
</tr>
<tr id="row19362357"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p24847075"><a name="p24847075"></a><a name="p24847075"></a>run_env_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p66456062"><a name="p66456062"></a><a name="p66456062"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p14231917"><a name="p14231917"></a><a name="p14231917"></a>发布的环境名</p>
</td>
</tr>
<tr id="row60978392"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p40302689"><a name="p40302689"></a><a name="p40302689"></a>run_env_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p43292338"><a name="p43292338"></a><a name="p43292338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p17018484"><a name="p17018484"></a><a name="p17018484"></a>发布的环境编号</p>
</td>
</tr>
<tr id="row18948630"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p58444100"><a name="p58444100"></a><a name="p58444100"></a>publish_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p36351670"><a name="p36351670"></a><a name="p36351670"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p58804181"><a name="p58804181"></a><a name="p58804181"></a>发布记录的编号</p>
</td>
</tr>
<tr id="row59475584"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p52793037"><a name="p52793037"></a><a name="p52793037"></a>throttle_apply_id</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p48377594"><a name="p48377594"></a><a name="p48377594"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p26271023"><a name="p26271023"></a><a name="p26271023"></a>与流控策略的绑定关系编号</p>
</td>
</tr>
<tr id="row35112621"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p25550018"><a name="p25550018"></a><a name="p25550018"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p56285555"><a name="p56285555"></a><a name="p56285555"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p62836138"><a name="p62836138"></a><a name="p62836138"></a>绑定的流控策略名称</p>
</td>
</tr>
<tr id="row37358398"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p6131397"><a name="p6131397"></a><a name="p6131397"></a>apply_time</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p26881140"><a name="p26881140"></a><a name="p26881140"></a>Timestamp</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p490214367555"><a name="p490214367555"></a><a name="p490214367555"></a>已绑定的流控策略的绑定时间</p>
</td>
</tr>
<tr id="row16577124415"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p8658312243"><a name="p8658312243"></a><a name="p8658312243"></a>auth_type</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p8658412247"><a name="p8658412247"></a><a name="p8658412247"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p765891210419"><a name="p765891210419"></a><a name="p765891210419"></a>API的认证方式</p>
</td>
</tr>
<tr id="row18792676513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.1 "><p id="p4792117258"><a name="p4792117258"></a><a name="p4792117258"></a>req_uri</p>
</td>
<td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.4.1.2 "><p id="p57924711516"><a name="p57924711516"></a><a name="p57924711516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="60%" headers="mcps1.2.4.1.3 "><p id="p779287456"><a name="p779287456"></a><a name="p779287456"></a>API的访问地址</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
	"total": 2,
	"size": 2,
	"apis": [{
		"id": "5bbc47e2-95b0-4a56-904e-a3cdc422f8e9",
		"name": "查询分组列表",
		"type": 1,
		"remark": "查询分组列表",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"group_name": "api_group_001",
		"run_env_name": "RELEASE",
		"run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"publish_id": "65e6fe53-1ac3-4481-ba36-9f0bc6f22057",
		"auth_type": "APP",
		"req_uri": "/test"
	},
	{
		"id": "6632a062-9dcf-4f18-9646-3cabb925a290",
		"name": "查询API列表",
		"type": 1,
		"remark": "查询API列表",
		"group_id": "73c58022-f20d-495a-a188-85d718647f09",
		"group_name": "api_group_001",
		"run_env_name": "RELEASE",
		"run_env_id": "DEFAULT_ENVIRONMENT_RELEASE_ID",
		"publish_id": "374a6d5a-20c7-4ea1-82e1-19fce4556956",
		"auth_type": "APP",
		"req_uri": "/test"
	}]
}
```

## 状态码<a name="section22264173"></a>

**表 5**  返回消息说明

<a name="table35774575"></a>
<table><thead align="left"><tr id="row113656"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p9206198"><a name="p9206198"></a><a name="p9206198"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p7504548"><a name="p7504548"></a><a name="p7504548"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row3888618"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p46542641"><a name="p46542641"></a><a name="p46542641"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p11857568"><a name="p11857568"></a><a name="p11857568"></a>OK</p>
</td>
</tr>
<tr id="row39609255"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p54233062"><a name="p54233062"></a><a name="p54233062"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p30801890"><a name="p30801890"></a><a name="p30801890"></a>Bad Request</p>
</td>
</tr>
<tr id="row8781554"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p40217235"><a name="p40217235"></a><a name="p40217235"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p36370597"><a name="p36370597"></a><a name="p36370597"></a>Unauthorized</p>
</td>
</tr>
<tr id="row58899919"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p6164173"><a name="p6164173"></a><a name="p6164173"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p29536015"><a name="p29536015"></a><a name="p29536015"></a>Forbidden</p>
</td>
</tr>
<tr id="row64497550"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p56919025"><a name="p56919025"></a><a name="p56919025"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p47038350"><a name="p47038350"></a><a name="p47038350"></a>Not Found</p>
</td>
</tr>
<tr id="row20691969"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p65436773"><a name="p65436773"></a><a name="p65436773"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p26951156195313"><a name="p26951156195313"></a><a name="p26951156195313"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

