# 导入API到已有分组<a name="apig-zh-api-190108258"></a>

## 功能介绍<a name="section39777523194"></a>

导入swagger格式的文件, 在已有分组中创建或更新API。swagger文件支持json以及yaml格式。

## URI<a name="section1199919551442"></a>

HTTP/HTTPS请求方法以及URI如下表所示。

**表 1** 

<a name="table1030719520475"></a>
<table><thead align="left"><tr id="row1130715217477"><th class="cellrowborder" valign="top" width="20.57%" id="mcps1.2.3.1.1"><p id="p130795213478"><a name="p130795213478"></a><a name="p130795213478"></a>请求方法</p>
</th>
<th class="cellrowborder" valign="top" width="79.43%" id="mcps1.2.3.1.2"><p id="p13307135204712"><a name="p13307135204712"></a><a name="p13307135204712"></a>URI</p>
</th>
</tr>
</thead>
<tbody><tr id="row15307252144718"><td class="cellrowborder" valign="top" width="20.57%" headers="mcps1.2.3.1.1 "><p id="p1930714525475"><a name="p1930714525475"></a><a name="p1930714525475"></a>PUT</p>
</td>
<td class="cellrowborder" valign="top" width="79.43%" headers="mcps1.2.3.1.2 "><p id="p19454226101515"><a name="p19454226101515"></a><a name="p19454226101515"></a>/v1.0/apigw/openapi?group_id={0}&amp;mode={1}</p>
</td>
</tr>
</tbody>
</table>

URI中的参数说明如下表所示。

**表 2**  参数说明

<a name="table871144945810"></a>
<table><thead align="left"><tr id="row14734499589"><th class="cellrowborder" valign="top" width="17.87178717871787%" id="mcps1.2.5.1.1"><p id="p1973174918589"><a name="p1973174918589"></a><a name="p1973174918589"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="14.041404140414041%" id="mcps1.2.5.1.2"><p id="p4731749125817"><a name="p4731749125817"></a><a name="p4731749125817"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.511151115111511%" id="mcps1.2.5.1.3"><p id="p1730491589"><a name="p1730491589"></a><a name="p1730491589"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="56.57565756575658%" id="mcps1.2.5.1.4"><p id="p1073649175817"><a name="p1073649175817"></a><a name="p1073649175817"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row15201144012331"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="p142011240183311"><a name="p142011240183311"></a><a name="p142011240183311"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="p112014407332"><a name="p112014407332"></a><a name="p112014407332"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="p120384023318"><a name="p120384023318"></a><a name="p120384023318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="p162039406337"><a name="p162039406337"></a><a name="p162039406337"></a>分组 ID</p>
</td>
</tr>
<tr id="row13868431333"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="p16386174316334"><a name="p16386174316334"></a><a name="p16386174316334"></a>mode</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="p12386164313315"><a name="p12386164313315"></a><a name="p12386164313315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="p03861443143312"><a name="p03861443143312"></a><a name="p03861443143312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="p159102715173"><a name="p159102715173"></a><a name="p159102715173"></a>导入模式，可选merge和override。</p>
<p id="p338634311333"><a name="p338634311333"></a><a name="p338634311333"></a>当API定义冲突时，merge保留原有API，override会覆盖原有API。</p>
</td>
</tr>
<tr id="row11890741245"><td class="cellrowborder" valign="top" width="17.87178717871787%" headers="mcps1.2.5.1.1 "><p id="p12891154343"><a name="p12891154343"></a><a name="p12891154343"></a>extend_mode</p>
</td>
<td class="cellrowborder" valign="top" width="14.041404140414041%" headers="mcps1.2.5.1.2 "><p id="p6531195013518"><a name="p6531195013518"></a><a name="p6531195013518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.511151115111511%" headers="mcps1.2.5.1.3 "><p id="p1089114945"><a name="p1089114945"></a><a name="p1089114945"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="56.57565756575658%" headers="mcps1.2.5.1.4 "><p id="p1089213410413"><a name="p1089213410413"></a><a name="p1089213410413"></a>扩展信息导入模式，可选merge和override。</p>
<p id="p10778501566"><a name="p10778501566"></a><a name="p10778501566"></a>当扩展信息定义冲突时，merge保留原有扩展信息，override会覆盖原有扩展信息。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section178868115223"></a>

**表 3**  参数说明

<a name="table9773163143319"></a>
<table><thead align="left"><tr id="row57739315330"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="p1777313115338"><a name="p1777313115338"></a><a name="p1777313115338"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.2"><p id="p16773123153311"><a name="p16773123153311"></a><a name="p16773123153311"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="p1077314311338"><a name="p1077314311338"></a><a name="p1077314311338"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.44554455445545%" id="mcps1.2.5.1.4"><p id="p57731931163310"><a name="p57731931163310"></a><a name="p57731931163310"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row2773153115338"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p207735314331"><a name="p207735314331"></a><a name="p207735314331"></a>swagger</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p9773153173314"><a name="p9773153173314"></a><a name="p9773153173314"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p4773123193314"><a name="p4773123193314"></a><a name="p4773123193314"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p67736311339"><a name="p67736311339"></a><a name="p67736311339"></a>固定值2.0</p>
</td>
</tr>
<tr id="row37747316331"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p8774193183317"><a name="p8774193183317"></a><a name="p8774193183317"></a>info</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p1377493113317"><a name="p1377493113317"></a><a name="p1377493113317"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p6774133117331"><a name="p6774133117331"></a><a name="p6774133117331"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p147741931103310"><a name="p147741931103310"></a><a name="p147741931103310"></a>参考<a href="#table17777531133316">表4</a></p>
</td>
</tr>
<tr id="row12774431113317"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p277493110331"><a name="p277493110331"></a><a name="p277493110331"></a>paths</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p177741231183318"><a name="p177741231183318"></a><a name="p177741231183318"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p1977483118331"><a name="p1977483118331"></a><a name="p1977483118331"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p2774183118334"><a name="p2774183118334"></a><a name="p2774183118334"></a>参考<a href="#table4779143143311">表 paths参数说明</a></p>
</td>
</tr>
<tr id="row1775193115334"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p13775103110336"><a name="p13775103110336"></a><a name="p13775103110336"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p377573120333"><a name="p377573120333"></a><a name="p377573120333"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p19775153113336"><a name="p19775153113336"></a><a name="p19775153113336"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p77751231153315"><a name="p77751231153315"></a><a name="p77751231153315"></a>公用响应定义，可以被引用在{method}的操作中，参考<a href="#table1179216319331">表9</a></p>
</td>
</tr>
<tr id="row0775183113319"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p177519318331"><a name="p177519318331"></a><a name="p177519318331"></a>securityDefinitions</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p1377519316332"><a name="p1377519316332"></a><a name="p1377519316332"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p197751031193315"><a name="p197751031193315"></a><a name="p197751031193315"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p9775183103319"><a name="p9775183103319"></a><a name="p9775183103319"></a>定义鉴权方式，参考<a href="#table8801831163318">表13</a></p>
</td>
</tr>
<tr id="row15840124816259"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p1884194822510"><a name="p1884194822510"></a><a name="p1884194822510"></a>x-apigateway-access-controls</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p13841148172510"><a name="p13841148172510"></a><a name="p13841148172510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p1784154813256"><a name="p1784154813256"></a><a name="p1784154813256"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p384164813253"><a name="p384164813253"></a><a name="p384164813253"></a>访问控制信息，参考<a href="#table2090754816252">表 x-apigateway-access-controls参数说明</a></p>
</td>
</tr>
<tr id="row684144814253"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p98411348102518"><a name="p98411348102518"></a><a name="p98411348102518"></a>x-apigateway-ratelimits</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.2 "><p id="p13841134852518"><a name="p13841134852518"></a><a name="p13841134852518"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p178411048152517"><a name="p178411048152517"></a><a name="p178411048152517"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.44554455445545%" headers="mcps1.2.5.1.4 "><p id="p28411648202513"><a name="p28411648202513"></a><a name="p28411648202513"></a>流量空时信息，参考<a href="#table18913124872513">表 x-apigateway-ratelimits参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 4**  info参数说明

<a name="table17777531133316"></a>
<table><thead align="left"><tr id="row677763153314"><th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.1"><p id="p577710314330"><a name="p577710314330"></a><a name="p577710314330"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="p6777531153318"><a name="p6777531153318"></a><a name="p6777531153318"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.3"><p id="p777713120337"><a name="p777713120337"></a><a name="p777713120337"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="p3777133113314"><a name="p3777133113314"></a><a name="p3777133113314"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1777814313334"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p07787319338"><a name="p07787319338"></a><a name="p07787319338"></a>title</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p2778193118331"><a name="p2778193118331"></a><a name="p2778193118331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p13778183193320"><a name="p13778183193320"></a><a name="p13778183193320"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p12778123119338"><a name="p12778123119338"></a><a name="p12778123119338"></a>API分组名称，导入到已有分组时不生效</p>
</td>
</tr>
<tr id="row20778153110339"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p177812316339"><a name="p177812316339"></a><a name="p177812316339"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1177813318338"><a name="p1177813318338"></a><a name="p1177813318338"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p15778153118331"><a name="p15778153118331"></a><a name="p15778153118331"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p1778123113337"><a name="p1778123113337"></a><a name="p1778123113337"></a>版本号，用户输入自定义版本号或者使用默认的当前时间</p>
</td>
</tr>
<tr id="row077853163317"><td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.1 "><p id="p8778113183311"><a name="p8778113183311"></a><a name="p8778113183311"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p8778431183314"><a name="p8778431183314"></a><a name="p8778431183314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.3 "><p id="p197782315338"><a name="p197782315338"></a><a name="p197782315338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p177791731183310"><a name="p177791731183310"></a><a name="p177791731183310"></a>分组描述信息</p>
</td>
</tr>
</tbody>
</table>

**表 5**  paths参数说明

<a name="table4779143143311"></a>
<table><thead align="left"><tr id="row1977953115332"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p07801431173316"><a name="p07801431173316"></a><a name="p07801431173316"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.2"><p id="p4780531143317"><a name="p4780531143317"></a><a name="p4780531143317"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.3"><p id="p978093183319"><a name="p978093183319"></a><a name="p978093183319"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="p17780163110337"><a name="p17780163110337"></a><a name="p17780163110337"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1278010312334"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2078003123313"><a name="p2078003123313"></a><a name="p2078003123313"></a>uri</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.2 "><p id="p1478019313332"><a name="p1478019313332"></a><a name="p1478019313332"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.3 "><p id="p5780153153312"><a name="p5780153153312"></a><a name="p5780153153312"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1578083193319"><a name="p1578083193319"></a><a name="p1578083193319"></a>API访问地址，参考<a href="#table87808315333">表6</a></p>
</td>
</tr>
</tbody>
</table>

**表 6**  uri参数说明

<a name="table87808315333"></a>
<table><thead align="left"><tr id="row5781163103316"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1781131163318"><a name="p1781131163318"></a><a name="p1781131163318"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p77811031173316"><a name="p77811031173316"></a><a name="p77811031173316"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p11781143193313"><a name="p11781143193313"></a><a name="p11781143193313"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="p778111311338"><a name="p778111311338"></a><a name="p778111311338"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row167811731183313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p19781203143311"><a name="p19781203143311"></a><a name="p19781203143311"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p5781831123315"><a name="p5781831123315"></a><a name="p5781831123315"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p9781133113333"><a name="p9781133113333"></a><a name="p9781133113333"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1878113112334"><a name="p1878113112334"></a><a name="p1878113112334"></a>API访问方法，参考<a href="#table1178111318331">表7</a></p>
</td>
</tr>
</tbody>
</table>

**表 7**  method参数说明

<a name="table1178111318331"></a>
<table><thead align="left"><tr id="row678213153314"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p178293118331"><a name="p178293118331"></a><a name="p178293118331"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p107821531103315"><a name="p107821531103315"></a><a name="p107821531103315"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p7782153120336"><a name="p7782153120336"></a><a name="p7782153120336"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="55.00000000000001%" id="mcps1.2.5.1.4"><p id="p87821031153311"><a name="p87821031153311"></a><a name="p87821031153311"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row12849144802517"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p08503484253"><a name="p08503484253"></a><a name="p08503484253"></a>operationId</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p0850204842510"><a name="p0850204842510"></a><a name="p0850204842510"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p085094842516"><a name="p085094842516"></a><a name="p085094842516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p485094872511"><a name="p485094872511"></a><a name="p485094872511"></a>API的名称</p>
</td>
</tr>
<tr id="row37829315332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p3783931103316"><a name="p3783931103316"></a><a name="p3783931103316"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p157839316331"><a name="p157839316331"></a><a name="p157839316331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1678373143312"><a name="p1678373143312"></a><a name="p1678373143312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1178393114337"><a name="p1178393114337"></a><a name="p1178393114337"></a>API的描述信息</p>
</td>
</tr>
<tr id="row078320314332"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2078310314338"><a name="p2078310314338"></a><a name="p2078310314338"></a>schemes</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p578323193319"><a name="p578323193319"></a><a name="p578323193319"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p878312318330"><a name="p878312318330"></a><a name="p878312318330"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p197831317339"><a name="p197831317339"></a><a name="p197831317339"></a>API的请求协议对象数组定义，支持http、https</p>
</td>
</tr>
<tr id="row1968814364917"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1533713935518"><a name="p1533713935518"></a><a name="p1533713935518"></a>tags</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p2337039165520"><a name="p2337039165520"></a><a name="p2337039165520"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p7837754145511"><a name="p7837754145511"></a><a name="p7837754145511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1337133918551"><a name="p1337133918551"></a><a name="p1337133918551"></a>API标签对象数组定义</p>
</td>
</tr>
<tr id="row07831431123313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p127831531103319"><a name="p127831531103319"></a><a name="p127831531103319"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p4783203173316"><a name="p4783203173316"></a><a name="p4783203173316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p87831631133312"><a name="p87831631133312"></a><a name="p87831631133312"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p27833313337"><a name="p27833313337"></a><a name="p27833313337"></a>请求参数对象数组定义，参考<a href="#table87881431123317">表 前端parameters参数说明</a></p>
</td>
</tr>
<tr id="row1078313110336"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p177846311333"><a name="p177846311333"></a><a name="p177846311333"></a>responses</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p8784031193315"><a name="p8784031193315"></a><a name="p8784031193315"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p2784143113334"><a name="p2784143113334"></a><a name="p2784143113334"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p11784131123317"><a name="p11784131123317"></a><a name="p11784131123317"></a>响应定义，参考<a href="#table1179216319331">表9</a></p>
</td>
</tr>
<tr id="row6852144810252"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p15852648132516"><a name="p15852648132516"></a><a name="p15852648132516"></a>security</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p985254812519"><a name="p985254812519"></a><a name="p985254812519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p20852948192520"><a name="p20852948192520"></a><a name="p20852948192520"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1185244832513"><a name="p1185244832513"></a><a name="p1185244832513"></a>API的认证类型对象数组定义，参考<a href="#table986594862513">表 security参数说明</a></p>
</td>
</tr>
<tr id="row185314892514"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p8853748182515"><a name="p8853748182515"></a><a name="p8853748182515"></a>x-apigateway-access-control</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p18853114818258"><a name="p18853114818258"></a><a name="p18853114818258"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p885316488254"><a name="p885316488254"></a><a name="p885316488254"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p885318487254"><a name="p885318487254"></a><a name="p885318487254"></a>API绑定的访问控制对象数组定义</p>
</td>
</tr>
<tr id="row11853104814258"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1385324810256"><a name="p1385324810256"></a><a name="p1385324810256"></a>x-apigateway-backend</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p7853248172514"><a name="p7853248172514"></a><a name="p7853248172514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p6853184852511"><a name="p6853184852511"></a><a name="p6853184852511"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p4853174816257"><a name="p4853174816257"></a><a name="p4853174816257"></a>API的后端信息，参考<a href="#table387619483252">表 x-apigateway-backend参数说明</a></p>
</td>
</tr>
<tr id="row1685384815256"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1485334813258"><a name="p1485334813258"></a><a name="p1485334813258"></a>x-apigateway-backend-policies</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p685464852511"><a name="p685464852511"></a><a name="p685464852511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p785419483251"><a name="p785419483251"></a><a name="p785419483251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p18541148122518"><a name="p18541148122518"></a><a name="p18541148122518"></a>API的策略后端信息，参考<a href="#table1988034862512">表 x-apigateway-backend-policies参数说明</a></p>
</td>
</tr>
<tr id="row6854164802518"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1285414488259"><a name="p1285414488259"></a><a name="p1285414488259"></a>x-apigateway-cors</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p13854104814259"><a name="p13854104814259"></a><a name="p13854104814259"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p198541648152518"><a name="p198541648152518"></a><a name="p198541648152518"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p1985410480253"><a name="p1985410480253"></a><a name="p1985410480253"></a>是否支持跨域</p>
</td>
</tr>
<tr id="row16854154817253"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p2085454816256"><a name="p2085454816256"></a><a name="p2085454816256"></a>x-apigateway-match-mode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p98551248162511"><a name="p98551248162511"></a><a name="p98551248162511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p14855948102517"><a name="p14855948102517"></a><a name="p14855948102517"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p18551948122513"><a name="p18551948122513"></a><a name="p18551948122513"></a>API的匹配方式</p>
</td>
</tr>
<tr id="row11855164832513"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1885514480253"><a name="p1885514480253"></a><a name="p1885514480253"></a>x-apigateway-ratelimit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p5855648142511"><a name="p5855648142511"></a><a name="p5855648142511"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p885504815254"><a name="p885504815254"></a><a name="p885504815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p15855124810253"><a name="p15855124810253"></a><a name="p15855124810253"></a>API绑定的流量控制名称</p>
</td>
</tr>
<tr id="row885554810255"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p5855144872514"><a name="p5855144872514"></a><a name="p5855144872514"></a>x-apigateway-request-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p4855144822512"><a name="p4855144822512"></a><a name="p4855144822512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p108550488256"><a name="p108550488256"></a><a name="p108550488256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="55.00000000000001%" headers="mcps1.2.5.1.4 "><p id="p28561348162511"><a name="p28561348162511"></a><a name="p28561348162511"></a>API的类型</p>
</td>
</tr>
</tbody>
</table>

**表 8**  前端parameters参数说明

<a name="table87881431123317"></a>
<table><thead align="left"><tr id="row178813319331"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="p1178853117333"><a name="p1178853117333"></a><a name="p1178853117333"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="p178823116333"><a name="p178823116333"></a><a name="p178823116333"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="p27881931113310"><a name="p27881931113310"></a><a name="p27881931113310"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="p12788133113333"><a name="p12788133113333"></a><a name="p12788133113333"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row16788133123313"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p19788331183319"><a name="p19788331183319"></a><a name="p19788331183319"></a>maximum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1278823120331"><a name="p1278823120331"></a><a name="p1278823120331"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1578853103319"><a name="p1578853103319"></a><a name="p1578853103319"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p20789203117333"><a name="p20789203117333"></a><a name="p20789203117333"></a>参数为数值类型时，最大参数值</p>
</td>
</tr>
<tr id="row878903118339"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p14789103114338"><a name="p14789103114338"></a><a name="p14789103114338"></a>minimum</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p117891531183316"><a name="p117891531183316"></a><a name="p117891531183316"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1978911312333"><a name="p1978911312333"></a><a name="p1978911312333"></a>Float</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p57891331193316"><a name="p57891331193316"></a><a name="p57891331193316"></a>参数为数值类型时，最小参数值</p>
</td>
</tr>
<tr id="row0789193118332"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p10789163183315"><a name="p10789163183315"></a><a name="p10789163183315"></a>maxLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p117891316330"><a name="p117891316330"></a><a name="p117891316330"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p17789143117337"><a name="p17789143117337"></a><a name="p17789143117337"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p187891931143313"><a name="p187891931143313"></a><a name="p187891931143313"></a>参数为字符串类型时，参数的最大长度</p>
</td>
</tr>
<tr id="row177892031203312"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p37899310336"><a name="p37899310336"></a><a name="p37899310336"></a>minLength</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p7789131103317"><a name="p7789131103317"></a><a name="p7789131103317"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1578912315336"><a name="p1578912315336"></a><a name="p1578912315336"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p15789153115331"><a name="p15789153115331"></a><a name="p15789153115331"></a>参数为字符串类型时，参数的最小长度</p>
</td>
</tr>
<tr id="row9790143133311"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p979083110332"><a name="p979083110332"></a><a name="p979083110332"></a>pattern</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p879023110332"><a name="p879023110332"></a><a name="p879023110332"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p87901316339"><a name="p87901316339"></a><a name="p87901316339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p127901319332"><a name="p127901319332"></a><a name="p127901319332"></a>参数值为正则匹配表达式</p>
</td>
</tr>
<tr id="row07901831143311"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p379073113311"><a name="p379073113311"></a><a name="p379073113311"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p1790133153313"><a name="p1790133153313"></a><a name="p1790133153313"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p20790123110339"><a name="p20790123110339"></a><a name="p20790123110339"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p1279013133314"><a name="p1279013133314"></a><a name="p1279013133314"></a>参数类型</p>
</td>
</tr>
<tr id="row11790331123320"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p379018310339"><a name="p379018310339"></a><a name="p379018310339"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p2790331153310"><a name="p2790331153310"></a><a name="p2790331153310"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1779003113338"><a name="p1779003113338"></a><a name="p1779003113338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p179023118333"><a name="p179023118333"></a><a name="p179023118333"></a>参数默认值</p>
</td>
</tr>
<tr id="row18790173123319"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p779073111339"><a name="p779073111339"></a><a name="p779073111339"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p7791113183311"><a name="p7791113183311"></a><a name="p7791113183311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p2791123173315"><a name="p2791123173315"></a><a name="p2791123173315"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p67911731183313"><a name="p67911731183313"></a><a name="p67911731183313"></a>参数描述信息</p>
</td>
</tr>
<tr id="row10791231183316"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p1479123117331"><a name="p1479123117331"></a><a name="p1479123117331"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p137911631153311"><a name="p137911631153311"></a><a name="p137911631153311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p97911331173318"><a name="p97911331173318"></a><a name="p97911331173318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p979112312330"><a name="p979112312330"></a><a name="p979112312330"></a>参数名称</p>
</td>
</tr>
<tr id="row1779173173314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p1579153110335"><a name="p1579153110335"></a><a name="p1579153110335"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p97914312337"><a name="p97914312337"></a><a name="p97914312337"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p12791173114338"><a name="p12791173114338"></a><a name="p12791173114338"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p20791331103320"><a name="p20791331103320"></a><a name="p20791331103320"></a>参数位置，支持path、header、query、formData、body</p>
</td>
</tr>
<tr id="row9791113163312"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p177922031143318"><a name="p177922031143318"></a><a name="p177922031143318"></a>required</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p9792831153314"><a name="p9792831153314"></a><a name="p9792831153314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p679293111333"><a name="p679293111333"></a><a name="p679293111333"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p1792173123313"><a name="p1792173123313"></a><a name="p1792173123313"></a>参数是否必需，参数位置为path时必需</p>
</td>
</tr>
</tbody>
</table>

**表 9**  responses参数说明

<a name="table1179216319331"></a>
<table><thead align="left"><tr id="row8792731153315"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1779373116337"><a name="p1779373116337"></a><a name="p1779373116337"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p16793123114337"><a name="p16793123114337"></a><a name="p16793123114337"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p979313111338"><a name="p979313111338"></a><a name="p979313111338"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p157931310332"><a name="p157931310332"></a><a name="p157931310332"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row079333183320"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p167931931183315"><a name="p167931931183315"></a><a name="p167931931183315"></a>default</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p67931731123311"><a name="p67931731123311"></a><a name="p67931731123311"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p779311315332"><a name="p779311315332"></a><a name="p779311315332"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1079363115336"><a name="p1079363115336"></a><a name="p1079363115336"></a>缺省响应，描述未定义的响应码</p>
</td>
</tr>
<tr id="row1779315314339"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p77931031143318"><a name="p77931031143318"></a><a name="p77931031143318"></a>status_code</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p079412319339"><a name="p079412319339"></a><a name="p079412319339"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p137941731133315"><a name="p137941731133315"></a><a name="p137941731133315"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p0794331153315"><a name="p0794331153315"></a><a name="p0794331153315"></a>响应状态码，值为响应对象，参考<a href="#table107974312335">表11</a></p>
</td>
</tr>
<tr id="row1774720508918"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p774812501894"><a name="p774812501894"></a><a name="p774812501894"></a>x-apigateway-result-failure-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p474815020916"><a name="p474815020916"></a><a name="p474815020916"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p11749105017914"><a name="p11749105017914"></a><a name="p11749105017914"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p14749750398"><a name="p14749750398"></a><a name="p14749750398"></a>失败返回示例，描述API的异常返回信息</p>
</td>
</tr>
<tr id="row71795541897"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p1117913541917"><a name="p1117913541917"></a><a name="p1117913541917"></a>x-apigateway-result-normal-sample</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p517914541191"><a name="p517914541191"></a><a name="p517914541191"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p171791554493"><a name="p171791554493"></a><a name="p171791554493"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p111791154598"><a name="p111791154598"></a><a name="p111791154598"></a>正常响应示例，描述API的正常返回信息</p>
</td>
</tr>
</tbody>
</table>

**表 10**  security参数说明

<a name="table986594862513"></a>
<table><thead align="left"><tr id="row086674852515"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="p986654810257"><a name="p986654810257"></a><a name="p986654810257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="12.871287128712872%" id="mcps1.2.5.1.2"><p id="p986624819250"><a name="p986624819250"></a><a name="p986624819250"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="p188661348112516"><a name="p188661348112516"></a><a name="p188661348112516"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54.45544554455446%" id="mcps1.2.5.1.4"><p id="p14866248132510"><a name="p14866248132510"></a><a name="p14866248132510"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row17866114810256"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p696102820583"><a name="p696102820583"></a><a name="p696102820583"></a>apig-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="12.871287128712872%" headers="mcps1.2.5.1.2 "><p id="p7961172855819"><a name="p7961172855819"></a><a name="p7961172855819"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1996117280588"><a name="p1996117280588"></a><a name="p1996117280588"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54.45544554455446%" headers="mcps1.2.5.1.4 "><p id="p696252813588"><a name="p696252813588"></a><a name="p696252813588"></a>API的认证类型对象数组定义，为空数组</p>
<p id="p6722101419557"><a name="p6722101419557"></a><a name="p6722101419557"></a>apig-auth-type支持：</p>
<a name="ul3401225145518"></a><a name="ul3401225145518"></a><ul id="ul3401225145518"><li>APP认证： apig-auth-app</li><li>IAM认证：apig-auth-iam</li><li>NONE：不填写</li></ul>
</td>
</tr>
</tbody>
</table>

**表 11**  status code参数说明

<a name="table107974312335"></a>
<table><thead align="left"><tr id="row1798831113311"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p11798193120338"><a name="p11798193120338"></a><a name="p11798193120338"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p19798163113335"><a name="p19798163113335"></a><a name="p19798163113335"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p479813115331"><a name="p479813115331"></a><a name="p479813115331"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p18798183116337"><a name="p18798183116337"></a><a name="p18798183116337"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row67981311335"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p17798173103315"><a name="p17798173103315"></a><a name="p17798173103315"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p137981131183317"><a name="p137981131183317"></a><a name="p137981131183317"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p17798431113320"><a name="p17798431113320"></a><a name="p17798431113320"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1379983114336"><a name="p1379983114336"></a><a name="p1379983114336"></a>响应描述信息</p>
</td>
</tr>
<tr id="row979933133313"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p20799143193310"><a name="p20799143193310"></a><a name="p20799143193310"></a>schema</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p1179953153314"><a name="p1179953153314"></a><a name="p1179953153314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p6799113103314"><a name="p6799113103314"></a><a name="p6799113103314"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p27991431193317"><a name="p27991431193317"></a><a name="p27991431193317"></a>响应正文定义，参考<a href="#table47999312330">表12</a></p>
</td>
</tr>
</tbody>
</table>

**表 12**  schema参数说明

<a name="table47999312330"></a>
<table><thead align="left"><tr id="row5800143114331"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.5.1.1"><p id="p1280083113332"><a name="p1280083113332"></a><a name="p1280083113332"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="14.000000000000002%" id="mcps1.2.5.1.2"><p id="p148001231173318"><a name="p148001231173318"></a><a name="p148001231173318"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p18800123153320"><a name="p18800123153320"></a><a name="p18800123153320"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p13800113113310"><a name="p13800113113310"></a><a name="p13800113113310"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row18800173163318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p158009313336"><a name="p158009313336"></a><a name="p158009313336"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p980016317332"><a name="p980016317332"></a><a name="p980016317332"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1800531193312"><a name="p1800531193312"></a><a name="p1800531193312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p2800331193316"><a name="p2800331193316"></a><a name="p2800331193316"></a>BODY体描述</p>
</td>
</tr>
<tr id="row19800131173318"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.5.1.1 "><p id="p18800133173314"><a name="p18800133173314"></a><a name="p18800133173314"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="14.000000000000002%" headers="mcps1.2.5.1.2 "><p id="p11800163153314"><a name="p11800163153314"></a><a name="p11800163153314"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p8801133113311"><a name="p8801133113311"></a><a name="p8801133113311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p980119311336"><a name="p980119311336"></a><a name="p980119311336"></a>BODY体类型：FORM/STREAM（表单/字节流）</p>
</td>
</tr>
</tbody>
</table>

**表 13**  securityDefinitions参数说明

<a name="table8801831163318"></a>
<table><thead align="left"><tr id="row14801193113339"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.5.1.1"><p id="p58010316337"><a name="p58010316337"></a><a name="p58010316337"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.2"><p id="p12801123110331"><a name="p12801123110331"></a><a name="p12801123110331"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="11.881188118811881%" id="mcps1.2.5.1.3"><p id="p5801133113331"><a name="p5801133113331"></a><a name="p5801133113331"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="53.46534653465347%" id="mcps1.2.5.1.4"><p id="p20801431193316"><a name="p20801431193316"></a><a name="p20801431193316"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row188011831183315"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.5.1.1 "><p id="p88012031193317"><a name="p88012031193317"></a><a name="p88012031193317"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.2 "><p id="p280153111337"><a name="p280153111337"></a><a name="p280153111337"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="11.881188118811881%" headers="mcps1.2.5.1.3 "><p id="p1380133119339"><a name="p1380133119339"></a><a name="p1380133119339"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="53.46534653465347%" headers="mcps1.2.5.1.4 "><p id="p080211318331"><a name="p080211318331"></a><a name="p080211318331"></a>自定义鉴权方式名称，参考<a href="#table12802183116332">表14</a></p>
</td>
</tr>
</tbody>
</table>

**表 14**  name参数说明

<a name="table12802183116332"></a>
<table><thead align="left"><tr id="row580253113313"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p13802331103315"><a name="p13802331103315"></a><a name="p13802331103315"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1802133118337"><a name="p1802133118337"></a><a name="p1802133118337"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p2080263113332"><a name="p2080263113332"></a><a name="p2080263113332"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p1580263113332"><a name="p1580263113332"></a><a name="p1580263113332"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row13802193114334"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p18802133120331"><a name="p18802133120331"></a><a name="p18802133120331"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1802203115333"><a name="p1802203115333"></a><a name="p1802203115333"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1580263113333"><a name="p1580263113333"></a><a name="p1580263113333"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p128031531183313"><a name="p128031531183313"></a><a name="p128031531183313"></a>鉴权类型，支持apiKey</p>
</td>
</tr>
<tr id="row2080393143310"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1880373133318"><a name="p1880373133318"></a><a name="p1880373133318"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p18031331183311"><a name="p18031331183311"></a><a name="p18031331183311"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p8803123193312"><a name="p8803123193312"></a><a name="p8803123193312"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p9803143113331"><a name="p9803143113331"></a><a name="p9803143113331"></a>apiKey参数名称</p>
</td>
</tr>
<tr id="row5803731203310"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1380333114333"><a name="p1380333114333"></a><a name="p1380333114333"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p5803631143310"><a name="p5803631143310"></a><a name="p5803631143310"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p4803103117336"><a name="p4803103117336"></a><a name="p4803103117336"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p108031731183316"><a name="p108031731183316"></a><a name="p108031731183316"></a>apiKey参数位置</p>
</td>
</tr>
<tr id="row118031231163320"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p14803183117335"><a name="p14803183117335"></a><a name="p14803183117335"></a>x-apigateway-auth-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p48031531153311"><a name="p48031531153311"></a><a name="p48031531153311"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p2080313173313"><a name="p2080313173313"></a><a name="p2080313173313"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p10804193119337"><a name="p10804193119337"></a><a name="p10804193119337"></a>扩展鉴权类型，基于apiKey鉴权方式的扩展，网关自定义的鉴权方式，支持AppSigv1、IAM、IAM_NONE</p>
</td>
</tr>
</tbody>
</table>

**表 15**  x-apigateway-backend参数说明

<a name="table387619483252"></a>
<table><thead align="left"><tr id="row1487734812520"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p487734814254"><a name="p487734814254"></a><a name="p487734814254"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p58771548122516"><a name="p58771548122516"></a><a name="p58771548122516"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p287774812511"><a name="p287774812511"></a><a name="p287774812511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p13877134815251"><a name="p13877134815251"></a><a name="p13877134815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row10877114822512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p2878144892516"><a name="p2878144892516"></a><a name="p2878144892516"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p15878648182515"><a name="p15878648182515"></a><a name="p15878648182515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p587811480258"><a name="p587811480258"></a><a name="p587811480258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p2878134802519"><a name="p2878134802519"></a><a name="p2878134802519"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="row8878174811255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p187864862516"><a name="p187864862516"></a><a name="p187864862516"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p387834820252"><a name="p387834820252"></a><a name="p387834820252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p0878848142512"><a name="p0878848142512"></a><a name="p0878848142512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1887854802516"><a name="p1887854802516"></a><a name="p1887854802516"></a>后端参数对象数组定义，参考<a href="#table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="row1387834892518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1587934817256"><a name="p1587934817256"></a><a name="p1587934817256"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p587924822511"><a name="p587924822511"></a><a name="p587924822511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p20879124802513"><a name="p20879124802513"></a><a name="p20879124802513"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p19879134862517"><a name="p19879134862517"></a><a name="p19879134862517"></a>API后端定义</p>
<p id="p9879144815251"><a name="p9879144815251"></a><a name="p9879144815251"></a>backend_define支持：</p>
<a name="ul587916489258"></a><a name="ul587916489258"></a><ul id="ul587916489258"><li>httpEndpoints，参考<a href="#table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
</tbody>
</table>

**表 16**  x-apigateway-backend-policies参数说明

<a name="table1988034862512"></a>
<table><thead align="left"><tr id="row788004814256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p148801248112517"><a name="p148801248112517"></a><a name="p148801248112517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p28801048112514"><a name="p28801048112514"></a><a name="p28801048112514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p5880164872513"><a name="p5880164872513"></a><a name="p5880164872513"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p8881948132519"><a name="p8881948132519"></a><a name="p8881948132519"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row118811748112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p688117485256"><a name="p688117485256"></a><a name="p688117485256"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p688164822510"><a name="p688164822510"></a><a name="p688164822510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p178819481257"><a name="p178819481257"></a><a name="p178819481257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p13881448102510"><a name="p13881448102510"></a><a name="p13881448102510"></a>API后端类型，支持HTTP、HTTP-VPC、FUNCTION、MOCK</p>
</td>
</tr>
<tr id="row9881134862515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p19881204822515"><a name="p19881204822515"></a><a name="p19881204822515"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1888114862515"><a name="p1888114862515"></a><a name="p1888114862515"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p78817484250"><a name="p78817484250"></a><a name="p78817484250"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1588144814252"><a name="p1588144814252"></a><a name="p1588144814252"></a>后端策略名称</p>
</td>
</tr>
<tr id="row588184817258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p2882124882517"><a name="p2882124882517"></a><a name="p2882124882517"></a>parameters</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p988244811251"><a name="p988244811251"></a><a name="p988244811251"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p5882248152519"><a name="p5882248152519"></a><a name="p5882248152519"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p188218488257"><a name="p188218488257"></a><a name="p188218488257"></a>后端参数对象数组定义，参考<a href="#table14884114882511">表 后端parameters参数说明</a></p>
</td>
</tr>
<tr id="row1188204822510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p19882184892513"><a name="p19882184892513"></a><a name="p19882184892513"></a>backend_define</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p6882104862512"><a name="p6882104862512"></a><a name="p6882104862512"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p138821548172512"><a name="p138821548172512"></a><a name="p138821548172512"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p15882164816258"><a name="p15882164816258"></a><a name="p15882164816258"></a>API后端定义</p>
<p id="p188214481259"><a name="p188214481259"></a><a name="p188214481259"></a>backend_define支持：</p>
<a name="ul0883104814256"></a><a name="ul0883104814256"></a><ul id="ul0883104814256"><li>httpEndpoints，参考<a href="#table1788894822518">表 后端httpEndpoints参数说明</a></li><li>httpVpcEndpoints，参考<a href="#table1089314812254">表 后端httpVpcEndpoints参数说明</a></li><li>functionEndpoints，参考<a href="#table18971648202512">表 后端functionEndpoints参数说明</a></li><li>mockEndpoints，参考<a href="#table1790184862513">表 后端mockEndpoints参数说明</a></li></ul>
</td>
</tr>
<tr id="row48838483257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p18883948172520"><a name="p18883948172520"></a><a name="p18883948172520"></a>conditions</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p6883184852518"><a name="p6883184852518"></a><a name="p6883184852518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p68846483259"><a name="p68846483259"></a><a name="p68846483259"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p988404813253"><a name="p988404813253"></a><a name="p988404813253"></a>策略条件对象数组定义，参考<a href="#table1790444832520">表 conditions参数说明</a></p>
</td>
</tr>
<tr id="row8601019134513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p7826184743414"><a name="p7826184743414"></a><a name="p7826184743414"></a>effectMode</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p15826134712343"><a name="p15826134712343"></a><a name="p15826134712343"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p58262047113410"><a name="p58262047113410"></a><a name="p58262047113410"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p17355191291320"><a name="p17355191291320"></a><a name="p17355191291320"></a>关联的策略组合模式，支持ANY、ALL</p>
</td>
</tr>
</tbody>
</table>

**表 17**  后端parameters参数说明

<a name="table14884114882511"></a>
<table><thead align="left"><tr id="row1088574822512"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p88856489251"><a name="p88856489251"></a><a name="p88856489251"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p18885048132510"><a name="p18885048132510"></a><a name="p18885048132510"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p19885124810250"><a name="p19885124810250"></a><a name="p19885124810250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p188851448172515"><a name="p188851448172515"></a><a name="p188851448172515"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row138861748112511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p788674832520"><a name="p788674832520"></a><a name="p788674832520"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p148868484256"><a name="p148868484256"></a><a name="p148868484256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1688664812515"><a name="p1688664812515"></a><a name="p1688664812515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p14886948102519"><a name="p14886948102519"></a><a name="p14886948102519"></a>参数名称，由字母、数字、下划线、连线、点组成，以字母开头，最长32字节</p>
<p id="p1988624813251"><a name="p1988624813251"></a><a name="p1988624813251"></a>header位置的参数名称不区分大小写</p>
</td>
</tr>
<tr id="row388674862513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1888620480254"><a name="p1888620480254"></a><a name="p1888620480254"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p98861548152515"><a name="p98861548152515"></a><a name="p98861548152515"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p0886174810255"><a name="p0886174810255"></a><a name="p0886174810255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p19886748182513"><a name="p19886748182513"></a><a name="p19886748182513"></a>参数值，当参数来源为REQUEST时，值为请求参数名称</p>
</td>
</tr>
<tr id="row10886148132513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p13887134822517"><a name="p13887134822517"></a><a name="p13887134822517"></a>in</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1788764862518"><a name="p1788764862518"></a><a name="p1788764862518"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p18887164815251"><a name="p18887164815251"></a><a name="p18887164815251"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p8887174812258"><a name="p8887174812258"></a><a name="p8887174812258"></a>参数位置，支持header、query、path</p>
</td>
</tr>
<tr id="row788711486259"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p4887148182510"><a name="p4887148182510"></a><a name="p4887148182510"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1588714814252"><a name="p1588714814252"></a><a name="p1588714814252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p14887144815254"><a name="p14887144815254"></a><a name="p14887144815254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p9887104882515"><a name="p9887104882515"></a><a name="p9887104882515"></a>参数映射来源，支持REQUEST、CONSTANT</p>
</td>
</tr>
<tr id="row10888204816254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1988894882514"><a name="p1988894882514"></a><a name="p1988894882514"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1788864811250"><a name="p1788864811250"></a><a name="p1788864811250"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1288854812255"><a name="p1288854812255"></a><a name="p1288854812255"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p17888184822511"><a name="p17888184822511"></a><a name="p17888184822511"></a>参数含义描述</p>
</td>
</tr>
</tbody>
</table>

**表 18**  后端httpEndpoints参数说明

<a name="table1788894822518"></a>
<table><thead align="left"><tr id="row988984817253"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p18892048172520"><a name="p18892048172520"></a><a name="p18892048172520"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p12889204812514"><a name="p12889204812514"></a><a name="p12889204812514"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p168897485253"><a name="p168897485253"></a><a name="p168897485253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p4889144818251"><a name="p4889144818251"></a><a name="p4889144818251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7889164818257"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p158899481251"><a name="p158899481251"></a><a name="p158899481251"></a>address</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p19889134812514"><a name="p19889134812514"></a><a name="p19889134812514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p289054818257"><a name="p289054818257"></a><a name="p289054818257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p389044816256"><a name="p389044816256"></a><a name="p389044816256"></a>后端服务地址，格式为：&lt;域名或IP&gt;:[port]</p>
</td>
</tr>
<tr id="row13890348152517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p48902486252"><a name="p48902486252"></a><a name="p48902486252"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p198901048142519"><a name="p198901048142519"></a><a name="p198901048142519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p188901488253"><a name="p188901488253"></a><a name="p188901488253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p689013488253"><a name="p689013488253"></a><a name="p689013488253"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="row88902048112520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p13890134816252"><a name="p13890134816252"></a><a name="p13890134816252"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1089013489252"><a name="p1089013489252"></a><a name="p1089013489252"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p118901148172513"><a name="p118901148172513"></a><a name="p118901148172513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1989074812515"><a name="p1989074812515"></a><a name="p1989074812515"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="row7890104822514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p5890144882519"><a name="p5890144882519"></a><a name="p5890144882519"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p28911948182519"><a name="p28911948182519"></a><a name="p28911948182519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p68915482252"><a name="p68915482252"></a><a name="p68915482252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p188912048192510"><a name="p188912048192510"></a><a name="p188912048192510"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="row13891204812255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p58911948132514"><a name="p58911948132514"></a><a name="p58911948132514"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1389194814256"><a name="p1389194814256"></a><a name="p1389194814256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p889124812510"><a name="p889124812510"></a><a name="p889124812510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p189264813251"><a name="p189264813251"></a><a name="p189264813251"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="row7635433104612"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p191691539173611"><a name="p191691539173611"></a><a name="p191691539173611"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p916993963610"><a name="p916993963610"></a><a name="p916993963610"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p317073923616"><a name="p317073923616"></a><a name="p317073923616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p5170539163616"><a name="p5170539163616"></a><a name="p5170539163616"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 19**  后端httpVpcEndpoints参数说明

<a name="table1089314812254"></a>
<table><thead align="left"><tr id="row489354813256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p16893104820253"><a name="p16893104820253"></a><a name="p16893104820253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p14893548102518"><a name="p14893548102518"></a><a name="p14893548102518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p7893184852520"><a name="p7893184852520"></a><a name="p7893184852520"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p1789304832517"><a name="p1789304832517"></a><a name="p1789304832517"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row389304819258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p089494814258"><a name="p089494814258"></a><a name="p089494814258"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p188941948112519"><a name="p188941948112519"></a><a name="p188941948112519"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p2089418484250"><a name="p2089418484250"></a><a name="p2089418484250"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p78948486252"><a name="p78948486252"></a><a name="p78948486252"></a>VPC通道名称</p>
</td>
</tr>
<tr id="row19894104862518"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1089464852513"><a name="p1089464852513"></a><a name="p1089464852513"></a>scheme</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p138945480256"><a name="p138945480256"></a><a name="p138945480256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p989454862516"><a name="p989454862516"></a><a name="p989454862516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p2894248162512"><a name="p2894248162512"></a><a name="p2894248162512"></a>后端请求协议定义，支持http、https</p>
</td>
</tr>
<tr id="row1189484812512"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1589413486258"><a name="p1589413486258"></a><a name="p1589413486258"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p148947482254"><a name="p148947482254"></a><a name="p148947482254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1689418486254"><a name="p1689418486254"></a><a name="p1689418486254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p2089444817252"><a name="p2089444817252"></a><a name="p2089444817252"></a>后端请求方法，支持GET、POST、PUT、DELETE、HEAD、OPTIONS、PATCH、ANY</p>
</td>
</tr>
<tr id="row14895164817252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p11895194818252"><a name="p11895194818252"></a><a name="p11895194818252"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p28958484255"><a name="p28958484255"></a><a name="p28958484255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p13895448142512"><a name="p13895448142512"></a><a name="p13895448142512"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1189594813254"><a name="p1189594813254"></a><a name="p1189594813254"></a>后端请求路径，支持路径变量</p>
</td>
</tr>
<tr id="row1689594819251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p0895104832517"><a name="p0895104832517"></a><a name="p0895104832517"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p11895184862514"><a name="p11895184862514"></a><a name="p11895184862514"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p108951948172512"><a name="p108951948172512"></a><a name="p108951948172512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1289515487258"><a name="p1289515487258"></a><a name="p1289515487258"></a>后端请求超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="row18895184802511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p2895134820259"><a name="p2895134820259"></a><a name="p2895134820259"></a>host</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p9895144815256"><a name="p9895144815256"></a><a name="p9895144815256"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p168952482254"><a name="p168952482254"></a><a name="p168952482254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p9896194812253"><a name="p9896194812253"></a><a name="p9896194812253"></a>VPC通道代理主机</p>
</td>
</tr>
<tr id="row126916399464"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1205124114618"><a name="p1205124114618"></a><a name="p1205124114618"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p11205204144619"><a name="p11205204144619"></a><a name="p11205204144619"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p172056411467"><a name="p172056411467"></a><a name="p172056411467"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1520564144612"><a name="p1520564144612"></a><a name="p1520564144612"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 20**  后端functionEndpoints参数说明

<a name="table18971648202512"></a>
<table><thead align="left"><tr id="row14897184815257"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1389711486257"><a name="p1389711486257"></a><a name="p1389711486257"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1589724814251"><a name="p1589724814251"></a><a name="p1589724814251"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p589714815258"><a name="p589714815258"></a><a name="p589714815258"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p389818487257"><a name="p389818487257"></a><a name="p389818487257"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row58981348182516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1689814802516"><a name="p1689814802516"></a><a name="p1689814802516"></a>function-urn</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p7898114818255"><a name="p7898114818255"></a><a name="p7898114818255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p13898114852515"><a name="p13898114852515"></a><a name="p13898114852515"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p589884811259"><a name="p589884811259"></a><a name="p589884811259"></a>函数URN地址</p>
</td>
</tr>
<tr id="row128984488256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p12899648152514"><a name="p12899648152514"></a><a name="p12899648152514"></a>version</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1189984814258"><a name="p1189984814258"></a><a name="p1189984814258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p178991448162510"><a name="p178991448162510"></a><a name="p178991448162510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1899174832517"><a name="p1899174832517"></a><a name="p1899174832517"></a>函数版本</p>
</td>
</tr>
<tr id="row0899134815250"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p9899348162513"><a name="p9899348162513"></a><a name="p9899348162513"></a>invocation-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p289910485254"><a name="p289910485254"></a><a name="p289910485254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p18991348102516"><a name="p18991348102516"></a><a name="p18991348102516"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p189984818250"><a name="p189984818250"></a><a name="p189984818250"></a>函数调用类型，支持async、sync</p>
</td>
</tr>
<tr id="row28995482255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1290018487253"><a name="p1290018487253"></a><a name="p1290018487253"></a>timeout</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p490010489253"><a name="p490010489253"></a><a name="p490010489253"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p3900148112515"><a name="p3900148112515"></a><a name="p3900148112515"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p3900154822516"><a name="p3900154822516"></a><a name="p3900154822516"></a>函数超时时间，单位毫秒，缺省值为5000，取值范围为1 ~ 60000</p>
</td>
</tr>
<tr id="row4948164516468"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p417724714468"><a name="p417724714468"></a><a name="p417724714468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p20177147174614"><a name="p20177147174614"></a><a name="p20177147174614"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p2178184712466"><a name="p2178184712466"></a><a name="p2178184712466"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p131781547144613"><a name="p131781547144613"></a><a name="p131781547144613"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 21**  后端mockEndpoints参数说明

<a name="table1790184862513"></a>
<table><thead align="left"><tr id="row1901104812518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p6902348122511"><a name="p6902348122511"></a><a name="p6902348122511"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p690215486256"><a name="p690215486256"></a><a name="p690215486256"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p7902548202519"><a name="p7902548202519"></a><a name="p7902548202519"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p17902148202518"><a name="p17902148202518"></a><a name="p17902148202518"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row69021348202511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p14902448112512"><a name="p14902448112512"></a><a name="p14902448112512"></a>result-content</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p8902104816254"><a name="p8902104816254"></a><a name="p8902104816254"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p19903648122510"><a name="p19903648122510"></a><a name="p19903648122510"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p12903948172517"><a name="p12903948172517"></a><a name="p12903948172517"></a>MOCK返回结果</p>
</td>
</tr>
<tr id="row4433155454616"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1576125519468"><a name="p1576125519468"></a><a name="p1576125519468"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1857675514611"><a name="p1857675514611"></a><a name="p1857675514611"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p105761955174616"><a name="p105761955174616"></a><a name="p105761955174616"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p05768551462"><a name="p05768551462"></a><a name="p05768551462"></a>API后端描述</p>
</td>
</tr>
</tbody>
</table>

**表 22**  conditions参数说明

<a name="table1790444832520"></a>
<table><thead align="left"><tr id="row199040482254"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p169051248112512"><a name="p169051248112512"></a><a name="p169051248112512"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p590554862518"><a name="p590554862518"></a><a name="p590554862518"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p190564892511"><a name="p190564892511"></a><a name="p190564892511"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p4905194815251"><a name="p4905194815251"></a><a name="p4905194815251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row390544872514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p69056485258"><a name="p69056485258"></a><a name="p69056485258"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1290514820256"><a name="p1290514820256"></a><a name="p1290514820256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p190574819257"><a name="p190574819257"></a><a name="p190574819257"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1190554892513"><a name="p1190554892513"></a><a name="p1190554892513"></a>策略条件类型，支持equal、enum、pattern</p>
</td>
</tr>
<tr id="row590619487256"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p59061248132511"><a name="p59061248132511"></a><a name="p59061248132511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p159064483250"><a name="p159064483250"></a><a name="p159064483250"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1990644812258"><a name="p1990644812258"></a><a name="p1990644812258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1390694812519"><a name="p1390694812519"></a><a name="p1390694812519"></a>策略条件值</p>
</td>
</tr>
<tr id="row19906114813251"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p209067480258"><a name="p209067480258"></a><a name="p209067480258"></a>origin</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p14906184813256"><a name="p14906184813256"></a><a name="p14906184813256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1690694811252"><a name="p1690694811252"></a><a name="p1690694811252"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p159071748102517"><a name="p159071748102517"></a><a name="p159071748102517"></a>策略条件输入来源，支持source、request</p>
</td>
</tr>
<tr id="row16907248202516"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p6907648162519"><a name="p6907648162519"></a><a name="p6907648162519"></a>parameter</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1290714882519"><a name="p1290714882519"></a><a name="p1290714882519"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1690719487254"><a name="p1690719487254"></a><a name="p1690719487254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p149071484250"><a name="p149071484250"></a><a name="p149071484250"></a>策略条件输入来源为request时，请求入参的名称</p>
</td>
</tr>
</tbody>
</table>

**表 23**  x-apigateway-access-controls参数说明

<a name="table2090754816252"></a>
<table><thead align="left"><tr id="row179081748172515"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p209087484253"><a name="p209087484253"></a><a name="p209087484253"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1490854819254"><a name="p1490854819254"></a><a name="p1490854819254"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p09082048122514"><a name="p09082048122514"></a><a name="p09082048122514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p390944819252"><a name="p390944819252"></a><a name="p390944819252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row5909114852510"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p18909174811252"><a name="p18909174811252"></a><a name="p18909174811252"></a>acl_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p109091448202516"><a name="p109091448202516"></a><a name="p109091448202516"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p79098488251"><a name="p79098488251"></a><a name="p79098488251"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p11909114819251"><a name="p11909114819251"></a><a name="p11909114819251"></a>指定名称的访问控制策略，参考<a href="#table39092048142510">表 acl_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 24**  acl\_name参数说明

<a name="table39092048142510"></a>
<table><thead align="left"><tr id="row191014812256"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p991017483255"><a name="p991017483255"></a><a name="p991017483255"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p69108489253"><a name="p69108489253"></a><a name="p69108489253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p1591016486250"><a name="p1591016486250"></a><a name="p1591016486250"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p891110481252"><a name="p891110481252"></a><a name="p891110481252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49111048102517"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p129110482258"><a name="p129110482258"></a><a name="p129110482258"></a>acl-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p20911104892511"><a name="p20911104892511"></a><a name="p20911104892511"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p13911174815258"><a name="p13911174815258"></a><a name="p13911174815258"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p17911174882519"><a name="p17911174882519"></a><a name="p17911174882519"></a>访问控制行为，支持PERMIT、DENY</p>
</td>
</tr>
<tr id="row191154882520"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1191254820251"><a name="p1191254820251"></a><a name="p1191254820251"></a>entity-type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p169121248142514"><a name="p169121248142514"></a><a name="p169121248142514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p691294818254"><a name="p691294818254"></a><a name="p691294818254"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p8912948182515"><a name="p8912948182515"></a><a name="p8912948182515"></a>访问控制对象，支持IP、DOMAIN</p>
</td>
</tr>
<tr id="row1391211489258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p11912194872511"><a name="p11912194872511"></a><a name="p11912194872511"></a>value</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p3912248192514"><a name="p3912248192514"></a><a name="p3912248192514"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p6912848192513"><a name="p6912848192513"></a><a name="p6912848192513"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p9913194862512"><a name="p9913194862512"></a><a name="p9913194862512"></a>访问控制策略值，多个值以“,”间隔</p>
</td>
</tr>
</tbody>
</table>

**表 25**  x-apigateway-ratelimits参数说明

<a name="table18913124872513"></a>
<table><thead align="left"><tr id="row17913648192518"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p19913848152517"><a name="p19913848152517"></a><a name="p19913848152517"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p891324822519"><a name="p891324822519"></a><a name="p891324822519"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p591411483253"><a name="p591411483253"></a><a name="p591411483253"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p15914144811250"><a name="p15914144811250"></a><a name="p15914144811250"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1391424802514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p99141748112512"><a name="p99141748112512"></a><a name="p99141748112512"></a>throttle_name</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p149141489252"><a name="p149141489252"></a><a name="p149141489252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p99145487257"><a name="p99145487257"></a><a name="p99145487257"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p39151248192510"><a name="p39151248192510"></a><a name="p39151248192510"></a>指定名称的流控策略，参考<a href="#table179155483256">表 throttle_name参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 26**  throttle\_name参数说明

<a name="table179155483256"></a>
<table><thead align="left"><tr id="row3915114811258"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1191616488258"><a name="p1191616488258"></a><a name="p1191616488258"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p199164484253"><a name="p199164484253"></a><a name="p199164484253"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p29161648202514"><a name="p29161648202514"></a><a name="p29161648202514"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p89168486252"><a name="p89168486252"></a><a name="p89168486252"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row39169488253"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p119161548182514"><a name="p119161548182514"></a><a name="p119161548182514"></a>api-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1391664819255"><a name="p1391664819255"></a><a name="p1391664819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p19174485250"><a name="p19174485250"></a><a name="p19174485250"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p59171489257"><a name="p59171489257"></a><a name="p59171489257"></a>API访问次数限制</p>
</td>
</tr>
<tr id="row14917194852515"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p189171648112514"><a name="p189171648112514"></a><a name="p189171648112514"></a>user-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p18917174813252"><a name="p18917174813252"></a><a name="p18917174813252"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p199171348162512"><a name="p199171348162512"></a><a name="p199171348162512"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p4917448162510"><a name="p4917448162510"></a><a name="p4917448162510"></a>用户访问次数限制</p>
</td>
</tr>
<tr id="row129177484252"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p6918104872519"><a name="p6918104872519"></a><a name="p6918104872519"></a>app-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1091894814255"><a name="p1091894814255"></a><a name="p1091894814255"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p891804811257"><a name="p891804811257"></a><a name="p891804811257"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p1918748152512"><a name="p1918748152512"></a><a name="p1918748152512"></a>应用访问次数限制</p>
</td>
</tr>
<tr id="row5918648192514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p179181648112513"><a name="p179181648112513"></a><a name="p179181648112513"></a>ip-limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p15918548132512"><a name="p15918548132512"></a><a name="p15918548132512"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p69181248132518"><a name="p69181248132518"></a><a name="p69181248132518"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p169192488255"><a name="p169192488255"></a><a name="p169192488255"></a>源IP访问次数限制</p>
</td>
</tr>
<tr id="row79191948142513"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p491994816255"><a name="p491994816255"></a><a name="p491994816255"></a>interval</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p11919114819255"><a name="p11919114819255"></a><a name="p11919114819255"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p79191648132510"><a name="p79191648132510"></a><a name="p79191648132510"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p119195483257"><a name="p119195483257"></a><a name="p119195483257"></a>流控策略时间周期</p>
</td>
</tr>
<tr id="row199198489254"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p1919154812517"><a name="p1919154812517"></a><a name="p1919154812517"></a>unit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1391916487253"><a name="p1391916487253"></a><a name="p1391916487253"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p292015486259"><a name="p292015486259"></a><a name="p292015486259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p3920748112517"><a name="p3920748112517"></a><a name="p3920748112517"></a>流控策略时间周期单位，支持SECOND、MINUTE、HOUR、DAY</p>
</td>
</tr>
<tr id="row14920174811258"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p7920948132515"><a name="p7920948132515"></a><a name="p7920948132515"></a>shared</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p192019487254"><a name="p192019487254"></a><a name="p192019487254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1920124892513"><a name="p1920124892513"></a><a name="p1920124892513"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p17920174842518"><a name="p17920174842518"></a><a name="p17920174842518"></a>是否共享流控策略</p>
</td>
</tr>
<tr id="row1392010481255"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p6921194816259"><a name="p6921194816259"></a><a name="p6921194816259"></a>special</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p29212489254"><a name="p29212489254"></a><a name="p29212489254"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p792119480253"><a name="p792119480253"></a><a name="p792119480253"></a>Object</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p15921144832520"><a name="p15921144832520"></a><a name="p15921144832520"></a>特殊流控策略对象数组定义，参考<a href="#table6921174842513">表 special参数说明</a></p>
</td>
</tr>
</tbody>
</table>

**表 27**  special参数说明

<a name="table6921174842513"></a>
<table><thead align="left"><tr id="row5922248112514"><th class="cellrowborder" valign="top" width="21%" id="mcps1.2.5.1.1"><p id="p1492234818256"><a name="p1492234818256"></a><a name="p1492234818256"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="13%" id="mcps1.2.5.1.2"><p id="p1292214818252"><a name="p1292214818252"></a><a name="p1292214818252"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="12%" id="mcps1.2.5.1.3"><p id="p1192217488256"><a name="p1192217488256"></a><a name="p1192217488256"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="54%" id="mcps1.2.5.1.4"><p id="p19922144810251"><a name="p19922144810251"></a><a name="p19922144810251"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row109221348122519"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p4923448142518"><a name="p4923448142518"></a><a name="p4923448142518"></a>type</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p792311483258"><a name="p792311483258"></a><a name="p792311483258"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p392311487256"><a name="p392311487256"></a><a name="p392311487256"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p292315488259"><a name="p292315488259"></a><a name="p292315488259"></a>特殊流控策略类型，支持APP、USER</p>
</td>
</tr>
<tr id="row1692304842514"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p192311482252"><a name="p192311482252"></a><a name="p192311482252"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p1292364814256"><a name="p1292364814256"></a><a name="p1292364814256"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p1092344819252"><a name="p1092344819252"></a><a name="p1092344819252"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p13923134817259"><a name="p13923134817259"></a><a name="p13923134817259"></a>访问次数</p>
</td>
</tr>
<tr id="row13923948122511"><td class="cellrowborder" valign="top" width="21%" headers="mcps1.2.5.1.1 "><p id="p15923248172511"><a name="p15923248172511"></a><a name="p15923248172511"></a>instance</p>
</td>
<td class="cellrowborder" valign="top" width="13%" headers="mcps1.2.5.1.2 "><p id="p4924448162510"><a name="p4924448162510"></a><a name="p4924448162510"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="12%" headers="mcps1.2.5.1.3 "><p id="p119249482253"><a name="p119249482253"></a><a name="p119249482253"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="54%" headers="mcps1.2.5.1.4 "><p id="p5924154822518"><a name="p5924154822518"></a><a name="p5924154822518"></a>特殊APP或USER的对象标识</p>
</td>
</tr>
</tbody>
</table>

请求消息样例：

```
{
	"swagger": "2.0",
	"info": {
		"description": "api group test",
		"title": "APIGroup_test",
		"version": "2019-09-12-17:38:10"
	},

	"paths": {
		"/test/{path}": {
			"get": {
				"security": [
					{
						"apig-auth-app": []
					}
				],
				"description": "api test",
				"schemes": [
					"https"
				],
				"operationId": "API_test",
				"parameters": [
					{
						"type": "string",
						"description": "header parameter",
						"name": "header",
						"in": "header",
						"required": true
					},
					{
						"type": "string",
						"description": "path parameter",
						"name": "path",
						"in": "path",
						"required": true
					},
					{
						"type": "number",
						"default": "123",
						"description": "query parameter",
						"name": "query",
						"in": "query"
					}
				],
				"responses": {
					"default": {
						"$ref": "#/responses/default"
					},
					"x-apigateway-result-failure-sample": "",
					"x-apigateway-result-normal-sample": "success"
				},
				"x-apigateway-backend": {
					"httpEndpoints": {
						"address": "1.1.1.1:443",
						"description": "",
						"method": "GET",
						"path": "/test/{path}",
						"scheme": "https",
						"timeout": 5000
					},
					"parameters": [
						{
							"description": "",
							"in": "HEADER",
							"name": "header",
							"origin": "REQUEST",
							"value": "header"
						},
						{
							"description": "",
							"in": "PATH",
							"name": "path",
							"origin": "REQUEST",
							"value": "path"
						},
						{
							"description": "",
							"in": "QUERY",
							"name": "query",
							"origin": "REQUEST",
							"value": "query"
						}
					],
					"type": "HTTP"
				},
				"x-apigateway-backend-policies": [
					{
						"conditions": [
							{
								"origin": "param",
								"parameter": "path",
								"type": "exact",
								"value": "path"
							},
							{
								"origin": "source",
								"parameter": "",
								"type": "",
								"value": "1.0.0.0/8"
							}
						],
						"effectMode": "ANY",
						"httpVpcEndpoints": {
							"method": "POST",
							"name": "VPC_n9ct",
							"path": "/",
							"scheme": "HTTPS",
							"timeout": 5000
						},
						"name": "policy_test",
						"type": "HTTP-VPC"
					}
				],
				"x-apigateway-cors": false,
				"x-apigateway-match-mode": "NORMAL",
				"x-apigateway-request-type": "public"
			}
		}
	},
	"responses": {
		"default": {
			"description": "response example"
		}
	},
	"securityDefinitions": {
		"apig-auth-app": {
			"type": "apiKey",
			"name": "Authorization",
			"in": "header",
			"x-apigateway-auth-type": "AppSigv1"
		},
		"apig-auth-iam": {
			"type": "apiKey",
			"name": "unused",
			"in": "header",
			"x-apigateway-auth-type": "IAM"
		}
	}
}
```

## 响应消息<a name="section3346174120197"></a>

**表 28**  参数说明

<a name="table17320161865510"></a>
<table><thead align="left"><tr id="row20324111812552"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="p1032791895512"><a name="p1032791895512"></a><a name="p1032791895512"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="p16328111805514"><a name="p16328111805514"></a><a name="p16328111805514"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="p183299183551"><a name="p183299183551"></a><a name="p183299183551"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row7519312131514"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p10520712111516"><a name="p10520712111516"></a><a name="p10520712111516"></a>group_id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p13520151211157"><a name="p13520151211157"></a><a name="p13520151211157"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p352061212159"><a name="p352061212159"></a><a name="p352061212159"></a>分组ID</p>
</td>
</tr>
<tr id="row4331151855520"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p782812469154"><a name="p782812469154"></a><a name="p782812469154"></a>success</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p1029215518551"><a name="p1029215518551"></a><a name="p1029215518551"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p3336918115517"><a name="p3336918115517"></a><a name="p3336918115517"></a>导入成功信息</p>
</td>
</tr>
<tr id="row153379185556"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p1433831818554"><a name="p1433831818554"></a><a name="p1433831818554"></a>failure</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p333831825520"><a name="p333831825520"></a><a name="p333831825520"></a>Array</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p4340111810552"><a name="p4340111810552"></a><a name="p4340111810552"></a>导入失败信息</p>
</td>
</tr>
</tbody>
</table>

**表 29**  success参数说明

<a name="table2981672313"></a>
<table><thead align="left"><tr id="row898177103111"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="p109837183116"><a name="p109837183116"></a><a name="p109837183116"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="p1098474319"><a name="p1098474319"></a><a name="p1098474319"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="p1398197193117"><a name="p1398197193117"></a><a name="p1398197193117"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row49812719314"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p18981672315"><a name="p18981672315"></a><a name="p18981672315"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p209815717318"><a name="p209815717318"></a><a name="p209815717318"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p8980773120"><a name="p8980773120"></a><a name="p8980773120"></a>导入成功的API ID</p>
</td>
</tr>
<tr id="row119827123112"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p159814710314"><a name="p159814710314"></a><a name="p159814710314"></a>action</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p1698871311"><a name="p1698871311"></a><a name="p1698871311"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p43372294157"><a name="p43372294157"></a><a name="p43372294157"></a>导入行为：</p>
<a name="ul18322112914151"></a><a name="ul18322112914151"></a><ul id="ul18322112914151"><li>update：表示更新API</li><li>create：表示新建API</li></ul>
</td>
</tr>
<tr id="row1919781375316"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p8197131345315"><a name="p8197131345315"></a><a name="p8197131345315"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p3197101395317"><a name="p3197101395317"></a><a name="p3197101395317"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p41971813165317"><a name="p41971813165317"></a><a name="p41971813165317"></a>API请求方法</p>
</td>
</tr>
<tr id="row998187163114"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p129814713315"><a name="p129814713315"></a><a name="p129814713315"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p13987723113"><a name="p13987723113"></a><a name="p13987723113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p109819712314"><a name="p109819712314"></a><a name="p109819712314"></a>API请求路径</p>
</td>
</tr>
</tbody>
</table>

**表 30**  failure参数说明

<a name="table15660564193"></a>
<table><thead align="left"><tr id="row137265631919"><th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.1"><p id="p173165641915"><a name="p173165641915"></a><a name="p173165641915"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="20.792079207920793%" id="mcps1.2.4.1.2"><p id="p187385616195"><a name="p187385616195"></a><a name="p187385616195"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.415841584158414%" id="mcps1.2.4.1.3"><p id="p1876256171919"><a name="p1876256171919"></a><a name="p1876256171919"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row138175661920"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p11458112915203"><a name="p11458112915203"></a><a name="p11458112915203"></a>error_code</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p38145613190"><a name="p38145613190"></a><a name="p38145613190"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p1882175612193"><a name="p1882175612193"></a><a name="p1882175612193"></a>导入失败的错误码</p>
</td>
</tr>
<tr id="row18262135516207"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p142627557208"><a name="p142627557208"></a><a name="p142627557208"></a>error_msg</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p1426220553205"><a name="p1426220553205"></a><a name="p1426220553205"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p32621855152010"><a name="p32621855152010"></a><a name="p32621855152010"></a>导入失败的错误信息</p>
</td>
</tr>
<tr id="row236592717212"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p1836592772116"><a name="p1836592772116"></a><a name="p1836592772116"></a>method</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p736592710219"><a name="p736592710219"></a><a name="p736592710219"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p1036518272216"><a name="p1036518272216"></a><a name="p1036518272216"></a>API请求方法</p>
</td>
</tr>
<tr id="row17854183118217"><td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.1 "><p id="p5854731142118"><a name="p5854731142118"></a><a name="p5854731142118"></a>path</p>
</td>
<td class="cellrowborder" valign="top" width="20.792079207920793%" headers="mcps1.2.4.1.2 "><p id="p5854143112210"><a name="p5854143112210"></a><a name="p5854143112210"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="58.415841584158414%" headers="mcps1.2.4.1.3 "><p id="p128541531162113"><a name="p128541531162113"></a><a name="p128541531162113"></a>API请求路径</p>
</td>
</tr>
</tbody>
</table>

响应消息样例：

```
{
  "group_id": "27aa2317e3514c5bb5aab5587a5e50ea",
  "success": [
    {
      "id": "aea39194d8db46408be0174b0bd15931",
      "action": "create",
      "method": "GET",
      "path": "/test01"
    }
  ],
  "failure": [
    {
      "error_code": "APIG.2011",
      "error_msg": "Parameter value does not match the rules,parameterName:backend_type",
      "method": "GET",
      "path": "/test02"
    }
  ]
}
```

## 状态码<a name="section67075185"></a>

**表 31**  返回消息说明

<a name="table15714732"></a>
<table><thead align="left"><tr id="row24997277"><th class="cellrowborder" valign="top" width="20%" id="mcps1.2.3.1.1"><p id="p11513591"><a name="p11513591"></a><a name="p11513591"></a>状态码</p>
</th>
<th class="cellrowborder" valign="top" width="80%" id="mcps1.2.3.1.2"><p id="p60185706"><a name="p60185706"></a><a name="p60185706"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row43203997"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p9862840"><a name="p9862840"></a><a name="p9862840"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p73578115452"><a name="p73578115452"></a><a name="p73578115452"></a>OK</p>
</td>
</tr>
<tr id="row9362312"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p20149775"><a name="p20149775"></a><a name="p20149775"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p21519099"><a name="p21519099"></a><a name="p21519099"></a>Bad Request</p>
</td>
</tr>
<tr id="row43351211"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p21787193"><a name="p21787193"></a><a name="p21787193"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p13949586"><a name="p13949586"></a><a name="p13949586"></a>Forbidden</p>
</td>
</tr>
<tr id="row63248959"><td class="cellrowborder" valign="top" width="20%" headers="mcps1.2.3.1.1 "><p id="p22892027"><a name="p22892027"></a><a name="p22892027"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="80%" headers="mcps1.2.3.1.2 "><p id="p14947689"><a name="p14947689"></a><a name="p14947689"></a>Server Internal Error</p>
</td>
</tr>
</tbody>
</table>

